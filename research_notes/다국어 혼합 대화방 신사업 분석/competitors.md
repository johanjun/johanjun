# 경쟁사·인접 플레이어 분석: "3개 이상 모국어가 섞인 그룹채팅, 각자 자기 언어로 자동 표시, 회사 계정 불필요, 폰 전용" (한국 우선, 글로벌 확장 검토)

> 조사 기준일: 2026-11-04.
> 조사 방법상 한계: 이번 세션에서는 WebFetch가 거의 모든 호스트(apps.apple.com, producthunt.com, hankyung.com, mtn.co.kr, timekettle.co, vasco-translator.com, theguru.co.kr 등)에서 DNS 차단으로 실패했습니다. 그래서 아래 내용은 모두 **웹 검색 결과의 요약·스니펫**을 근거로 합니다. "공식 페이지 검증"이라고 적은 항목도 공식 페이지를 직접 연 것이 아니고, 검색엔진이 요약한 공식 페이지 내용입니다. 중간에 세션 전체의 WebSearch 한도(200회)도 소진되어 일부 항목(애니챗 상세, Viber 2026 업데이트, 다문화가족 앱, 시프티·알바몬, IMO·Messenger, Telegram 공식 문서)은 추가 확인을 못 했습니다. 이 항목들은 Gaps에 따로 적었습니다.
> 표기 규칙: 【공식】은 회사 공식 페이지·도움말·앱스토어·공식 블로그를 검색 요약으로 확인한 것, 【보도】는 언론 보도(보도자료 기반이 많음), 【제3자】는 리뷰·애그리게이터·블로그·포럼입니다.

---

## Q1. 전용 다국어 채팅 앱 (Shavely, DoTalk, MultiTalk, Interpreter, JotMe 등)은 무엇을 하며, 얼마나 직접 경쟁하는가

### Takeaway
"그룹방에서 각자 자기 언어로 읽기"라는 핵심 기능은 이미 여러 소형 앱이 구현했습니다. 가장 근접한 것은 Vasco MultiTalk(최대 100명, 105~107개 언어, QR 참여, 무료, 음성 메시지 번역), Timekettle Chat Mode(최대 200명, 40개 언어), Shavely(29개 언어, 개인별 번역, 팀 용어집), FlaiChat(40+ 언어, 텍스트·음성, 가족 메신저 지향), 한국의 애니챗(20개 언어, 인도네시아 파트너 투자 보도)입니다. 하지만 대부분 견인력(다운로드·매출·투자)이 확인되지 않는 소규모 제품이거나, 하드웨어 판매의 부가 기능(Vasco, Timekettle)입니다. 한국 외국인 근로자의 롱테일 언어(네팔어, 크메르어, 버마어, 우즈베크어, 싱할라어, 몽골어, 벵골어) 지원 여부는 앱별로 거의 확인되지 않았습니다. 대형사의 다자간 대화 번역은 오히려 철수했습니다(Microsoft Translator 다중기기 대화 2026-06-30 종료, Amazon SayHi 2024 종료).

### Cited Findings

**Shavely (일본, B-track Inc.)**
- 【제3자/런치페이지】 모바일 그룹채팅 앱이며 각 독자에게 메시지를 자동 번역해 보여줍니다. 29개 언어, 별도 번역기에 복사할 필요 없음 — [Product Hunt 런치](https://www.producthunt.com/posts/shavely), [chatgate.ai](https://chatgate.ai/post/shavely)
- 【제3자】 조직이 사내 용어 번역을 직접 정하는 커스텀 팀 사전을 지원하고, 원문이 중요할 때 메시지별로 번역을 끌 수 있습니다 — [chatgate.ai](https://chatgate.ai/post/shavely), [feedbagel](https://feedbagel.com/post/shavely-mobile-team-chat-app-with-real-time-multilingual-translation-for-global-)
- 【제3자】 첫 목표 시장은 크로스보더 이커머스 고객지원이며, 다른 플랫폼이 쓸 수 있도록 API 공개를 준비 중이라고 제작자가 밝혔습니다 — [Product Hunt](https://www.producthunt.com/posts/shavely)
- 【제3자】 freemium, iOS·Android·웹. Capterra는 "employee communication" 카테고리로 분류합니다 — [AlternativeTo](https://alternativeto.net/software/shavely/about), [Capterra CA](https://www.capterra.ca/software/1087212/Shavely)
- 【제3자】 AlternativeTo는 종단간 암호화를 기능으로 적었지만 공식 출처로 확인되지 않습니다 — [AlternativeTo](https://alternativeto.net/software/shavely/about)
- 【제3자】 창업자는 Tatsuya Murakami(B-track Inc. founder)로 보입니다. 도쿄 글로벌 IT기업에서 10년간 일하며 비원어민의 영어 소통 문제를 겪은 것이 출발점이라고 합니다 — [Product Hunt 프로필](https://www.producthunt.com/@tatsuya_murakami), [Product Hunt](https://www.producthunt.com/products/shavely)
- 가격(유료 플랜 단가), 다운로드 수, 투자, 그룹 인원 상한, 음성 메시지 번역 여부, 롱테일 언어 지원은 검색으로 확인되지 않았습니다(아래 Gaps).

**Vasco MultiTalk (폴란드, Vasco Electronics: 번역기 하드웨어 회사)**
- 【공식】 무료 그룹채팅 앱이며 최대 100명이 참여합니다. 한 Vasco 글에는 107개 언어, 다른 Vasco 페이지에는 105개 언어로 적혀 있어 자사 자료끼리도 수치가 다릅니다 — [Vasco 블로그](https://vasco-translator.com/articles/languages/multilingual-conversation-made-easy/), [Vasco translate-chat 기능 페이지](https://vasco-translator.com/features/translate-chat)
- 【공식】 App Store 설명: "MultiTalk will automatically translate every text and audio message". 즉 텍스트와 **음성 메시지 모두** 자동 번역합니다. 방을 만들면 게스트가 QR 코드나 채팅방 이름·번호로 참여합니다 — [App Store: Vasco MultiTalk](https://apps.apple.com/us/app/-/id1673051523)
- 【공식, 마케팅 수치】 번역 정확도를 한 페이지는 96%, 다른 페이지는 99%라고 주장합니다. 독립 측정은 아닙니다 — [Vasco 블로그](https://vasco-translator.com/articles/languages/multilingual-conversation-made-easy/)
- 【보도】 CES 2020에서 처음 공개, 2020년 Android 출시, 최대 100명 초대 — [wwwhatsnew (2020-06)](https://wwwhatsnew.com/2020/06/05/multitalk-para-traducir-en-tiempo-real-las-conversaciones-entre-varias-personas-al-mismo-tiempo/), [ITwiz (PL)](https://itwiz.pl/?p=49697)
- iOS 앱 ID(1673051523)로 보아 iOS판은 2023년 무렵 별도 출시된 것으로 보입니다(추정). 평점·다운로드는 확인하지 못했습니다.

**DoTalk (호주, 2017)**
- 【보도, 2017】 약 90개 언어 텍스트 번역, 50+ 언어 음성(hold & talk) 번역, 최대 10명 그룹채팅 — [Travel Weekly AU](https://www.travelweekly.com.au/article/new-app-lets-you-speak-90-languages/), [iTWire](https://itwire.com/your-it-news/apps/dotalk-breaks-down-language-barriers)
- 【보도, 2017】 1:1은 무료, 그룹채팅은 유료 구독(월 US$7.99부터) — [Startup Daily 아카이브](https://archive.startupdaily.net/?p=63697)
- 【공식】 현행 App Store 설명은 그룹채팅을 프리미엄 기능으로 두고 "10 different languages"라고 씁니다. "10"이 인원인지 언어 수인지 출처마다 다릅니다 — [App Store FR: DoTalk](https://apps.apple.com/fr/app/dotalk/id1582289519)
- 앱 ID(1582289519)가 2021년 무렵 값이라 재출시된 것으로 보입니다(추정). 보도는 2017년 이후 거의 없어 정체된 제품일 가능성이 큽니다(추론).

**Interpreter - Live Translate Chat**
- 【제3자/런치페이지】 3명이 각자 언어로 대화하는 공간. 3인 프라이빗 룸, 메시지 저장 안 함, 2025-04-14 Product Hunt 출시 — [Product Hunt](https://www.producthunt.com/products/interpreter-live-translate-chat)
- 앱스토어 페이지, 가격, 플랫폼은 확인되지 않았습니다. 같은 이름의 앱(Samsung Interpreter, "Interpreter: Live Translator" 등)이 많아 혼동하기 쉽습니다 — [Product Hunt](https://www.producthunt.com/products/interpreter-live-translate-chat)

**JotMe**
- 【공식】 기본은 멀티링구얼 회의·이벤트용 실시간 번역·전사 데스크톱 앱입니다("Run every multilingual meeting and event smoothly"). 모바일 앱도 있습니다 — [jotme.io](https://jotme.io/)
- 【공식 블로그】 자사 블로그가 "각자 자기 언어로 입력하고 상대는 자기 언어로 읽는" 업무용 다국어 채팅방을 소개합니다. 자사 마케팅 자료이므로 걸러 봐야 합니다 — [JotMe 블로그 (한국어)](https://www.jotme.io/ko/blog/best-multilingual-team-chat-apps)
- 【공식】 "jotme a16z" 블로그 글이 있어 a16z 관련 투자를 시사하지만, 검색 스니펫에는 금액·일자·리드 투자자가 없습니다. Dealroom은 유료 벽 뒤에 있습니다 — [JotMe 블로그](https://jotme.io/blog/jotme-a16z), [Dealroom](https://app.dealroom.co/companies/jotme)
- 회의 중심 제품이라 "폰 전용 생활 그룹채팅"과는 간접 경쟁입니다(추론).

**FlaiChat (멀티링구얼 가족 메신저)**
- 【공식/제3자】 텍스트와 음성 메시지를 40+ 언어로 자동 번역합니다. 다국어 가족·그룹이 주 타깃이고 "hybrid dialects"도 다룬다고 합니다 — [App Store: FlaiChat](https://apps.apple.com/app/id1575884028), [moge.ai](https://moge.ai/product/flaichat)
- 【공식】 유료 "FlaiChat Plus"로 "Speak Together: Live Conversation Translation"을 해제합니다. 발신자 목소리로 음성을 번역해 들려주는 기능이 리뷰에 언급됩니다 — [App Store](https://apps.apple.com/app/id1575884028), [moge.ai](https://moge.ai/product/flaichat)
- 【제3자】 그룹채팅에 스레드·일정·알림 기능이 있고, 전화번호나 이메일 없이 가입할 수 있다고 강조합니다 — [moge.ai (KO)](https://moge.ai/ko/product/flaichat)
- 【제3자】 SourceForge 제목은 "Multilingual Family Messenger"이며 웹·데스크톱은 개발 중입니다 — [SourceForge](https://sourceforge.net/app/flaichat/web-app/)
- 투자 정보는 확인되지 않았습니다. 2024-09 Reddit r/androidapps에서 개발자가 "다문화 가족 속에서 단절감을 느껴 만들었다"고 홍보한 흔적이 있습니다 — [Reddit 미러](https://lr.eu.psf.lt/r/androidapps/comments/1fdq5y1/i_felt_disconnected_from_my_multicultural_family/lmhhy9k/?context=3)

**Timekettle (중국 선전, 번역 이어버드·하드웨어)**
- 【공식】 앱의 "Chat Mode": 그룹 최대 200명, 최대 40개 언어, 메시지에 이중언어 자막. 표시 언어를 바꾸려면 그룹에 다시 들어가야 합니다(2022 베타 시작) — [Timekettle 블로그](https://www.timekettle.co/blogs/news/timekettle-chat-mode-instant-message-translated-in-max-40-languages-max-200-people-in-group)
- 【공식】 "Remote Mode"(베타): 원격지 사용자용, 40개 언어, 재참여 시 최근 25개 메시지 복원 — [Timekettle 블로그](https://www.timekettle.co/blogs/news/timekettle-all-new-feature-remote-mode)
- 【제3자】 WT2 Edge 이어버드: 대면 6인 이중언어 미팅, 원격 그룹채팅 최대 40명·40개 언어 — [TechHive Shop](https://shop.techhive.com/sales/timekettle-wt2-edge-real-time-2-way-translator-earbuds-w-offline-translation)
- 【보도】 X1 Interpreter Hub: 한 방에 최대 20명·5개 언어, 게스트는 자기 기기로 참여, 호스트가 최대 50명 입장 허용 — [Android Authority](https://androidauthority.com/timekettle-x1-meeting-translator-hands-on-3681162), [techigar](https://techigar.com/timekettle-x1-ai-interpreter-hub-translates-in-real-time)
- 앱 Chat Mode를 하드웨어 없이 쓸 수 있는지, 가격이 얼마인지는 확인하지 못했습니다(Gaps).

**Talkey: Spin to Translate**
- 【공식】 같은 Wi-Fi에서 최소 20명이 실시간 음성 번역 채팅방에 참여하고, Bluetooth로는 최대 4명까지 됩니다. 14개 언어 — [App Store: Talkey](https://apps.apple.com/us/app/-/id6761222476)
- 대면·근거리 중심이라 원격 비동기 그룹채팅과는 다른 사용 상황입니다(추론).

**iTranslate Converse / Pocketalk / Papago / Google 번역 (1:1 대면 통역형)**
- 【공식】 iTranslate Converse: 2인 음성 통역, 38개 언어, 무료+인앱결제. 그룹 기능은 없습니다 — [App Store](https://apps.apple.com/US/app/id1241264761), [itranslate.com](https://itranslate.com/converse/)
- 【보도】 Pocketalk 앱: 82개 언어 양방향 통역(2022). 다인원 룸 기능은 확인되지 않았고, 회의용은 별도 제품(Sentio)·Enterprise App으로 나뉩니다 — [techbuzzireland (2022)](https://techbuzzireland.com/2022/09/06/pocketalk-introduces-mobile-app-for-conversational-translations-wherever-you-go-2/), [Pocketalk](https://pocketalk.com/additional-industries)
- 【공식/보도】 Papago: 앱스토어 설명은 14개 국어(한·영·일·중 간체/번체·스페인·프랑스·베트남·태국·인도네시아·러시아·독일·이탈리아·아랍)인데, 2024-02 아랍어 추가 보도는 16개 언어라고 합니다. 다자간 그룹 대화 번역 근거는 없습니다 — [App Store KR: Papago](https://apps.apple.com/kr/app/%EB%84%A4%EC%9D%B4%EB%B2%84-%ED%8C%8C%ED%8C%8C%EA%B3%A0-ai-%ED%86%B5%EB%B2%88%EC%97%AD/id1147874819), [KED Global (2024-02)](https://amp.kedglobal.com/newsAmp/ked202402020001)
- 【보도】 Papago Plus(네이버클라우드, 2024-09): 기업용, 1:1 대화 번역·용어집·팀 기능 — [Asiae (2024-09)](https://www.asiae.co.kr/en/article/2024092709190857172)
- 【보도】 Papago 월 사용자 2,000만 명 돌파(2024-06), 해외 사용자 27% 증가 — [Asiae (2024-06)](https://www.asiae.co.kr/en/article/2024061009080907110)
- 네팔어·크메르어·버마어·우즈베크어·몽골어·싱할라어·벵골어는 위 Papago 언어 목록에 없습니다(위 목록 기준).

**한국 및 기타 소형 번역 메신저**
- 【보도, 2022-05】 애니챗(ANYCHAT, 한국, 2021 설립): 채팅방에서 각자 자기 언어로 입력하면 화면에는 자국어 번역만 보입니다. 출시 당시 14개 언어. 자체 딥러닝 엔진으로 구어체·신조어를 처리한다고 주장합니다 — [데일리안](https://www.dailian.co.kr/news/view/1116240/)
- 【공식】 애니챗 App Store(일본 페이지): 현재 20개 언어, 향후 30개 이상 예정. 파일·사진·동영상 전송, 연락처 기반 친구 찾기 — [App Store JP: 애니챗](https://apps.apple.com/jp/app/%EC%95%A0%EB%8B%88%EC%B1%97-anychat/id6670591400)
- 【보도, 연도 불명확】 "실시간 AI번역 애니챗, 인니 사업 본격화… 현지 파트너사 260억원 베팅". 인도네시아 파트너가 약 2,000만 달러 투자 의향을 밝혔다는 단독 보도입니다(기사 연도와 실제 집행 여부는 미확인) — [더구루](https://www.theguru.co.kr/news/article.html?no=55007)
- 【제3자】 Slaap(나이지리아 개발자, Gemini API 대회 출품작): 발송 전 수신자 선호 언어로 번역 — [Google AI 대회](https://ai.google.dev/competition/projects/slaap?hl=ko); BabelTalk(한국 팀, 대회 출품작): 웹 기반, 링크·QR 초대, 관심사 채팅방 — [Google AI 대회](https://ai.google.dev/competition/projects/babeltalk?hl=ko)

**대형사의 다자간 번역 기능 철수**
- 【공식 앱 릴리스노트/보도】 Microsoft Translator의 다중기기 대화(Converse, 여러 사람이 각자 기기로 같은 대화방에 들어와 각자 언어로 보는 기능)가 **2026-06-30 종료**되었습니다. 릴리스노트 26.7.1: "The multi-device conversation feature has been retired." — [WhistleOut](https://www.whistleout.com/CellPhones/Guides/is-microsoft-translator-worth-downloading), [APKMirror](https://www.apkmirror.com/apk/microsoft/microsoft-translator/)
- 【공식】 Microsoft는 2022년에 이미 웹앱의 대화 시작·호스팅 기능을 제거했습니다 — [Microsoft Translator Blog (2022-08)](https://www.microsoft.com/en-us/translator/blog/2022/08/03/transitioning-the-microsoft-translator-web-app-to-a-simplified-experience)
- 【제3자】 리뷰 정리에 따르면 Microsoft Translator의 대화·그룹 번역은 "unreliable or non-functional and cannot be started"라는 불만이 있었습니다 — [Unstar](https://unstar.app/blog/google-translate-deepl-itranslate-microsoft-translator-translation-apps-ranked-2026)
- 【제3자, 포럼】 Amazon의 SayHi 번역 앱은 2024-08-05자로 종료(공지만 남고 사유 없음) — [rblind 포럼](https://rblind.com/post/6611706), [lemm.ee](https://lemm.ee/post/38944567) (어느 게시물이 원문인지 검색 요약으로는 특정하지 못했습니다. 신뢰도 낮음)

### Inferences
- "그룹방 + 개인별 자동번역" 자체는 기술적으로 범용화(commodity)되었습니다. MultiTalk·Timekettle·Shavely·FlaiChat·애니챗·DoTalk가 모두 구현했습니다. 차별화는 번역 기능에서 나오기 어렵고, (a) 한국 현장에 맞는 롱테일 언어 품질, (b) 가입 없는 초대(QR·링크)와 한국 관리자 쪽 UX(카카오톡 수준의 익숙함), (c) 음성 메시지 번역, (d) 공지 확인·읽음 확인 같은 "현장 기능", (e) 유통 채널에서 나올 가능성이 큽니다.
- 대형사(Microsoft, Amazon)가 다자간 소비자 번역 대화 기능을 접은 것은 두 갈래로 해석됩니다. 소비자 다자간 번역 대화의 사용량·수익성이 낮다는 경고일 수도 있고, 대형사가 빠져 빈자리가 생겼다는 신호일 수도 있습니다. Microsoft 기능이 주로 "대면 회의·교실용 일회성 대화"였던 반면 이 사업은 "상시 그룹 메신저"라는 차이가 있습니다.
- 가장 직접적인 기능 경쟁자는 Vasco MultiTalk입니다(무료, 100명, 100+ 언어, QR, 음성 포함). 하지만 하드웨어 판매 보조용이고 한국어 마케팅이나 한국 현장 맞춤은 없어 보입니다(검색상 한국 관련 언급 없음).
- 애니챗은 한국 기반 직접 경쟁자이지만 출시(2022) 후 20개 언어 수준이고, 인도네시아로 방향을 돌린 것으로 보입니다. 한국 외국인 근로자 시장에서의 존재감은 확인되지 않습니다.

### Gaps
- 앱별 롱테일 언어(베트남어, 네팔어, 크메르어, 버마어, 우즈베크어, 인도네시아어, 태국어, 타갈로그어, 몽골어, 싱할라어, 벵골어) 지원 목록을 하나도 직접 확인하지 못했습니다. 앱스토어·공식 페이지 접속이 막혔기 때문입니다. MultiTalk(105~107개)나 DoTalk(90개)는 Google·Microsoft 엔진을 쓴다면 대부분 포함할 것으로 보이지만 미검증입니다.
- 다운로드 수, 평점, 리뷰 수: Google Play·App Store 접속 불가로 전 앱 미확인.
- Shavely·Interpreter·FlaiChat·Timekettle Chat Mode의 가격, MultiTalk의 그룹 기능 유료화 여부, 하드웨어 없이 Timekettle 앱만 쓸 수 있는지.
- 애니챗의 회사명·대표·투자 집행 여부·한국 사용자 수(검색 한도 소진으로 추가 확인 못 함).
- Lingmo, Talkao: 검색에 나오지 않았습니다. Langogo: 조사하지 못했습니다.
- Google 번역 대화 모드는 1:1 단일기기 대면 통역으로 알려져 있지만, 이번 세션에서 출처로 확인하지 못했습니다.

---

## Q2. 한국 플레이어: hiWorker, DL이앤씨 어깨동무M, 포스코 앱, 외국인 근로자 소통·안전 스타트업, 다문화·학교 알림 번역

### Takeaway
한국 시장은 "B2B 현장 안전·TBM·공지 통역" 쪽에서 빠르게 붐비고 있습니다. hiWorker(하이로컬, 카카오벤처스 투자, HJ중공업 전국 현장 도입), 플리토(한화오션 '오톡', 대한산업안전협회 MOU), KS인더스트리 Ami/AmiX(24개 언어, 무가입 다국어 통역룸), 켐토피아 '안전 다통해'(40+ 언어), AI 안전함(스마트안전모)이 있습니다. 대형 건설·조선사는 아예 자체 개발합니다(대우건설·롯데건설×롯데이노베이트, DL이앤씨 어깨동무M, HD현대중공업). 반대로 **회사 계정 없이, 관리자가 아닌 일반인이 만드는 혼합 언어 단체방**은 한국에서 뚜렷한 강자가 확인되지 않았습니다. 학교 알림(하이클래스, 클래스팅)에서도 번역 기능이 확인되지 않아 빈자리로 보입니다.

### Cited Findings

**hiWorker / 하이로컬 (가장 직접적인 국내 B2B 경쟁자)**
- 【공식 앱스토어】 "외국인 근로자를 고용 중인 공장, 물류, 건설 현장의 관리자 및 대표님들을 위한 AI 통역 및 안전교육 전문 앱". 쌍방향 실시간 다국어 통역, AI 안전교육 콘텐츠, 공지 전달·확인, 대화 기록, 맞춤 용어집을 제공합니다 — [App Store: hiWorker](https://apps.apple.com/us/app/-/id6749565624)
- 【채용공고】 하이로컬은 2020년 설립, 제조·건설·조선 현장용 AI 통번역 에이전트 'HiWorker'를 제공하는 B2B SaaS 기업입니다 — [원티드](https://www.wanted.co.kr/wd/361805), [TheVC](https://thevc.kr/hilokal), [혁신의숲](https://www.innoforest.co.kr/company/CP00001746)
- 【보도】 원래 외국인과의 음성 대화(언어교환) 플랫폼을 운영하다가, AI 튜터·다국어 통번역으로 외국인 근로자 안전교육·소통 B2B로 사업을 넓혔습니다(피벗) — [혁신의숲](https://www.innoforest.co.kr/company/CP00001746/%ED%95%98%EC%9D%B4%EB%A1%9C%EC%BB%AC)
- 【보도】 카카오벤처스가 2023-01 투자했고, 보도 시점 누적 투자액은 약 15억 원입니다. 윤정호 대표가 전국 150여 현장을 방문해 설계했으며, 건설 현장용 "1:N 동시 통역"으로 출시했습니다 — [유니콘팩토리 (해당 기사로 추정, 검색 요약이 출처 URL을 명확히 하지 않음)](https://www.unicornfactory.co.kr/article/2024102215582058284)
- 【보도】 삼성물산 오픈이노베이션에서 3개월 실증. 40개국 언어 실시간 통번역, 이미지 번역, AI 튜터 교육, 음성인식·번역 정확도 80% 이상(회사 발표) — [비즈워치](https://news.bizwatch.co.kr/special/2025/view/202507170017), [헤럴드경제](https://mbiz.heraldcorp.com/article/10774114) (검색 요약이 두 기사 중 어디서 나온 수치인지 특정하지 않았습니다)
- 【보도, 2026-09】 HJ중공업이 하이워커를 전국 건설현장으로 넓혀 안전교육, TBM, 업무지시에 활용합니다. TBM 통역 무전기, 데스크톱 번역기도 포함합니다 — [한경 머니 (2026-09)](https://magazine.hankyung.com/money/article/202609043973c)
- 가격은 검색으로 확인되지 않았습니다(Gaps).

**대기업 자체 구축 사례 (시장 상단은 내재화 중)**
- 【보도, 2024-12】 DL이앤씨 어깨동무M: 2022년 자체 개발한 카카오톡 기반 챗봇으로 출입 확인, 안전 공지, 업무 알림을 전달합니다. ChatGPT 기반 AI 자동번역을 추가해 근로자 국적 정보에 따라 중국어, 베트남어, 카자흐어, 캄보디아어 등으로 자동 변환해 보냅니다. TBM과 사고 사례 알림으로 확장할 계획입니다 — [메트로서울 (2024-12)](https://www.metroseoul.co.kr/article/20241210500074), [스마트투데이](https://www.smarttoday.co.kr/ko-kr/articles/66734), [TF미디어](https://www.tfmedia.co.kr/news/article.html?no=174206)
- 【보도, 2026-06】 대우건설: 과천 G-TOWN 현장에서 아침조회, TBM, 안전교육을 다국어로 실시간 제공하고, 외국인은 QR을 찍으면 바로 번역을 봅니다. 롯데이노베이트와 건설 은어·전문용어 사전을 반영한 전용 번역기를 자체 개발했습니다(구매형이 아님) — [한국경제 (2026-06)](https://www.hankyung.com/amp/2026062443536), [SBS Biz](https://biz.sbs.co.kr/amp/article/20000318557), [헤럴드K](https://www.heraldk.com/article/2026062316093279286)
- 【보도】 롯데건설: 2025-07 롯데이노베이트와 건설 특화 번역 모델을 자체 개발해 전국 40개 현장에 도입했고, 20개 언어를 지원합니다 — [스마트투데이](https://www.smarttoday.co.kr/ko-kr/articles/107971) (검색 요약 기준, 해당 기사로 추정)
- 【보도, 2026-09】 플리토 × 한화오션·한화시스템 '오톡(OTalk)': 조선소 은어·사투리 데이터로 맞춤 용어집을 만들었습니다. 7개 언어(한·영·베트남·태국 등), 경상도 억양 인식, 5단계 수음 조정 등 10여 개 기능. 시범운영에서 외국인 근로자 사용률 약 96%(플리토 발표)였고 협력사 근로자로 확대했습니다 — [벤처스퀘어](https://www.venturesquare.net/1114035/), [MTN](https://news.mtn.co.kr/news-detail/2026091610011317518), [이코노미스트](https://economist.co.kr/article/view/ecn202609160012)
- 【보도】 HD한국조선해양도 외국인 근로자용 AI 번역 기술을 발표했습니다 — [Business & Human Rights Resource Centre](https://www.business-humanrights.org/my/%E1%80%9E%E1%80%90%E1%80%84/s-korea-hd-korea-shipbuilding-says-new-ai-translation-tech-will-support-migrant-workers-guarantee-safety-on-worksites)

**스타트업·중견 솔루션**
- 【보도, 2026-07】 KS인더스트리 'Ami' + 기업용 'AmiX': 조선·국방·제조 현장용, 24개 언어, 근로자·관리자가 직접 등록하는 산업 용어 사전, **가입 절차 없이 마이크 버튼만으로** 1:1 순차 통역과 다국어 통역룸을 씁니다. 정서지원 AI 친구·학습 콘텐츠도 있고, 스마트글라스 정비 솔루션 'SentinAI'로 가는 발판입니다. 특허 5건 출원 — [아시아경제 (2026-07)](https://view.asiae.co.kr/article/2026071315392438871), [딜사이트](https://dealsite.co.kr/articles/165267), [App Store: Ami](https://apps.apple.com/kr/app/ami-ai-%ED%95%A8%EA%BB%98-%EB%B3%B4%EA%B3%A0-%EB%8C%80%ED%99%94%ED%95%B4%EC%9A%94/id6689519949)
- 【보도, 2025-10】 켐토피아 '안전 다통해': 40여 개국 이상 언어로 실시간 안전교육, 위험성평가 기반 작업안전행동 지도, TBM·안전교육 현장 실시간 통역 — [헤럴드K (2025-10)](https://www.heraldk.com/article/2025101917230028734)
- 【보도, 2026-09】 플리토 × 대한산업안전협회 MOU: 안전보건교육용 실시간 다국어 통번역 체계와 산업안전 전문용어 DB를 구축하고, 협회의 AI 전산관리 솔루션에 통번역 API를 연동해 위험성평가·TBM을 다국어로 제공합니다. 플리토는 이미 '라이브 트랜스레이션'을 외국인 근로자 안전교육에 적용 중입니다 — [바이라인네트워크 (2026-09)](https://byline.network/2026/09/93849284902/), [헬로티](https://www.hellot.net/mobile/article.html?no=114869)
- 【보도, 2025-04】 플리토는 CU 편의점에서도 AI 통번역 솔루션을 시범 도입했습니다 — [Asiae EN](https://www.asiae.co.kr/en/article/2025040316464789636)
- 【보도, 2025-01】 '안전함'(한국스마트안전보건협회): 관리자 음성 방송을 스마트안전모로 실시간 통역해 전달하고 다국어 통역도 지원합니다. 3,000여 현장, 20만여 명 근로자가 사용했다고 주장합니다 — [CEO스코어데일리](https://www.ceoscoredaily.com/page/view/2025012420124529856)

**공공 프로그램 신호**
- 【보도, 2026-02】 부산진해경제자유구역청: 외국인 근로자 20인 이상을 고용한 입주기업 5곳을 시범 선정해 3월부터 1년간 실시간 다국어 AI 통역 앱 서비스를 무상 제공합니다 — [헤럴드K (2026-02)](https://www.heraldk.com/article/2026020818184417742)
- 【보도/정부, 2026-03】 고용노동부: 한국어 소통이 되는 합법 체류 외국인 200명을 '외국인 안전리더'로 양성합니다(AI 앱이 아니라 사람 통역 모델) — [고용노동부](https://moel.go.kr/news/enews/report/enewsView.do?news_seq=19074), [경기일보](https://www.kyeonggi.com/article/20260315580099) (검색 요약 기준)
- KOSHA(안전보건공단)가 직접 운영하는 AI 통역 앱은 검색에서 확인되지 않았습니다.

**외국인 대상 플랫폼 투자 동향 (인접)**
- 【보도】 워크비자(외국인 합법 구인구직): MYSC 프리시드(금액 비공개). 하이어다이버시티('하이어비자', 체류 행정): 2025-04 시리즈 A 50억 원(스톤브릿지·뮤렉스). JB인베스트먼트: 100억 원 규모 '제이비외국인플랫폼투자조합1호' 결성. VC들은 외국인 대상 스타트업이 M&A될 가능성이 높다고 봅니다 — [머니투데이 (2025-04)](https://www.mt.co.kr/future/2025/04/29/2025042817023749710), [유니콘팩토리 워크비자](https://www.unicornfactory.co.kr/hashtag/워크비자)

**다문화·학교 알림 번역**
- 【공식 앱스토어】 하이클래스(아이스크림미디어) 앱 설명에는 알림장 기능이 있지만 번역 기능은 확인되지 않았습니다 — [App Store KR: 하이클래스](https://apps.apple.com/KR/app/id1472488819)
- 【보도, 2020】 클래스팅 e알리미: 모바일 가정통신문을 카카오톡 알림톡으로 자동 발송하고 설문·전자서명을 지원합니다. 번역 언급은 없습니다 — [한국교육신문](https://hangyo.com/mobile/article.html?no=90879)
- 【학술, 2022】 서울 64개교 다문화 초등생 학부모 100명 연구: 모국어 번역 알림장이 교육정보 격차 해소, 학교 부적응 해소, 학습동기에 긍정적 효과 — [교보 스콜라](https://scholar.kyobobook.co.kr/article/detail/4050036984081)
- 【보도, 2025-12】 클레이언(Klayon) 'LXHUB': 외국인 학부모 상담용 AI 실시간 통역을 서울 학교 현장에서 시연 — [Asiae EN](https://www.asiae.co.kr/en/article/2025121110373789715)
- 【보도, 2025-01】 행정안전부: 민원서식 235종을 10개 언어로 번역해 제공 — [Asiae EN](https://www.asiae.co.kr/en/article/2025010510032112151)

### Inferences
- 한국 B2B 현장 시장은 "관리자 1명 → 외국인 N명" 방송·TBM·안전교육 구조(1:N)가 중심입니다. hiWorker의 "1:N 동시 통역", 어깨동무M의 국적별 공지 번역, 안전함의 안전모 방송이 그 예입니다. 근로자끼리 국적이 섞여 서로 대화하는 N:N 혼합 언어 단체방은 주력 기능이 아닌 것으로 보입니다. KS인더스트리의 "다국어 통역룸"이 가장 가깝습니다.
- 대형 건설·조선사(대우, 롯데, DL, 한화, HD현대)는 자체 구축하거나 대형 벤더(롯데이노베이트, 플리토, 한화시스템)와 손잡습니다. 따라서 스타트업이 공략할 곳은 중소 제조·농축산·어업·물류·소규모 건설 하도급, 그리고 회사 밖 생활 영역(기숙사, 집주인, 교회·공동체, 다문화 가족, 학부모)입니다.
- 부산진해경자청의 무상 제공 사업은 지자체·공공 예산으로 구매하는 경로(B2G2B)가 있다는 신호입니다.
- 학교·학부모 소통 앱(하이클래스, 클래스팅)에 번역 기능이 확인되지 않은 점, 그리고 번역 알림장의 효과를 보여주는 학술 근거가 있는 점은 "학급 학부모 단체방" 세그먼트의 빈자리를 시사합니다. 단, 검색 한계로 기능이 없다는 것을 확정할 수는 없습니다.
- 하이로컬의 피벗(언어교환 소셜 → B2B 현장 SaaS)은, 소비자 대상 언어 소통 앱의 수익화가 어려워 B2B로 옮겨간 국내 사례로 읽힙니다.

### Gaps
- hiWorker의 가격, 고객 수, 2023년 이후 추가 투자, 지원 언어 목록(네팔어·크메르어·버마어·우즈베크어 포함 여부), 근로자끼리 그룹채팅이 되는지: 앱스토어와 한경 원문 접속 실패, 검색 한도 소진.
- 포스코(포스코이앤씨) 외국인 근로자 회화집(phrasebook) 앱: 이번 조사에서 새 정보를 찾지 못했습니다.
- 켐토피아·Ami·안전함의 가격과 실제 도입 실적.
- 다문화 가족 소통 앱(다누리 등): 검색 한도 소진으로 미조사.
- 하이클래스·클래스팅·e알리미 번역 기능의 최신 여부: 공식 FAQ를 직접 확인하지 못함.
- 시프티, 알바몬·알바천국의 외국인 근로자용 번역 기능: 미조사.

---

## Q3. 프론트라인·데스크리스 근로자 커뮤니케이션 플랫폼의 번역 기능, 가격, 대상, 아시아 진출

### Takeaway
Beekeeper(100+ 언어 인라인 번역, 채팅 포함), Flip(DeepL, 50~60+ 언어, 메시지 자동 번역), Zoom Workplace for Frontline(채팅 메시지를 사용자 선호 언어로 자동 번역, 36개 언어), Connecteam(채팅은 메시지별 수동 번역, 공지 자동번역은 Expert 플랜), Blink·Speakap·Staffbase(주로 피드·게시물 번역, 유료 애드온)가 있습니다. 이들은 기술적으로 "개인별 번역"을 하지만 **회사가 계정을 발급하는 B2B 좌석형**입니다. 한국·아시아 진출은 검색에서 확인되지 않았습니다. Meta Workplace는 2026-06-01 종료 예정이었고, Beekeeper는 2025-07 LumApps와 합병했습니다(합산 가치 10억 달러 이상).

### Cited Findings
- 【공식】 Beekeeper: 인라인 번역을 Streams(피드)에서 시작해 Chat 메시지, Campaigns, Surveys로 넓혔습니다. 마케팅 페이지는 100+ 언어라고 하고, 초기 보도자료는 30개 언어였습니다 — [Beekeeper 블로그](https://www.beekeeper.io/?p=33931), [Hospitality Net](https://www.hospitalitynet.org/news/4084611.html)
- 【제3자】 Beekeeper 가격: GetApp은 사용자당 월 4(통화 미표기), 상위 6으로 표시합니다. G2에는 공식 가격 정보가 없습니다 — [GetApp](https://www.getapp.com/hr-employee-management-software/a/beekeeper/)
- 【보도】 Beekeeper 투자: 2022-11 시리즈 C 5,000만 달러, 2025-03 HSBC 이노베이션뱅킹 3,500만 달러(부채성), CB Insights 기준 누적 1억 7,101만 달러/13라운드. 2025-07 LumApps와 합병해 합산 가치 10억 달러 이상 — [Hospitality Net (Series C)](https://www.hospitalitynet.org/news/4113435.html), [Venture Kick](https://www.venturekick.ch/Beekeeper-secures-USD-35M-to-expand-frontline-workforce-platform), [CB Insights](https://www.cbinsights.com/company/beekeeper/financials), [Seedtable](https://seedtable.com/exits/beekeeper)
- 【공식 도움말】 Connecteam: 채팅은 앱 언어와 다른 메시지를 감지해 "Translate" 버튼을 보여주는 **메시지별 수동 번역**이고, 관리자가 켜고 끕니다. Updates(공지) 자동번역은 Communications Hub Expert 플랜 이상에서 추가 비용 없이 제공됩니다 — [Connecteam 도움말: 채팅 번역](https://help.connecteam.com/en/articles/15013840-translating-messages-in-the-chat), [Connecteam 도움말: Updates 자동번역](https://help.connecteam.com/en/articles/7900512-updates-automatic-translation)
- 【제3자】 Connecteam 가격: Expert는 허브당 월 99달러(연간)/119달러(월간)이며 30명까지 포함, 초과 사용자는 Communications Hub 기준 1인당 월 3달러(연간) 또는 3.6달러(월간) — [People Managing People](https://peoplemanagingpeople.com/tools/connecteam-pricing/), [noon.ai](https://www.noon.ai/blog/articles/431-connecteam-pricing-2026)
- 【공식】 Flip(독일): "50+ languages, automatically and in real time"(광고 페이지는 60+). DeepL 기반이며 앱스토어 설명은 "messages are automatically translated into your colleagues' language". KFC/Queensway 사례는 35+ 언어 tap-to-translate — [Flip 직원앱](https://www.getflip.com/platform/employee-app/), [Flip 광고 페이지](https://www.getflip.com/insights/ads/flip-employee-app/), [KFC 사례](https://www.getflip.com/customer-stories/kfc-queensway-europe/), [App Store: Flip](https://apps.apple.com/us/app/-/id1505736692)
- 【공식 도움말】 Speakap: Google Translate 기반 자동번역, 주로 새 게시물 대상, 유료 프리미엄 애드온 — [Speakap 도움말](https://support.speakap.com/hc/en-us/articles/28649746422172-Automatic-Translations-in-Speakap)
- 【공식 도움말】 Staffbase: 커뮤니케이션 콘텐츠 자동번역은 Staffbase가 활성화해야 하는 유료 기능 — [Staffbase 도움말](https://support.staffbase.com/hc/en-us/articles/12645272702738-How-to-automatically-translate-Staffbase-content-in-Communications-Control)
- 【공식 도움말】 Blink: 피드 게시물·댓글·페이지에 90+ 언어(Microsoft Translator가 지원하는 모든 언어), 자동번역은 추가 비용 프리미엄 애드온 — [Blink 도움말](https://helpdesk.joinblink.com/en/articles/6979853-on-demand-translation), [Blink 언어](https://helpdesk.joinblink.com/en/articles/6979854-different-languages-on-blink)
- 【공식 도움말】 Workvivo(Zoom): Amazon Translate 기반 화면 번역(웹·모바일). 새 언어를 추가하려면 엔지니어링 작업이 필요합니다 — [Workvivo 도움말](https://support.workvivo.com/hc/en-gb/articles/4918031966365)
- 【공식】 Zoom Workplace for Frontline: 채팅 메시지를 사용자 선호 언어로 자동 번역하고, 근무조 기반 채팅그룹을 자동 생성합니다. 2025-04 출시. 파트너 자료 기준 AI Companion 콘텐츠 번역 36개 언어 — [Zoom Frontline](https://www.zoom.com/en/frontline-workers/), [HIT Consultant (2025-04)](https://hitconsultant.net/2025/04/16/zoom-launches-ai-workplace-platform-for-frontline-workers/), [Presidio 브리프 (2026-06)](https://www.presidio.com/wp-content/uploads/2026/06/Zoom-Workplace-Solutions-Brief-_-AI-Companion.pdf)
- 【제3자】 Yoobic: 태스크·커뮤니케이션·모바일 러닝 올인원. 자동 채팅 번역은 확인되지 않음 — [SourceForge 비교](https://www.sourceforge.net/software/compare/Workvivo-vs-YOOBIC)
- 【보도/공식】 Workplace from Meta: 2025-08-31 정상 이용 종료, 2025-09-01~2026-05-31 읽기·다운로드 전용, 2026-06-01 접근 종료·삭제 예정. 유일한 공식 이전 파트너는 Workvivo by Zoom입니다. 2025-09부터 종료 시까지 무료 — [YOOBIC 블로그](https://yoobic.com/blog/meta-is-closing-workplace/), [People Matters](https://www.peoplematters.in/news/employee-engagement/meta-pulls-the-plug-on-workplace-its-enterprise-social-network-41315), [Mobile World Live](https://mobileworldlive.com/meta/meta-platforms-to-shutter-enterprise-app-workplace)
- 【공식/제3자】 Microsoft Teams: 사용자별 설정으로 "자동 번역" 켜기, 번역하지 않을 언어 선택, 선호 언어는 기본값이 OS 언어. 모바일 100+ 언어, 데스크톱 자동번역은 2024-04~05 롤아웃 — [Microsoft Translator 블로그 (2022-10)](https://www.microsoft.com/en-us/translator/blog/2022/10/24/announcing-intelligent-message-translation-in-microsoft-teams-for-mobile-devices/), [M365 Admin](https://m365admin.handsontek.net/microsoft-teams-intelligent-message-translation-in-chats/), [SuperSimple365](https://supersimple365.com/intelligent-message-translation-in-teams-chat-on-desktop)

### Inferences
- 프론트라인 플랫폼들은 "공지·피드 번역"을 먼저 만들고 채팅은 나중에 붙였습니다(Beekeeper가 대표적). 번역은 대부분 유료 애드온이거나 상위 플랜입니다(Speakap, Staffbase, Blink, Connecteam). 즉 번역이 업셀 수단이라는 점에서 기업이 지불 의사를 갖는다는 검증 신호입니다.
- 이들은 모두 Microsoft·Google·DeepL·Amazon 엔진을 감싼 형태라 롱테일 언어 지원은 엔진에 따라 갈립니다. DeepL 기반인 Flip은 동남·남아시아 롱테일 언어에 약할 가능성이 있습니다(추론, DeepL 언어 목록 미검증). Microsoft 기반 Blink(90+)는 넓을 가능성이 큽니다.
- 한국 내 영업 흔적이 검색에 전혀 없어 한국 중소 현장에서는 당장 위협이 낮습니다. 다만 Zoom(Workvivo+Frontline)과 Microsoft(Teams Frontline)는 글로벌 확장 단계에서 B2B 경쟁자가 됩니다.
- Meta Workplace 종료와 Beekeeper-LumApps 합병은, 프론트라인 커뮤니케이션이 "독립 소셜형"에서 "대형 스위트 통합형"으로 재편되고 있다는 신호입니다.

### Gaps
- Microsoft Teams Frontline(F 라이선스)과 일반 Teams의 번역 기능 차이: 확인 안 됨.
- 각 플랫폼의 한국·아시아 고객과 현지 법인: 검색 결과 없음.
- Beekeeper·Flip·Zoom의 정확한 언어 목록(네팔어·크메르어·버마어 등 포함 여부).
- Staffbase·Flip·Speakap 좌석당 공식 가격.

---

## Q4. 한국 SME용 협업툴(잔디, 네이버웍스, 플로우, 카카오워크, 시프티, 알바몬·알바천국)의 번역 기능과 외국인 현장 타깃 여부 (+ Lark 무료 플랜)

### Takeaway
네이버웍스는 메시지방 단위 "자동 통역"이 있어(사용자가 정한 언어로 표시, LINE WORKS 기준 전 플랜) 기능상 가장 근접한 국내 협업툴입니다. 잔디는 AI '스프링클러'로 14개 언어 입력 번역과 원클릭 수신 번역을 제공합니다. 플로우의 번역 기능은 확인되지 않았고, 카카오워크는 종료 공지가 없습니다. **Lark의 무료 Starter 플랜(최대 20명)은 무제한 실시간 번역과 18개 언어 자동번역을 제공**해, 회사 계정 장벽이 사실상 낮은 무료 대안입니다. 다만 이들 모두 "조직(테넌트)"을 만들어야 하고, 지원 언어가 주요 언어 위주여서 외국인 근로자 롱테일 언어나 현장 타깃은 확인되지 않았습니다.

### Cited Findings
- 【공식 도움말】 네이버웍스: 메시지방에서 특정 메시지를 번역하거나 대화를 자동 통역하도록 설정할 수 있고, 상대 언어와 무관하게 내가 정한 언어로 통역됩니다 — [네이버웍스 도움말: 메시지 번역 및 통역](https://help.worksmobile.com/ko/use-guides/message/check-message/translation/)
- 【보도, 2022】 네이버웍스: 9개국 언어 메시지 자동 통번역 — [ZDNet Korea (2022-04)](https://zdnet.co.kr/view/?no=20220426084420)
- 【공식 도움말】 네이버웍스 노트·메일 번역 언어: 영어, 일본어, 중국어(간체/번체), 프랑스어, 베트남어, 태국어, 인도네시아어, 스페인어, 포르투갈어. 메시지도 같은 목록인지는 미확인 — [네이버웍스 도움말: 메일 번역](https://help.worksmobile.com/ko/use-guides/mail/check-mail/translate-mail/)
- 【공식 도움말】 LINE WORKS(일본): 트크 번역·자동 통역은 "LINE WORKS 서비스의 모든 플랜에서 이용 가능" — [LINE WORKS 도움말 (JA)](https://help.worksmobile.com/ja/use-guides/message/check-message/translation/)
- 【보도, 2025-07】 잔디(토스랩): AI '스프링클러'로 입력창에서 영어·일본어·중국어·베트남어 등 14개 언어 실시간 번역, 외국어 수신 메시지 원클릭 번역(더네이쳐홀딩스 사례) — [디지털데일리 (2025-07)](https://www.ddaily.co.kr/page/view/2025070110345670183), [벤처스퀘어](https://www.venturesquare.net/990342/)
- 【공식 블로그, 2020】 잔디: Google 번역 API로 번역 봇을 직접 만드는 가이드(기본 기능 아님) — [JANDI 블로그](https://blog.jandi.com/blog/2020/02/jandi-google-translation/)
- 【공식/보도】 플로우(마드라스체크): 번역 기능은 확인되지 않음(언어 선택 설정만 있음). 2026-09 ChatGPT·Claude 공식 앱 등록 — [App Store: flow](https://apps.apple.com/us/app/flow-ai-collaboration-tool/id939143477?l=ar), [바이라인네트워크 (2026-09)](https://byline.network/2026/09/17-600/)
- 【공식】 카카오워크: 종료 공지나 보도는 확인되지 않았고 앱 업데이트가 계속되는 것으로 보입니다. 2020-09 출시 — [App Store KR: 카카오워크](https://apps.apple.com/KR/app/id1505289743), [카카오 보도자료](https://www.kakaocorp.com/page/detail/8823)
- 【공식】 Lark 요금제(한국어 페이지): Starter(무료)에 "무제한 실시간 번역"이 포함되고, 채팅·문서·메일 AI 번역이 무제한입니다. Starter는 최대 20명, 100GB, 메시지 기록 18개월 — [Lark 요금제 (KO)](https://www.larksuite.com/ko_kr/plans), [Lark 요금제 (EN)](https://www.larksuite.com/en_us/plans)
- 【공식】 Lark 메신저: "auto-translate all the messages to your own language", 18개 언어(영어, 중국어 간체/번체, 일본어, 한국어, 태국어, 프랑스어, 독일어, 스페인어, 러시아어, 아랍어, 베트남어 등) — [Lark Messenger](https://www.larksuite.com/en_us/product/messenger?from=zero), [Lark 블로그](https://www.larksuite.com/blog/chat-translation)

### Inferences
- Lark 무료 플랜은 "회사 계정 없음" 조건을 기술적으로 거의 충족하는 가장 위험한 무료 대체재입니다(20명 이하 소규모 현장·동호회). 하지만 (a) 조직 생성·이메일 초대 같은 업무툴 온보딩, (b) 18개 언어에 네팔어·크메르어·버마어·우즈베크어·몽골어·싱할라어가 빠져 있을 가능성(위 목록 기준), (c) 한국 현장 인지도 부족이 한계입니다.
- 네이버웍스는 한국 SME 유통력과 메시지 자동 통역을 모두 갖춰, "외국인 근로자 현장용 패키지"를 내면 즉시 위협이 될 수 있습니다. 현재 언어 목록(9~10개)은 동남아 주요 언어(베트남·태국·인도네시아)까지만 포함하는 것으로 보입니다.
- 국내 협업툴 중 외국인 근로자 현장을 명시적으로 타깃한 사례는 검색에서 확인되지 않았습니다.

### Gaps
- 시프티(근태관리), 알바몬·알바천국의 외국인용 번역·소통 기능: 검색 한도 소진으로 미조사.
- 네이버웍스 메시지 자동 통역의 현재 언어 목록과 무료 플랜 포함 여부(한국판).
- 잔디 스프링클러의 요금제 조건.
- Lark 18개 언어 전체 목록(인도네시아어·타갈로그어 포함 여부).

---

## Q5. 이주민이 많이 쓰는 메신저(Zalo, Viber, IMO, Messenger)와 주요 소비자 메신저의 그룹 자동번역 현황

### Takeaway
2026-11 기준, 회사 계정 없이 쓰는 소비자 메신저 중 **그룹에서 "읽는 사람마다 자동으로 자기 언어"를 무료로, 롱테일 언어까지** 해주는 곳은 확인되지 않았습니다. WhatsApp은 수동 번역(Android 6개, iOS 19+ 언어)에 iOS 자동번역(약 21개 언어)을 베타 중이고, Telegram은 Premium 사용자에게 채팅 전체 번역을 줍니다. Zalo는 길게 눌러 번역 + zCloud(유료 클라우드) 사용자에게 자동번역 옵션, Viber는 길게 눌러 번역(Google 엔진), KakaoTalk은 말풍선 번역 + 발송 메시지 번역(19개 언어), iMessage는 iOS 26 9개 언어 자동번역입니다. Galaxy AI는 KakaoTalk·WhatsApp 등 타사 앱 위에서 채팅 번역을 해줍니다. **Google Chat "Translate for me"의 개인 계정 확대 여부는 공식(Workspace 유료 애드온 전용)과 보도(개인 계정 포함) 사이에 충돌이 있습니다.**

### Cited Findings
- 【공식 블로그】 WhatsApp 메시지 번역: Android는 영어·스페인어·힌디어·포르투갈어·러시아어·아랍어 6개로 시작했고, iPhone은 19+ 언어 — [WhatsApp 블로그](https://blog.whatsapp.com/introducing-message-translations)
- 【보도】 iOS 언어에는 한국어, 베트남어, 일본어 등이 포함됩니다(2025-09~10) — [MacRumors](https://www.macrumors.com/2025/09/24/whatsapp-rolls-out-message-translation/)
- 【보도, 2026-03, 베타】 iOS 자동 메시지 번역 베타, 1단계 약 21개 언어, Apple 온디바이스 언어팩 사용(E2E 유지). 전체 사용자 출시는 미확인 — [9to5Mac (2026-03)](https://9to5mac.com/2026/03/20/whatsapp-for-iphone-may-soon-offer-automatic-message-translation-across-21-languages/)
- 【제3자】 Telegram: 다른 언어 그룹·채널 상단에 번역 바가 뜨고, 누르면 새 메시지까지 전체 번역합니다(Premium 기능). Premium 약 월 4.99달러(앱스토어), @PremiumBot 경유 약 3.99달러 — [messengerbot.app (제3자 블로그)](https://messengerbot.app/?p=263019)
- 【제3자, 사용자 불만】 Telegram 버그트래커: 번역이 자주 취소되거나 매우 오래 걸린다는 불만, 그룹 번역이 오류로 비활성화되는 사례 — [Telegram Bugs #51699](https://bugs.telegram.org/c/51699/223), [Telegram Bugs #16062 (그룹 자동번역 요청)](https://bugs.telegram.org/c/16062/3)
- 【보도】 Zalo: zCloud 사용자 그룹에 "자동 메시지 번역 및 번역본 전송" 옵션이 추가되었고, iPhone에서는 iOS 번역 앱과 결합해 영어·중국어·한국어 외 17개 언어를 더 지원합니다(일자 불명확) — [VnExpress](https://vnexpress.net/ba-tinh-nang-moi-cua-zalo-5097444.html)
- 【제3자】 Zalo 기본 사용법: 메시지를 길게 눌러 "Dịch"(번역) 선택. 최신 OS 기기에서만 됩니다 — [XTmobile](https://www.xtmobile.vn/cach-dich-tin-nhan-tren-zalo)
- 【제3자】 Zalo Web은 비공식 Chrome 확장으로 자동 번역합니다(공식 기능 아님) — [Chrome Web Store](https://chromewebstore.google.com/detail/abeeejocabhdahopehakmmgmdfkbnemb)
- 【제3자, 2018 기준】 Viber: 메시지를 길게 눌러 번역하면 원문 아래에 번역이 나옵니다. 앱 설정 언어 기준, Google Translate 엔진. 그룹 자동번역 근거는 없음 — [cbw.ge](https://cbw.ge/world/8-viber-features-about-which-you-must-know). 2026-04로 표시된 "Viber gets in-chat translation" 기사가 있으나 실제 날짜와 내용을 확인하지 못했습니다 — [iClarified](https://www.iclarified.com/67313/viber-gets-inchat-translation-feature-video)
- 【보도】 KakaoTalk: 기존 "말풍선 번역"(받은 메시지)을 확장해 발송 메시지까지 번역해 보낼 수 있게 했고, 19개 언어입니다(2024년 말, v11.3.0 무렵, 검색 요약 기준) — [TV리포트](https://tvreport.co.kr/msn/article/868521/), [인사이트](https://www.insight.co.kr/news/156976) (원문 날짜 미확인)
- 【공식】 KakaoTalk 6차 정기 업데이트(2026-07-15, v26.6.0): 채팅방별 대화 요약, ChatGPT for Kakao PC 확대, 오픈채팅 챗봇(beta). 자동번역 언급은 없음 — [카카오 보도자료](https://www.kakaocorp.com/page/detail/12082)
- 【공식】 LINE: 2026년 안에 토크방에서 "Agent i in chat"을 부르는 기능을 제공할 예정입니다. 현재 AI 기능은 답장 제안, 화제 제안, 무드 분석, 어조 변환, 오타 수정(무료 하루 3회). 개인 LINE 자동번역 통합은 확인되지 않음 — [LY Corp 보도자료](https://www.lycorp.co.jp/ja/news/release/020594/), [jetstream.blog (2025-09)](https://jetstream.blog/2025/09/05/line-ai-talk-suggest-public/)
- 【보도】 iMessage(iOS 26) Live Translation: 9개 언어(영어, 프랑스어, 독일어, 이탈리아어, 일본어, 한국어, 포르투갈어, 스페인어, 중국어 간체). 그룹채팅에도 적용되고 Apple Intelligence 기기·언어팩이 필요합니다 — [AppleInsider](https://appleinsider.com/articles/25/06/11/new-ios-26-translation-tool-works-inside-calls-chats-video), [Engadget](https://www.engadget.com/big-tech/apple-introduces-ai-powered-live-translation-tools-at-wwdc-2025-173605234.html), [BGR](https://bgr.com/2018777/how-to-use-best-new-iphone-messages-features-ios-26-guide)
- 【공식/보도】 Galaxy AI Chat Translation: Samsung Messages, Google Messages, KakaoTalk, WhatsApp, Instagram, Google Chat, Signal, LINE 등 타사 앱에서 동작합니다(국가별 상이). 2024-04 기준 13개 언어로 출발해 이후 추가 — [Samsung Newsroom AU](https://news.samsung.com/au/galaxy-ai-now-supports-more-languages-with-latest-update), [Korea Daily](https://en.koreadaily.com/?p=37415)
- 【보도】 Galaxy Live Translate(통화): One UI 6.1.1부터 KakaoTalk, WhatsApp, Telegram, LINE, WeChat 등 타사 음성통화에 적용 — [GSMArena](https://m.gsmarena.com/samsung_live_translate_third_party_voice_calling_apps-news-63751.php)
- 【공식】 Google Chat "Translate for me": Gemini Business/Enterprise 또는 AI Meetings and Messaging 애드온이 있는 Workspace 고객 대상. 2024-12-13(Rapid), 2025-01-15(Scheduled) 롤아웃 — [Workspace Updates 블로그](https://workspaceupdates.googleblog.com/2024/12/translate-for-me-in-google-chat.html)
- 【보도, 충돌】 9to5Google·PhoneArena는 이 Chat 개편이 개인 Google 계정에도 적용된다고 보도했습니다(웹 먼저, 모바일 나중) — [9to5Google (2024-12)](https://9to5google.com/2024/12/13/google-chat-translation/), [PhoneArena](https://www.phonearena.com/news/google-chat-generative-ai-automatic-translation-feature-for-workspace_id165878)

### Inferences
- 기존 메신저의 번역은 대부분 (a) 수동(길게 눌러 번역), (b) 유료(Telegram Premium, Zalo zCloud), (c) 언어 수가 적음(온디바이스 언어팩 기반 iMessage 9개, WhatsApp iOS 약 21개), (d) 특정 OS 전용(WhatsApp Android 자동번역, iMessage) 중 하나 이상의 제약이 있습니다. "혼합 3개 이상 언어 + 모든 독자 무료 + 롱테일 언어" 조합은 아직 비어 있습니다.
- 온디바이스 번역(Apple·WhatsApp iOS)은 E2E 암호화를 지키는 대신 언어 수가 제한됩니다. 네팔어·크메르어·버마어·우즈베크어·싱할라어·몽골어 같은 저자원 언어는 늦게 들어갈 가능성이 큽니다(추론). 서버 번역을 쓰는 신규 앱은 이 공백을 노릴 수 있지만, 프라이버시 메시징에서는 불리합니다.
- Galaxy AI는 KakaoTalk 위에서 OS 단계 번역을 해줍니다. 한국 갤럭시 점유율을 생각하면, "카톡 그대로 쓰고 폰이 번역"하는 대안이 될 수 있습니다. 다만 사용자 본인 기기 기준(독자 각각 갤럭시 필요)이고 언어 수가 제한됩니다.
- Google Chat이 개인 계정에 개인별 자동번역(120+ 언어)을 연다면 기능상 가장 완벽한 무료 대체재가 됩니다. 하지만 한국 이주민·관리자 사이의 Google Chat 사용률은 낮을 것으로 보입니다(추론, 미검증).

### Gaps
- IMO, Facebook Messenger의 번역 기능: 검색 한도 소진으로 미조사.
- Telegram 공식 문서(telegram.org) 기준의 번역 기능·가격 확인 못 함(제3자 블로그만 확인).
- Zalo 자동번역의 출시일, 무료 여부, 그룹 적용 범위.
- KakaoTalk 19개 언어 목록과 받은 메시지 자동 번역(설정형)이 있는지.
- Google Chat 개인 계정의 "Translate for me" 현재 제공 상태(2025년 이후 출처 없음).

---

## Q6. 시장 검증·실패 신호 (투자, 종료, 피벗, 앱 리뷰 불만)

### Takeaway
검증 신호는 주로 **B2B 현장 안전 통역**과 **프론트라인 플랫폼**에 몰려 있습니다. 하이로컬 카카오벤처스 투자와 HJ중공업 도입, 플리토-한화오션·대한산업안전협회, KS인더스트리 출시, 지자체 무상 지원, Beekeeper-LumApps 10억 달러+ 합병이 그 예입니다. 반면 **소비자용 다자간 번역 대화**는 실패·철수 신호가 많습니다. Microsoft Translator Converse 종료(2026-06), Amazon SayHi 종료(2024-08), DoTalk 정체, Meta Workplace 종료가 있고, 하이로컬은 소셜 언어교환에서 B2B로 피벗했습니다. 앱 리뷰 불만의 핵심은 "번역 지연·실패"와 "저자원 언어 품질"입니다.

### Cited Findings
- 【보도】 하이로컬: 2023-01 카카오벤처스 투자, 누적 약 15억 원 — [유니콘팩토리 (추정)](https://www.unicornfactory.co.kr/article/2024102215582058284); 2026-09 HJ중공업 전국 현장 도입 — [한경 머니](https://magazine.hankyung.com/money/article/202609043973c)
- 【보도】 애니챗: 인도네시아 파트너사 260억 원(약 2,000만 달러) "베팅" 보도(연도·집행 미확인) — [더구루](https://www.theguru.co.kr/news/article.html?no=55007)
- 【공식】 JotMe: a16z 관련 투자를 시사하는 자사 블로그(금액 미확인) — [JotMe 블로그](https://jotme.io/blog/jotme-a16z)
- 【보도】 Beekeeper: 시리즈 C 5,000만 달러(2022-11), HSBC 3,500만 달러(2025-03), LumApps 합병(2025-07, 합산 10억 달러+) — [Hospitality Net](https://www.hospitalitynet.org/news/4113435.html), [Venture Kick](https://www.venturekick.ch/Beekeeper-secures-USD-35M-to-expand-frontline-workforce-platform), [Seedtable](https://seedtable.com/exits/beekeeper)
- 【보도】 외국인 대상 플랫폼: 하이어다이버시티 시리즈 A 50억 원(2025-04), JB인베스트먼트 100억 원 전용 조합 — [머니투데이](https://www.mt.co.kr/future/2025/04/29/2025042817023749710)
- 【보도】 공공: 부산진해경자청 AI 통역 앱 무상 제공(2026) — [헤럴드K](https://www.heraldk.com/article/2026020818184417742)
- 【공식 릴리스노트/보도】 Microsoft Translator 다중기기 대화 종료(2026-06-30) — [WhistleOut](https://www.whistleout.com/CellPhones/Guides/is-microsoft-translator-worth-downloading), [APKMirror](https://www.apkmirror.com/apk/microsoft/microsoft-translator/)
- 【제3자, 포럼, 신뢰도 낮음】 Amazon SayHi 종료(2024-08-05) — [rblind](https://rblind.com/post/6611706)
- 【보도】 Meta Workplace 종료(2026-06-01 삭제 예정) — [YOOBIC 블로그](https://yoobic.com/blog/meta-is-closing-workplace/)
- 【보도】 DoTalk: 2017 보도 이후 활동이 거의 확인되지 않음 — [Startup Daily 아카이브](https://archive.startupdaily.net/?p=63697)
- 【보도】 하이로컬 피벗: 외국인 음성 대화 플랫폼 → B2B 현장 안전교육·통번역 — [혁신의숲](https://www.innoforest.co.kr/company/CP00001746/%ED%95%98%EC%9D%B4%EB%A1%9C%EC%BB%AC)
- 【제3자, 리뷰 분석】 같은 앱이 독일어→영어는 출판 수준인데 타갈로그어→영어는 쓸 수 없는 수준이었다는 1~3점 리뷰. 화상통화 번역은 지연, 누락, 다음 화자와 겹침 — [Unstar](https://unstar.app/blog/google-translate-deepl-itranslate-microsoft-translator-translation-apps-ranked-2026)
- 【제3자, 사용자 불만】 Telegram 번역이 자주 취소되거나 오래 걸림 — [Telegram Bugs](https://bugs.telegram.org/c/51699/223)
- 【보도】 한화오션 오톡 시범 사용률 96%(플리토 발표) — 현장 맞춤(은어·사투리 용어집)이 채택률을 좌우한다는 주장 — [벤처스퀘어](https://www.venturesquare.net/1114035/)

### Inferences
- 소비자 다자간 번역 앱은 "가끔 쓰는 여행·회의용 일회성 도구"로 머물렀고, 반복 사용과 수익화에 실패한 것으로 보입니다(Microsoft와 Amazon 철수, DoTalk 정체). 이 사업은 일회성 통역이 아니라 **상시 관계형 그룹(같은 현장, 같은 기숙사, 같은 가족, 같은 학급)**에 붙어야 반복 사용이 생깁니다.
- 국내에서 돈이 확인된 쪽은 "안전·법적 의무"(중대재해처벌법 맥락의 안전교육, TBM 기록) 기능입니다. 소비자 앱으로 시작하더라도 수익화는 사장님·관리자 결제나 공공 예산으로 가야 할 가능성이 큽니다.
- 리뷰 불만(지연, 실패, 저자원 언어 품질)은 곧 차별화 기회입니다. 롱테일 언어 품질을 측정하고 공개하는 것(예: 네팔어·크메르어 품질 보증)이 신뢰 요소가 될 수 있습니다.
- 언어학습 앱(Tandem, HelloTalk, Speaky 등)은 "번역 없이 서로 배우는" 모델이라 이 사업과 목적이 다릅니다. 하이로컬처럼 언어교환에서 출발한 팀이 현장 통역으로 옮겨오는 사례는 있습니다(추론, 아래 Gaps 참조).

### Gaps
- Lingvanex Messenger, Speaky, Tandem, HelloTalk 등의 현황과 펀딩: 이번 조사에서 출처를 확보하지 못했습니다.
- Unbabel 채팅 제품의 이력, 기타 "번역 메신저 스타트업 종료" 사례: 검색에서 확인되지 않았습니다.
- 각 전용 앱의 앱스토어 리뷰 원문(그룹 번역 관련 불만): 앱스토어 접속 불가.

---

## Q7. 종합: 화이트 스페이스와 가장 위험한 경쟁자

### Takeaway
화이트 스페이스는 **"한국에서, 회사 계정·관리자 SaaS 없이 누구나 QR·링크로 만드는 상시 혼합 언어 단체방(3개 이상 언어), 롱테일 아시아 언어 품질 보장, 음성 메시지 번역, 독자는 무료"**입니다. 대상은 B2B 현장 솔루션이 닿지 않는 중소 현장 근로자끼리 대화, 기숙사·집주인, 다문화 가족, 학급 학부모, 종교·동호회 공동체입니다. 가장 위험한 경쟁자는 단일 스타트업이 아니라 **KakaoTalk(+Galaxy AI)**입니다. 한국 쪽 방장(관리자·학부모 대표·가족)이 이미 거기 있고, 이미 19개 언어 번역을 갖췄기 때문입니다. 기능 면에서 가장 근접한 것은 Lark 무료 플랜과 Vasco MultiTalk, 국내 B2B 진입 경로에서 가장 위험한 것은 hiWorker입니다.

### Cited Findings (종합의 근거로 쓰인 핵심 사실 재정리)
- KakaoTalk은 받은 메시지 말풍선 번역 + 발송 메시지 번역(19개 언어)을 갖췄지만 개인별 자동 표시는 확인되지 않음 — [TV리포트](https://tvreport.co.kr/msn/article/868521/), [카카오 6차 업데이트](https://www.kakaocorp.com/page/detail/12082)
- Galaxy AI 채팅 번역은 KakaoTalk 위에서 동작 — [Korea Daily](https://en.koreadaily.com/?p=37415), [Samsung Newsroom AU](https://news.samsung.com/au/galaxy-ai-now-supports-more-languages-with-latest-update)
- Lark Starter 무료(20명)에 무제한 실시간 번역, 18개 언어 — [Lark 요금제](https://www.larksuite.com/ko_kr/plans), [Lark Messenger](https://www.larksuite.com/en_us/product/messenger?from=zero)
- Vasco MultiTalk: 무료, 100명, 105~107개 언어, QR, 텍스트·음성 자동번역 — [App Store](https://apps.apple.com/us/app/-/id1673051523), [Vasco](https://vasco-translator.com/articles/languages/multilingual-conversation-made-easy/)
- Timekettle Chat Mode: 200명, 40개 언어 — [Timekettle](https://www.timekettle.co/blogs/news/timekettle-chat-mode-instant-message-translated-in-max-40-languages-max-200-people-in-group)
- hiWorker: 관리자 대상 B2B, 40개국 언어, 공지 전달·확인, 용어집, 카카오벤처스 투자, HJ중공업 도입 — [App Store](https://apps.apple.com/us/app/-/id6749565624), [한경 머니](https://magazine.hankyung.com/money/article/202609043973c)
- KS인더스트리 Ami: 무가입 다국어 통역룸, 24개 언어 — [아시아경제](https://view.asiae.co.kr/article/2026071315392438871)
- 대형 건설·조선은 자체 구축 — [한국경제(대우건설)](https://www.hankyung.com/amp/2026062443536), [벤처스퀘어(한화오션 오톡)](https://www.venturesquare.net/1114035/), [메트로서울(DL이앤씨)](https://www.metroseoul.co.kr/article/20241210500074)
- Microsoft Translator 다중기기 대화 종료 — [WhistleOut](https://www.whistleout.com/CellPhones/Guides/is-microsoft-translator-worth-downloading)
- Google Chat 개인 계정 확대 여부 충돌 — [Workspace Updates](https://workspaceupdates.googleblog.com/2024/12/translate-for-me-in-google-chat.html) vs [9to5Google](https://9to5google.com/2024/12/13/google-chat-translation/)

**직접 경쟁도 평가표** (기준: "혼합 3개 이상 언어 그룹, 폰 전용, 회사 계정 불필요, 롱테일 언어". 아래 등급은 위 출처를 바탕으로 한 분석가 판단)

| 플레이어 | 개인별 자동 표시 | 3개 이상 혼합 그룹 | 회사계정 불필요 | 언어 수(확인치) | 음성 메시지 | 한국 현장 맞춤 | 직접 경쟁도 |
|---|---|---|---|---|---|---|---|
| Vasco MultiTalk | O | O (100명) | O (QR) | 105~107 | O | X | 높음(기능) / 낮음(시장) |
| Timekettle Chat Mode | O | O (200명) | O(추정) | 40 | 미확인 | X | 중간 |
| Shavely | O | O | O (freemium) | 29 | 미확인 | X(팀 사전은 있음) | 중간~높음 |
| FlaiChat | O | O | O | 40+ | O | X (가족 지향) | 중간~높음(가족 세그먼트) |
| 애니챗 (KR) | O | O | O | 20 | 미확인 | 한국 회사지만 인니로 전환 | 중간 |
| DoTalk | O | O(유료, 10) | O | ~90 | O(hold&talk) | X | 낮음(정체) |
| Interpreter LTC | O | 3명 한정 | 미확인 | 미확인 | 미확인 | X | 낮음 |
| JotMe | O(회의) | O | O | 다수 | 회의 음성 | X | 낮음~중간 |
| hiWorker (KR) | 통역·공지 중심(1:N) | 일부(1:N) | X(관리자 B2B) | 40 | 음성 통역 O | O (TBM, 용어집) | 높음(국내 B2B 진입로) |
| KS인더스트리 Ami | 통역룸 | O(통역룸) | O(무가입) | 24 | 음성 O | O (조선·제조) | 중간~높음 |
| 플리토 오톡/Live Translation | O | 미확인 | X(기업 구축) | 7(오톡) | 음성 O | O | 낮음(대기업 SI) |
| DL 어깨동무M | 국적별 공지 | X(방송) | X(자사) | 미확인 | X | O | 낮음(내재화) |
| Lark Starter | O | O | △(조직 생성 필요, 무료 20명) | 18 | 미확인 | X | 높음(무료 대체재) |
| 네이버웍스 | O(방별 자동 통역) | O | X(조직 계정) | 9~10 | 미확인 | X | 중간(유통력) |
| 잔디 | 원클릭(수동) | O | X | 14 | 미확인 | X | 낮음 |
| Beekeeper/Flip/Zoom Frontline | O | O | X(좌석형 B2B) | 36~100+ | 미확인 | X(한국 진출 미확인) | 낮음(국내) / 중간(글로벌) |
| KakaoTalk (+Galaxy AI) | X(수동 말풍선·발송 번역) | O | O | 19 | X | 기본 메신저 | **잠재 위협 최대** |
| WhatsApp | iOS 베타 자동(약 21), Android 6 | O | O | 6~21 | 미확인 | X | 중간(글로벌 확장 시 높음) |
| Telegram | O(Premium, 독자별 과금) | O | O | 미확인 | 미확인 | X | 중간 |
| Zalo | 길게 눌러 번역, zCloud 자동 | O | O | 3+17(iOS) | 미확인 | X(베트남인 커뮤니티) | 중간(베트남 세그먼트) |
| Viber | 수동 | O | O | 미확인 | X | X | 낮음 |
| iMessage | O(9개 언어) | O | O | 9 | X | X (안드로이드 다수 이주민 배제) | 낮음 |
| Google Chat Translate for me | O | O | 개인계정 여부 충돌 | 120+ | 미확인 | X | 잠재 위협(개인계정 확대 시) |

### Inferences
- **화이트 스페이스 정의(가설)**:
  1. **세그먼트**: 회사 밖이거나 회사 시스템이 닿지 않는 혼합 언어 상시 그룹. 중소 제조·농축산·어업(E-9·계절근로)의 근로자끼리 대화, 외국인 기숙사·집주인·편의점 점주, 다문화 가족(시댁+며느리+친정), 학급 학부모 단체방, 이주민 교회·사원·동호회. 대기업 현장은 이미 자체 구축(대우·롯데·DL·한화·HD)하고 있어 비켜 가야 합니다.
  2. **제품**: (a) 가입 없이 QR·링크로 참여(KS Ami·MultiTalk가 이미 증명한 UX), (b) 3개 이상 언어 자동 감지(언어쌍 선택 없음), (c) 롱테일 언어 품질 보증(네팔어, 크메르어, 버마어, 우즈베크어, 싱할라어, 몽골어, 벵골어, 타갈로그어). 기존 메신저(온디바이스 언어팩)와 국내 협업툴(9~18개 언어)이 약한 지점입니다. (d) 음성 메시지 번역(문해력이 낮은 근로자에게 핵심, MultiTalk·FlaiChat 외에는 드묾), (e) 한국어 원문 병기와 "읽음·이해 확인"(안전 공지용).
  3. **수익화**: 독자 무료 + 방장(사장·관리자·학교) 유료, 또는 공공 예산(지자체 무상 지원 사업). Telegram처럼 독자마다 Premium을 요구하는 구조와 정반대입니다.
- **가장 위험한 경쟁자: KakaoTalk(+Galaxy AI)**. 한국인 방장 쪽 네트워크 효과가 압도적이고, 이미 19개 언어 번역 UI와 AI 업데이트 주기(2026년 정기 업데이트에서 대화 요약·ChatGPT 연동)를 갖췄습니다. "방별 자동 번역 토글" 하나만 추가해도 주요 언어 사용자층은 대부분 흡수됩니다. 남는 방어선은 롱테일 언어 품질, 음성 번역, 현장 기능(공지 확인, 용어집), 외국인 쪽 메신저(Zalo, WhatsApp, Telegram, Viber)와의 브리지 정도입니다.
- **2순위 위험: hiWorker(국내 B2B 경로)**. 이미 투자자(카카오벤처스), 레퍼런스(HJ중공업, 삼성물산 실증), 40개 언어, 용어집, 공지 확인 기능을 갖췄습니다. 근로자 쪽 그룹채팅을 추가하면 "현장 단톡방" 세그먼트를 먼저 가져갈 수 있습니다. 다만 관리자 중심 B2B라 소비자·생활 그룹으로는 약합니다.
- **3순위 위험: Lark Starter(무료)와 Google Chat 개인 계정(확대 시)**. 기능은 완비했지만 한국 현장 인지도와 온보딩(조직 생성, 이메일)이 약점입니다.
- **글로벌 확장 시 위험**: WhatsApp(iOS 자동번역이 정식 출시되고 Android로 확대되면)이 가장 큽니다. 이주민 출신국 대부분의 기본 메신저이기 때문입니다. 다만 온디바이스 방식이라 롱테일 언어 확장은 느릴 가능성이 큽니다.
- **소형 전용 앱(MultiTalk, Shavely, FlaiChat, Timekettle, 애니챗)**은 기능상 직접 경쟁자입니다. 하지만 한국어 현장 맞춤과 국내 유통이 없어, 한국 1단계에서는 위협이 낮습니다. 오히려 "이 기능만으로는 확산이 안 된다"는 반면교사입니다.

### Gaps
- 이 평가표의 "미확인" 칸(특히 롱테일 언어, 음성 메시지, 가격)은 공식 페이지 직접 확인이 필요합니다. 이번 세션에서는 앱스토어와 공식 사이트 접속이 막혔습니다.
- KakaoTalk 번역 기능의 정확한 언어 목록과 로드맵, Galaxy AI 채팅 번역의 현재 언어 수(2024 이후 갱신치).
- 세그먼트별 시장 규모(외국인 근로자 수, 다문화 가구, 학부모 수)는 이 경쟁 조사의 범위 밖이라 다루지 않았습니다(다른 리서처 담당으로 추정).
