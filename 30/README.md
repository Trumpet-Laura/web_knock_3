# 30. JavaScriptファイルの読み込み
## index.html
```
<script type="module" src="main.js"></script>
```
## main.js
```
console.log("Hello, JavaScript!") 
```
## type="module" を付けるとどのような違いがあるか
通常の <script> は、HTMLの解析中にその場所で実行されるが、type="module" を付けると、基本的にHTMLの解析が終わってから実行される。
そのため、HTMLの要素がすべて読み込まれた状態でJavaScriptを実行でき、JavaScriptで操作したいボタンや文字などのHTML要素が、まだ読み込まれていないことによるエラーを防げる。
## スクリーンショット
<img width="790" height="788" alt="スクリーンショット 2026-11-10 23 46 28" src="https://github.com/user-attachments/assets/db684ebf-03ab-448e-998a-06567e13ec57" />
