# 通往軟體架構師的道路

> * 原文地址：[通往軟體架構師的道路](https://github.com/justinamiller/SoftwareArchitect)
> * 原文作者：[Justin Miller(justinamiller)](https://github.com/justinamiller)
> * 翻譯：[NeroCube](https://github.com/NeroCube)

翻譯:

[English](https://github.com/justinamiller/SoftwareArchitect) |
[繁體中文](https://github.com/NeroCube/software-architect-zh-tw)

## 內容
- [什麼是軟體架構師](#什麼是軟體架構師)
- [架構等級](#架構等級)
- [典型活動](#典型活動)
- [重要技能](#重要技能)
- [架構師技術路線圖](#架構師技術路線圖)
- [解決方案架構師類型](#解決方案架構師類型)
- [推薦書籍](#推薦書籍)

# 什麼是軟體架構師
* 軟體架構師是一位軟體專家，他可以進行高層設計架構選擇並決定技術標準，包括軟體編碼標準，工具和平台。（來源：維基百科：軟體架構師）
* 軟體體系結構是系統的基本組織，由其組件，它們之間的相互關係以及與環境的關係以及確定係統設計和演進的原理來表示。 （來源：軟件體系結構手冊）

# 架構等級
架構可以抽象為幾個層次。水平會影響必要技能的重要性。

由於存在許多可能的分類，因此我喜歡細分成以下3個級別：
* **應用程序層級**: 最低級別的架構. 專注於一個單一的應用程序。非常詳細的底層設計。通常在一個開發團隊中進行溝通。
* **解決方案層級**: 中間層級的架構. 專注於滿足業務需求（業務解決方案）的一個或多個應用程序之中一些高層次但主要是低層次的設計。多個開發團隊之間的溝通。
* **企業層級**: 最高級別的體系結構。專注於多種解決方案。高層次的抽象設計, 需要解決方案或應用程序架構師進行詳細說明. 整個組織的溝通. 參閱 [Link](https://github.com/justinamiller/EnterpriseArchitecture) to learn more.

有時，架構師也被視為不同利益相關者之間的“膠水”。

三個例子：
* **水平**：橋接業務與開發人員或不同開發團隊之間的溝通。
* **垂直**：在開發人員和管理人員之間架起溝通橋樑。
* **技術**：相互集成不同的技術或應用程序。

# 典型活動
要了解架構師所需的必要技能，我們首先需要了解典型活動。 我認為以下列表包含最重要的活動：

* 定義並確定開發技術和平台
* 定義開發標準，例如編碼標準，工具，審查流程，測試方法等。
* 支持識別和理解業務需求
* 設計系統並根據需求做出決策
* 記錄並傳達架構定義，設計和決策
* 檢查和審查架構和代碼，例如，檢查定義的模式和編碼標準是否正確實施
* 與其他架構師和商業關係人合作
* 指導並諮詢開發商
* 詳細說明並將高階設計改進為低階設計

   _注意：系統架構是一項連續的活動，尤其是在將其應用於敏捷軟件開發中時。 因此，這些活動需一遍又一遍地進行。_

# 重要技能
為了支持佈局活動，需要特定技能。 根據我的經驗經過閱讀書籍和討論，我們可以將其總結為每個軟件架構師應具備的十項技能：
   * 設計
   * 決策
   * 簡化
   * 代碼
   * 文件
   * 溝通
   * 評估 
   * 權衡
   * 諮詢
   * 市場

## (1) 設計
如何做一個好的設計? 這可能是最重要和最具挑戰性的問題. 我將在理論和實踐之間進行區分。 以我的經驗，兩者的結合是最有價值的。 讓我們從理論開始:

* **了解基本設計模式**: 模式是架構師開發可維護系統所需的最重要工具之一。 使用模式，你可以重複使用設計，以通過可靠的解決方案解決常見問題。John Vlissides，Ralph Johnson，Richard Helm和 Erich Gamma 撰寫的 Design Patterns: Elements of Reusable Object-Oriented Software 是所有從事軟體開發的人必讀的書。儘管該模式已發布20多年，但它們仍然是現代軟體開發架構的基礎。 例如，本書描述了模型-視圖-控制器（MVC）模式，該模式在許多領域都得到了應用，或者是更新模式的基礎，例如 MVVM。
* **深入研究模式和反模式**: 如果你已經了解所有基本的 GoF 模式，則可以使用更多的軟體設計模式來擴展你的知識。 或更深入地研究你感興趣的領域。我最喜歡的應用程序集成之一是 Gregor Hohpe 撰寫的“ Enterprise Integration Patterns”一書。 無論兩個應用程序需要交換數據，無論是來自某些舊系統的舊式文件交換還是現代微服務體系結構的交換，這本書都適用於各個領域。
* **了解品質衡量**: 定義架構並不是終點。 它有定義、應用和控制指南和編碼標準的原因。 你出於質量和非功能性要求而這樣做。 你想要的是一個可維護，可靠，適應性強，安全，可測試，可擴展，高可用的系統。要實現所有這些質量屬性，一件事情就是應用良好的架構工作。 你可以在維基百科上了解更多關於品質衡量。
理論很重要。 如果你不想成為像牙塔架構師，那麼實踐同樣重要，甚至更為重要。

* **嘗試並了解不同的技術堆棧**: 如果你想成為一名更好的架構師，我認為這是最重要的活動。 試用（新）技術堆棧，並了解它們的興衰。不同或新技術具有不同的設計方面和模式。 你很可能從翻閱抽象幻燈片中不會學到任何東西，但可以試著自己嘗試一下，並感受期待來的痛苦或緩解。 架構是不應該只有廣度也需要在某些領域有較深的知識。掌握所有技術堆棧並不重要，但要對你所在領域最重要的知識，有深入的了解。另外嘗試不屬於你領域的技術，例如：如果你專研 SAP R/3 你應該也試試 JavaScript ，反之亦然. 儘管如此，雙方仍會對 SAP S/4 最新進展感到驚訝哈哈哈。例如，你可以自己嘗試看看 SAP S/4，然後上 openSAP 的免費課程。 好奇並嘗試新事物。 還可以嘗試一些你幾年前不喜歡的東西。
* **分析和理解應用模式**: 看一下當前的任何框架，例如Angular。 你可以在實踐中研究很多模式，例如“可視化”。 嘗試了解它如何在框架中應用，為什麼要這樣做。 而且，如果你真的很專心，請更深入地研究代碼並了解其實現方式。
* **好奇並參加用戶群**. [聚會](https://www.meetup.com/)

## (2) 決策
架構師需要能夠做出決定並指導項目或整個組織朝正確的方向發展。

* **知道什麼是重要的**: 不要浪份實踐做不重要的決策 或活動。學習什麼是重要的 據我所知，沒有一本書包含這些信息。我個人的最愛是這兩個特徵，我通常會在評估某些事情是否重要時考慮這些特徵: 
  1. 概念完整性: 如果你決定以一種方式進行操作，請堅持執行，即使有時最好以其他方式進行。 通常，通常使得整體概念，易於理解並易於維護。。
  2. 一致性: 例如，如果你定義並應用命名規範 它不是大寫或小寫，而是以相同的方式將其應用到所有地方。
* **優先排序**: 一些決定非常關鍵。 如果不及早採取措施，則會形成足夠的解決方法，這些解決方法通常不太可能在以後刪除，這是維護的噩夢, 或更糟糕的是，開發人員直接停止工作直到做出決定。在這種情況下，有時最好做出“錯誤”的決定而不是沒有做決定。 但是在遇到這種情況之前，請考慮優先考慮即將做出的決定。有不同的方法可以做。 我建議看一下在敏捷軟件開發中廣泛使用的加權最短作業優先（WSJF）模型。 特別是時間緊迫性和風險降低措施對於評估架構決策的優先順序非常關鍵。
* **知道你的權責**: 不要決定不在你權責內的事。這很關鍵，因為如果不考慮的話，它可能會嚴重破壞你作為架構師的地位。 為避免這種情況，請與你的同伴明確你要承擔的責任以及角色的一部分。 如果架構師不止一個，那麼你應該尊重當前部署的架構級別。 作為較低級別的架構師，你最好提出有關高層架構的建議，而不是決策。此外，我建議總是與同伴一起檢查關鍵決策。
* **評估多個選項**: 如果涉及到決策，請務必提出多個選擇。 在我參與的大多數情況下，都有不止一種可能的（好的）選擇。 從兩個方面講，僅選擇一個選項是不好的: 首先，似乎你的工作做得不好，其次，它阻礙了做出正確的決定。 通過定義度量，可以基於事實而不是直覺來比較選項， 例如：授權費用或期限。 這通常會導致更好和更可持續的決策。 此外，可以輕鬆地將決策出售給不同的利益相關人。 此外，如果你沒有正確評估選項，則在討論中可能會失去論點。

## (3) 簡化
請記住解決問題的原則 Occam 的 Razor，它指出更傾向簡單。 我將原理解釋如下: 如果你對問題的假設太多而無法解決，則可能會出錯或導致不必要的複雜解決方案。應該減少（簡化）假設以得出好的解決方案。

* **搖動解決方案**: 為了簡化解決方案，通常有助於“搖動”解決方案並從不同位置查看它們。 嘗試通過自上而下和自下而上的方式來塑造解決方案。 如果你有數據流或流程，請首先從左到右，再從右到左思考。 提出以下問題："在理想環境中你的解決方案會發生什麼？" 或者："公司/人員 X 會做什麼？"（這裡 X 可能不是你的競爭對手，而是 GAFA（Google，Apple，Facebook 和 Amazon）公司之一。）這兩個問題都迫使你減少 Occam 的 Razor 建議的假設。
* **退後一步**: 經過長時間的激烈討論，通常會得出高度複雜的塗鴉。 你永遠都不應將這些視為最終結果。 退後一步：再次查看全局（抽象級別）。 還是有意義嗎？ 然後再次在抽象級別上進行遍歷並進行重構。 有時，它有助於停止討論並在第二天繼續。 至少我的大腦需要一些時間來處理並提出更好，更優雅，更簡單的解決方案。
* **分而治之**: 通過將問題分成更小的部分來簡化問題。 然後獨立解決它們。 然後驗證小塊是否匹配。最後退後一步以查看總體情況。
* **重構不是邪惡的**: 如果找不到更好的主意，從更複雜的解決方案開始完全可以。 如果解決方案遇到麻煩，你可以稍後重新考慮解決方案並應用你的學習。 重構不是邪惡的。 但是在開始重構之前，請記住要進行以下工作：

  1. 進行足夠的自動化測試，以確保系統的正確功能。

  2. 利益相關人的支持。 要了解更多有關重構的信息，建議閱讀"Refactoring. Improving the Design of Existing Code"，作者是 Martin Fowler。

## (4) 代碼
即使作為企業架構師（最抽象的體系結構級別），你仍然應該知道開發人員的日常工作。 而且，如果你不了解如何完成此操作，則可能會遇到兩個主要問題：
  1. 開發人員不會接受你的說法。 
  2. 你不了解開發人員的挑戰和需求。

* **有一個輔助項目**: 這樣做的目的是嘗試新技術和工具，以了解當今和未來的開發方式。 經驗是結合觀察情感和假設（Kurt Schneider的" 軟體工程中的經驗和知識管理"）。閱讀教程或一些利弊是好的。 但這僅僅是“書籍知識”。 僅當你自己嘗試事物時，你才能體驗到情緒並建立關於事物好壞的假設。 而且，你使用某項技術的時間越長，你的假設就會越好。 這將幫助你在日常工作中做出更好的決定。當我開始編程時，我沒有代碼完成，只有一些實用程序庫可以加快開發速度。 顯然，在這種背景下，我今天會做出錯誤的決定。 今天，我們擁有大量的編程語言，框架，工具，過程和實踐。 只有你對主要趨勢有一定的經驗和粗略的了解，才能參與對話並引導開發朝正確的方向發展。
* **找到合適的東西去嘗試**: 你無法嘗試所有內容。 這根本是不可能的。 你需要一種更有條理的方法。 我最近發現的一種來源是ThoughtWorks的Technology Radar。 他們將技術，工具，平台，語言和框架分為四類：採用，試用，評估和保留。 通過這種分類，更容易獲得新事物的概述及其準備情況，以更好地評估下一步要探索的趨勢。
  * 採納："強烈的意願為企業使用做好準備"。
  * 試用："企業應該在一個可以處理風險的項目中進行嘗試"。
  * 評估："探索它如何影響你的企業"。
  * 舉行："謹慎處理"。
  


## (5) 文件
架構文檔有時或多或少地重要。 重要文檔是例如架構決策或代碼準則。 編程開始之前通常需要初始文檔，並且需要不斷完善。 其他文檔可以自動生成，因為代碼也可以是文檔，例如 UML類圖。

* **簡潔程式碼**: 如果做對的話，代碼是最好的文檔。 一個好的架構師應該能夠區分好的代碼和壞的代碼。 Robert C. Martin 所著的 "Clean Code" 一書是了解更多關於好壞代碼的寶貴資源。
* **盡可能生成文檔**: 系統變化迅速，很難更新文檔。 無論是有關 API 還是 CMDB（配置管理數據庫）形式的系統格局： 基礎信息經常變化太快而無法手動更新相應的文檔。 示例：對於API，如果你是模型驅動的，則可以基於定義文件自動生成文檔或直接從源代碼中獲取。 為此，存在許多工具，我認為 Swagger 和 RAML 是學習更多內容的一個很好的起點。
* **盡可能少**: 無論你需要記錄什麼文件（例如決策文件），都應嘗試一次只關註一件事，並且僅包含關於這件事的必要信息。 大量的文檔很難閱讀和理解。 附加信息應存儲在附錄中。 特別是對於決策文件，講一個有說服力的故事而不是僅僅進行大量爭論，其更為重要。 此外，這為你和你的同事節省了很多時間，而後者需要閱讀。 看看你過去所做的一些文檔（源代碼，模型，決策文件等）並問自己以下問題："是否包含所有必要的信息才能理解它？"，"確實需要哪些信息，可以省略哪些信息？" 和"文檔中是否有紅線？"。
* **了解有關架構框架的更多信息**: 該點也可以應用於所有其他"技術"點。 我把它放在這裡，是因為 TOGAF 或Zachmann 之類的框架正在提供"工具"，這些工具在文檔站點上感覺很沉重，儘管它們的附加值並不限於文檔。 在這樣的框架中獲得認證可以教會你更系統地解決體系結構。

## (6) 溝通
在我的觀察這是一項最常被低估的技能. 如果你的設計精湛，卻無法傳達你的想法，那麼你的想法可能只有較小的影響力，甚至無法成功。

* **了解如何交流你的想法**: 在會議或白板簡報中, 如何適當地使用它將自己與夥伴的想法架構是必要的. 我找到這本書 “UZMO — Thinking With Your Pen” 是能提高我在這一領域技能的良好資源。 作為架構師，你通常不僅會參加會議，而且通常需要主持會議並緩頰會議。
* **與大型團體進行演講**: 將你的想法呈現給小型或大型團體應該對你來說可行。如果你對此感到不舒服，請先開始向你最好的朋友練習介紹。慢慢擴大小組。 這是你只能通過做和離開自己的舒適圈來學習的東西。 請保持耐心，此過程可能需要一些時間。
* **找到正確的溝通水平**: 不同的合夥人有不同的興趣和看法。 需要在其級別上對它們進行對應的言論。 在進行交流之前，請退後一步並檢查你要分享的信息是否具有在正確的級別，有關抽象性，內容，目標，動機等。例如：開發人員通常對解決方案的很少細節感興趣，經理則不同。 比較想知道哪個選項可以節省最多的錢。
* **經常交流**: 如果沒有人知道，那麼出色的架構，他將毫無價值可言。定期在每個組織級別上分發目標體系結構及其背後的想法。 安排與開發人員，架構師和管理人員的會議，以向他們展示所需或已定義的方式。
* **盡量透明**: 定期交流只能部分緩解缺少的透明度。 你需要使決策背後的原因透明化。 特別是，如果人們不參與決策過程，則很難理解和遵循其背後的決策和理由。
* **隨時準備發表演講**: 總會遇到有人提出問題，你想立即給出正確的答案。 嘗試將最重要的幻燈片放在一個可以展示和解釋的穩固的集合中。 它為你節省了大量時間，並為你提供安全保護。

## (7) 估計和評估
* **了解基本的項目管理原則**: 作為架構師或首席開發者，經常會要求你提供估計以實現你的想法：多長時間，多少，多少人，哪些技能等？ 當然，如果你打算引入新的工具或框架，則需要為此類“管理”問題提供答案。 最初，你應該能夠進行粗略的估算，例如幾天，幾個月或幾年。並且不要忘記，這不僅涉及實現，還有更多活動需要考慮，例如需求工程，測試和修復錯誤。因此，你應該了解所使用的軟體開發過程的活動。 你可以應用以獲得更好的估計的一件事是使用過去的數據並從中得出你的預測。 如果你沒有過去的數據，也可以嘗試使用 Barry W. Boehm 的 COCOMO 之類的方法。如果你部署在敏捷項目中，請學習如何估算和正確計劃： 這本書 “Agile Estimating and Planning” by Mike Cohn 在這方面提供了紮實的概述。
* **評估『未知』架構**: 作為架構師，你還應該能夠評估架構在當前或將來中的適用性。 這不是一件容易的事，但是你可以通過準備一系列常見於每種架構的問題來為它做準備。 它不僅與架構有關，而且與系統的管理方式有關, 因為這也使你對品質有深刻的了解。 我建議總是準備一些問題來備用。 關於一般性問題的一些想法：
  1. 設計實踐：體系結構遵循哪些模式？ 因此，它們是否正確使用？ 設計遵循紅線還是增長不受控制？ 是否有清晰的結構和關注點分離？
  2. 開發實踐: 代碼準則到位並遵循？ 代碼如何版本化？ 部署實踐？
  3. 質量保證：測試自動化範圍？ 靜態代碼分析到位並取得良好結果？ 同行評論到位？
  4. 安全性：有哪些安全概念？ 內置安全性？ 滲透測試或自動安全分析工具是否到位並經常使用？

## (8) 權衡
* **質量是有代價的**: 之前，我談到了質量和非功能性需求。如果你過度設計架構，則會增加成本並可能降低開發速度。 你需要平衡架構和功能需求。 應避免過度設計。
* **解決矛盾的目標**: 相互矛盾的目標的一個典型例子是短期和長期目標。 項目通常傾向於構建最簡單的解決方案，而架構師則具有長遠的眼光。 通常，簡單的解決方案不適合長期解決方案，並且有被以後拋棄的風險（降低成本）。 為了避免實現錯誤的方向，需要考慮兩點：
  1. 開發人員和企業需要了解長期願景及其收益，以適應其解決方案。 
  2. 負責預算的經理需要參與以了解財務影響。 不必直接將100％的遠景圖放置在適當的位置，但是開發的部分應該適合。
* **衝突管理**: 架構師通常是具有不同背景多個小組之間的接著劑。 這可能會在不同級別的溝通上發生衝突。 為了找到一個能夠反映長期戰略目標的平衡解決方案，通常架構師的作用就是幫助克服衝突。我的出發點是基於 Schulze von Thun 的 "Four-Ears Model" 溝通理論。 基於此模型很多可以顯示並推論。 但是，該理論需要一些實踐，在交流研討會上應該可以取得經驗。

## (9) 諮詢和輔導
在諮詢和輔導方面，積極主動可能是你最好的選擇。 如果你被問，通常為時已晚。 而你想要避免進行結構清理。 你需要預見接下來的幾週，幾個月甚至幾年的時間，並為下一步做好準備。

* **有遠見**: 如果您在部署一個項目，無論是傳統的瀑布式方法還是敏捷方法，你始終需要設定一個中長期你想要達到的目標。 這不是一個詳細的概念，而是一個每個人都可以工作的路線圖。 由於你無法一次完成所有工作（這是一段旅程），因此我更喜歡使用成熟度模型。它們給出了易於使用的清晰架構，並且每次給出當前的進度狀態。 對於不同的方面，我使用不同的模型，例如 開發實踐或持續交付。 成熟度模型中的每個級別都有明確的要求，這些要求遵循SMART準則，以便輕鬆衡量是否已達到要求。 我發現一個很好的例子是繼續交付。
* **建立實踐社區（CoP）**: 在一個共同興趣小組之間交流經驗和知識有助於分發思想和標準化方法。 例如，您可以每三個月左右將所有JavaScript開發人員和架構師聚集在一個房間中，討論過去和當前的挑戰以及如何解決它們或採用新的方法論和方法。 建築師可以共享，討論和調整其願景，開發人員可以共享經驗並向同行學習。 這樣的回合不僅可以為企業帶來極大的好處，而且對個人本身也非常有利，因為它有助於建立更強大的網絡並傳播思想。還可以查看共體時間 SAFe 框架中的文章，該框架在敏捷環境中解釋了CoP概念。
* **進行公開會議**: 誤解或模棱兩可的原因之一就是缺乏溝通。固定時間段，例如 每週30分鐘，用於與同行交流熱門話題。 本屆會議沒有任何議程可以討論。 嘗試當場解決小事。 安排對更複雜主題的後續行動。

## (10) Market
Your ideas are great and you have communicated them well but still nobody wants to follow? Then you probably lack marketing skills.

* **Motivate and convince**: How do companies convince you of buying a product? They demonstrate its value and benefits. But not just with 5 bullet points. They wrap it nicely and make it as easy as possible to digest.
  1. Prototypes: Show a prototype of your idea. There are plenty of tools for creating prototypes. In the context of enterprises who love SAP check out build.me in which you can create nice looking and clickable UI5 apps fast and easy. 
  2. Show a video: Instead of “boring slides” you can also show a video which demonstrates your idea or at least the direction. 
But please, don’t overdo marketing: In the long term, content is king. If your words do not come true, this will damage your reputation in the long term.
* **Fight for your ideas and be persistent**: People sometime do not like your ideas or they are just too lazy to follow them. If you are really convinced by your ideas, you should continuously go after them and “fight”. This is sometimes necessary. Architecture decisions with long term goals are often not the easiest one’s: Developers do not like them, as they are more complex to develop. Managers do not like them, as they are more expensive in the short term. This is your job to be persistent and to negotiate.
* **Find allies**: Establishing or enforcing your ideas on your own can be hard or even impossible. Try to find allies who can support and help convincing others. Use your network. If you do not have one yet, start building it now. You could start by talking to your (open-minded) peers about your ideas. If they like it, or at least parts of it, it is likely that they support your idea if asked by others (“The idea by X was interesting.”). If they don’t like it, ask for the why: Maybe you have missed something? Or your story is not convincing enough? Next step is to find allies with decision power. Ask for an open-minded discussion. If you fear the discussion, remember that sometimes you need to leave your comfort zone.
* **Repeat It, Believe It**: “[…] studies show that repeated exposure to an opinion makes people believe the opinion is more prevalent, even if the source of that opinion is only a single person.” (Source: The Financial Brand) If you publish few messages often enough, it can help to convince people more easily. But be aware: From my perspective such a strategy should be used wisely as it could backfire as a lousy marketing trick.


# 架構師技術路線圖
![Architect roadmap](./src/archRoadmap.jpg)

# 解決方案架構師類型
![TypesSolution](./src/typesofsolutionarchitects.jpg)


# 推薦書籍
 * **Refactoring. Improving the Design of Existing Code** by Martin Fowler
 * **Enterprise Integration Patterns** written by Gregor Hohpe 
 * **Design Patterns: Elements of Reusable Object-Oriented Software** by John Vlissides, Ralph Johnson, Richard Helm, Erich Gamma
 * **Experience and Knowledge Management in Software Engineering** by Kurt Schneider
 * **Clean Code** by Robert C. Martin
 * **UZMO — Thinking With Your Pen**
 * **Agile Estimating and Planning** by Mike Cohn
