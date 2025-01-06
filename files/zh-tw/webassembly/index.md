---
title: WebAssembly
slug: WebAssembly
page-type: landing-page
browser-compat:
  - webassembly.api
  - webassembly.BigInt-to-i64-integration
  - webassembly.bulk-memory-operations
  - webassembly.exception-handling
  - webassembly.extended-constant-expressions
  - webassembly.fixed-width-SIMD
  - webassembly.garbage-collection
  - webassembly.multiMemory
  - webassembly.multi-value
  - webassembly.mutable-globals
  - webassembly.non-trapping-float-to-int-conversions
  - webassembly.reference-types
  - webassembly.sign-extension-operations
  - webassembly.tail-calls
  - webassembly.threads-and-atomics
---

{{WebAssemblySidebar}}

WebAssembly 是一種可以在現代網頁瀏覽器中執行的程式碼類型——它是一種低階、類組合語言，具有緊湊的二進位格式，能夠以接近原生的效能執行，並為 C/C++、C# 和 Rust 等語言提供一個編譯目標，使它們可以在網頁上執行。它也被設計為可與 JavaScript 並行運作，讓兩者能夠協同合作。

## 簡而言之

WebAssembly 對網頁平台有著巨大的影響——它提供了一種方法，能夠以接近原生速度在網頁上執行多種語言編寫的程式碼，讓過去無法在網頁上運作的用戶端應用程式得以實現。

WebAssembly 被設計為與 JavaScript 互補並並行運作——使用 WebAssembly JavaScript API，你可以將 WebAssembly 模組載入 JavaScript 應用程式中，並在兩者之間共享功能。這使你能在同一個應用程式中同時利用 WebAssembly 的效能與強大功能，以及 JavaScript 的表達力與彈性，即使你不懂如何編寫 WebAssembly 程式碼。

更棒的是，它正在透過 [W3C WebAssembly 工作小組](https://www.w3.org/wasm/) 和 [社群小組](https://www.w3.org/community/webassembly/) 以網頁標準的形式開發，所有主要的瀏覽器廠商都積極參與其中。

## 指南

- [WebAssembly 概念](/zh-TW/docs/WebAssembly/Concepts)  
  -：透過閱讀 WebAssembly 的高階概念來開始學習——什麼是 WebAssembly，它為什麼如此有用，它如何融入網頁平台（以及更廣泛的領域），以及如何使用它。  
- [將新的 C/C++ 模組編譯為 WebAssembly](/zh-TW/docs/WebAssembly/C_to_Wasm)  
  -：當你用 C/C++ 編寫程式碼後，可以使用像 [Emscripten](https://emscripten.org/) 這樣的工具將其編譯成 Wasm。讓我們看看它是如何運作的。  
- [將現有的 C 模組編譯為 WebAssembly](/zh-TW/docs/WebAssembly/existing_C_to_Wasm)  
  -：WebAssembly 的核心使用案例之一是將現有的 C 函式庫生態系統帶入網頁，讓開發者能夠在網頁上使用它們。  
- [從 Rust 編譯到 WebAssembly](/zh-TW/docs/WebAssembly/Rust_to_Wasm)  
  -：如果你編寫了 Rust 程式碼，可以將其編譯為 WebAssembly！本教學將帶你瞭解將 Rust 專案編譯為 Wasm，並在現有的網頁應用程式中使用它所需的所有知識。  
- [載入並執行 WebAssembly 程式碼](/zh-TW/docs/WebAssembly/Loading_and_running)  
  -：在擁有 Wasm 模組後，本文將介紹如何使用 [WebAssembly JavaScript](/zh-TW/docs/WebAssembly/JavaScript_interface) API 結合 [Fetch](/zh-TW/docs/Web/API/Fetch_API) 或 [XHR](/zh-TW/docs/Web/API/XMLHttpRequest) API 來擷取、編譯和實例化它。  
- [使用 WebAssembly JavaScript API](/zh-TW/docs/WebAssembly/Using_the_JavaScript_API)  
  -：一旦你載入了 Wasm 模組，接下來就是如何使用它。本文將向你展示如何透過 WebAssembly JavaScript API 使用 WebAssembly。  
- [匯出的 WebAssembly 函式](/zh-TW/docs/WebAssembly/Exported_functions)  
  -：匯出的 WebAssembly 函式是 WebAssembly 函式在 JavaScript 中的映射，允許你從 JavaScript 呼叫 WebAssembly 程式碼。本文將描述它們的運作方式。  
- [瞭解 WebAssembly 文本格式](/zh-TW/docs/WebAssembly/Understanding_the_text_format)  
  -：本文將解釋 Wasm 文本格式，這是在瀏覽器開發者工具中進行偵錯時顯示的 Wasm 模組的低階文本表示。  
- [將 WebAssembly 文本格式轉換為 Wasm](/zh-TW/docs/WebAssembly/Text_format_to_Wasm)  
  -：本文提供了將文本格式的 WebAssembly 模組轉換為 Wasm 二進位檔案的指南。  

## API 參考

- [WebAssembly 指令參考](/zh-TW/docs/WebAssembly/Reference)  
  -：包含互動範例的 WebAssembly 運算元參考文件。  
- [WebAssembly JavaScript 介面](/zh-TW/docs/WebAssembly/JavaScript_interface)  
  -：此物件作為所有 WebAssembly 相關功能的命名空間。  
- [`WebAssembly.Global()`](/zh-TW/docs/WebAssembly/JavaScript_interface/Global)  
  -：`WebAssembly.Global` 物件表示一個全域變數實例，可從 JavaScript 存取，並可在多個 [`WebAssembly.Module`](/zh-TW/docs/WebAssembly/JavaScript_interface/Module) 實例之間進行匯入/匯出。  
- [`WebAssembly.Module()`](/zh-TW/docs/WebAssembly/JavaScript_interface/Module)  
  -：`WebAssembly.Module` 物件包含由瀏覽器編譯好的無狀態 WebAssembly 程式碼，可有效地與 Worker 共享，並多次實例化。  
- [`WebAssembly.Instance()`](/zh-TW/docs/WebAssembly/JavaScript_interface/Instance)  
  -：`WebAssembly.Instance` 物件是 `Module` 的有狀態、可執行實例，包含所有可從 JavaScript 呼叫的匯出 WebAssembly 函式。  

## 範例

- [WASMSobel](https://github.com/JasonWeathersby/WASMSobel)  
- 更多範例請參考我們的 [webassembly-examples](https://github.com/mdn/webassembly-examples/) 儲存庫。  

## 規範

{{Specifications}}

## 瀏覽器相容性

{{Compat}}

## 參見

- [Mozilla Research 上的 WebAssembly](https://research.mozilla.org/)  
- [webassembly.org](https://webassembly.org/)  
- [Mozilla Hacks 部落格上的 WebAssembly 文章](https://hacks.mozilla.org/category/webassembly/)  
- [W3C WebAssembly 社群小組](https://www.w3.org/community/webassembly/)  
- [將 C 函式庫轉換為 Wasm](https://web.dev/articles/emscripting-a-c-library)  