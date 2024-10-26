### 三角形を作成する方法
- web制作でやった時はborderを使用したものがデファクトな作り方だった
  ```css
  .triangle {
    border-left: 30px solid transparent;
    border-right: 30px solid transparent;
    border-bottom: calc(tan(60deg) * 30px) solid #ffffff;
  }
  ```
- `clip-path`を使用した方法で三角形を作成する
  ```css
  .triangle {
    background: #ffffff;
    height: calc(tan(60deg) * 60px / 2);
    width: 60px;
    clip-path: polygon(50% 0, 100% 100%, 0 100%);
  }
  ```
