# 다국어 혼합 대화방의 실시간 개인별 번역: 기술 타당성과 단위 경제성 (한국 관련 롱테일 언어 중심)

> 조사 기준일: 2026-11-04. 가격·언어 지원 수치 옆에 확인 날짜를 적었다.
> 조사 제약: 이 세션은 네트워크가 제한되어 developers.google.com, docs.cloud.google.com, deepl.com, learn.microsoft.com, azure.microsoft.com, aws.amazon.com, ncloud.com, arxiv.org, aclanthology.org, huggingface.co, openai.com 원문을 직접 열지 못했다. 그래서 (a) 열 수 있었던 1차 출처(cloud.google.com 가격 페이지, anthropic.com, microsoft.com/translator, GitHub 원본 파일, developer.apple.com)와 (b) WebSearch 요약을 함께 썼다. (b)는 "검색 요약 기준"이라고 따로 표시했다. 조사 중간에 세션 전체의 WebSearch 한도(200회)가 소진되어 STT/TTS 벤더별 언어표, 지연시간 실측치, back-translation 연구 원문 등은 확인하지 못했다. 이 항목들은 각 섹션의 Gaps에 적었다.

## 1. 엔진별 언어 커버리지: 어떤 엔진이 20개 언어를 지원하고, 어디가 비어 있는가

### Takeaway
20개 대상 언어를 텍스트 번역으로 (거의) 모두 지원한다고 확인된 엔진은 Microsoft Translator(Tetum만 미등재)와 Meta NLLB-200(Tetum 미포함, 단 모델 가중치가 CC-BY-NC 4.0이라 상용 사용 제약)뿐이다. Google Cloud Translation은 언어 수(약 189개, 2차 출처)로 볼 때 모두 지원할 가능성이 높지만, 이 세션에서 언어표 원문은 확인하지 못했다. Papago, DeepL, Android ML Kit 온디바이스 번역은 Khmer, Burmese, Lao, Nepali, Sinhala, Kyrgyz, Tetum 쪽에 공백이 크다. Tetum은 거의 모든 오픈 모델(NLLB, SeamlessM4T, Whisper)에서 빠져 있어 가장 어려운 언어다.

### Cited Findings

**Google Cloud Translation**
- 언어표 원문(docs.cloud.google.com/translate/docs/languages)은 이 세션에서 403으로 막혀 확인하지 못했다. 2026년 2차 리뷰 페이지 제목은 "Google Cloud Translation Review (2026): Gemini, 189 Languages & Pricing"이다. — [toolworthy.ai](https://www.toolworthy.ai/tool/google-cloud-translation) (검색 결과 제목 기준)
- 가격 페이지에 NMT, Translation LLM, Adaptive translation, Custom models가 별도 모델로 나뉘어 있다. 모델마다 지원 언어가 다를 수 있다는 뜻이다(LLM 모델의 언어 범위는 미확인). — [Cloud Translation pricing](https://cloud.google.com/translate/pricing) (2026-11-04 확인)

**Papago (Naver Cloud Platform, Papago Translation API)**
- 공식 가이드는 과금 단위(100만 자)와 계량 방식만 확인되었다. 지원 언어 목록 원문(ncloud-docs)은 이 세션에서 열지 못했다. — [Papago Translation API 사용 가이드](https://guide.ncloud-docs.com/docs/papagotranslation-api), [Papago Translation 개요](https://guide.ncloud-docs.com/docs/papagotranslation-overview) (검색 요약 기준)

**DeepL**
- 2025-06-24: Vietnamese와 Hebrew를 발표하고 Thai는 early access로 발표했다. Thai는 API에 먼저 제공되었다. — [DeepL blog: Vietnamese, Thai, Hebrew launch](https://www.deepl.com/en/blog/vietnamese-thai-hebrew-launch) (검색 요약 기준)
- 2025년 말 보도자료: "100개 이상 언어"로 확대하면서 약 70개를 엔터프라이즈 고객 대상 **beta**로 추가했다. APAC 신규 언어로 Hindi, Malay, Tagalog, Bengali, Marathi, Tamil, Urdu를 명시했다. — [DeepL press release](https://www.deepl.com/en/press-release/deepl-accelerates-global-business-connectivity-and-document-translation-with-new-languages) (검색 요약 기준)
- DeepL Translator 언어 페이지에는 Bengali, Kazakh, Mongolian, Nepali, Tagalog, Uzbek이 포함되어 있다. **Khmer는 DeepL의 어떤 목록에서도 확인되지 않았다.** Burmese, Lao, Sinhala, Kyrgyz, Tetum의 포함 여부는 확인하지 못했다. — [DeepL Translator languages](https://support.deepl.com/hc/en-us/articles/360019925219-DeepL-Translator-languages) (검색 요약 기준)
- 2026-02 changelog 기준 v2/languages는 source 101개, target 106개다. 총 언어 수는 출처마다 다르다(API 109개 vs Wikipedia 120개). — [DeepL roadmap & release notes](https://developers.deepl.com/docs/resources/roadmap-and-release-notes), [Wikipedia: DeepL Translator](https://en.wikipedia.org/wiki/DeepL_Translator) (검색 요약 기준)
- DeepL OpenAPI 명세 v3.14.0에는 언어 enum이 더 이상 없고 `GET /v3/languages`를 조회하라고 되어 있다. beta 언어는 `include=beta`로 조회한다. 이전 `enable_beta_languages` 파라미터는 "has no effect"로 deprecated되었다. — [DeepLcom/openapi openapi.yaml](https://github.com/DeepLcom/openapi) (2026-11-04 확인)

**Microsoft Translator / Azure AI Translator**
- Microsoft Translator 언어 페이지의 Text 열에서 Korean, Vietnamese, Nepali, Khmer, Myanmar (Burmese), Uzbek (Latin), Russian, Kazakh, Kyrgyz, Indonesian, Thai, Filipino, Mongolian (Cyrillic/Traditional), Sinhala, Tamil, Bangla, Urdu, Lao, Chinese Simplified, English가 모두 "Yes"다. **Tetum은 목록에 없다.** — [Microsoft Translator Languages](https://www.microsoft.com/en-us/translator/languages/) (2026-11-04 확인)
- 과거 발표: Khmer, Lao, Myanmar, Nepali는 9개 언어 일괄 추가 때, Kyrgyz, Mongolian, Uzbek (Latin)은 12개 언어 추가 때, Sinhala는 Konkani, Maithili, Sindhi와 함께 추가되었다. — [machinetranslate.org: Microsoft](https://machinetranslate.org/microsoft), [Neowin](https://www.neowin.net/news/microsoft-translator-adds-support-for-nine-additional-languages/) (검색 요약 기준)

**Amazon Translate**
- 2020-11에 Mongolian, Sinhala, Kazakh 등 16개 언어·변형을 추가했다. Khmer, Lao, Burmese, Nepali, Tetum 지원 여부는 이 세션에서 확인하지 못했다. — [AWS What's New 2020-11](https://aws.amazon.com/about-aws/whats-new/2020/11/amazon-translate-adds-support-for-sixteen-more-languages-and-variants), [Supported languages](https://docs.aws.amazon.com/translate/latest/dg/what-is-languages.html) (검색 요약 기준)

**Meta NLLB-200 (오픈 가중치)**
- FLORES-200 언어 코드 목록에 kor_Hang, vie_Latn, npi_Deva, khm_Khmr, mya_Mymr, uzn_Latn, rus_Cyrl, kaz_Cyrl, kir_Cyrl, ind_Latn, tha_Thai, tgl_Latn, khk_Cyrl(Halh Mongolian), sin_Sinh, tam_Taml, ben_Beng, urd_Arab, lao_Laoo, zho_Hans, eng_Latn이 있다. **Tetum(tet_Latn)은 없다**(Tok Pisin tpi_Latn은 있음). — [FLORES-200 README](https://github.com/facebookresearch/flores/blob/main/flores200/README.md) (2026-11-04 확인)
- NLLB-200 모델은 54.5B MoE, 3.3B, 1.3B Dense와 Distilled 1.3B, 600M으로 공개되어 있다. "All models are licensed under CC-BY-NC 4.0"이고 코드는 MIT다. — [fairseq nllb README](https://github.com/facebookresearch/fairseq/blob/nllb/README.md) (2026-11-04 확인)

**Meta SeamlessM4T v2**
- 지원표에서 Bengali, Mandarin, English, Indonesian, Korean, Russian, Tagalog, Thai, Urdu, Northern Uzbek, Vietnamese는 Source와 Target 모두 Speech+Text를 지원한다. Kazakh, Halh Mongolian, Khmer, Kyrgyz, Lao, Burmese, Nepali, Tamil은 Source가 Speech+Text이고 Target은 Text만이다. **Sinhala와 Tetum은 표에 없다.** — [seamless_communication docs/m4t README](https://github.com/facebookresearch/seamless_communication/blob/main/docs/m4t/README.md) (2026-11-04 확인)
- SeamlessM4T v1/v2와 SeamlessStreaming 모델은 CC-BY-NC 4.0이다. — [seamless_communication README (License)](https://github.com/facebookresearch/seamless_communication/blob/main/README.md) (2026-11-04 확인)

**Android ML Kit 온디바이스 번역**
- ML Kit 공식 언어 페이지를 링크하는 Flutter 래퍼의 `TranslateLanguage` enum에는 59개 언어가 있다. 대상 언어 중 korean, vietnamese, russian, indonesian, thai, tagalog, tamil, bengali, urdu, chinese, english는 **포함**되고, **Nepali, Khmer, Burmese, Uzbek, Kazakh, Kyrgyz, Mongolian, Sinhala, Lao, Tetum은 없다**. — [google_ml_kit_flutter on_device_translator.dart](https://github.com/flutter-ml/google_ml_kit_flutter/blob/master/packages/google_mlkit_translation/lib/src/on_device_translator.dart) (2026-11-04 확인)
- 이탈리아어 Firebase 문서도 "59 lingue"로 숫자가 일치한다. 공식 페이지는 "50개 이상"이라고 표기한다. — [Firebase ML Kit translation (it)](https://firebase.google.com/docs/ml-kit/translation?hl=it), [ML Kit translation](https://developers.google.com/ml-kit/language/translation) (검색 요약 기준)

**Apple Translation framework (iOS)**
- 개발자 문서에는 `LanguageAvailability`(지원 언어 목록 `supportedLanguages`, `status(from:to:)`로 언어쌍 설치·가용 상태 확인, `init(preferredStrategy:)`)와 `TranslationSession`이 있다. 정적인 언어 목록은 문서에 없고 런타임에 조회하는 구조다. — [Apple Developer: Translation](https://developer.apple.com/documentation/translation), [LanguageAvailability](https://developer.apple.com/documentation/translation/languageavailability) (2026-11-04 확인)
- Apple Translate 앱에는 Indonesian, Thai가 2022-06-22에, Vietnamese가 2022-07-27에 추가되었다. — [Wikipedia: Translate (Apple)](https://en.wikipedia.org/wiki/Translate_(Apple)) (검색 요약 기준)
- iOS 26.1에서 Apple Intelligence 언어에 Vietnamese, Korean, Chinese 등이 포함되었다. Thai, Indonesian은 이 목록에 없다. — [9to5Mac 2025-11-11](https://9to5mac.com/2025/11/11/ios-26-1-brings-apple-intelligence-to-these-eight-new-languages/) (검색 요약 기준)

#### 커버리지 매트릭스 (텍스트 번역; 위 인용을 요약)
범례: ✔ = 출처에서 확인, ✘ = 출처 목록에 없음, ? = 이 세션에서 미확인, β = beta. Papago의 Korean/Mandarin/English와 각 엔진의 English는 기본 언어라서 ✔로 표기했지만, 이 세션에서 원문을 확인하지는 않았다.

| 언어 | Google | Papago | DeepL | Microsoft | Amazon | NLLB-200 | Seamless v2 (텍스트) | ML Kit 온디바이스 |
|---|---|---|---|---|---|---|---|---|
| Korean | ? | ✔ | ? (장기 지원으로 알려짐) | ✔ | ? | ✔ | ✔ | ✔ |
| Vietnamese | ? | ? | ✔ (2025-06) | ✔ | ? | ✔ | ✔ | ✔ |
| Nepali | ? | ? | ✔ (목록) | ✔ | ? | ✔ | ✔ | ✘ |
| Khmer | ? | ? | ✘ (미발견) | ✔ | ? | ✔ | ✔ | ✘ |
| Burmese | ? | ? | ? | ✔ | ? | ✔ | ✔ | ✘ |
| Uzbek | ? | ? | ✔ (목록) | ✔ | ? | ✔ | ✔ | ✘ |
| Russian | ? | ? | ? | ✔ | ? | ✔ | ✔ | ✔ |
| Kazakh | ? | ? | ✔ (목록) | ✔ | ✔ (2020) | ✔ | ✔ | ✘ |
| Kyrgyz | ? | ? | ? | ✔ | ? | ✔ | ✔ | ✘ |
| Indonesian | ? | ? | ? | ✔ | ? | ✔ | ✔ | ✔ |
| Thai | ? | ? | ✔ (2025) | ✔ | ? | ✔ | ✔ | ✔ |
| Tagalog/Filipino | ? | ? | ✔ β | ✔ | ? | ✔ | ✔ | ✔ |
| Mongolian | ? | ? | ✔ (목록) | ✔ | ✔ (2020) | ✔ | ✔ | ✘ |
| Sinhala | ? | ? | ? | ✔ | ✔ (2020) | ✔ | ✘ | ✘ |
| Tamil | ? | ? | ✔ β | ✔ | ? | ✔ | ✔ | ✔ |
| Bengali | ? | ? | ✔ β | ✔ | ? | ✔ | ✔ | ✔ |
| Urdu | ? | ? | ✔ β | ✔ | ? | ✔ | ✔ | ✔ |
| Lao | ? | ? | ? | ✔ | ? | ✔ | ✔ | ✘ |
| Tetum | ? | ? | ? | ✘ | ? | ✘ | ✘ | ✘ |
| Mandarin | ? | ✔ | ? | ✔ | ? | ✔ | ✔ | ✔ |
| English | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |

### Inferences
- 20개 언어 전체를 하나의 상용 NMT API로 처리하려면 Google(언어 수로 볼 때 유력, 검증 필요) 또는 Microsoft(Tetum만 빠짐)가 현실적인 기본값이다. Papago는 한국어 품질과 국내 데이터 처리라는 장점이 있지만 롱테일 언어 공백이 클 가능성이 높아(아래 Gaps 참조) 보조 엔진에 가깝다.
- DeepL의 신규 롱테일 언어는 "엔터프라이즈 beta"로 출시되었다. 이주노동자용 대중 앱에 기본 엔진으로 쓰기에는 가용성과 품질이 불확실하다.
- 오픈 모델(NLLB, SeamlessM4T)은 커버리지는 넓지만 CC-BY-NC 4.0이어서, 상용 서비스에 쓰려면 별도 라이선스 검토나 다른 오픈 모델(라이선스가 허용적인 LLM 등)이 필요하다.
- Tetum은 오픈 MT/ASR 계열 전반에서 빠져 있으므로 범용 LLM(또는 Google)에 의존하고, 품질 검증 비용을 따로 잡아야 한다.
- 온디바이스 번역은 Android ML Kit 기준으로 Nepali, Khmer, Burmese, Uzbek, Kazakh, Kyrgyz, Mongolian, Sinhala, Lao가 빠져 있다. 정작 이주노동자 핵심 언어 다수가 온디바이스 무료 옵션을 쓸 수 없다는 뜻이다.

### Gaps
- Google Cloud Translation의 언어별 지원표(특히 Tetum, 그리고 Translation LLM 모델의 언어 범위)를 원문으로 확인하지 못했다(docs.cloud.google.com 접근 차단).
- Papago API 지원 언어 목록 원문을 확인하지 못했다. 기존 지식으로는 ko/en/ja/zh-CN/zh-TW/vi/th/id/fr/es/ru/de/it 등 10여 개 언어이고 Nepali, Khmer, Burmese, Uzbek, Kazakh, Kyrgyz, Tagalog, Mongolian, Sinhala, Tamil, Bengali, Urdu, Lao, Tetum은 미지원으로 알고 있지만, **2026년 현재 기준으로 검증되지 않았다**. 보고서에 쓰기 전에 ncloud 콘솔에서 확인해야 한다.
- DeepL `/v3/languages`의 실제 응답(Burmese, Lao, Sinhala, Kyrgyz, Tetum 포함 여부, 각 언어의 stable/beta 상태)은 확인하지 못했다.
- Amazon Translate 최신 언어표, LLM(Claude, GPT, Gemini, Qwen, Gemma)의 언어별 공식 "지원" 선언은 확인하지 못했다. LLM은 대개 공식 지원 목록이 없거나 일부만 명시하므로 자체 평가가 필요하다.
- Apple Translation framework의 실제 지원 언어 목록(iOS 26 기준)은 문서에 정적 목록이 없어 확인하지 못했다. 기기에서 `supportedLanguages`를 조회해야 한다.

## 2. 저자원 언어쌍의 번역 품질 근거 (Korean↔X, X↔Y, 저자원 언어의 품질 하락폭)

### Takeaway
Khmer, Burmese, Lao, Nepali 같은 언어의 품질 근거는 대부분 **English↔X** FLORES-200 기준이고, **Korean↔X 또는 X↔Y 직접 언어쌍을 평가한 공개 연구는 이번 조사에서 찾지 못했다**. 확인된 수치를 보면 영어에서 저자원 언어로 가는 방향(en→km chrF 약 43, en→my 약 54, Gemini-2.5-Flash 기준)이 저자원 언어에서 영어로 오는 방향(km→en 약 73, my→en 약 68)보다 훨씬 낮다. 즉 "한국어 → 롱테일 언어" 방향(예: 한국인 관리자의 안전 지시)이 가장 위험한 방향이다. NLLB 54B는 FLORES-200 전체 40,602개 방향의 chrF++를 공개하고 있어 X↔Y 직접쌍의 베이스라인 자료로 쓸 수 있다.

### Cited Findings
- **LingBench++** (arXiv 2507.16809): Gemini-2.5-Flash의 chrF는 Burmese가 en→my 53.93, my→en 68.35이고, Central Khmer가 en→km 43.45, km→en 73.44다. — [LingBench++](https://arxiv.org/abs/2507.16809) (검색 요약 기준, 원문 미열람)
- **TULUN** (arXiv 2505.18683): FLORES-200 devtest의 저자원 6개 언어 평균 chrF++가 NLLB-54B 38.26, TULUN 결합 시스템 41.09다. Gemini 2.0 Flash 단독도 NLLB-54B를 자주 앞섰다고 서술한다. 6개 언어가 무엇인지는 요약에서 확인하지 못했다. — [TULUN](https://arxiv.org/abs/2505.18683) (검색 요약 기준)
- **Compositional Translation** (arXiv 2503.04554): Burmese, Khmer, Lao를 포함한 English→X FLORES-200 BLEU/chrF++를 보고한다(수치 미확인). — [Compositional Translation](https://arxiv.org/abs/2503.04554) (검색 요약 기준)
- **Aya** (arXiv 2402.07827): Korean, Khmer, Lao, Burmese→English FLORES-200 chrF++ 표가 있다(모델별 열은 요약에서 판독 불가). — [Aya Model](https://arxiv.org/abs/2402.07827) (검색 요약 기준)
- **LLaMAX** (arXiv 2407.05975): LLM 번역 능력을 100개 이상 언어로 확장하는 연구다(세부 수치 미확인). — [LLaMAX](https://arxiv.org/abs/2407.05975) (검색 요약 기준)
- **NLLB-200 metrics 공개 범위**: 54B MoE 모델은 FLORES-200 **40,602개 전 방향**의 chrF++, spBLEU(SPM-200), spBLEU(SPM-100)를 `metrics.csv`로 공개한다. 다른 모델(3.3B/1.3B/600M distilled 등)은 영어 중심 402개 방향과 비영어 200개 샘플 방향의 chrF++만 공개한다. — [fairseq nllb modeling README](https://github.com/facebookresearch/fairseq/blob/nllb/examples/nllb/modeling/README.md) (2026-11-04 확인)
- NLLB-200의 원 논문과 Nature 게재본 — [No Language Left Behind (arXiv 2207.04672)](https://arxiv.org/abs/2207.04672), [Nature 2024: Scaling neural machine translation to 200 languages](https://www.nature.com/articles/s41586-024-07335-x)
- **한국어 관련 KCI 연구**: 한국어-일본어 NMT가 한국어-영어보다 단어·문장 번역 정확도가 높았다(문자 체계·어순 유사성 효과). 베트남어나 네팔어 등을 다룬 연구는 이번 검색에서 나오지 않았다. — [KCI: 단어 임베딩 분석을 통한 신경망 기계 번역 시스템의 성능 비교](https://www.kci.go.kr/kciportal/ci/sereArticleSearch/ciSereArtiView.kci?sereArticleSearchBean.artiId=ART002810550) (검색 요약 기준)
- 도메인 특화(법률·특허) 한영 맞춤형 MT 엔진의 수동 평가 사례 — [번역학연구 24권 1호 (2023)](https://journal.kci.go.kr/kats/archive/articlePdf?artiId=ART002945403) (검색 요약 기준)
- 한국어↔베트남어, 이주노동자 대상 네팔어 MT를 직접 평가한 논문은 검색에서 확인되지 않았다(이번 조사의 "부재" 결과). — 같은 검색 결과 요약

### Inferences
- 영어→저자원 방향의 chrF가 40~55 수준이고, 저자원→영어 방향은 68~73이다. 이 차이를 보면 "생성 쪽 언어가 저자원일 때" 품질이 크게 떨어진다. 한국어→Khmer/Burmese/Lao/Nepali는 영어 피벗을 거치든 직접 번역하든 이 구간에 속할 가능성이 높다(추정).
- X↔Y 직접쌍(예: Vietnamese↔Nepali)은 NLLB 54B metrics.csv로 "영어 피벗 대비 직접 번역" 품질을 정량 비교할 수 있는 유일한 대규모 공개 자료다. 보고서 작성 단계에서 이 CSV(kor_Hang 및 대상 언어 간 방향)를 내려받아 표로 만드는 것이 다음 단계로 적절하다(이번 세션에서는 다운로드 호스트 차단).
- LLM(Gemini 계열)이 NLLB-54B와 비슷하거나 낫다는 신호(TULUN)가 있다. 따라서 "전용 NMT보다 LLM이 롱테일 언어에서 열등하다"는 가정은 더 이상 기본값이 아니다. 다만 언어별 편차가 크므로 엔진 선정은 **자체 평가셋(작업장 안전 지시, 학교 공지, 가족 대화 문장)** 으로 결정해야 한다.
- FLORES-200은 위키 기반의 문어체 문장이다. 채팅체, 존댓말, 은어, 코드스위칭 품질은 FLORES 점수로 예측하기 어렵다(추정).

### Gaps
- Korean↔{Nepali, Khmer, Burmese, Lao, Sinhala, Mongolian} 직접 방향의 chrF++/COMET 수치(NLLB metrics.csv는 존재가 확인되었지만 값은 미확보).
- WMT 공식 결과(예: WMT24/25 general task, WMT24++의 ko/vi/th/fil/ta/bn/ur 포함 여부), Claude/GPT/Qwen/Gemma의 저자원 아시아 언어 평가 원문 수치. arxiv와 aclanthology 접근이 막혀 확인하지 못했다.
- Papago, DeepL의 언어별 품질 공개 지표는 찾지 못했다.
- 한국어 존댓말, 방언, 현장 은어에 대한 MT 평가 연구(KCI 포함)는 이번 검색에서 확인되지 않았다.

## 3. 음성: STT/TTS 언어 지원과 오류율, 공백 지점

### Takeaway
Whisper large-v3 기준으로 Korean(CER 3.1), Russian(5.0), Indonesian(6.1), Mandarin(CER 7.7), Thai(CER 8.4), Vietnamese(8.6)는 실사용 수준이다. Filipino(13.0), Tamil(18.3), Urdu(20.6)는 중간이고, Kazakh(32.4), Nepali(40.2), Bengali(50.0)는 오류가 매우 크다. Khmer, Burmese, Lao, Uzbek, Mongolian, Sinhala는 차트에 아예 나오지 않는다(2차 출처상 large-v2에서 Khmer 약 100%, Burmese 약 116%, Lao 약 102% WER). Kyrgyz와 Tetum은 Whisper 지원 언어 자체가 아니다. 음성 출력(TTS)은 SeamlessM4T 기준으로 Khmer, Burmese, Lao, Nepali, Kazakh, Kyrgyz, Mongolian, Tamil이 텍스트 출력만 가능하다. **음성 메시지는 롱테일 언어에서 가장 큰 품질 리스크다.**

### Cited Findings
- **Whisper large-v3 FLEURS WER/CER(%)** (OpenAI 공식 저장소 차트, 2023-11-06 생성. Korean, Thai, Mandarin, Japanese는 CER): Korean 3.1, English 4.1, Russian 5.0, Indonesian 6.1, Mandarin 7.7, Thai 8.4, Vietnamese 8.6, Filipino 13.0, Tamil 18.3, Urdu 20.6, Kazakh 32.4, Nepali 40.2, Bengali 50.0. — [openai/whisper language-breakdown.svg](https://github.com/openai/whisper/blob/main/language-breakdown.svg) (2026-11-04, SVG 값 라벨에서 추출)
- **Whisper large-v3 Common Voice 15 WER/CER(%)**: Korean 5.2, Thai 5.8, Russian 5.8, Indonesian 7.2, Mandarin(CN) 12.8, Urdu 20.4, **Vietnamese 39.8**, Bengali 40.3, Nepali 40.4, Kazakh 47.6, Tamil 51.5. FLEURS(낭독)보다 Common Voice(크라우드 녹음)에서 Vietnamese 등이 크게 나빠진다. — [openai/whisper language-breakdown.svg](https://github.com/openai/whisper/blob/main/language-breakdown.svg)
- 위 FLEURS 차트(61개 언어)에 **Khmer, Burmese, Lao, Uzbek, Mongolian, Sinhala는 표시되지 않는다**. 같은 출처에서 차트 최하위는 Bengali 50.0이다. — 같은 출처
- Whisper 원 논문(large-v2) 기준 FLEURS WER은 Nepali 약 47.1%, Khmer 약 99.7%, Lao 약 101.5%, Burmese 약 115.7%다. Sinhala는 Whisper FLEURS 평가에 포함되지 않는다. OpenAI는 large-v3의 언어별 표를 공개하지 않았다고 서술한다. — [vocova.app 블로그](https://vocova.app/blog/transcription-accuracy-by-language) (2차 출처, 검색 요약 기준. 원 논문 [Whisper paper](https://cdn.openai.com/papers/whisper.pdf)와 대조하지 못함)
- Whisper tokenizer의 지원 언어에는 ko, vi, ne, km, my(myanmar), uz, ru, kk, id, th, tl, mn, si, ta, bn, ur, lo, zh, en이 있고 **ky(Kyrgyz)와 Tetum은 없다**. — [openai/whisper tokenizer.py](https://github.com/openai/whisper/blob/main/whisper/tokenizer.py) (2026-11-04 확인)
- 81개 FLEURS 언어별로 large-v3를 fine-tuning한 연구에 따르면, 고유 문자 체계 언어(Thai, Georgian, Burmese, Khmer)가 fine-tuning 효과를 가장 적게 받았다. — [Fine-tuning Whisper Across 81 Languages (SCiL 2026)](https://aclanthology.org/2026.scil-main.37/) (검색 요약 기준)
- **SeamlessM4T v2 음성**: 대상 20개 언어 중 Sinhala와 Tetum을 제외한 전부가 speech source(STT/음성번역 입력)를 지원한다. speech target(음성 출력)은 Bengali, Mandarin, English, Indonesian, Korean, Russian, Tagalog, Thai, Urdu, Uzbek, Vietnamese만 지원한다. — [seamless_communication m4t README](https://github.com/facebookresearch/seamless_communication/blob/main/docs/m4t/README.md) (2026-11-04 확인)
- **Microsoft Translator(앱) 기능표** (Text / Speech / Image / TTS): Korean, Mandarin, English, Filipino, Indonesian은 4개 모두 Yes다. Vietnamese, Thai, Tamil, Russian은 Speech와 TTS가 Yes다. Khmer, Lao, Myanmar, Kazakh, Bangla, Urdu, Uzbek은 Text와 TTS만 Yes(Speech 공란)다. **Nepali, Kyrgyz, Mongolian, Sinhala는 Text만 Yes**다. — [Microsoft Translator Languages](https://www.microsoft.com/en-us/translator/languages/) (2026-11-04 확인. Azure Speech 서비스 자체의 언어표와는 다를 수 있음)
- **Google Speech-to-Text v2 가격**: Standard 모델은 0~500,000분 구간 $0.016/분, 이후 구간별 $0.01, $0.008, $0.004/분이다. Dynamic Batch는 $0.003/분이고, Standard에는 chirp(V2 전용) 등이 포함된다. Dynamic batch는 요청을 1초 단위로 올림한다. — [Speech-to-Text pricing](https://cloud.google.com/speech-to-text/pricing) (2026-11-04 확인)
- **Google Text-to-Speech 가격**: Chirp 3: HD $30/100만 자(무료 100만 자), Instant custom voice $60/100만 자, WaveNet과 Standard $4/100만 자(무료 400만 자), Neural2 $16/100만 자(무료 100만 자), Studio $160/100만 자다. Gemini 3.8 Flash TTS(Preview)는 2026-12-31까지 입력 텍스트 $0.50/1M tokens, 출력 오디오 $9.00/1M tokens이고, 2027-01-01부터 $1.00/$18.00이다. — [Text-to-Speech pricing](https://cloud.google.com/text-to-speech/pricing) (2026-11-04 확인)
- **Gemini 오디오 입력 가격**(STT 대용): Gemini 3.1 Flash-Lite audio input $0.50/1M tokens, Gemini 2.5 Flash-Lite audio input $0.30/1M tokens, Gemini 2.5 Flash audio input $1.00/1M tokens. — [Vertex AI generative AI pricing](https://cloud.google.com/vertex-ai/generative-ai/pricing) (2026-11-04 확인)

### Inferences
- 음성 품질 등급(추정, Whisper 기준): **A(바로 사용 가능)** Korean, Russian, Indonesian, Mandarin, Thai, Vietnamese(낭독 기준. 실제 대화 녹음에서는 Common Voice 39.8로 크게 악화) / **B(보정 필요)** Filipino, Tamil, Urdu / **C(위험)** Kazakh, Nepali, Bengali / **D(사실상 불가 또는 미지원)** Khmer, Burmese, Lao, Uzbek, Mongolian, Sinhala, Kyrgyz, Tetum.
- 공사장 소음, 사투리, 코드스위칭은 FLEURS/CV 조건보다 나쁘다. 따라서 음성 메시지는 "STT 결과를 발화자에게 먼저 보여주고 확인받은 뒤 번역"하는 UX(발신자 측 텍스트 확인)가 필요하다(추정).
- D등급 언어는 음성 메시지를 번역하지 않고 원음 그대로 전달하면서 "자동 전사 불가"로 표시하거나, 해당 언어 사용자에게는 음성 대신 텍스트 입력을 권장하는 정책이 현실적이다(추정).
- TTS 출력(읽어주기)은 Khmer, Lao, Burmese 등에서 Microsoft에 TTS가 있다는 신호가 있다. 반면 Nepali, Mongolian, Sinhala, Kyrgyz는 Microsoft와 Seamless 모두 음성 출력이 확인되지 않아 공백일 가능성이 높다(추정).

### Gaps
- Google Chirp 2/3의 언어별 지원·WER, Azure Speech(STT/TTS) 언어표, Naver CLOVA Speech와 CLOVA Voice 지원 언어, ElevenLabs 지원 언어(Nepali, Khmer, Lao, Burmese 등)를 확인하지 못했다(문서 호스트 차단과 검색 한도 소진).
- Whisper large-v3의 Khmer, Burmese, Lao, Uzbek, Mongolian 실제 수치(차트 미표시 사유가 "50% 초과"인지 "미평가"인지 확인 불가).
- Gemini 오디오의 초당 토큰 수(비용 모델에서는 32 tokens/초로 가정)를 이 세션에서 공식 문서로 확인하지 못했다.
- 한국 작업장 소음 환경, 한국어 코드스위칭 음성의 STT 평가 연구.

## 4. 가격(2026-11 기준)과 단위 경제성: 방당·MAU당 비용, 엔진 비교, 하이브리드 효과

### Takeaway
가정한 방(20명, 4개 언어, 하루 100메시지, 평균 40자, 20%는 10초 음성)의 월 비용은 다음과 같다. 문자 과금 NMT(Google $20/100만 자) 기준 번역만 **약 $7.2/방/월(MAU당 $0.36)** 이고, 음성(STT+TTS)을 포함하면 **약 $10/방/월(MAU당 약 $0.5)** 이다. 저가 LLM(Claude Haiku 5.5 $0.10/$0.50 per MTok)으로 메시지당 1회 호출해 3개 언어를 한꺼번에 생성하면 번역비는 **약 $0.5/방/월(MAU당 약 $0.02)** 로 NMT의 1/15 수준이다. 이 구간에서는 번역보다 **STT($1.6/방/월)가 더 큰 비용 항목**이 된다. 번역 비용은 언어 수(fan-out)에 비례해 늘어나고, 사용자 수에는 직접 비례하지 않는다.

### Cited Findings (가격, 확인일 2026-11-04)
- **Google Cloud Translation – NMT**: 월 500,000자 무료(매월 $10 크레딧), 초과분 **$20/100만 자**(Flexible Savings Plan 1년 $18, 3년 $16). "input characters per target language" 기준으로 과금한다. 즉 대상 언어마다 다시 과금된다. — [Cloud Translation pricing](https://cloud.google.com/translate/pricing)
- **Google Translation LLM**: 입력 **$10/100만 자 + 출력 $10/100만 자**("making it cost equivalent with NMT"). Adaptive translation은 입력과 출력 각각 $25/100만 자다. Custom 모델은 $80/100만 자(사용량 구간별 $60/$40/$30)이고 학습비는 $45/시간(최대 $300)이다. glossary 생성 등 기타 요청은 과금하지 않는다. 무료 티어는 LLM에 적용되지 않는다. — [Cloud Translation pricing](https://cloud.google.com/translate/pricing)
- **Azure AI Translator S1**: **$10/100만 자**(Microsoft Q&A 답변, 2025). 3rd-party 자료는 Document Translation $15, Custom $40/100만 자로 적고 있다. 무료 F0 200만 자의 "영구 여부"는 출처마다 다르다. Azure의 LLM 번역을 $10+$10으로 적은 2차 자료가 있지만 공식 확인은 하지 못했다. — [Microsoft Q&A](https://learn.microsoft.com/en-us/answers/questions/5551059/i-want-to-know-costing-information-for-azure-ai-tr), [openapipricing](https://openapipricing.com/translation/azure-ai-translator), [chatscontrol](https://chatscontrol.com/blog/translation-api-pricing-2026-deepl-google-azure), [beri.net](https://www.beri.net/article/machine-translation-pricing-per-character-vs-per-token-llm-nmt-post-editing-cost) (검색 요약 기준)
- **Papago Translation (NCP)**: 요청 글자 수 기준으로 과금하고 과금 단위는 1,000,000자다. 공백과 특수문자를 포함하며, 언어 감지는 별도 과금하지 않는다. 월 한도를 넘는 마지막 호출도 허용되고 실제 글자 수로 과금된다. **원화 단가는 검색 결과에서 확인되지 않았다.** — [Papago Translation API 가이드](https://guide.ncloud-docs.com/docs/papagotranslation-api), [ncloud Papago Translation 상품 페이지](https://www.ncloud.com/product/aiService/papagoTranslation) (검색 요약 기준)
- **DeepL API**: `context` 파라미터에 넣은 문자는 과금에 포함되지 않는다("will not be counted toward billing"). 단가는 이 세션에서 확인하지 못했다. — [DeepLcom/openapi](https://github.com/DeepLcom/openapi)
- **Claude (Anthropic API)**: Haiku 5.5는 프롬프트 100K tokens 이하에서 입력 **$0.10/MTok, 출력 $0.50/MTok**이다(100K 초과 시 $0.50/$2.50). 프롬프트 캐시 읽기 $0.01, 쓰기 $0.125/MTok. Sonnet 5.5는 입력 $2/출력 $10. — [Anthropic pricing](https://www.anthropic.com/pricing) (2026-11-04 확인). 이전 세대 Haiku 4.5는 $1/$5이고, Batch API는 비동기 처리 시 50% 할인이다. 이 두 수치의 출처는 Claude API 참조 문서(2026-10-06 캐시, URL 없음)다. Batch 할인은 실시간 채팅에는 적용할 수 없다.
- **Gemini (Vertex AI)**: Gemini 3.8/3.7/3.6 Flash는 2026-12-31까지 도입가 **$0.75/$3.75** per 1M tokens이고, **2027-01-01부터 $1.5/$7.5**다. Gemini 3.5 Flash-Lite는 $0.30/$2.50(global), Gemini 3.1 Flash-Lite는 $0.25/$1.50, Gemini 2.5 Flash-Lite는 $0.10/$0.40, Gemini 2.5 Flash는 $0.30/$2.50이다. — [Vertex AI generative AI pricing](https://cloud.google.com/vertex-ai/generative-ai/pricing)
- **OpenAI**: 2차 가격 집계 사이트들은 모델명과 가격이 서로 맞지 않는다(예: "GPT-6 Luna $0.10/$0.50", "GPT-5.5 $5/$30", "GPT-5.6 Sol $4/$20 프로모션"). GPT-5 mini에 대한 언급은 찾지 못했다. 공식 가격은 확인하지 못했다. — [benchlm.ai OpenAI pricing](https://benchlm.ai/openai/api-pricing), [vakati-tech LLM pricing](https://www.vakati-tech.ai/llm-pricing) (검색 요약 기준, 신뢰도 낮음)
- **Google STT/TTS**: 섹션 3 참조(STT Standard $0.016/분, TTS Standard $4, Neural2 $16, Chirp 3 HD $30 per 1M chars). — [STT pricing](https://cloud.google.com/speech-to-text/pricing), [TTS pricing](https://cloud.google.com/text-to-speech/pricing)

### Inferences — 워크드 예제(모든 가정은 명시)

#### 가정
| 항목 | 값 | 비고 |
|---|---|---|
| 방 인원 | 20명 (MAU 20으로 간주) | 한 사용자가 여러 방에 속하면 MAU당 비용은 올라감 |
| 언어 수 L | 4 (예: ko, vi, ne, km) | fan-out = L−1 = 3 |
| 메시지 | 100건/일 × 30일 = 3,000건/월 | 작업장 단체방 기준. 가족방은 더 적을 것 |
| 평균 길이 | 40자 | 원문 120,000자/월 → 번역 입력 360,000자/월 |
| 캐시 | 메시지별·대상언어별 1회 번역 후 캐시 | 동일 언어 독자 여러 명에게 재사용. 중복 메시지 캐시 효과는 0으로 보수적으로 가정 |
| LLM 호출 방식 | 메시지당 1회 호출로 3개 언어를 JSON으로 동시 생성 | NMT는 대상 언어별 과금 |
| LLM 토큰(기본) | 입력 530 (지시문·용어집 300 + 직전 대화 컨텍스트 200 + 메시지 30) / 출력 210 (언어당 60 × 3 + JSON 30) | 롱테일 문자 토큰 팽창 미반영 |
| LLM 토큰(팽창) | 입력 630 / 출력 525 (출력 ×2.5) | Khmer/Burmese/Lao 등 비라틴 문자의 토큰 비효율 가정 |
| NMT 출력/입력 문자비 | 1.0 (민감도 1.3) | Google Translation LLM 출력 과금용 |
| 음성 | 메시지의 20%가 음성(평균 10초) → 600건, 100분/월 | |
| TTS | 음성 메시지를 각 대상 언어로 합성(50자 × 3언어) → 90,000자/월 | 텍스트 메시지 읽어주기는 제외 |
| DeepL 단가 | $25/100만 자로 **가정(미검증)** | |
| Papago 단가 | 약 $15/100만 자로 **가정(미검증)** | 과거 공시 20,000원/100만 자 수준이라는 기억에 기반, 검증 필요 |
| 무료 티어 | 미반영 | 규모가 커지면 무시할 수준 |

#### 번역 비용 (방/월, MAU/월, 메시지당)
| 엔진 | 방/월 | MAU/월 | 메시지당 |
|---|---|---|---|
| Google NMT ($20/M chars) | $7.20 | $0.36 | $0.0024 |
| Google Translation LLM ($10+$10, 출력비 1.0 / 1.3) | $7.20 / $8.28 | $0.36 / $0.41 | — |
| Azure Translator S1 ($10/M, 2차 출처) | $3.60 | $0.18 | $0.0012 |
| DeepL (가정 $25/M) | $9.00 | $0.45 | $0.0030 |
| Papago (가정 $15/M) | $5.40 | $0.27 | $0.0018 |
| Claude Haiku 5.5 (기본 / 팽창) | $0.47 / $0.98 | $0.024 / $0.049 | $0.00016 / $0.00033 |
| Claude Haiku 4.5 | $4.74 / $9.77 | $0.24 / $0.49 | $0.0016 |
| Claude Sonnet 5.5 | $9.48 / $19.53 | $0.47 / $0.98 | $0.0032 |
| Gemini 3.8 Flash (2026년 도입가 / 2027 정가) | $3.55 / $7.11 | $0.18 / $0.36 | $0.0012 / $0.0024 |
| Gemini 3.5 Flash-Lite | $2.05 / $4.50 | $0.10 / $0.23 | $0.0007 |
| Gemini 3.1 Flash-Lite | $1.34 / $2.83 | $0.07 / $0.14 | $0.0004 |
| Gemini 2.5 Flash-Lite | $0.41 / $0.82 | $0.02 / $0.04 | $0.00014 |

#### 음성 비용 (방/월)
- STT: Google Standard $0.016/분 × 100분 = **$1.60**. Dynamic Batch($0.003/분)는 $0.30이지만 비실시간이다. Gemini 3.1 Flash-Lite 오디오 입력은 32 tokens/초 **가정** 시 192K tokens × $0.50/M ≈ $0.10에 전사 출력 약 $0.03을 더한 수준이다(오디오 토큰률 미검증).
- TTS: 90,000자 기준 Standard/WaveNet $0.36, Neural2 $1.44, Chirp 3 HD $2.70.

#### 합계 시나리오 (방/월 → MAU/월)
- A. Google NMT + Google STT + Neural2 TTS: **$10.24 → $0.51**
- B. Claude Haiku 5.5 + Google STT + Standard TTS: **$2.43 → $0.12**
- C. Gemini 3.8 Flash(2027 정가) + Google STT + Neural2: **$10.15 → $0.51**
- D. Claude Sonnet 5.5(전량) + Google STT + Chirp 3 HD: **$13.78 → $0.69**

#### 하이브리드: 쉬운 언어쌍은 소형·온디바이스 모델, 어려운 경우만 LLM으로 승급
- 소형 모델 처리분의 한계비용을 ≈$0(온디바이스) 또는 자체 GPU 고정비로 보면, 번역비는 "승급 비율 × 상위 모델 비용"이 된다.
  - Sonnet 5.5로 승급: 10% $0.95, 20% $1.90, 30% $2.84 /방/월 (전량 Sonnet $9.48 대비 70~90% 절감)
  - Gemini 3.8 Flash(2027 정가)로 승급: 10% $0.71, 20% $1.42, 30% $2.13
  - Haiku 4.5로 승급: 10% $0.47, 20% $0.95, 30% $1.42
- 다만 저가 LLM(Haiku 5.5, Gemini 2.5 Flash-Lite) 전량 처리가 이미 $0.4~1.0/방/월이므로, 하이브리드의 **비용 절감 효과는 고급 모델을 기본값으로 쓸 때만 크다**. 저가 LLM을 기본값으로 쓰면 하이브리드의 주된 이점은 비용이 아니라 지연시간, 오프라인 동작, 프라이버시다.
- 그리고 ML Kit 온디바이스가 Nepali, Khmer, Burmese, Uzbek, Kazakh, Kyrgyz, Mongolian, Sinhala, Lao를 지원하지 않으므로(섹션 1), "흔한 언어쌍"을 온디바이스로 처리할 수 있는 범위는 ko↔{vi, th, id, tl, ru, zh, en, ta, bn, ur}로 한정된다.

#### 민감도
- **언어 수(fan-out)**: Google NMT 방/월 비용은 언어 2개 $2.4, 3개 $4.8, 4개 $7.2, 5개 $9.6, 6개 $12.0, 8개 $16.8로 선형 증가한다. LLM 일괄 호출은 입력이 공유되므로 8개 언어(fan-out 7)에서도 Haiku 5.5 약 $0.83, Sonnet 5.5 약 $16.7, Gemini 3.8 Flash(2027) 약 $12.5다. 언어가 많을수록 LLM 일괄 호출이 상대적으로 유리하다.
- **Back-translation 표시**: 발신자에게 역번역을 보여주면 번역량이 대략 2배(fan-out × 2)가 된다. 저가 LLM 기준으로는 방/월 +$0.5~1 수준이다.
- **용어집·컨텍스트 주입**: 지시문과 용어집이 2,000 tokens 이상이 되면 프롬프트 캐시 대상이 된다(최소 캐시 길이는 모델별로 다름). Haiku 5.5의 캐시 읽기는 $0.01/MTok이어서 용어집 주입 비용은 사실상 0에 가깝다.
- **가격 변동 리스크**: Gemini 3.8 Flash는 2027-01-01에 가격이 2배가 된다. 2026년 가격으로 사업계획을 세우면 과소추정된다.

### Gaps
- Papago와 DeepL의 2026년 공식 단가, Amazon Translate 단가, OpenAI 소형 모델(GPT mini 계열)의 공식 단가는 확인하지 못했다.
- 언어별 실제 토큰 수(Claude, Gemini 토크나이저에서 Khmer, Burmese, Lao, Sinhala 40자당 토큰)는 측정하지 못해 "팽창 ×2.5"는 가정이다. 실제 메시지 샘플로 `count_tokens` 측정이 필요하다.
- NLLB, Whisper 자체 호스팅 GPU 비용(인스턴스 단가, 처리량)은 확인하지 못했다.
- 짧은 메시지("네", "OK", "감사합니다")의 캐시 적중률에 대한 실측 자료는 없다.

## 5. 지연시간과 온디바이스 옵션 (저사양 Android 포함)

### Takeaway
지연시간 실측 수치는 이번 세션에서 확보하지 못했다. 구조적 근거만 있다. DeepL은 `latency_optimized` 모델 타입을, Apple은 `preferredStrategy`를 제공하고, Gemini와 Claude는 소형·고속 모델을 따로 두고 있다. 온디바이스 번역은 Android ML Kit(59개 언어, 롱테일 상당수 미지원)와 iOS Translation framework(런타임 조회)가 있다. 오픈 모델로는 NLLB-200-Distilled 600M/1.3B가 있지만 CC-BY-NC 라이선스와 저사양 단말의 메모리 문제가 걸린다.

### Cited Findings
- DeepL API의 `model_type`은 `quality_optimized`, `prefer_quality_optimized`, `latency_optimized` 중에서 고를 수 있다. 응답에 실제 사용된 모델(`model_type_used`)이 표시된다. — [DeepLcom/openapi](https://github.com/DeepLcom/openapi) (2026-11-04 확인)
- Apple Translation framework의 `LanguageAvailability`에는 `init(preferredStrategy:)`와 `status(from:to:)`(언어쌍 설치·준비 여부 확인)가 있다. `TranslationSession`은 문자열을 하나씩 또는 batch로 번역한다. — [Apple Developer: Translation](https://developer.apple.com/documentation/translation), [LanguageAvailability](https://developer.apple.com/documentation/translation/languageavailability) (2026-11-04 확인)
- ML Kit 온디바이스 번역 지원 언어는 59개다(대상 언어 중 ko, vi, ru, id, th, tl, ta, bn, ur, zh, en만 해당). — [google_ml_kit_flutter enum](https://github.com/flutter-ml/google_ml_kit_flutter/blob/master/packages/google_mlkit_translation/lib/src/on_device_translator.dart)
- NLLB-200-Distilled는 600M과 1.3B Dense 체크포인트로 공개되어 있다(CC-BY-NC 4.0). — [fairseq nllb README](https://github.com/facebookresearch/fairseq/blob/nllb/README.md)
- Claude Haiku 5.5는 Anthropic 가격 페이지에 "Fastest, most cost-efficient model"로 소개되어 있다. — [Anthropic pricing](https://www.anthropic.com/pricing)
- Google은 Gemini 3.8 Live API(실시간 스트리밍, 텍스트/오디오 입력) 가격을 별도로 책정한다. 스트리밍 음성 처리 경로가 존재한다는 뜻이다. — [Vertex AI generative AI pricing](https://cloud.google.com/vertex-ai/generative-ai/pricing)

### Inferences
- 메모리 산술(추정): NLLB 600M 파라미터는 fp16 약 1.2GB, int8 약 0.6GB다. 3~4GB RAM급 저가 Android에서 앱 내 상시 로드는 부담이 크고, 언어별로 모델을 나누는 ML Kit 방식보다 무겁다.
- 짧은 채팅 메시지(40자)는 출력 토큰이 수십 개라서 LLM 지연의 대부분이 "첫 토큰까지 시간(TTFT)"과 네트워크 왕복에서 나온다(추정). 스트리밍의 이득은 크지 않다. 대신 (1) 원문을 먼저 즉시 표시하고 번역을 비동기로 채우는 UX, (2) 고속 모델 기본 + 고급 모델 사후 교정 구조가 체감 지연을 줄인다.
- 온디바이스는 지원 언어(섹션 1)가 이주노동자 핵심 언어와 잘 겹치지 않는다. "온디바이스 우선"은 한국어↔베트남어, 태국어, 인도네시아어, 필리핀어, 중국어 같은 대형 그룹에 한정한 최적화로 보는 것이 맞다.
- 음성 메시지는 녹음 종료 후 STT, 번역, (선택) TTS로 이어지는 3단 파이프라인이다. 실시간 통화가 아니라 "보이스 메모" 형태라면 수 초 지연도 허용 가능할 것으로 본다(추정, 사용자 조사 필요).

### Gaps
- Google, Azure, DeepL, Papago API와 Claude, Gemini, GPT 소형 모델의 짧은 메시지 p50/p95 지연 실측치.
- ML Kit 언어 모델 크기(언어당 MB), 저사양 단말(예: 2~4GB RAM)에서의 번역 속도, iOS Translation framework의 실제 지원 언어와 온디바이스 여부.
- Gemma 등 허용적 라이선스 소형 LLM의 롱테일 언어 온디바이스 번역 품질과 속도 자료.

## 6. 실패 모드와 완화책 (안전 지시, 존댓말, 코드스위칭, 짧은 메시지, 고유명사, back-translation)

### Takeaway
API 차원의 완화 도구는 이미 갖춰져 있다. DeepL은 비과금 `context`, 최대 5개 glossary, 최대 10개 `custom_instructions`, `formality`를 제공하고, Google은 무료 glossary 생성과 Adaptive translation, DeepL은 품질평가 beta를 제공한다. 그러나 **back-translation을 사용자에게 신뢰 신호로 보여주는 것의 효과에 대한 연구 원문은 이번 세션에서 확인하지 못했다**. 안전이 중요한 메시지(숫자, 부정, 단위, 날짜)는 엔진 품질과 별개로 규칙 기반 검증 레이어가 필요하다는 것이 이번 조사의 추론이다.

### Cited Findings
- DeepL `context`: 번역에 영향을 주지만 번역되지는 않는 추가 문맥이며 과금하지 않는다. 직전 대화 메시지를 넣는 용도로 적합하다. — [DeepLcom/openapi](https://github.com/DeepLcom/openapi)
- DeepL `glossary_ids`는 번역 요청당 최대 5개 용어집을 적용한다. `custom_instructions`는 최대 10개, 각 300자까지 지정할 수 있다(예: "Use a friendly, diplomatic tone"). translation memory 사용 시에는 custom_instructions와 함께 쓸 수 없다. `formality`와 `style_id`(스타일 규칙)도 있다. — [DeepLcom/openapi](https://github.com/DeepLcom/openapi)
- DeepL은 문서 번역에 대해 품질평가 기능을 **beta**로 제공한다. 세그먼트별 품질 이슈를 오류 유형·심각도와 문자 위치로 반환한다(`enable_quality_evaluation`, `GET /v1/quality-evaluations/{job_id}`). — [DeepLcom/openapi](https://github.com/DeepLcom/openapi)
- Google Cloud Translation은 glossary 생성 같은 요청을 과금하지 않는다. Adaptive translation(예시 기반 맞춤)은 입력·출력 각 $25/100만 자다. — [Cloud Translation pricing](https://cloud.google.com/translate/pricing)
- 건설 현장 등 산업 현장 특화 AI 통번역 앱이 베트남, 캄보디아 노동자와의 소통에 쓰이고 있다. 소음 환경과 현장 은어(예: "나라시") 인식에 초점을 둔다고 보도되었다. — [다음 뉴스: "나라시 좀 잘 해봐" 한 마디에...](https://v.daum.net/v/5P7lNtMVSJ) (검색 요약 기준)
- 고유 문자 체계 언어(Burmese, Khmer, Thai)는 STT fine-tuning 이득도 작다. 음성 경로의 오류가 번역 단계로 그대로 넘어갈 위험이 크다. — [Fine-tuning Whisper Across 81 Languages](https://aclanthology.org/2026.scil-main.37/) (검색 요약 기준)

### Inferences
- **안전 지시(숫자, 부정, 단위, 날짜)**: 원문과 번역문에서 숫자, 단위(m, kg, ℃, 층), 시각, 날짜 토큰을 추출해 일치하는지 검사하고, 부정어("하지 마", "금지", "절대")를 극성 검사한다. 불일치 시 경고 배지와 원문 병기, 상위 모델 재번역을 거는 결정론적 레이어가 엔진 선택보다 효과가 클 것으로 본다(추정). 숫자와 날짜는 번역 전에 placeholder로 치환하고 사후 복원하는 방식도 쓸 수 있다.
- **작업장 용어집**: "나라시", "공구리", "아시바" 같은 일본어 기원 현장어와 약어를 한국어 표준어 + 대상 언어로 매핑한 glossary가 필요하다. DeepL glossary, Google glossary, LLM 프롬프트 주입(캐시로 비용 미미, 섹션 4)으로 적용할 수 있다.
- **짧은 메시지와 맥락 부족**: "네", "됐어요", "그거 갖고 와" 같은 메시지는 직전 3~5개 메시지를 컨텍스트로 넣어야 대명사와 생략 해석이 가능하다(DeepL `context` 비과금, LLM은 입력 토큰 소액).
- **존댓말과 어조**: 한국어 존대 수준(합쇼체/해요체/반말)은 대상 언어로 일대일 대응이 안 된다. 역방향(X→ko)에서는 화자-청자 관계(관리자↔근로자, 교사↔학부모)를 방 설정 메타데이터로 받아 존대 수준을 지정하는 것이 현실적이다(DeepL `formality`, LLM 지시문).
- **코드스위칭**("내일 meeting 3시 OK?"): NMT는 단일 원어를 가정하므로 문장 단위 언어 감지가 흔들릴 수 있다. LLM은 혼합 입력에 상대적으로 강할 가능성이 있다(추정, 근거 미확보).
- **고유명사**: 사람 이름, 현장명, 학교명은 방 단위 "번역 금지 사전"으로 관리한다. 짧은 이름이 일반명사로 오역되는 것을 막는다.
- **신뢰 신호 UI**: (1) 원문 토글, (2) 발신자에게 back-translation 미리보기("상대에게는 이렇게 전달됩니다"), (3) 안전 키워드 검출 시 "확인했어요" 수신 확인 버튼, (4) 저신뢰 언어(D등급)에는 고정 배지를 다는 식의 human-in-the-loop가 가능하다(추정). Back-translation은 오류를 숨길 수 있으므로(정방향과 역방향이 같은 실수를 상쇄) 품질 보증이 아니라 보조 신호로만 써야 한다(추정).

### Gaps
- **Back-translation의 사용자 신뢰 신호 효과에 대한 연구 원문을 이번 세션에서 확인하지 못했다.** 검증이 필요한 후보 문헌(기억 기반, 서지 미검증):
  - Zouhar et al., "Backtranslation Feedback Improves User Confidence in MT, Not Quality" (NAACL 2021). 제목대로 신뢰는 높이지만 품질은 높이지 않는다는 결과로 기억한다.
  - Mehandru et al., "Physician Detection of Clinical Harm in Machine Translation: Quality Estimation Aids in Reliance and Backtranslation Identifies Critical Errors" (EMNLP 2023 Findings).
  - Khoong et al., Google Translate의 응급실 퇴원 안내문 Spanish/Chinese 번역 정확도와 위해 가능성 평가(JAMA Internal Medicine, 2019).
  - WMT Quality Estimation 공유과제의 Critical Error Detection(2021~) 트랙.
- 숫자, 부정, 단위 오역률을 저자원 아시아 언어로 측정한 연구, 한국어 존댓말 보존을 평가한 연구, 한국어-영어 코드스위칭 MT 평가 연구는 이번 검색에서 확인하지 못했다.
- 엔진별 confidence score 제공 여부: Google과 Azure 텍스트 번역 API에 문장 신뢰도 점수가 있는지 확인하지 못했다. 이번 세션에서 확인된 것은 DeepL의 문서용 품질평가 beta뿐이다.

## 7. 프라이버시: 3rd-party 번역 API의 보관·학습 정책과 온디바이스/자체 호스팅 대안

### Takeaway
확인된 1차 정책은 둘이다. Microsoft Translator(No-Trace)는 텍스트·음성을 영구 저장하지 않고 학습에도 쓰지 않는다. Anthropic 상용 약관은 고객 콘텐츠로 모델을 학습하지 않는다고 명시한다. Google, DeepL, Papago, OpenAI의 보관 정책 원문은 확인하지 못했다. 자체 호스팅 대안인 NLLB와 SeamlessM4T는 CC-BY-NC 4.0이어서 상용 서비스에 그대로 쓰기 어렵다.

### Cited Findings
- **Microsoft No-Trace**: Translator(standard와 custom), Speech service, Microsoft Translator Speech API, Office의 텍스트 번역 기능에 제출된 고객 데이터는 영구 저장소에 기록되지 않는다("not written to persistent storage"). 데이터센터에 기록이 남지 않으며, 오디오와 텍스트는 학습에 사용되지 않는다. 페이지는 구 명칭 "Azure Cognitive Services"를 쓰고 있어 최신 개정 여부를 확인할 필요가 있다. — [Microsoft Translator No-Trace](https://www.microsoft.com/en-us/translator/business/notrace/) (2026-11-04 확인)
- **Anthropic 상용 약관**: "Anthropic may not train models on Customer Content from Services." — [Anthropic Commercial Terms](https://www.anthropic.com/legal/commercial-terms) (2026-11-04 확인)
- **Anthropic 보관 옵션**(Claude API 참조 문서, 2026-10-06 캐시, URL 없음): 조직 단위 zero data retention(ZDR) 구성이 있다. 단 Claude Fable 5.1은 30일 보관이 필수다. message threads 기능은 ZDR 대상이 아니다. 번역용 Haiku 계열의 ZDR 적용 조건은 계약 시 확인이 필요하다.
- **오픈 모델 라이선스**: NLLB-200 전 모델은 CC-BY-NC 4.0(코드는 MIT)이다. SeamlessM4T v1/v2와 SeamlessStreaming은 CC-BY-NC 4.0이고, Seamless/SeamlessExpressive는 별도 Seamless License다. — [fairseq nllb README](https://github.com/facebookresearch/fairseq/blob/nllb/README.md), [seamless_communication README](https://github.com/facebookresearch/seamless_communication/blob/main/README.md) (2026-11-04 확인)
- **온디바이스**: Android ML Kit과 iOS Translation framework는 언어 모델을 단말에 내려받아 번역하는 구조다(언어쌍 "설치" 상태 확인 API 존재). — [Apple LanguageAvailability](https://developer.apple.com/documentation/translation/languageavailability), [ML Kit translation](https://developers.google.com/ml-kit/language/translation) (Apple은 2026-11-04 확인, ML Kit은 검색 요약 기준)

### Inferences
- 가족방과 학교 공지에는 아동과 가족의 개인정보가, 작업장 방에는 산재·근태 정보가 섞인다. 기본 엔진은 "학습 미사용 + 무보관(또는 단기 보관)"을 계약으로 보장하는 곳으로 고르고, 앱 개인정보 처리방침에 국외 이전(번역 API 리전)을 명시해야 한다(추정. 한국 개인정보보호법상 국외 이전 요건은 별도 규제 노트에서 확인 필요).
- 온디바이스로 처리할 수 있는 언어쌍(ko↔vi/th/id/tl/ru/zh/en 등)은 프라이버시 민감 방(가족, 학교)에서 기본 경로로 쓰고, 롱테일 언어만 서버로 보내는 "프라이버시 등급별 라우팅"이 가능하다(추정).
- 자체 호스팅은 NLLB와 Seamless의 비상업 라이선스 때문에 상용 앱의 기본 경로로 쓰기 어렵다. 허용적 라이선스 LLM(예: Gemma, Qwen 계열)의 저자원 언어 품질을 별도로 검증해야 한다(라이선스 조건 자체도 이 세션에서 미확인).

### Gaps
- Google Cloud Translation 데이터 사용 정책(docs.cloud.google.com/translate/data-usage), Vertex AI/Gemini 데이터 거버넌스, DeepL API Pro의 보관·삭제·학습 정책, Papago API(NCP)의 로그 보관 정책, OpenAI API 보관 기간·학습 정책, Amazon Translate 데이터 사용(opt-out) 정책 원문을 확인하지 못했다(호스트 차단과 검색 한도 소진).
- Gemma와 Qwen 모델의 상용 라이선스 조건, 롱테일 언어 성능.
- 번역 API 사용이 한국 개인정보보호법상 "처리위탁"인지 "국외 이전"인지에 대한 해석(규제 노트와 교차 확인 필요).
