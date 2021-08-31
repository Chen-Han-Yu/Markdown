<!-- 使用markdown教學測試 -->
# 非本科學習中：Markdown  
> OpenDate:2021-08-29  
> IDE:Visual Studio Code  
> Code:Markdown  
> Author:柴犬陪唸書  

# <h2 id="1">1.動機與目標</h2>

* ##### 動機
  >- 工作一陣子後的短暫休息，想整理意外中學到的紀錄。
  >- 嘗試極簡生活，不想堆太多紙，但不是很了解的基礎還是會寫在筆記本上。
  >- 想加速學習時間，即便買了iPad，寫Code就是要實作。
  >- 想學Git/GitHub。
* ##### 目標
  >- 短期：Git/GitHub至少會操作。
  >- 中期：看幾本Git書。
  >- 長期：整理Python的程式碼。
  >- 長期：整理R的程式碼。

# <h2 id="2">2.目錄</h2>

 - [1.動機與目標](#1)
 - [2.目錄](#2)
 - [3.實作與筆記：Markdwon篇標題](#3)
    - [3.1.標題](#3.1)
    - [3.2.粗體](#3.2)
    - [3.3.斜體](#3.3)
    - [3.4.底線](#3.4)
    - [3.5.刪除線](#3.5)
    - [3.6.轉文字/文字凸顯](#3.6)
    - [3.7.引言與換行](#3.7)
    - [3.8.文字連結與圖片連結](#3.8)
    - [3.9.清單](#3.9)
    - [3.10.選項圖示(還需Debug)](#3.10)
    - [3.11.分隔線](#3.11)
    - [3.12.表格](#3.12)


# <h2 id="3">3.實作與筆記：Markdwon篇</h2>

# <h4 id="3.1">3.1.標題</h4>
  >- 有六種HTML的標籤  `<h1>`~`<h6>`  
  >- Setext與Atx型式，下述為Atx
  ```
  [Input:]
  # 這是h1
  ## 這是h2
  ### 這是h3
  #### 這是h4
  ##### 這是h5
  ###### 這是h6

  [Output]:
  ```
  # 這是h1
  ## 這是h2
  ### 這是h3
  #### 這是h4
  ##### 這是h5
  ###### 這是h6  
# <h4 id="3.2">3.2.粗體</h4>
```
[Input]:
**這是粗體**  
__這是粗體__  

[Output]:
```
> **這是粗體**  
> __這是粗體__  
# <h4 id="3.3">3.3.斜體</h4>
```
[Input]:
*這是斜體*
_這是斜體_
```
```
[Output]:
```
> *這是斜體*  
> _這是斜體_  
# <h4 id="3.4">3.4.底線</h4>
```
[Input]:
<u>底線</u>

[Output]:
```
> <u>底線</u>
# <h4 id="3.5">3.5.刪除線</h4>
```
[Input]:
~~刪除線~~
[Output]:
```
> ~~刪除線~~  
# <h4 id="3.6">3.6.轉文字/文字凸顯</h4>
  >- 文字底有塗滿
  >- 特殊字如`<br>`文字顯示可以使用
  ```
  [Input]:
  `這是文字`
  '<br>`
  '<h1>`

  [Output]:
  ```
  >`這是文字`  
  >`<br>`  
  >`<h1>`  
# <h4 id="3.7">3.7.引言與換行</h4>
  > 引言為`>`符號  
  > 換行可以用`<br>` `</br>` `兩個空白`
  > 若是使用VSCode，空白兩格失敗，需要進行設定，詳見參考資料
  ```
  [Input]:
  > 有換行的(跑時把頓號拿掉)`<br>`  
  > 沒換行的
  > 有換行的(多兩個空白) 
  > 結束 
  [Output]:
  ```
  > 有換行的(跑時把頓號拿掉)<br>
  > 沒換行的
  > 有換行的(多兩個空白)  
  > 結束
# <h4 id="3.8">3.8.文字連結與圖片連結</h4>
  >- 文字[連結文字](位置)
  >- 圖片[連結圖片](位置)  
     [連結圖片]前面加驚嘆號回直接出現相關內容
  ```
  [Input]:
  [柴犬介紹](https://zh.wikipedia.org/wiki/%E6%9F%B4%E7%8A%AC)
  [柴犬圖](https://zh.wikipedia.org/wiki/%E6%9F%B4%E7%8A%AC#/media/File:Shiba_inu_taiki.jpg)

  [Output]:
  ```
  >[柴犬介紹](https://zh.wikipedia.org/wiki/%E6%9F%B4%E7%8A%AC)
  [柴犬圖](https://zh.wikipedia.org/wiki/%E6%9F%B4%E7%8A%AC#/media/File:Shiba_inu_taiki.jpg)
# <h4 id="3.9">3.9.清單</h4>
  ```
  [Input]:
  * 清單
  + 清單
  - 清單
  1. 有順序的清單
  2. 有順序的清單

  [Output]:
  ```
  > * 清單
  > + 清單
  > - 清單
  > 1. 有順序的清單
  > 2. 有順序的清單
# <h4 id="3.10">3.10.選項圖示</h4>
  > 
<br>目前使用的VSCode顯示不出來
<br>該要有的空白要有，沒空白上傳Github顯示不出來
  ```
  [Input]:
  - [ ] 沒完成
  - [X] 有完成

  [Output]:
  ```
- [ ] 沒完成
- [X] 有完成

 
# <h4 id="3.11">3.11.分隔線</h4>

  ```
  [Input]:
  ---
  ***
  ___

  [Output]:
  ```
  ---
  ***
  ___
# <h4 id="3.12">3.12.表格</h4>
  ```
  [Input]:
  |名字|出生|性別|屬性|
  |:-:|-:|:-|-|
  |陪念書|04.29|女|人類|
  |阿柴|12.24|母|柴犬|
  冒號的位子代表
  1. :-: 置中
  2. :-  偏左
  3. -:  偏右

  [Output]:
  ```
  |名字|出生日期|性別|屬性|
  |:-:|-:|:-|-|
  |陪念書|04.29|女|人類|
  |阿柴|12.24|母|柴犬|

## 4.參考資料

* ##### [Markdown Shortcuts / Markdown Preview Github Styling](https://ithelp.ithome.com.tw/articles/10190508)
  >- 預覽設定是Ctrl + K V那個  

* ##### [Markdown Preview Enhanced](https://jonny-huang.github.io/projects/02_markdown_preview_enhanced/)  
  > - 支援資料彙整，輸出成PDF
  > - 可以用@import將外部資料載入
  > - 可以用@import匯入圖檔
  > - 用筆記管理專案  

* ##### Markdown語法
  >- [內轉目錄](https://dotblogs.com.tw/yitingblog/2018/08/07/144059)
  >- [內轉目錄，目前查到github說內轉不試用此方法???](https://www.cnblogs.com/JohnTsai/p/4027229.html)
  >- [在文件中使用連結](https://docs.microsoft.com/zh-tw/contribute/how-to-write-links)
  >- [Visul Studio Code 移除行尾空白](https://tech.goescat.site/2019/10/visual-studio-code.html)  
  >- [選項圖示](https://tiida54.github.io/2018/01/03/3%E5%88%86%E9%90%98%E5%AD%B8%E6%9C%83Markdown%E5%B8%B8%E7%94%A8%E8%AA%9E%E6%B3%95/)
  >- [GitHub圖示](https://sam.webspace.tw/2020/01/10/Markdown%20%E5%B8%B8%E7%94%A8%E8%AA%9E%E6%B3%95%E6%95%B4%E7%90%86/)
