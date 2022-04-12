# 三碼注音方案

配方： ℞ arsenali/rime-triple-pinyin

[Rime](https://rime.im/) 大致按“聲母、介韻、聲調”的順序三碼輸入一個帶調注音音節，15鍵內無重音

## 安裝

[東風破](https://github.com/rime/plum) 安裝口令： <code> bash rime-install arsenali/rime-triple-pinyin-bopomofo </code>

本方案詞庫依賴於 [地球拼音](https://github.com/rime/rime-terra-pinyin) ℞ rime-terra-pinyin，安裝本方案前請先安裝 ℞ rime-terra-pinyin。

皮膚（主題）文件依賴於 [同文安卓輸入法平臺](https://github.com/osfans/trime) ℞ trime，安卓平臺使用本方案前請先安裝 ℞ trime。


## 簡介

三碼注音是[三碼拼音](https://github.com/arsenali/rime-triple-pinyin)系列方案的一種，為方便注音用戶使用，單獨開設一個項目進行介紹。

“[三碼拼音](https://github.com/arsenali/rime-triple-pinyin)”是專為觸屏手機打字而設計的一套漢字輸入方案，它相當於是注音和雙拼方案的結合，特點是按鍵大、無重音、碼長短、重碼率低，具體請參閱三碼拼音方案說明。

三碼拼音方案的聲母和韻母鍵位可以在三拼規則內隨意調整，**三碼拼音之三碼注音**方案的聲母、韻母鍵位按照大千注音鍵位排列，方便注音用戶使用。為適配qwerty鍵盤和手機界面，鍵位採取橫向排列方式。


<br>


- 第一碼輸入聲母

||1行|2行|3行|4行|5行
:---:|:---:|:---:|:---:|:---:|:---:
1列|ㄅ|ㄆ|ㄇ|ㄖㄈ|ㄓㄗ
2列|ㄉ|ㄊ|ㄋ|ㄌ|ㄔㄘ
3列|ㄍㄐ|ㄎㄑ|ㄏㄒ|〇|ㄕㄙ

_零聲母音節需要先打一個“〇”。

其中部分聲母共鍵，共鍵聲母將在第二碼區分。

- 第二碼同時輸入介母和韻母

||1行|2行|3行|4行|5行
:---:|:---:|:---:|:---:|:---:|:---:
1列|ㄚㄞㄢ|ㄛㄟㄣ|ㄜㄠㄤ|ㄝㄡㄥ|ㄩ-ㄦ\_ㄢ
2列|ㄧ-ㄚㄞㄢ|ㄧ-ㄛㄧㄣ|ㄧ-\_ㄠㄤ|ㄧ-ㄝㄡㄥ|ㄩ-\_\_ㄣ
3列|ㄨ-ㄚㄞㄢ|ㄨ-ㄛㄟㄣ|ㄨ-\_\_ㄤ|ㄨ-\_ㄨㄥ|ㄩ-ㄝㄩㄥ

_不存在的音節以“\_”代示。

在第二碼中，把大千鍵盤上相鄰的三個韻母（或介韻組合）作為一組置於一鍵，把鍵盤分為4個區域：
- 第一區：第1列4鍵 —— 空介韻母
- 第二區：第2列4鍵 —— 介母ㄧ+韻母
- 第三區：第3列4鍵 —— 介母ㄨ+韻母
- 第四區：第5行3鍵 —— 介母ㄩ+韻母

第一二三區各有4組韻母，在第四區，由於ㄩ後不跟ㄜㄠㄤ，故第四區略過第三組韻母。


為保證任意三碼無重音，部分音節進行了調整合併，包括：
1. 單韻母音節 ㄦ=ㄩㄚ
2. 單韻母音節 ㄧ=ㄧㄟ
3. 單韻母音節 ㄨ=ㄨㄡ
4. 單韻母音節 ㄩ=ㄩㄡ
5. 空韻 ㄭ=ㄛ
_空韻也需輸入一個韻母“ㄭ”。

在第二碼，第一碼中的共鍵聲母得以區分，分為兩類：
- ㄍㄐ、ㄎㄑ、ㄏㄒ和零聲母，由於它們所跟介母不同，故在第二碼被自然區分；
- ㄓㄗ,ㄔㄘ,ㄕㄙ,ㄖㄈ四组共鍵聲母，由於都不跟介母ㄧㄩ，故把ㄓㄔㄕㄖ所跟音節置於第一三區，把ㄗㄘㄙㄈ所跟音節置於第二四區。

以此保證了任意前兩碼組合都只產生3個重複音節，重複音節將在第三碼進行區分。



- 第三碼進行音節去重，同時輸入聲調

以第一組韻母為例，在第三碼的鍵位分佈是：

||1行|2行|3行|4行|5行
:---:|:---:|:---:|:---:|:---:|:---:
1列|ㄚˉ|ㄚˊ|ㄚˇ|ㄚˋ|ㄚ˙
2列|ㄞˉ|ㄞˊ|ㄞˇ|ㄞˋ|ㄞ˙
3列|ㄢˉ|ㄢˊ|ㄢˇ|ㄢˋ|ㄢ˙

以1-3列區分韻母（或介韻組合），以1-5行輸入聲調。

如此，輸入三碼之後便得到了唯一的一個一個帶調音節，任意三碼組合不會產生重複音節。

本方案亦有無聲調模式，如果不想區分聲調，可長按或上滑T鍵切換為無聲調模式，此時可以第5行輸入無聲調音節。

<br>

“三碼注音”方案(triple_pinyin_smpy_bopomofo)採用動態鍵盤，每次按鍵後鍵盤顯示隨之變化，列示出下一碼的鍵位分佈，以方便用戶熟悉鍵位，但動態鍵盤只可打三碼全碼；熟悉鍵位之後可使用“三碼注音快打”方案(triple_pinyin_smpy_bopomofo_express)，它採用靜態鍵盤，可打首碼簡拼和前兩碼簡拼，此時類似於一般的有重音的雙拼方案，第三碼相當於是直接輔助碼。


---

主題文件自帶簡單教程，請點擊“幫助”查看。

默認只載入地球拼音詞庫，如需更多詞庫請移步網盤或QQ羣下載。

下載地址：[永碩E盤http://www.lssp.ysepan.com/](http://www.lssp.ysepan.com/)

QQ羣：[150478288](https://jq.qq.com/?_wv=1027&k=5wf1uTQ)

歡迎入羣討論！

<br>

### &#8627; Stargazers
[![Stargazers repo roster for @arsenali/rime-triple-pinyin-bopomofo](https://reporoster.com/stars/arsenali/rime-triple-pinyin-bopomofo)](https://github.com/arsenali/rime-triple-pinyin-bopomofo/stargazers)

### &#8627; Forkers
[![Forkers repo roster for @arsenali/rime-triple-pinyin-bopomofo](https://reporoster.com/forks/arsenali/rime-triple-pinyin-bopomofo)](https://github.com/arsenali/rime-triple-pinyin-bopomofo/network/members)
