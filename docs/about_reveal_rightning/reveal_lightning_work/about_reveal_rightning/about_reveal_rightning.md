### reveal_lightningについて

https://github.com/yukimura1227/reveal_lightning
![](reveal_lightning_work/about_reveal_rightning/1516283310742.png)
<!-- .element: style="width: 50%" -->

----------

## 何者か？

- [reveal.js](https://github.com/hakimel/reveal.js)用のhttpサーバつき  
markdownエディタ

---

## 見た目
- editor + markdown preview + reveal.js preview

![](reveal_lightning_work/about_reveal_rightning/1516353538281.png)
<!-- .element: style="width: 70%" -->

---

## reveal.jsとは？

- 今見てもらっているようなCoolな  
LT用資料を作れるツール
- 基本はhtmlで記述するが  
markdownもサポートしている
- see: [reveal.js demo](https://revealjs.com)

----------

## なぜ作ったのか？

---

１. reveal.jsが一番markdownで  
  LT用の資料を作りやすい

---

２. でも,clipbordから画像を直接貼れる  
エディタが見つからない

---

３．こんな風に
- 文章を少しずつ表示する<!-- .element: class="fragment" -->
- fragment機能の構文を<!-- .element: class="fragment" -->
- 覚えられない<!-- .element: class="fragment" -->

---

４. んじゃぁフロントエンドの勉強がてら  
electronで作ってみよう

---

５. とりあえず個人ユースに  
耐えられるものできた  

↑イマココ!!
<!-- .element: class="fragment grow" -->

----------

## 機能

---

### functions(1/2)

|#|できること|
|:---|:---|
|1|clipboardの画像を<b>直接貼り付け</b>る|
|2|保存するディレクトリを切替える<br/><b>(Dropbox連携が容易)</b>|
|3|<b>GitHubPageで使える形式</b>でexportする|
|4|themeの切り替え|

---

### functions(2/2)

|#|できること|
|:---|:---|
|5|reveal.jsのpreview部分のページの自動追従|
|6|自動保存|
|7|発表用にシステムのデフォルトブラウザ起動|
|8|pdf出力用にシステムのデフォルト<br/>ブラウザ起動|

---

### clipboardの画像を直接貼り付け
- (macの場合) スクショ取る(Command+Ctrl+Shift+4)  
-> 貼り付け(Command+Alt+v)

![](reveal_lightning_work/about_reveal_rightning/image_paste.gif)

---

### 保存するディレクトリを切替える
1. メニューのPreferenceを開く
1. 「contents dir」に保存先の  
ディレクトリを設定する
1. メニューのFile->Openで、対象を開く
1. もしくは、File->Newで新規作成

Dropboxユーザの私的には同期できて嬉しい<!-- .element: class="fragment grow" -->

---

### GitHubPageで使える形でexport
1. メニューのPreferenceを開く
1. 「export to」にexport先のディレクトリ  
を設定する
1. メニューのFile->Exportで、exportされる  
(初回は必要なjsライブラリも吐き出すので若干時間がかかる)
1. GitHubにpushする(GitHubPagesの設定は済ませておくこと)

---

## themeの切り替え
1. メニューのPreferenceを開く
1. themeを切替える

![](reveal_lightning_work/about_reveal_rightning/change_theme.gif)
<!-- .element: style="width: 55%" -->

---

### 発表用にデフォルトブラウザ起動
- macのChromeなら最大化してCommand+Shift+Fで全画面表示できてよい

![](reveal_lightning_work/about_reveal_rightning/open_browser.gif)
<!-- .element: style="width: 70%" -->

---

### pdf用にデフォルトブラウザ起動
- chromeの印刷で行う

![](reveal_lightning_work/about_reveal_rightning/open_browser_for_pdf.gif)
<!-- .element: style="width: 80%" -->

----------

## よく使うショートカット

---

|#|機能|ショートカット(mac)
|:---|:---|:---|
|1|clipboardの画像を<br/>直接貼り付け|⌘ + ⌥ + V|
|2|reveal.jsのpreviewエリアのreload|⌘ + R|
|3|設定設定ダイアログを表示|⌘ + ,|
|4|新規資料の作成|⌘ + N|
|5|既存資料の読込|⌘ + O|

----------

## 追加したい機能

- エディターの設定変更機能
- アプリの自動update機能
- コンテキストメニューの整理
- 有用なショートカットの拡充
- markdown preview部分の数式対応

----------

## 依存しているoss
- electron
- reveal.js
- highlight.js
- mathjax
- ace editor
- uikit
- font-awesome
- marked.js
- node-static
- vex.js
- yarn
- jquery
