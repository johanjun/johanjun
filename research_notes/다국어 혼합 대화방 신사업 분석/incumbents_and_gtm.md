# 인컴번트 추격 리스크 및 이주민·다국어 커뮤니티 GTM·비즈니스모델 벤치마크 (기준일: 2026-11-04)

> 조사 방법 메모: 이번 세션에서는 WebFetch가 시도한 모든 외부 도메인(apple.com, wabetainfo.com, 9to5mac.com, kakaocorp.com, bloter.net, en.wikipedia.org, namu.wiki)에서 DNS 단계에서 차단되어 원문을 열람하지 못했다. 아래 인용은 모두 WebSearch(extended) 결과의 요약과 스니펫에 근거하며, 링크는 해당 검색 결과가 가리킨 원문 URL이다. 조사 후반에는 세션 공유 웹검색 할당량(200회)이 소진되어, Kakao 2026 로드맵 세부, Galaxy S26/One UI 8.5 Chat Assist 언어 목록, Google I/O 2026, LINE 2026 신기능, Snapchat→Instagram Stories 사례는 추가 검증을 하지 못했다(해당 항목은 각 Gaps에 기재). 상태 표기는 [발표]=공식 발표, [출시]=일반 배포 확인, [베타]=베타/TestFlight, [루머/미확인]=2차 출처만 있음.

---

## A1. 인컴번트별 2025–2026 메시지 번역 발표·출시 현황과 추가된 장꼬리 언어

### Takeaway
"그룹 안에서 각자 자기 언어로 받는" 경험은 WhatsApp(Android 한정, 자동번역)과 Telegram(Premium 한정)이 이미 제공하고 있다. 다만 2026-11 기준으로 한국어가 들어간 Android 자동번역, 그리고 네팔어·크메르어·미얀마어·우즈베크어·몽골어·싱할라어·벵골어를 지원하는 소비자 메신저는 확인되지 않았다. 한국 시장에서 가장 직접적인 위협인 카카오는 2026-11까지 "받은 메시지 자동번역"이나 그룹 단위 번역을 발표하지 않았다(발표가 있었다는 근거를 찾지 못함).

### Cited Findings

**카카오 (KakaoTalk / Kanana / Kakao i 번역)**
- [출시] 2024-12-19: KakaoTalk 11.3.0 업데이트로 '실험실'에 있던 번역·맞춤법 기능이 정식 기능이 됨. 19개 언어를 지원하며 외국어 문장을 한국어로 옮기는 것도 가능해졌다는 보도 — [대화방 자동번역 해볼까…카카오톡, 번역·맞춤법 기능 업데이트 (다음/뉴스)](https://v.daum.net/v/20241219143320903); [카카오톡, 맞춤법·19개 언어 번역 기능 정식 출시했다 (경제일보)](https://m.kyungjeilbo.com/amp/20241219125244891)
- 사용 방식: 텍스트를 입력한 뒤 '번역' 아이콘을 누르면 한국어·영어·중국어·인도네시아어 등 19개 언어로 번역됨. 즉 입력(발신) 단계의 번역이며, 받은 메시지의 자동번역은 아님 — [카카오톡, 맞춤법 교정·자동 번역 기능 추가 (한국아이닷컴)](https://www.hankooki.com/news/articleView.html?idxno=217738); 인도네시아어 포함 — [카카오톡서 19개 언어 번역된다…인도네시아어 포함 (인니투데이)](https://inni-today.com/korea-company/2024-kor-biz-194/)
- [출시·실험실] 2023-02-02: iOS 실험실 기능으로 '말풍선 번역'(받은 외국어 말풍선을 번역)이 먼저 나왔고, 당시에는 한국어→외국어 번역을 지원하지 않았음. 엔진은 카카오엔터프라이즈의 '카카오 i 번역' — [언어장벽 허무는 카카오톡…19개 외국어 번역해준다 (뉴시스)](https://newsis.com/view/?id=NISX20230202_0002178991)
  - 주의: 의뢰서 배경의 "KakaoTalk은 발신 메시지만 번역"과 일부 다를 수 있다. 수동 말풍선 번역(외국어→한국어)이 2023년 iOS 실험실에 있었기 때문이다. 현재 정식판에 남아 있는지는 확인하지 못했다.
- 카카오 뉴스룸에 「카카오 번역 서비스 개편...19개 언어 번역 가능해져」라는 페이지(detail/8689)가 있다 — [kakaocorp.com](https://www.kakaocorp.com/page/detail/8689?lang=ENG). 원문 날짜는 열람하지 못했다. 페이지 ID(8689)가 if(kakao)25 보도자료(11684·11713, 2025-09)보다 작아서 2025-09 이전 글일 가능성이 있으며, 배경 정보의 "2026년 6월 개편"과 날짜가 맞는지 검증이 필요하다.
- [발표] if(kakao)25 (2025-09-23~25, 용인 카카오 AI 캠퍼스): "15년 만의 최대 개편"을 발표하고 KakaoTalk을 AI 기반 '일상 플랫폼'으로 재정의함. 온디바이스 모델 'Kanana Nano' 기반의 'Kanana in KakaoTalk'(대화 요약, 통화 녹음, 기존 #검색을 대체하는 'Kanana Search')를 2025-10 중순부터 테스트한다고 밝힘. 검색 결과로 확인한 발표 내용에는 번역 기능 언급이 없었음 — [카카오톡과 AI의 결합…카카오, 'if(kakao)25'에서 '일상 AI' 비전 공개](https://www.kakaocorp.com/page/detail/11713?lang=ENG); [KakaoTalk and AI Combined (Kakao)](https://www.kakaocorp.com/page/detail/11725?lang=ENG); [[이프카카오 2025] 카카오톡, '카나나' 입는다 (딜사이트)](https://dealsite.co.kr/articles/148700); [[Q&AI] if 카카오 25 발표 내용 총정리 (AI매터스)](https://aimatters.co.kr/news-report/ai-news/31870/)
- 프라이버시를 이유로 온디바이스 방식을 택했다고 카카오가 밝힘 — [Kakao 보도자료](https://www.kakaocorp.com/page/detail/11725?lang=ENG)
- [발표, 2024-10-22] 카카오가 AI 메신저 'Kanana'를 2025년 상반기에 출시하겠다고 발표 — [Kakao to launch AI messenger service Kanana in H1 2025 (KED Global)](https://www.kedglobal.com/artificial-intelligence/newsView/ked202410220015)
- 현장에서 쓰이는 우회 수단: 갤럭시 사용자는 Galaxy AI의 '대화 번역'(입력창 아래 AI 버튼)으로 KakaoTalk 대화를 번역함. 2026-10 하순 Samsung Members 커뮤니티에 "카카오 자동번역이 업데이트 후 다시 된다"는 글이 올라옴. 원인이 삼성 쪽인지 카카오 쪽인지는 불명확하며, OS 오버레이 방식이 불안정하다는 정황으로 볼 수 있음 — [Samsung Members 커뮤니티](https://r1.community.samsung.com/t5/%EA%B0%A4%EB%9F%AD%EC%8B%9C-s/%EC%B9%B4%EC%B9%B4%EC%98%A4-%EC%9E%90%EB%8F%99%EB%B2%88%EC%97%AD%EC%9D%B4-%EC%9D%B4%EC%A0%9C-%EB%93%9C%EB%94%94%EC%96%B4-%EB%8B%A4%EC%8B%9C-%EB%90%A9%EB%8B%88%EB%8B%A4/m-p/40094734)
- 국제결혼 중개업체가 고객에게 "카카오톡 자동번역 기능 설정 방법"을 안내함. 다문화 부부가 단말기 수준의 번역에 의존한다는 신호 — [국제결혼 진행 시 카카오톡 자동번역 기능설정 방법 (봄 실장 게시판)](http://wtcim.com/35/?bmode=view&idx=167295785)

**네이버 (Band / Papago / NAVER WORKS / LINE·LY Corp)**
- Naver Band: 게시글·채팅에 번역 기능이 내장되어 있다는 근거를 찾지 못함. App Store 설명의 채팅 기능 항목에도 번역 언급이 없음 — [BAND - App for all groups (App Store)](https://apps.apple.com/us/app/band-app-for-all-groups/id542613198)
- NAVER WORKS(기업용)는 여러 언어가 섞인 대화방에서 모든 메시지를 사용자가 설정한 언어로 자동번역하는 기능이 있음 — [메시지 번역 및 통역 - 네이버웍스](https://help.worksmobile.com/en/use-guides/message/check-message/translation/). 게시글 번역은 NAVER WORKS Core 또는 WORKS Approval을 신청해야 사용할 수 있음(유료 기업 티어에 묶임) — [Translate posts - NAVER WORKS](https://help.worksmobile.com/en/use-guides/board/check-post/translate-post/)
- Papago: 2024-02-01 아랍어를 추가해 총 16개 언어 — [파파고, 아랍어도 번역한다…지원 언어 16개로 확대 (뉴시스)](https://www.newsis.com/view/NISX20240201_0002612973). 이보다 앞서 베트남어·태국어·인도네시아어 등 4개 언어를 추가함 — [네이버 파파고, 베트남·태국 등 4개 언어 추가 (아이뉴스24)](https://www.inews24.com/view/1047588). 2026-10의 신규 기능은 외국인 여행자용 장소 추천 등이며, 언어 추가는 확인되지 않음 — [파파고, AI 여행 서비스 확대 (YTN, 2026-10-19)](https://www.ytn.co.kr/_ln/0102_202610191324463540)
- LINE: 대화방 메뉴 '≡' > '通訳' > '通訳機能の使用'을 켜는 대화방 단위 통역 기능이 안내되고 있음(2023년 글) — [LINEで翻訳する方法とは？ (linestep)](https://linestep.jp/2023/01/11/line-translation/). LY Corp는 대화방 안에서 AI 에이전트가 대화를 돕는 'Agent i in chat'을 발표함(날짜는 원문 미확인) — [LINEヤフー、「LINE」新機能「Agent i in chat」発表 (AIsmiley)](https://aismiley.co.jp/ai_news/line-yahoo-agent-in-chat/). 'LINE AIアシスタント'는 이미지 번역 등을 지원함 — [LINEヤフー プレスリリース](https://www.lycorp.co.jp/ja/news/release/007735/). 구 'LINE AIアシスタント'가 종료됐다는 2026-08 글도 있어 출처 간에 엇갈림 — [LINE AI機能の使い方完全ガイド (2026年8月)](https://genai-ai.co.jp/ai-kanri/blog/cc-line-ai-guide/)

**Meta (WhatsApp / Instagram / Messenger)**
- [출시] 2025-09-23: WhatsApp 'Message Translations' 출시. Android는 6개 언어(영어·스페인어·힌디어·포르투갈어·러시아어·아랍어), iPhone은 19개 이상. 1:1·그룹·채널 업데이트에서 작동함. 대화 전체 자동번역은 Android에만 있으며, 번역은 기기 안에서 처리되어 WhatsApp이 내용을 볼 수 없음 — [Introducing Message Translations (WhatsApp Blog)](https://blog.whatsapp.com/introducing-message-translations); [About Meta](https://about.fb.com/news/2025/09/introducing-message-translations-whatsapp/); [9to5Google](https://9to5google.com/2025/09/23/whatsapp-message-translations-auto-translation-support-exclusive-to-android/)
- iPhone 지원 언어에는 한국어, 베트남어, 일본어, 우크라이나어 등이 포함됨(Apple Translate 앱 지원 언어와 같음) — [Engadget](https://www.engadget.com/apps/whatsapp-starts-rolling-out-message-translations-on-ios-and-android-150132823.html)
- [베타] 2026-03: Android 베타에 13개 언어 팩 추가. 체코어·독일어·프랑스어·인도네시아어·이탈리아어·라트비아어·네덜란드어·폴란드어·스웨덴어·터키어·우크라이나어·우르두어·중국어 간체 — [WhatsApp beta for Android adds 13 language packs (WABetaInfo)](https://wabetainfo.com/whatsapp-beta-for-android-adds-13-language-packs-for-message-translations/); [Shmooz AI](https://shmooz.ai/blogs/whatsapp-translation-language-packs). 이 목록에는 한국어·베트남어·태국어와 장꼬리 언어가 없음.
- [베타] 2026-03-20: iPhone용 대화방 단위 'Translate messages'(자동번역) 토글이 TestFlight에서 발견됨. Apple Translate 지원 언어(21개)에 연동됨 — [9to5Mac](https://9to5mac.com/2026/03/20/whatsapp-for-iphone-may-soon-offer-automatic-message-translation-across-21-languages/)
- 2026 하반기 가이드에 따르면 대화 전체 자동번역은 여전히 Android 전용이고, iPhone은 메시지 단위 번역만 가능함 — [How to translate WhatsApp messages (2026) (Intermind)](https://intermind.com/blog/whatsapp-translate)
- [출시] 2025년 초: Instagram DM에서 메시지 스트림 안 번역을 시작함. Meta 번역 시스템 기반으로 99개 언어 — [Instagram Adds New DM Features (Social Media Today)](https://www.socialmediatoday.com/news/instagram-dm-updates-scheduled-messages-translations/740301/)
- 2026-04 Meta AI의 기반 모델이 'Muse Spark'로 교체되었다는 2차 가이드가 있음. Meta AI가 DM 메시지를 번역한다는 근거는 찾지 못함 — [Meta AI on Instagram (inro)](https://www.inro.social/blog/meta-ai-instagram-guide)

**Telegram**
- [출시] 무료 사용자는 메시지를 하나씩 번역할 수 있고, Premium은 대화방·채널 전체를 실시간 번역함. Premium 출시 전부터 있던 기능은 무료로 유지됨 — [Telegram Premium FAQ](https://telegram.org/faq_premium)
- Premium 사용자의 AI Editor(재작성·번역) 일일 한도가 무료보다 50배 높다는 2026 가이드 — [TG Superstars](https://tgsuperstars.com/en/blog/telegram-premium-features/)

**Apple**
- [출시] iOS 26(2025-09)의 Messages Live Translation은 9개 언어(영어·중국어 간체·프랑스어·독일어·이탈리아어·일본어·한국어·브라질 포르투갈어·스페인어) — [MultiLingual](https://multilingual.com/apple-live-ai-translation-ios-26/); [iDownloadBlog](https://www.idownloadblog.com/2025/07/08/live-translation-messages-app/)
- Apple 지원 문서의 Messages Live Translation 언어 목록: 영어, 덴마크어, 네덜란드어, 프랑스어, 독일어, 이탈리아어, 노르웨이어, 포르투갈어, 스페인어, 스웨덴어, 터키어, 중국어(간체·번체), 일본어, 한국어, 베트남어 — [Translate messages, calls, and conversations on iPhone (Apple Support)](https://support.apple.com/en-md/guide/iphone/iph22b72984d/ios). iOS 27 기능 가용성 페이지에서도 Messages Live Translation 항목에 베트남어가 표시됨 — [iOS and iPadOS 27 - Feature Availability (Apple)](https://www.apple.com/ios/feature-availability/)
- [발표] WWDC 2026 → iOS 27: Apple Translate 앱이 21개에서 30개 언어·억양으로 늘어남(+9: 히브리어, 덴마크어, 스웨덴어 등). 베트남어와 태국어는 신규 추가 목록에 없음 — [iOS 27 adds nine new languages and accents to Apple Translate (9to5Mac, 2026-07-08)](https://9to5mac.com/2026/07/08/ios-27-adds-nine-new-languages-and-accents-to-apple-translate/); [Cult of Mac](https://www.cultofmac.com/news/apple-translate-ios-27-9-new-language-support)
- [루머/미확인] "iOS 27 Live Translate 38개 언어"라는 주장이 있으나 신뢰도가 낮고 Apple 공식 목록과 충돌함 — [Hawkdive](https://www.hawkdive.com/ios-27-live-translate-iphone-guide/)

**Google**
- [출시] Pixel의 Live Translate는 Google Messages 등 메시징 앱에서 원문 아래에 번역을 표시함. 지원 언어는 "20개 이상"(Google 블로그), "23개"(Google Store), "21개"(Pixel 10 관련 기사)로 출처마다 다름 — [3 ways you can use Pixel for translation help this Lunar Year (Google Blog, 2026)](https://blog.google/products-and-platforms/devices/pixel/lunar-new-year-2026-translation-tools/); [Pixel Live Translate (Google Store)](https://store.google.com/in/magazine/pixel-live-translate?hl=en-IN); [Lowyat.NET (2025)](https://www.lowyat.net/2025/363390/live-translate-features-google-pixel-10-series/)
- 오프라인 Live Translate는 Pixel 9·10·11에서 11개 언어(항상 영어와 짝) — [Android Police](https://www.androidpolice.com/google-translate-offline-live-translate-release/)
- [출시] 2026-06-09: Gemini 3.5 Live Translate 공개. 70개 이상 언어의 실시간에 가까운 음성→음성 번역을 Google Translate 앱(Android·iOS)에 배포하며, Google Messages 언급은 없음 — [Fluid, natural voice translation with Gemini 3.5 Live Translate (Google Blog)](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-live-3-5-translate/)
- Gemini in Google Messages는 RCS가 켜져 있어야 하는 어시스턴트 대화이며, Gemini와의 대화는 종단간 암호화되지 않음. RCS 그룹 자동번역에 대한 발표는 찾지 못함 — [Use Gemini in Google Messages (Google Support)](https://support.google.com/messages/answer/14599070?hl=en)
- [출시] 2026-03-26: Google Translate의 헤드폰 실시간 번역이 iOS에 출시됨 — [9to5Mac](https://9to5mac.com/2026/03/26/google-translates-live-headphone-translation-feature-lands-on-ios/)

**Samsung (Galaxy AI)**
- 필리핀어(Filipino)와 구자라트어가 추가되어 총 22개(날짜는 2026 이전으로 추정) — [SamMobile](https://www.sammobile.com/news/samsung-galaxy-ai-adds-support-for-2-new-languages-for-a-total-of-22/); [SamMobile (Gujarati/Filipino)](https://www.sammobile.com/news/samsung-galaxy-ai-gujarati-filipino-languages-download/)
- [출시 진행 중] 2026-10: 헝가리어·말레이어가 추가되어 Call Assist·Note Assist·Interpreter·Transcript Assist가 24개 언어가 됨. 2026-10-14 호주부터 단계적으로 배포. Bixby에는 폴란드어·태국어·베트남어가 추가됨 — [PhoneArena](https://www.phonearena.com/news/galaxy-ai-features-language-boost_id184052); [NPowerUser](https://nokiapoweruser.com/samsung-is-expanding-galaxy-ai-and-bixby-to-more-languages-globally/); [Techzei](https://techzei.com/galaxy-ai-bixby-new-languages/); [Samsung Members](https://r2.community.samsung.com/t5/Galaxy-S/New-Galaxy-AI-Language-Support/m-p/23084739)

**B2B 특화 경쟁자 (인컴번트 외, 같은 공간)**
- [출시] 2026-09-16: 플리토·한화오션·한화시스템이 조선 현장용 AI 통번역 '오톡(OTalk)'을 구축함. 7개 언어, 1:1·그룹 채팅, 문서·이미지 번역, 교육 실시간 번역 등 10여 개 기능과 작업장 소음을 고려한 5단계 수음 조정을 갖춤. 현장 은어('땡크')와 사투리 대응이 목적 — [플리토, 한화오션 통번역 AI 구축 (MTN)](https://news.mtn.co.kr/news-detail/2026091610011317518); [조선소의 '땡크'도 알아듣는다 (벤처스퀘어)](https://www.venturesquare.net/1114035); [테크월드](https://www.epnc.co.kr/news/articleView.html?idxno=407017)
- [출시] 2026-11-04: 제네시스네스트의 엔터프라이즈 채팅 솔루션 '챗플래닛'이 15개 언어 실시간 자동번역을 탑재함 — [글로벌이코노믹](https://g-enews.com/article/ICT/2026/11/202611041403293564638475ab2b_1)

### Inferences
- 제품 개념 자체(수신자별 자동번역)는 이미 인컴번트가 출시한 상태다(WhatsApp Android 자동번역은 수신 기기에서 각자의 언어로 번역하고, Telegram Premium은 대화방 전체를 번역함). 차별점은 '아이디어'가 아니라 다음 세 가지 공백에 있다. ① 한국어+장꼬리 언어 조합, ② 안드로이드와 iOS 양쪽에서 같은 경험, ③ 한국에서 실제로 쓰이는 네트워크(KakaoTalk) 위의 대화방.
- 인용된 목록(WhatsApp Android 6+13, Apple Messages 16, Apple Translate 30, Galaxy 24, Papago 16, Kakao 19)을 맞춰 보면, 타깃 장꼬리 언어 중 대형 플랫폼이 다루는 언어는 베트남어(Apple·Kakao·Papago), 인도네시아어(Kakao·Papago·WhatsApp 베타), 태국어(Papago 및 일부 Galaxy 기능), 필리핀어(Galaxy) 정도다. 네팔어·크메르어·미얀마어·우즈베크어·몽골어·싱할라어·벵골어를 메신저 번역에 넣었다는 발표는 이번 조사에서 하나도 확인되지 않았다(Galaxy AI 전체 목록은 원문을 확인하지 못해 단정하지 않음).
- 가장 위험한 단일 변수는 카카오다. 19개 언어 엔진, 수신 말풍선 번역 실험 이력(2023), 온디바이스 Kanana가 이미 있어서 '받은 메시지 자동번역'과 '그룹방 단위 자동번역'을 켜는 것은 기술적으로 작은 확장이다. 하지만 2026-11 기준 발표된 바는 없다.
- Meta는 Instagram DM에서 99개 언어를 이미 운영하고 있다. 장꼬리 언어 기술 역량은 있다는 뜻이며, WhatsApp에서 이것을 막는 것은 기술보다 E2EE와 온디바이스 처리라는 설계 제약으로 보인다(WhatsApp은 기기 내 번역을 강조함).

### Gaps
- Kakao i 번역 "2026년 6월 개편"과 "ChatGPT 카카오톡 탑재(2025-10)"는 이번 세션에서 직접 확인하지 못했다(카카오 뉴스룸 접속 차단, 검색 할당량 소진). 해당 19개 언어의 전체 목록(장꼬리 언어 포함 여부)도 미확인이다.
- Naver Band에 번역 기능이 없다는 것은 "찾지 못함" 수준이며, 공식 고객센터로 확인하지 못했다.
- Galaxy AI의 Chat Assist(채팅 번역)가 서드파티 앱에서 지원하는 언어 목록과 One UI 8.5/9의 변경 사항, Galaxy Unpacked 2026 발표는 확인하지 못했다.
- Google I/O 2026과 Android 17의 시스템 수준 메시지 번역 발표, LINE의 2025–2026 번역 신기능 날짜, Messenger 번역은 확인하지 못했다.
- iOS 26/27 Messages Live Translation이 그룹 대화에서 작동하는지, 그리고 iOS 26.x 중 언어가 추가된 정확한 날짜는 미확인이다.

---

## A2. 인컴번트가 니치 메신저·소셜 스타트업 기능을 모방한 속도와 그 스타트업의 결과

### Takeaway
확인된 사례(Clubhouse)에서는 대형 플랫폼이 핵심 기능을 수개월 안에 복제했고, 원조 스타트업은 정점 후 1~2년 사이에 핵심 형식을 포기했다. 다만 번역 기능은 인컴번트가 한꺼번에가 아니라 언어별로 점진 확장한다. 카카오는 실험실에서 정식 출시까지 약 22개월, WhatsApp은 출시 6개월 뒤에도 iPhone 자동번역이 베타였다. 따라서 '기능 복제'는 빠르고 '장꼬리 언어 확장'은 느리다는 비대칭이 있다.

### Cited Findings
- Clubhouse: Twitter는 Clubhouse가 대중화되기 전인 2020-11에 Spaces를 시작해 2021년 내내 확장함. Facebook·Twitter·LinkedIn·Telegram이 수개월 안에 핵심 기능을 복제했다는 분석 — [Clubhouse's death is Twitter's gain (IESE)](https://blog.iese.edu/the-media-industry/2021/07/05/clubhouses-death-is-twitters-gain/); [Clubhouse After the Boom (Think Insights)](https://thinkinsights.net/strategy/clubhouse-after-boom)
- Clubhouse의 사용자 감소 규모는 출처마다 다름. "2021-03 1,000만에서 2021-09 350만"(Medium, 저신뢰)과 "2021-06 정점 이후 6개월 만에 80% 감소"가 대립함 — [Medium](https://medium.com/@achu_83391/what-happened-to-clubhouse-a-data-driven-analysis-of-social-medias-fastest-rise-and-fall-7c1ee1386ec9); [DimeADozen (저신뢰)](https://www.dimeadozen.ai/sample-report/clubhouse)
- 2023-04 Clubhouse는 직원 절반 이상을 감원하고 라이브룸 형식을 버린 뒤 메시징형 소규모 제품으로 전환함. 2026년에도 작은 팀으로 운영 중 — [Think Insights](https://thinkinsights.net/strategy/clubhouse-after-boom); [Clubhouse (app) - Wikipedia](https://en.wikipedia.org/wiki/Clubhouse_(app))
- 복제품 일부도 접힘: Spotify Greenroom(2021-04 출시, 2022-08 종료), Reddit Talk(2021-08 출시 후 종료). 이 날짜는 저신뢰 출처에서 나온 것으로, 다른 출처의 Spaces 출시일과 충돌함 — [DimeADozen](https://www.dimeadozen.ai/sample-report/clubhouse)
- BeReal: 주간 다운로드가 2022-10 정점 이후 2022-12 중순까지 50% 이상 줄어 140만이 됨. Clubhouse가 1년 앞서 거의 같은 궤적을 밟았다는 분석 — [Is BeReal Going to Be Gone Like Clubhouse? (Appfigures)](https://appfigures.com/resources/insights/20221216/amp?f=2)
- 번역 기능의 점진 확장 속도(인컴번트 내부 비교):
  - 카카오: iOS 실험실 말풍선 번역 2023-02 → 정식 19개 언어 2024-12(약 22개월) — [뉴시스](https://newsis.com/view/?id=NISX20230202_0002178991); [경제일보](https://m.kyungjeilbo.com/amp/20241219125244891)
  - WhatsApp: 2025-09 Android 6개 언어 → 2026-03 베타 13개 추가(6개월), iPhone 자동번역은 2026-03 TestFlight → 2026 하반기에도 Android 전용 상태 — [WhatsApp Blog](https://blog.whatsapp.com/introducing-message-translations); [WABetaInfo](https://wabetainfo.com/whatsapp-beta-for-android-adds-13-language-packs-for-message-translations/); [Intermind](https://intermind.com/blog/whatsapp-translate)
  - Apple: iOS 26 Messages 9개 언어(2025-09) → 지원 문서 16개(베트남어 포함) → iOS 27 Translate 앱 +9개(장꼬리 언어 없음) — [MultiLingual](https://multilingual.com/apple-live-ai-translation-ios-26/); [Apple Support](https://support.apple.com/en-md/guide/iphone/iph22b72984d/ios); [9to5Mac](https://9to5mac.com/2026/07/08/ios-27-adds-nine-new-languages-and-accents-to-apple-translate/)
  - Samsung: 22 → 24개 언어(2026-10, 헝가리어·말레이어) — [PhoneArena](https://www.phonearena.com/news/galaxy-ai-features-language-boost_id184052)
- 번역 메신저 스타트업이 서비스를 종료했다는 기사·공지는 검색으로 찾지 못함. 파파고 API 기반 실시간 번역 채팅 '푸파고'(부스트캠프 2020 프로젝트)와 키보드형 번역기 앱 정도만 확인됨 — [boostcamp-2020 Pupago (GitHub)](https://github.com/boostcamp-2020/Project02-A-RealTime-Translation-Messenger); [키보드 번역기 (App Store)](https://apps.apple.com/kr/app/%ED%82%A4%EB%B3%B4%EB%93%9C-%EB%B2%88%EC%97%AD%EA%B8%B0-%EC%B1%84%ED%8C%85-%EB%A9%94%EC%8B%9C%EC%A7%80-%EC%8B%A4%EC%8B%9C%EA%B0%84-%EB%B2%88%EC%97%AD-%EC%95%B1/id1502909594)

### Inferences
- 소셜 '형식'(오디오룸, 스토리 등)은 3~9개월 안에 복제되었고, 원조 앱이 무너진 핵심 원인은 네트워크(사용자가 이미 있는 곳)였다. 번역 메신저도 같은 논리라면, "누구나 쓰는 범용 다국어 단톡방" 포지션은 카카오·WhatsApp이 자동번역을 켜는 순간 가치가 크게 줄어든다.
- 반면 인컴번트의 번역 언어 확장 속도는 연 2~13개 수준이며, 늘 사용자 수가 많은 언어부터 추가되었다. 이 관찰을 연장하면, 타깃 장꼬리 언어 7개(네팔어·크메르어·미얀마어·우즈베크어·몽골어·싱할라어·벵골어)는 앞으로 1~2년 동안 대형 플랫폼 메신저 번역의 우선순위 밖에 남을 가능성이 높다(추정).
- 번역 스타트업의 '사망 사례'가 검색되지 않는 것은 시장 검증이 부족하다는 뜻일 수도 있다. 이 분야가 독립 소비자 앱으로 크게 성장한 사례가 거의 없고, B2B로 수렴했을 가능성이 있다(플리토 오톡, NAVER WORKS, 챗플래닛 등 기업형 사례만 확인됨).

### Gaps
- Snapchat Stories(2013)→Instagram Stories(2016), Houseparty→Messenger Rooms(2020)/Houseparty 종료(2021), Periscope→Facebook Live 등 고전 사례는 검색 할당량 소진으로 이번 세션에서 출처를 확보하지 못했다(보고서에 쓰려면 별도 검증 필요).
- 카카오가 국내 스타트업 기능을 복제한 구체적 사례와 당시 일정은 찾지 못했다.
- 번역 채팅 전용 스타트업(해외 포함)의 흥망 사례는 찾지 못했다.

---

## A3. 인컴번트가 쉽게 모방하기 어려운 요소

### Takeaway
모방이 어려운 순서는 대략 다음과 같다. ① 현장 도메인 용어집과 B2B 워크플로(안전 공지 확인, 사번·국적 연동, 협력사 배포), ② 이주민 커뮤니티의 신뢰와 오프라인 접점, ③ 장꼬리 언어 품질(LLM 발전으로 점차 약해짐). '혼합 언어 방 UX' 자체는 복제가 쉽다.

### Cited Findings
- 장꼬리 언어 품질: GPT-4 등 LLM의 저자원 언어 제로샷 번역은 상용 시스템에 뒤처지고, 204개 언어를 평가한 연구에서 ChatGPT가 대부분의 언어에서 전통적 MT보다 낮았다는 선행 연구가 인용됨 — [Nsanku (arXiv 2605.04208)](https://arxiv.org/pdf/2605.04208)
- 네팔어 등은 토크나이저가 단어 수보다 훨씬 많은 토큰으로 쪼개므로 비용과 품질 모두에 불리함 — [LoResLM 2025 (ACL Anthology)](https://aclanthology.org/2025.loreslm-1.33.pdf). 저자원 언어쌍에서는 신경망 MT 성능이 낮고 전문 번역의 품질 보증도 부족함(네팔어·싱할라어 FLoRes) — [FLoRes (arXiv 1902.01382)](https://arxiv.org/pdf/1902.01382)
- 미얀마어·크메르어: LLM에 검색 기반 few-shot을 적용한 방법이 일부 방향에서는 NLLB보다 낫고 일부에서는 그렇지 않음. 결과가 언어와 방향에 따라 갈림 — [Compositional Translation (EMNLP 2025 Findings)](https://aclanthology.org/2025.findings-emnlp.1216.pdf). 모델 순위가 언어마다 바뀌고 신경망 지표가 무너질 수 있어 chrF++와 사람 평가를 함께 쓰라는 권고 — [Hausa/Fongbe 평가 (arXiv 2606.22269)](https://arxiv.org/pdf/2606.22269)
- 도메인 용어집과 현장 적합성: 오톡은 조선소 은어와 억양이 센 사투리 때문에 생기는 소통 위험을 줄이는 것이 주 목적이며, 소음 환경을 위한 5단계 수음 조정도 넣음 — [벤처스퀘어](https://www.venturesquare.net/1114035); [아이티데일리](https://www.itdaily.kr/news/articleView.html?idxno=241658)
- 채택 효과(플리토 발표 수치): 한 대형 조선소 직영 외국인 근로자의 활성 사용자 비율이 도입 초기 약 20%에서 3개월 만에 약 96%로 올랐다는 주장 — [외국인 근로자 111만명…조선소 파고든 AI 통역 (네이트/이데일리)](https://m.news.nate.com/view/20260911n21717)
- B2B 관리 기능: 오톡은 협력사의 요청에 따라 사번 연동 작업을 거쳐 협력사 근로자에게 확대 배포됨 — [MTN](https://news.mtn.co.kr/news-detail/2026091610011317518). DL이앤씨 어깨동무M은 근로자의 국적 정보로 공지 언어를 자동 선택하고(중국·베트남·카자흐스탄·캄보디아 등), TBM(작업 전 안전점검)과 안전사고 사례 알림으로 확대할 계획 — [이투데이 (2024-12-10)](https://www.etoday.co.kr/news/view/2427855); [뉴스1](https://www.news1.kr/realestate/general/5626533)
- 기존 업무의 병목: 그동안 관리자가 새 공지를 언어별로 직접 번역해 전달해야 했음 — [한국경제](https://www.hankyung.com/article/2024121061646)
- 커뮤니티 신뢰와 오프라인 접점(송금업 사례): GME는 외국인 밀집 지역에 오프라인 지점을 두고 다국적 직원을 배치함 — [뉴스코리아](https://www.newskorea.ne.kr/news/articleView.html?idxno=21479). 한패스는 신규 가입의 약 60%가 친구 추천 등 자연 유입 — [블로터](https://www.bloter.net/news/articleView.html?idxno=656498)
- 프라이버시와 구조 제약: WhatsApp 번역은 기기에서 처리되어 회사가 볼 수 없음 — [WhatsApp Blog](https://blog.whatsapp.com/introducing-message-translations). 카카오는 프라이버시를 이유로 온디바이스 Kanana Nano를 택함 — [Kakao](https://www.kakaocorp.com/page/detail/11725?lang=ENG). Gemini in Messages 대화는 E2EE가 아님 — [Google Support](https://support.google.com/messages/answer/14599070?hl=en)

### Inferences
- 장꼬리 언어 품질: 인컴번트가 기기 안에서 처리하는 구조를 택했다는 것은 언어마다 기기용 모델·언어팩을 따로 내려받아야 한다는 뜻이다. 이 때문에 사용자가 적은 언어는 뒤로 밀리기 쉽다. 서버 측 LLM과 언어별 사후 교정(용어집, 사람 검수 데이터)을 쓰는 스타트업은 이 영역에서 12~24개월 정도 품질 우위를 가질 수 있다(추정). 다만 LLM 범용 성능이 오르면서 이 우위는 시간이 갈수록 줄어드는 해자다.
- 혼합 언어 방 UX(원문·번역 토글, 멤버별 언어, 음성·이미지 번역): 인컴번트가 마음먹으면 1~2 릴리스 주기 안에 복제할 수 있다. 해자로 보기 어렵다.
- 안전 공지 '이해 확인'(읽음이 아니라 자기 언어로 확인 응답), TBM 기록, 공지별 언어별 수신 증빙, 원청-협력사 계층 관리, 사번·국적 연동은 소비자 메신저의 제품 철학(개인용, 무계정 관리)과 맞지 않는다. 그래서 카카오·Meta가 소비자 앱 안에 만들 가능성은 낮다. 기업용(NAVER WORKS, Kakao Work 등)이나 플리토 같은 B2B 업체가 가장 가까운 경쟁자다.
- 이주민 커뮤니티 신뢰는 송금업 사례(오프라인 지점, 국적별 직원, 추천 유입)처럼 수년의 현장 운영으로 쌓인다. 인컴번트가 '기능'으로 복제할 수 없는 자산이다. 단 이 자산을 이미 가진 한패스·GME 같은 송금 슈퍼앱이 채팅을 붙이면 오히려 이들이 경쟁자가 될 수 있다.

### Gaps
- 타깃 언어별(네팔어·크메르어·미얀마어 등) 한국어 직역 품질을 인컴번트 엔진(Kakao i, Papago, Apple, Galaxy)과 LLM으로 직접 비교한 벤치마크는 찾지 못했다(대부분 영어 기준 평가).
- 중대재해처벌법 등 규제가 다국어 안전 공지 기록을 요구하는지, 그 법적 근거와 판례는 이번 조사 범위에서 확인하지 못했다.

---

## A4. 종합: 인컴번트 추격 리스크 평가와 타임라인 (추정)

### Takeaway
2026-11 기준으로 위협은 "범용 다국어 단톡방"에는 높고(12~24개월 안에 카카오나 OS 수준 기능이 메울 가능성), "장꼬리 언어+현장 워크플로"에는 낮거나 중간이다(24~36개월 이상). 아래 확률과 시점은 A1~A3의 인용 사실을 근거로 한 분석적 추정이며, 발표된 로드맵이 아니다.

### Cited Findings
- 현재 공백 확인용 근거: WhatsApp Android 자동번역 언어(6+베타 13)에 한국어 없음 — [WhatsApp Blog](https://blog.whatsapp.com/introducing-message-translations); [WABetaInfo](https://wabetainfo.com/whatsapp-beta-for-android-adds-13-language-packs-for-message-translations/). Telegram 전체 번역은 Premium 전용 — [Telegram FAQ](https://telegram.org/faq_premium). 카카오는 if(kakao)25에서 번역 발표 없음 — [Kakao](https://www.kakaocorp.com/page/detail/11713?lang=ENG). iOS 27의 신규 언어는 Translate 앱 9개이며 장꼬리 언어 없음 — [9to5Mac](https://9to5mac.com/2026/07/08/ios-27-adds-nine-new-languages-and-accents-to-apple-translate/). Galaxy AI는 24개 언어(2026-10) — [PhoneArena](https://www.phonearena.com/news/galaxy-ai-features-language-boost_id184052)
- 한국 내 외국인 규모: 2024년 말 체류 외국인 약 265만, 91일 이상 장기체류 204만 — [한국일보 (2025-08-15)](https://www.hankookilbo.com/News/Read/A2025081517180002074). 2026-11 은행권은 "290만 외국인 리테일"로 표현함 — [뉴스웨이 (2026-11-02)](https://newsway.co.kr/news/view?ud=2026110214345987201)

### Inferences
| 시점(추정) | 인컴번트 동작 | 가능성(추정) | 제품에 미치는 영향 |
|---|---|---|---|
| ~2027-06 | WhatsApp Android 13개 언어팩 정식 배포, iPhone 자동번역 정식 출시 | 높음(베타 진행 중) | 한국 외 해외 가족·지인 대화에서는 대체 효과가 있음. 한국어 Android 미지원이 유지되면 국내 현장 영향은 제한적 |
| ~2027-06 | Galaxy AI·iOS 27 언어 소폭 추가(주요 언어 위주) | 높음 | 베트남어·인도네시아어·태국어·필리핀어 사용자는 OS 오버레이로 "그럭저럭" 해결 가능해 차별성이 줄어듦 |
| 2027 (12~18개월) | 카카오가 KakaoTalk 받은 메시지 자동번역 또는 그룹방 자동번역 출시(19개 언어 엔진, Kanana 활용) | 중간 | 다문화가족·학부모 단톡방 같은 범용 수요가 크게 잠식됨. 가장 큰 단일 리스크 |
| 2027~2028 | Meta가 장꼬리 언어(Instagram DM의 99개 언어 수준)를 WhatsApp에 이식 | 낮음~중간(E2EE와 온디바이스 제약) | 국내 사용률이 낮은 WhatsApp에서는 영향이 제한적이나 해외 연결 대화는 잠식 |
| 2028+ | OS 수준 번역이 장꼬리 언어까지 확장 | 낮음~중간 | 품질 해자가 사라지고, 워크플로·기록·신뢰만 남음 |
- 결론: 소비자 범용 포지션은 18개월 안팎의 창(window)으로 보는 것이 안전하다. 해자는 B2B(현장 안전·공지 확인·협력사 관리)와 장꼬리 언어 품질·용어집에 두어야 한다.

### Gaps
- 카카오의 2026–2027 KakaoTalk 번역 로드맵에 대한 공식 발언, 인터뷰, 채용공고 등 선행 신호는 확인하지 못했다(검색 할당량 소진).
- 외국인 근로자의 메신저 점유율(KakaoTalk, Facebook Messenger, Zalo, Viber, imo, WhatsApp 등 국적별) 통계는 찾지 못했다. 위 영향 판단에서 가장 중요한 미확인 변수다.

---

## B1. 한국에서 이주민 사용자 획득에 성공한 앱 사례와 채널 (송금·구인구직·MVNO·정부앱)

### Takeaway
한국에서 이주민 사용자를 모은 앱(한패스, GME, 센트비, E9pay)의 공통 채널은 다음과 같다. ① 친구 추천과 동향인 네트워크(한패스 신규 가입의 약 60%가 자연 유입), ② 외국인 밀집 지역의 오프라인 지점·국적별 직원·공장·기숙사·식당 방문, ③ 모국어 고객센터와 콘텐츠, ④ 대형 금융·플랫폼과의 제휴 유통(토스-센트비, BC카드·신한카드). CAC 수치는 공개된 것이 없다.

### Cited Findings

**한패스 (Hanpass)**
- 누적 회원 100만 명 이상, MAU 약 42만, 월 신규 가입 약 1.8만 명, 그중 약 60%가 친구 추천 등 자연 유입. 20개국 언어 지원. 국내 체류 외국인 3명 중 1명이 회원이라는 회사 측 주장(IPO 간담회) — [한패스 "5분 송금·20개국 언어"…외국인 생활 플랫폼 목표 (블로터)](https://www.bloter.net/news/articleView.html?idxno=656498); [다음 미러](https://v.daum.net/v/1JT1QMDgd3)
- 2025-04: "매달 40만 대한외국인이 쓰는 한패스"로 비금융 서비스를 품은 슈퍼앱으로 전환 중 — [유니콘팩토리](https://www.unicornfactory.co.kr/article/2025042314311516947)
- 구인구직 '한워크'는 외국인 회원 약 9만, 최근 3개월 누적 매칭 8,000건. 본국 지인과 커뮤니티를 통해 채용 정보가 공유되면서 신규 유입이 늘었다고 설명 — [서울경제](https://www.sedaily.com/article/20062313)
- 2026-01-22 외국인 대상 이커머스 진출 — [뉴스핌](https://www.newspim.com/news/view/20260122000706). 2026-08 월 해외송금액 4,000억 원 돌파 — [네이트 뉴스 (2026-08-06)](https://m.news.nate.com/view/20260806n29438)
- 2026-10-15 '외국인 생활·금융 슈퍼앱'으로 전면 개편. 해외송금 월 이용자 약 20만, 송금 외 서비스 월 이용 약 400만 건, 중복을 뺀 이용자 약 45만 — [네이트 뉴스 (2026-10-15)](https://m.news.nate.com/view/20261015n22536)

**GME (글로벌머니익스프레스)**
- 외국인 밀집 지역 오프라인 지점과 다국어 인력 배치. 송금에서 카드·통신까지 생활금융으로 확대. "모르면 지점으로 오세요" 전략 — [뉴스코리아](https://www.newskorea.ne.kr/news/articleView.html?idxno=21479)
- 마케팅 직무를 국내 거주 외국인으로 한정해 채용하며, 업무에 공장·기숙사·식당 방문을 통한 고객 접점 마련이 포함됨 — [Kowork 채용공고](https://kowork.kr/post/7601). 태국·베트남·필리핀 등 아시아 유학생을 마케팅 인력으로 채용 — [연세대 GLC 공고](https://glc.yonsei.ac.kr/?kboard_content_redirect=887)
- BC카드와 제휴해 국내 거주 외국인(만 14세 이상)용 GME 카드 3종 출시 — [데일리안](https://www.dailian.co.kr/news/view/1305720/BC%EC%B9%B4%EB%93%9C%E2%80%A7GME-%EA%B5%AD%EB%82%B4-%EA%B1%B0%EC%A3%BC-%EC%99%B8%EA%B5%AD%EC%9D%B8-%ED%8A%B9-2023). 2024-11 BC카드·광주은행과 함께 한국민속촌에서 외국인 대상 이벤트를 열었고, 할인은 GME 앱 설치 고객에게 제공 — [네이트 뉴스](https://m.news.nate.com/view/20241103n04563)
- 국내 지점 10곳(동대문, 대림, 몽골타운, 부평, 안산, 수원, 화성, 송우리, 광주, 김해)이라는 채용 사이트 기업정보가 있으나 오래된 자료로 보임 — [원티드 기업정보](https://www.wanted.co.kr/company/5742) (검색 요약상 출처를 특정하기 어려움, 검증 필요)

**센트비 (SentBe)**
- 상담을 영어·중국어·베트남어·우즈베크어로 제공하고, 온·오프라인 상담은 베트남어·태국어·타갈로그어·네팔어 등으로 지원 — [디지털투데이](https://www.digitaltoday.co.kr/news/articleView.html?idxno=118881)
- 2022-04 첫 브랜드 캠페인 영상을 한국어·영어·베트남어·태국어·인도네시아어 버전으로 제작 — [전자신문](https://www.etnews.com/20220413000061)
- 한국 거주 인도네시아인 대상 월례 한국어 수업 '코리안 클래스'와 외국인 축구대회 운영(커뮤니티 이벤트형 획득) — [디지털투데이](https://www.digitaltoday.co.kr/news/articleView.html?idxno=118881) / [매드클럽](http://www.madclub.co.kr/news/articleView.html?idxno=8490) (검색 요약상 둘 중 어느 쪽이 원출처인지 불분명)
- 2025-07 토스와 국내 체류 외국인 전용 해외송금 서비스 출시(미국·중국·베트남·우즈베키스탄 4개국). 대형 앱 안에 들어가는 임베디드 유통 — [플래텀](https://platum.kr/archives/265048); [유니콘팩토리](https://www.unicornfactory.co.kr/article/2025070210514236221)

**E9pay (이나인페이)**
- 2017-08 기획재정부 소액해외송금업 1호 라이선스. E-9 비자 근로자를 주 고객으로 하며 송금·카드 발급 수수료로 수익. 코스닥 상장예비심사 청구. 임직원 105명(2026-07) — [THE VC](https://thevc.kr/e9pay); [핀테크 샌드박스](https://sandbox.fintech.or.kr/business/enterprise.do?lang=ko&id=99)
- 2025-01 신한카드와 외국인 전용 신용카드 출시. 16개국 언어 안내, 신청부터 발급까지 비대면 — [백세시대](https://www.100ssd.co.kr/news/articleView.html?idxno=121708)
- 중국동포·외국인용 앱으로 출시할 때 동포 매체(동포세계신문)를 통해 홍보 — [EKW 동포세계신문](https://www.ekw.co.kr/news/articleView.html?idxno=1385)

**구인구직**
- 잡코리아 '클릭(KLiK)': 출시 1년 만에 MAU 10만 돌파, 최근 3개월 MAU 242% 증가(6월 기준) — [플래텀](https://platum.kr/archives/267260). 반면 한 2026 비교 가이드는 "KLiK가 2026년 6월에 서비스를 종료했다"고 적어 충돌함 — [SeoulStart](https://seoulstart.com/ko/guides/korean-job-platforms) (공식 확인 필요)
- 사람인 '코메이트': 2024년 출시 이후 2026-10 말까지 2년간 외국인 회원 연평균 260.1% 증가, 지원 건수 323.4% 증가, 기업회원 159.4% 증가(절대 수치는 비공개) — [ZDNet Korea (2026-11-03)](https://zdnet.co.kr/view/?no=20261103180800)

**통신 MVNO**
- LG U+ '알닷'이 2025-03 알뜰폰 업계 최초로 외국인 셀프개통 페이지를 열고 5개 언어(중국어·베트남어·태국어·러시아어·영어) 가이드를 제공. 개통 사은품(최대 8.3만 원 상당)에 더해 추가 경품 — [LG 보도자료](https://lg.co.kr/media/release/28769); [경향신문](https://www.khan.co.kr/article/202503241041011)
- KB국민은행 리브모바일 외국인 전용 요금제: 연말까지 가입한 사람에게 3만 원 상당 금융쿠폰. 리브모바일 전체 가입자는 44.2만에서 42.9만으로 감소 — [신아일보](https://www.shinailbo.co.kr/news/articleView.html?idxno=5072991)
- 통신 3사가 장기체류 외국인 전용 요금제로 경쟁. SKT는 별도 요금제 없이 체류 코드가 있으면 모든 요금제 가입 가능 — [한국일보 (2025-08-15)](https://www.hankookilbo.com/News/Read/A2025081517180002074); [국민일보](https://www.kmib.co.kr/article/view.asp?arcid=0028439973)

**공공 채널 환경 변화**
- 고용노동부 외국인노동자지원센터 민간위탁 예산 전액 삭감. 거점 9곳 1월 1일부로 폐쇄. 대체 사업인 '외국인근로자 지역정착 지원사업'은 총 36억 원(국비 18억, 절반은 지자체 부담)으로, 기존 센터 예산 71.08억 원에 크게 못 미침(보도마다 연도 표기가 엇갈림. 2024년 전후로 판단) — [매일노동뉴스](https://www.labortoday.co.kr/news/articleView.html?idxno=219326); [매일노동뉴스](https://www.labortoday.co.kr/news/articleView.html?idxno=219887); [시사IN](https://www.sisain.co.kr/news/articleView.html?idxno=51759); [한국무역협회](https://www.kita.net/board/totalTradeNews/totalTradeNewsDetail.do?no=80540&siteId=1); [단비뉴스 '반쪽 부활'](http://www.danbinews.com/news/articleView.html?idxno=27053)

### Inferences
- 송금앱의 획득 엔진은 '돈을 보내는 사람이 받는 사람과 동료에게 앱을 알리는' 바이럴 구조다(추천 60%). 다국어 단톡방도 방 개설자 1명이 N명을 초대하는 구조라 추천 기반 성장에 유리하다. 핵심은 개설자(현장 반장, 다문화센터 직원, 학부모 대표)를 확보하는 일이다.
- 국적별 직원과 오프라인 현장 방문(공장·기숙사·식당)은 GME·센트비가 공통으로 쓴 방식이며, 초기 GTM에서 가장 재현 가능한 채널이다. 외국인노동자지원센터 예산 삭감으로 공공 네트워크가 약해졌으므로, 지역 커뮤니티 단체·종교시설·동포 매체 같은 민간 접점의 가치가 상대적으로 높아졌다(종교시설 제휴의 직접 근거는 미확인).
- 금융·통신권의 사은품과 쿠폰 수준(3만~8.3만 원)은 외국인 고객 1명의 획득 인센티브 가격대를 짐작하게 한다. 이들은 LTV가 높은 업종이므로 채팅 앱이 이 수준의 유료 획득을 감당하기는 어렵다. 유통 제휴(송금앱·MVNO·은행 앱에 임베드하거나 공동 프로모션) 쪽이 합리적이다.
- 한패스(슈퍼앱, 구직, 이커머스)와 은행권(KB·카카오뱅크의 '290만 외국인 리테일')은 잠재적 유통 파트너이면서 동시에 채팅 기능을 붙일 수 있는 잠재 경쟁자다.

### Gaps
- 어느 사례에서도 CAC나 마케팅 비용이 공개되지 않았다. 혁신의숲 MAU 지표도 원문 접속이 차단되어 확인하지 못했다.
- 국적별 인플루언서, 페이스북 그룹 마케팅, 교회·사찰 제휴의 구체 사례와 성과는 찾지 못했다.
- 'Hi Korea' 정부 앱의 다운로드와 이용자 수, '코리아잡스'는 확인하지 못했다.
- 외국인 전용 MVNO 가입자 수는 공개 통계를 찾지 못했다.

---

## B2. 누가 돈을 내는가: B2B 좌석당 가격, 국내 SME SaaS, B2G, B2B2C(원청 부담)

### Takeaway
비용을 내는 주체로 가장 명확한 근거가 있는 것은 원청·대기업이 협력사 근로자까지 포함해 비용을 부담하는 B2B2C(한화오션-플리토 오톡, DL이앤씨 어깨동무M 자체 개발)다. 국내 SME 가격 기준점은 근태·현장형 1인당 월 2,000~4,000원(시프티), 협업툴 1인당 월 9,000~12,000원(플로우)이다. 해외 프론트라인 툴은 1인당 월 약 1~9달러다. B2G는 민원실 AI 통번역기 단위의 소규모 도입이 대부분이고, 무상 라이선스 사례도 있어 매출원이라기보다 레퍼런스용에 가깝다.

### Cited Findings

**해외 프론트라인 커뮤니케이션 툴**
- Connecteam: 10명까지 무료. Communications Hub Basic은 연간결제 시 월 29달러(처음 30명), Advanced 49달러, Expert 99달러이며 인원 추가 시 비용이 붙음. 허브(운영, 커뮤니케이션, HR)별로 따로 과금 — [Connecteam](https://connecteam.com/best-team-communication-apps/); [G2 비교](https://www.g2.com/compare/beekeeper-vs-connecteam)
- Beekeeper: Capterra·GetApp에 Essential 1인당 월 4달러, Core 6달러, 상위 9달러로 기재됨. LumApps에 인수된 뒤 공개 가격 페이지가 사라져 견적제로 바뀜. Essential 티어에서 '언어 장벽 해소'를 내세우지만 번역 가격은 별도 공개되지 않음 — [Capterra](https://www.capterra.com/p/156917/Beekeeper/); [GetApp](https://www.getapp.com/it-communications-software/a/beekeeper/); [Research.com](https://research.com/software/reviews/beekeeper)

**국내 SME SaaS**
- 플로우(Flow) 비즈니스(2026-05-01 이후 가입자 기준): 월간결제 최소 5인 월 60,000원, 5인 초과 시 1인당 12,000원. 연간결제 최소 5인 월 45,000원, 1인당 9,000원 — [플로우 고객센터](https://support.flow.team/ko/flow/234707787); [플로우 고객센터 (유료 플랜)](https://support.flow.team/ko/flow/17299017042585)
- 시프티(Shiftee): Basic 1인당 월 2,000원(연간 1,800원), Standard 4,000원(연간 3,500원), 30일 무료체험 — [임팩트플로우](https://impactflow.kr/product/shiftee); [TechView](https://www.techview.best/software/321)
- 잔디(JANDI): 매월 1일 정회원 수 기준 월간 청구 또는 연간 일괄 청구 구조만 확인되고, 금액은 확인하지 못함 — [잔디 요금제 정책](https://support.jandi.com/ko/articles/billing-policy-b485865d)
- NAVER WORKS: 게시글 번역은 Core/Approval 유료 상품을 신청해야 제공됨 — [NAVER WORKS](https://help.worksmobile.com/en/use-guides/board/check-post/translate-post/)

**B2B2C: 원청·대기업 부담**
- 한화오션: AX사업부가 기획하고 한화시스템·플리토가 함께 구축한 '오톡'. 협력사에서 도입 요청이 이어져 사번 연동 후 협력사 근로자에게도 배포(2026-09) — [MTN](https://news.mtn.co.kr/news-detail/2026091610011317518); [머니투데이 더벨](https://www.mt.co.kr/stock/2026/09/16/2026091609359684693); [테크월드](https://www.epnc.co.kr/news/articleView.html?idxno=407017)
- DL이앤씨: 2022년 자체 개발한 카카오톡 기반 챗봇 플랫폼 '어깨동무M'(출입 확인, 안전 공지, 업무 알림)에 2024-12 ChatGPT 기반 안전 공지 실시간 번역을 탑재함. 외부 구매가 아니라 자체 개발 — [이투데이](https://www.etoday.co.kr/news/view/2427855); [비즈워치](https://news.bizwatch.co.kr/article/real_estate/2024/12/10/0019); [아주경제](https://www.ajunews.com/view/20241210090649866)
- 은행권: KB국민은행의 29억 원 규모 AI 통번역 화상상담 시스템(은행 사업. 검색 요약상 언급이며 원문 미확인) — [뉴스웨이 (2026-11-02)](https://newsway.co.kr/news/view?ud=2026110214345987201)

**B2G: 지자체·공공**
- 대구 남구(2026-04): 민원실에 65개 언어 AI 실시간 통·번역기 도입. 외국인 주민 2021년 1,827명에서 2025년 2,377명으로 증가 — [아주경제](https://www.ajunews.com/view/20260417122849942); 2026-10 현장 보도 — [매일신문](https://www.imaeil.com/page/view/2026102515080234087)
- 대구 달성군(2026-04): 논공읍 공단출장소에 100여 개 언어 AI 통번역 시스템 — [다음/뉴스](https://v.daum.net/v/20260427104325210)
- 울산(2026-02): 울주군은 200여 개 언어 AI 기기, 동구는 AI 통번역기 4대 — [네이트 뉴스](https://news.nate.com/view/20260206n35416)
- 경북 문경시: 외국인 AI 통번역 '토마톡'을 시 예산 없이 전용 기기와 플랫폼 라이선스를 무상 지원받아 구축(벤더 보조 파일럿) — [이뉴스투데이](http://www.enewstoday.co.kr/news/articleView.html?idxno=2482140). 부산 남구(2026-10)는 다문화 해피로센터 사업과 연계해 민원실 태블릿에서 토마톡 120개 언어 채팅 통번역 제공 — [네이트 뉴스](https://news.nate.com/view/20261020n21480)
- 계약 규모 기준점: 경남 중소기업 통·번역 지원사업(2020) 총 3,640만 원, 제한경쟁(최저가) — [GNTI 공지](https://gnti.co.kr/notice/345); 법무부 「2026년 중앙부처·지방정부 외국인정책 담당공무원 교육 위탁 운영」 3,827.6만 원 — [나라장터 공고 첨부](https://www.g2b.go.kr/pn/pnp/pnpe/UntyAtchFile/downloadFile.do?bidPbancNo=R26BK01337731&bidPbancOrd=000&fileType=&fileSeq=2&prcmBsneSeCd=03); 번역 단가계약 사례로 1쪽(250단어) 45,000원 — [KIND 입찰공고](https://www.kindkorea.or.kr/api/v1/attachment/c812dbee-d0f5-4392-aa67-ee8584d6bf22/download)
- 지자체 용역 수의계약 기준: 추정가격 2천만 원 이하는 수의계약 가능, 2천만 원 초과 1억 원 이하는 소기업·소상공인 여부 확인 필요 — [찾기쉬운 생활법령정보](https://easylaw.go.kr/CSP/CnpClsMain.laf?popMenu=ov&csmSeq=1302&ccfNo=1&cciNo=1&cnpClsNo=2)
- 공공 외국인 노동자 지원 예산 축소: 센터 예산 71.08억 원에서 0원, 대체 사업 36억 원 — [매일노동뉴스](https://www.labortoday.co.kr/news/articleView.html?idxno=219887)

**학교·보육 (학부모 세그먼트)**
- 하이클래스: 다문화 가정과 외국인 학교를 위해 11개 언어 번역 기능 제공 — [하이클래스](https://www.hiclass.net/). 앱 언어를 바꾼 뒤 알림장의 '번역' 버튼을 누르는 방식 — [Google Play 개발사 답변](https://play.google.com/store/apps/details?id=com.iscreammedia.app.hiclass.android&hl=en_US)
- 키즈노트: 교사는 한국어로 쓰고 학부모가 번역을 켜서 자기 언어로 봄(6개 언어) — [키즈노트 공식 블로그](https://blog.kidsnote.com/32)
- 알림장·가정통신문 번역 앱 '알번역' 프로젝트 — [세상파일](https://www.sesang-file.com/project/project03)

### Inferences
- 가격 가설: SME 현장형(공장, 농가, 소규모 건설) 기준으로 근로자 1인당 월 2,000~5,000원(시프티 수준). 관리자 좌석은 플로우 수준(1인당 9,000~12,000원)으로 이원화하는 방안이 국내 기준점과 맞는다. 해외 Connecteam(30명 29달러로 1인당 약 1달러)과 비교해도 1인당 월 1~4달러 구간이 무난하다.
- 원청 모델: 한화오션 사례처럼 원청이 사이트 단위로 계약하고 협력사 근로자에게 무상 배포하는 구조가 이미 작동한다. 다만 대형 원청은 자체 개발(DL이앤씨)이나 대형 SI(한화시스템)를 선호하므로, 스타트업에게 현실적인 고객은 중견 건설사·조선 2~3차 협력사 연합·제조 산업단지 단위일 가능성이 높다(추정).
- B2G: 민원실 기기형 도입이 주류이고 무상 파일럿 사례(문경)도 있다. 계약은 수의계약 한도(2천만 원) 안팎의 소규모 건으로 예상된다. 반복 매출원으로 보기 어렵고, 레퍼런스와 다문화가족지원센터 등을 통한 유통 채널로 쓰는 편이 현실적이다. 외국인 노동자 지원 국비가 축소되었으므로 B2G 의존은 정책 리스크가 크다.
- 학부모 세그먼트: 교사→학부모 일방향 공지는 하이클래스·키즈노트가 이미 번역을 제공한다. 남은 틈새는 학부모끼리의 단톡방(쌍방향, 혼합 언어)이다. 다만 이 세그먼트는 지불 주체가 불분명해 무료 획득 채널로 보는 것이 적절하다.

### Gaps
- 나라장터의 실제 "외국인 통번역" 낙찰 금액, 다누리콜센터와 지자체 다문화센터의 통번역 예산 규모는 원문 조회가 차단되어 확인하지 못했다.
- 플리토 오톡 계약 금액, 한화오션의 사용자 수, 협력사 배포 범위는 공개된 것을 찾지 못했다.
- 잔디의 1인당 가격, Beekeeper·Connecteam의 번역 기능 추가 과금 여부는 확인하지 못했다.
- 하이클래스·키즈노트 번역 기능의 유료 여부와 과금 주체(학교, 교육청, 학부모)는 확인하지 못했다.

---

## B3. 메신저·번역 앱의 프리미엄(유료 전환)과 소비자 수익화 벤치마크

### Takeaway
번역을 유료 기능으로 묶은 가장 큰 사례는 Telegram Premium이다. 유료 구독자는 1,500만 명 이상(2025-05)이지만 MAU 대비 약 1.5%에 그치고, 번역은 여러 혜택 가운데 하나다. 소비자 구독만으로는 니치 다국어 메신저의 수익 기반이 되기 어렵다. 이주민 대상 앱들은 구독보다 거래 수수료(송금·카드)로 수익을 냈다.

### Cited Findings
- Telegram Premium 유료 구독자는 1,500만 명 이상(Pavel Durov, 2025-05) — [Pavel Durov on X](https://x.com/durov/status/1927460225461662111). 2024-12 대비 300만 명 증가, MAU 대비 약 1.5%(집계 사이트) — [DemandSage](https://www.demandsage.com/telegram-statistics/). 2023-12에는 약 400만 명이었다는 집계 — [Backlinko](https://backlinko.com/telegram-users) (집계 사이트 기준)
- Telegram 2024년 총매출 10억 달러 돌파, 흑자 전환, 현금 5억 달러 이상(Durov) — [Techeconomy](https://techeconomy.ng/telegram-is-now-profitable-pavel-durov-announces-1-billion-revenue-milestone). 2025년 상반기 Premium 매출 2.23억 달러, 총매출 8.7억 달러라는 FT 인용 2차 집계(직접 검증 못함) — [SQ Magazine](https://sqmagazine.co.uk/telegram-statistics/)
- Telegram의 번역 구조: 무료는 메시지 단위, Premium은 대화방·채널 전체 실시간 번역 — [Telegram Premium FAQ](https://telegram.org/faq_premium)
- 기업용 번역 유료화: NAVER WORKS 게시글 번역은 유료 Core/Approval 필요 — [NAVER WORKS](https://help.worksmobile.com/en/use-guides/board/check-post/translate-post/)
- Discord 번역 봇의 규모(업체 주장): Discord Translator 서버 30만 개 이상, 활성 사용자 100만 이상을 주장하며 봇 목록에는 서버 311,579개로 표시 — [NVU](https://nvu.io/en/bots/discord-translator/); [top.gg](https://top.gg/bot/360081866461806595). Interaction Bot 서버 55,961개, 사용자 1,190만 — [Interaction Bot](https://interaction-bot.com/blog/best-discord-translation-bot-2026/). BabelBot 2,098개 서버, 104만 명 — [BabelBot](https://www.babelbot.app/). iTranslator는 자체 수치가 서로 충돌함 — [iTranslator](https://itranslator.app/en)
- 이주민 앱의 수익 구조: E9pay는 송금 수수료와 카드 발급 수수료 — [THE VC](https://thevc.kr/e9pay). 한패스는 월 송금 4,000억 원을 기반으로 이커머스·구직으로 확장 — [네이트 뉴스](https://m.news.nate.com/view/20260806n29438); [뉴스핌](https://www.newspim.com/news/view/20260122000706)

### Inferences
- 거대 MAU(약 10억)를 가진 Telegram도 유료 전환율이 약 1.5%다. 국내 체류 외국인 약 265만~290만 명 시장에서 소비자 구독만으로 의미 있는 매출을 내기는 어렵다. 예를 들어 이용자 10만 명 × 2% × 월 3,000원이면 월 600만 원 수준이다(가정 기반 계산).
- 소비자 프리미엄은 장꼬리 언어 고품질 모드, 음성·이미지 번역, 해외 가족 그룹 같은 부가 기능 정도로 제한하는 것이 맞다. 매출의 주축은 B2B(현장, 원청)와 B2B2C(송금앱·통신사·은행 제휴, 수익 공유)에 두는 구조가 근거와 부합한다.
- Discord 번역 봇 규모(수만~수십만 서버)는 "기존 네트워크 위에 얹는 번역" 수요가 실재한다는 증거다. 하지만 이 봇들의 대부분이 프리미엄 구독으로 운영된다는 사실과 그 가격은 이번 조사에서 확인하지 못했다.

### Gaps
- Telegram Premium 정확한 가격(국가별), Papago 유료 구독과 번역 앱 구독 매출(DeepL, iTranslate 등)은 검색 할당량 소진으로 확인하지 못했다.
- Discord·Telegram 번역 봇의 유료 전환율과 가격은 확인하지 못했다.

---

## B4. '레이어' 전략(키보드·오버레이, KakaoTalk 챗봇, LINE/Telegram 봇)과 독립 앱 비교

### Takeaway
일방향 공지(안전·출입·업무 알림)는 KakaoTalk 챗봇이나 알림톡 레이어로 충분하다(DL이앤씨 어깨동무M 사례, 건당 약 7~13원). 하지만 쌍방향 혼합 언어 단톡방은 KakaoTalk 그룹방에 봇을 공식적으로 넣는 경로가 불명확하다. 키보드 레이어는 발신만, OS 오버레이(Galaxy AI)는 기기와 버전에 따라 불안정하다. 따라서 "레이어로 진입하고 독립 방으로 전환하는" 하이브리드가 근거상 합리적이다.

### Cited Findings
- DL이앤씨 어깨동무M: 카카오톡 기반 챗봇으로 출입 확인·안전 공지·업무 알림을 전달하고(2022), 2024-12 ChatGPT 번역을 탑재해 근로자 국적 정보 기반으로 언어별 자동 번역·발송 — [이투데이](https://www.etoday.co.kr/news/view/2427855); [한국경제](https://www.hankyung.com/article/2024121061646); [뉴스1](https://www.news1.kr/realestate/general/5626533)
- 카카오 챗봇의 구조적 제약: 오픈빌더 봇의 운영 채널 메시지가 스킬 서버로 가지 않고 1:1 상담으로만 들어간 사례(카카오 데브톡). 챗봇은 카카오톡 채널(1:1) 연결이 기본 구조 — [카카오 데브톡](https://devtalk.kakao.com/t/1-1/152245). 블로그에는 채팅봇을 일반·팀 채팅방에서 쓸 수 있고(앱 v25.4.0 이상) 오픈채팅·채널 채팅방에서는 제한된다는 설명이 있으나 공식 문서는 아님 — [ONNA 블로그](https://onna.kr/%EC%B9%B4%EC%B9%B4%EC%98%A4%ED%86%A1-%EB%8B%A8%ED%86%A1%EB%B0%A9-%EC%B1%84%ED%8C%85%EB%B4%87-%ED%99%9C%EC%9A%A9%EB%B2%95-%EC%B4%88%EB%8C%80-%EC%A0%9C%EA%B1%B0-%EC%B9%B4%ED%86%A1-%EC%B1%97%EB%B4%87)
- 알림톡 비용: 2026-01 기준 정가 10원, 프로모션가 8원이라는 자료 — [AtoZsoft](https://www.atozsoft.co.kr/insights/alimtalk-price-comparison-2026); 2026-07 기준 공식 딜러 인포뱅크 비즈고 5,000건 35,600원(건당 약 7.12원), 스윗트래커 비즈엠 건당 8원, 솔라피 건당 13원 — [비즈고 블로그](https://blog.bizgo.io/inside/alimtalk-provider-selection-guide/); 솔라피 기본 13원(VAT 별도), 월 2,000만 건 이상 5.5원 — [솔라피 가격](https://solapi.com/pricing); [솔라피 구간 할인](https://solapi.com/guides/tiered-pricing). 2026-01부터 친구톡이 '브랜드 메시지'로 통합됨 — [오마고](https://www.omago.ai/ko/blog/kakaotalk-brand-message-2026). 카카오는 유형별 공식 원단가를 공개하지 않는다는 설명 — [오마고](https://www.omago.ai/ko/blog/kakaotalk-message-pricing-logic)
- Telegram 봇: 그룹의 주 언어와 다른 메시지를 자동 번역하는 오픈소스 TgTranslator가 있음(규모 비공개) — [GitHub Dubzer/TgTranslator](https://github.com/Dubzer/TgTranslator). Telegram 자체 Premium 번역과 경쟁 관계 — [Telegram FAQ](https://telegram.org/faq_premium)
- Discord 봇: 언어별 채널을 연결해 메시지를 다른 채널에 자동으로 번역·미러링하는 방식(사실상 '혼합 언어 방'을 채널 미러링으로 구현) — [TranslateBot V2](https://v2.translatebot.app/). 서버 수만~수십만 규모(업체 주장) — [NVU](https://nvu.io/en/bots/discord-translator/)
- 키보드 레이어: 카카오톡·WhatsApp 등 여러 메신저에서 쓰는 '키보드 번역기' 앱(발신 번역) — [App Store](https://apps.apple.com/kr/app/%ED%82%A4%EB%B3%B4%EB%93%9C-%EB%B2%88%EC%97%AD%EA%B8%B0-%EC%B1%84%ED%8C%85-%EB%A9%94%EC%8B%9C%EC%A7%80-%EC%8B%A4%EC%8B%9C%EA%B0%84-%EB%B2%88%EC%97%AD-%EC%95%B1/id1502909594)
- OS 오버레이의 불안정성: Galaxy AI의 카카오톡 자동번역이 업데이트 후 작동하지 않다가 복구됐다는 사용자 보고(2026-10 하순) — [Samsung Members](https://r1.community.samsung.com/t5/%EA%B0%A4%EB%9F%AD%EC%8B%9C-s/%EC%B9%B4%EC%B9%B4%EC%98%A4-%EC%9E%90%EB%8F%99%EB%B2%88%EC%97%AD%EC%9D%B4-%EC%9D%B4%EC%A0%9C-%EB%93%9C%EB%94%94%EC%96%B4-%EB%8B%A4%EC%8B%9C-%EB%90%A9%EB%8B%88%EB%8B%A4/m-p/40094734)
- 독립 앱도 채택될 수 있다는 근거(B2B 강제 배포 맥락): 오톡의 활성 사용률이 3개월 만에 20%에서 96%로 올랐다는 플리토 주장 — [네이트/이데일리](https://m.news.nate.com/view/20260911n21717)

### Inferences
- 레이어의 장점: 설치가 필요 없고 기존 네트워크를 그대로 쓴다. 어깨동무M은 2022년부터 운영되며 번역까지 붙였다. 일방향 공지 기준으로 근로자 1인당 하루 수 건 × 약 8원이면 월 1인당 수백 원 수준의 원가로 가능하다(계산 추정).
- 레이어의 한계: ① KakaoTalk 그룹방 봇 참여가 공식적으로 보장되지 않아 쌍방향 혼합 언어 단톡방을 KakaoTalk 안에 구현하기 어렵다. ② 카카오가 자체 자동번역을 출시하면 레이어의 가치가 즉시 0에 가까워진다(플랫폼 리스크). ③ 브랜드 메시지·알림톡 정책과 단가가 카카오 결정에 종속된다(2026-01 친구톡 개편 사례).
- 독립 앱의 조건: B2B 맥락(관리자가 방을 만들고 근로자를 초대하며 사번·국적이 연동됨)에서는 독립 앱 채택이 가능하다는 근거가 있다(오톡 96%). 소비자 맥락(다문화가족, 커뮤니티)에서는 네트워크 효과 때문에 독립 앱이 불리하다.
- 권장 구조(추정): ① 관리자용 독립 앱과 웹(방 생성, 용어집, 공지 확인, 기록), ② 근로자는 앱 설치 없이도 KakaoTalk 알림톡·채널 링크나 웹 링크로 참여(첫 참여 마찰 최소화), ③ 그 뒤 쌍방향 대화가 필요해지는 시점에 앱으로 전환하는 퍼널. Telegram·Discord 봇은 국내 이주노동자 메신저 점유율 근거가 없으므로 우선순위를 낮춘다.

### Gaps
- 카카오 공식 정책(오픈빌더 챗봇을 그룹채팅방에 초대할 수 있는지, 그룹방 봇의 메시지 읽기 권한, 상업적 이용 제한)과 챗봇·상담톡 비용 체계는 공식 문서로 확인하지 못했다.
- LINE 공식 계정·봇을 그룹에 넣는 방식의 비용과 정책, LINE이 한국 내 이주민(태국·인도네시아·대만 출신 등)에게 얼마나 쓰이는지는 확인하지 못했다.
- 어깨동무M의 이용자 수, 현장 수, 번역 기능 이용률은 공개된 수치가 없다.
