# Introduction

---

Kotlin 是一個基於 JVM 的新的編程語言，由 JetBrains 開發。 Kotlin 可以編譯成 Java 字節碼，也可以編譯成 JavaScript，方便在沒有 JVM 的設備上運行。

coding style guildes：https://github.com/raywenderlich/kotlin-style-guide

## 優勢

* 多平台開發的可能 ：基於 JVM 的開發，Android 開發，Web 開發，Native（原生）開發。其中 Web 開發可以結合 Spring 框架，而且 Kotlin 也可以編譯生成 JavasSript 模塊，可以在一些 JavaScript 的虛擬機上編譯。 Native 開發就更厲害了，目前Kotlin 官方在 Github 開源了 Native 開發的[原始碼](https://github.com/JetBrains/kotlin-native)，基於 LLVM（Low Level Virtual Machine 的縮寫，表示「底層虛擬機」。LLVM 是一種編譯器基礎設施，以 C++ 寫成。它是為了任意一種編程語言而寫成的程序，利用虛擬技術創造出編譯時期、連接時期、運行時期以及閒置時期的最優化。）的後端，方便為各個平台編寫原生應用，比如 Mac OS，iOS，Linux，嵌入式系統，等等。
* 開源：閉源項目總歸比較有限。眾人拾柴火焰高，代碼開源可以更快速地發現 Bug，有了全世界各地程序員的貢獻，Kotlin 的優秀代碼和庫會越來越多。 Linux 系統就是開源的很好例子。
* 和 Java 100% 兼容 ：Kotlin 調用 Java 已有的代碼或庫沒有問題。在一個項目中也可以同時用 Java 和 Kotlin 來編寫代碼。 Android Studio 和 IntelliJ IDEA 都可以實現一鍵轉換 Java 代碼到 Kotlin。官方也有專頁介紹：https://www.jetbrains.com/help/idea/2017.1/mixing-java-and-kotlin-in-one-project.html
* 安全 ：大家聊得最多的肯定是可以輕鬆防止在 Java 中很常見的 NullPointerException（空指針異常）問題咯。做 Android 開發的一定深有體會，一般 app 奔潰，基本都是因為 NullPointerException，很多時候規避機制就是加一個 if 語句的判斷，很累贅。
* 容易學習 ：Kotlin 語法很簡單，和主流語言類似，語法高效，入門非常容易。好比當初蘋果發布 Swift 也是因為 OC 的語法奇怪，學習曲線比較陡峭。
* Lambda 表達式。
* 變量類型推斷。
* when 語句塊 ：告別繁瑣的 Switch 和 if... else if... else 語句塊。
* 非常方便的運算符重載。
* 不再需要手動添加 get 和 set 方法對了，直接對類的私有變量賦值和取值。
* Anko 這樣的 Kotlin 的官方庫可以使 Android 應用開發更快捷。
* 函數/方法 的關鍵字是 fun，而不是 function。真的很簡潔也很有趣（fun 是英語「有趣」的意思）。
* Var 和 Val 關鍵字 ：和 fun 關鍵字類似，也很簡潔。 Var 是 Variable（英語「可變的」之意）的縮寫，表示「可變的」變量。 Val 應該是 Value （英語「值」之意）的縮寫，表示只能賦值，而不能改寫其值，是表示「只讀的」變量，有點類似 C 語言中的 const 變量。這兩個關鍵字的起名應該是參考了 Scala 語言。
* 類的方法擴展很方便。
* 可以創建自定義的 DSL（領域特定語言）。
* 優秀工具的支持 ：JetBrains 公司開發了那麼多優秀的工具，Kotlin 可以完全享用。
* Coroutine ：協程。

![](/assets/e51da780fe5b556c4847a14e7291c34e.png)

