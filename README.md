# 李氏注音方案

## 簡介

鑒於傳統的41鍵大千式注音鍵位佈局不便於手機打字，本方案對大千鍵位做合併調整，把鍵位壓縮至15鍵，同時保證帶聲調、無重音，通過“聲母+介韻+去重碼&聲調”三碼輸入一個帶調音節，是一種改良版的大千注音鍵盤佈局。

## 安裝

本方案是 [李氏三拼](https://github.com/arsenali/rime-triple-pinyin-lssp) 係列方案之一，依賴於李氏三拼基礎方案，安裝本方案前請先安裝 ℞ `rime-triple-pinyin-lssp`。

各平台安裝方法同李氏三拼，請參考：

[安卓版和windows版](https://github.com/arsenali/rime-triple-pinyin-lssp/wiki/安卓版和windows版)

[苹果版](https://github.com/arsenali/rime-triple-pinyin-lssp/wiki/苹果版)

<br>

## 鍵位圖

<div align="normal">
  <img src="https://github.com/user-attachments/assets/5016e0e8-e563-4a63-8478-c6f7d9b38b1f" 
       alt="4x4豎版鍵盤佈局" 
       width="50%"
       style="border: 1px solid #eee; 
              border-radius: 12px;
              box-shadow: 0 4px 12px rgba(0,0,0,0.15);
              margin: 20px 0;">
 <i> <p style="color: #666; font-style: italic; margin-top: 12px;">
    △4x4豎版鍵盤佈局
  </p></i>
</div>

_截圖使用的是“磐石”主題，“IOS”配色_

鍵盤佈局有3x5、4x4、4x4豎版等多種，4x4豎版鍵盤佈局和大千式佈局排列順序一致，較易上手，推薦使用4x4豎版鍵盤佈局。

<br>

## 編碼規則

- **第一碼：聲母**

聲母合併在15鍵上，按以下規則合併：

<table>
  <tr>
    <td></td>
    <td align="center"><strong>1排</strong></td>
    <td align="center"><strong>2排</strong></td>
    <td align="center"><strong>3排</strong></td>
    <td align="center"><strong>4排</strong></td>
  </tr>
  <tr>
    <td align="center"><strong>1列</strong></td>
    <td align="center">ㄅ</td>
    <td align="center">ㄉ</td>
    <td align="center">ㄍㄐ</td>
    <td align="center">ㄓㄗ</td>
  </tr>
  <tr>
    <td align="center"><strong>2列</strong></td>
    <td align="center">ㄆ</td>
    <td align="center">ㄊ</td>
    <td align="center">ㄎㄑ</td>
    <td align="center" rowspan="2">ㄔㄘ</td>
  </tr>
  <tr>
    <td align="center"><strong>3列</strong></td>
    <td align="center">ㄇ</td>
    <td align="center">ㄋ</td>
    <td align="center">ㄏㄒ</td>
    <!-- 空单元格，因为上一行的 td 已经占用位置 -->
  </tr>
  <tr>
    <td align="center"><strong>4列</strong></td>
    <td align="center">ㄖㄈ</td>
    <td align="center">ㄌ</td>
    <td align="center">〇</td>
    <td align="center">ㄕㄙ</td>
  </tr>
</table>

部分聲母共鍵，在第二碼去重。

零聲母音節需先打“〇”。

- **第二碼：介韻**

第二碼將介、韻合併，一併安排在15鍵上，按以下規則排列：

<table>
  <tr>
    <td></td>
    <td align="center"><strong>1排</strong></td>
    <td align="center"><strong>2排</strong></td>
    <td align="center"><strong>3排</strong></td>
    <td align="center"><strong>4排</strong></td>
  </tr>
  <tr>
    <td align="center"><strong>1列</strong></td>
    <td align="center">ㄚㄞㄢ</td>
    <td align="center">ㄧ-ㄚㄞㄢ</td>
    <td align="center">ㄨ-ㄚㄞㄢ</td>
    <td align="center">ㄩ-ㄦ _ ㄢ</td>
  </tr>
  <tr>
    <td align="center"><strong>2列</strong></td>
    <td align="center">ㄛㄟㄣ</td>
    <td align="center">ㄧ-ㄛㄧㄣ</td>
    <td align="center">ㄨ-ㄛㄟㄣ</td>
    <td align="center" rowspan="2">ㄩ- _ _ ㄣ</td>
  </tr>
  <tr>
    <td align="center"><strong>3列</strong></td>
    <td align="center">ㄜㄠㄤ</td>
    <td align="center">ㄧ- _ ㄠㄤ</td>
    <td align="center">ㄨ- _ _ ㄤ</td>
    <!-- 空单元格，因为上一行的 td 已经占用位置 -->
  </tr>
  <tr>
    <td align="center"><strong>4列</strong></td>
    <td align="center">ㄝㄡㄥ</td>
    <td align="center">ㄧ-ㄝㄡㄥ</td>
    <td align="center">ㄨ- _ ㄨㄥ</td>
    <td align="center">ㄩ-ㄝㄩㄥ</td>
  </tr>
</table>

在第二碼中消除了第一碼的共鍵聲母，去重原理見[第二碼去重原理](https://github.com/arsenali/rime-triple-pinyin-bopomofo/wiki#第二碼去重原理)。

第二碼把相鄰的韻母（或介韻組合）安排在同一鍵位，每個鍵位上安排三個韻母（或介韻組合），在第三碼進行去重。

不存在的音節以“_”示之。

- **第三碼：去重碼&聲調**

前兩碼產生三個不同的韻母（或介韻組合），在第三碼中進行去重，以第一組韻母為例，第三碼鍵位排列如下：

<table>
  <tr>
    <td></td>
    <td align="center"><strong>1排</strong></td>
    <td align="center"><strong>2排</strong></td>
    <td align="center"><strong>3排</strong></td>
    <td align="center"><strong>4排</strong></td>
  </tr>
  <tr>
    <td align="center"><strong>1列</strong></td>
    <td align="center">ㄚˉ</td>
    <td align="center">ㄞˉ</td>
    <td align="center">ㄢˉ</td>
    <td align="center">ㄚ˙</td>
  </tr>
  <tr>
    <td align="center"><strong>2列</strong></td>
    <td align="center">ㄚˊ</td>
    <td align="center">ㄞˊ</td>
    <td align="center">ㄢˊ</td>
    <td align="center" rowspan="2">ㄞ˙</td>
  </tr>
  <tr>
    <td align="center"><strong>3列</strong></td>
    <td align="center">ㄚˇ</td>
    <td align="center">ㄞˇ</td>
    <td align="center">ㄢˇ</td>
    <!-- 空单元格，因为上一行的 td 已经占用位置 -->
  </tr>
  <tr>
    <td align="center"><strong>4列</strong></td>
    <td align="center">ㄚˋ</td>
    <td align="center">ㄞˋ</td>
    <td align="center">ㄢˋ</td>
    <td align="center">ㄢ˙</td>
  </tr>
</table>

三個韻母分別安排在1-3排，以1-4列和第4排輸入五聲調。

如果不想區分聲調，可使用無聲調模式，此時可用第5排輸入無聲調音節。

<br>

---

**本方案相當於注音和雙拼的結合版，可打前兩碼簡拼，此時類似於普通的有重音的雙拼，第三碼相當於直接輔助碼。**

亦可使用筆畫碼篩選去重，筆畫碼相當於間接輔助碼。

主題文件中自帶簡單教程，可點擊“幫助”查看。

點擊“反查”可使用拼音或筆畫進行編碼反查。

默認只載入地球拼音詞庫，加載“八股文”語言模型，如需使用萬象等詞庫需自行下載並在詞庫列表文件terra_pinyin.extended.dict.yaml中啟用，使用其他語言模型請修改grammar.custom.yaml文件。

下載地址：http://www.lssp.ysepan.com/

QQ羣：[150478288](https://jq.qq.com/?_wv=1027&k=5wf1uTQ)

<br>

## 收藏和克隆

### &#8627; Stargazers
[![Stargazers repo roster for @arsenali/rime-triple-pinyin-bopomofo](https://reporoster.com/stars/arsenali/rime-triple-pinyin-bopomofo)](https://github.com/arsenali/rime-triple-pinyin-bopomofo/stargazers)

### &#8627; Forkers
[![Forkers repo roster for @arsenali/rime-triple-pinyin-bopomofo](https://reporoster.com/forks/arsenali/rime-triple-pinyin-bopomofo)](https://github.com/arsenali/rime-triple-pinyin-bopomofo/network/members)

