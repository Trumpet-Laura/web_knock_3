# 31. 変数・配列・オブジェクトの基本
## コード
### index.html
```
<script type="module" src="main.js"></script>
```
### main.js
```
// 再代入できない変数const
const username ="Hanako";
console.log(username);

// 再代入可能な変数let
let age = 20;
age = 21;
console.log(age);

// 配列
const fukuoka = ["ラーメン", "明太子", "もつ鍋", "水炊き", "ごまさば"];
console.log(fukuoka);

// オブジェクト
const user = {
    name: "Hanako",
    age: 21,
    city: "Fukuoka"
  };
  
  console.log(user);
```
## varを使わない理由
`var` は古い仕様で、変数の有効範囲が広く、意図しない上書きやバグが発生しやすいため。基本的には `const` と `let` を使用する。
### 変数宣言の比較
| 項目 | const | let | var |
|---|---|---|---|
| 再宣言 | 不可 | 不可 | 可能 |
| 再代入 | 不可 | 可能 | 可能 |
| ブロックスコープ | あり | あり | なし |
 
**再宣言**：一度宣言した変数名で再度宣言すること。
```
// 再宣言
var num1 = 1;
var num1 = 2;
console.log(num1);  // 2
```
**再代入**：値が入っている変数に上書きで代入すること。   
**スコープ**：宣言した変数が有効な範囲を表す。  
**ブロックスコープ**：if文などの`{ }` （ブロック）内で宣言した変数は外からアクセスできない。 `const` と `let` はブロックスコープを持つが `var` は持たないため、意図せず変数の有効範囲が広くなりやすい。変数を広い範囲から変更できると、どこで値が変更されたのか把握しづらくなり、バグの原因になる。

## スクリーンショット
<img width="785" height="785" alt="スクリーンショット 2026-11-11 1 21 46" src="https://github.com/user-attachments/assets/27b4f9b0-640b-46bf-86de-1b59499ce455" />



