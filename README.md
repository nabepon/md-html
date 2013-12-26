
md-html
==================================

2013年12月27日　渡辺 貴明 <siokosyo@gmail.com>

概要
----------------------------------
markdown形式で記述したhtmlをファイルをjavascriptで変換して表示します  
htmlの上部にjs読み込みの記述するだけで、特別なビューワを必要とせずに  
markdownを表示することができます

使い方
----------------------------------
htmlの上部に次の3行を書き足します

```
<!-- saved from url=(0017)http://localhost/ -->
<meta http-equiv="X-UA-Compatible" content="IE=9,chrome=1">
<script src="src/md-html.js"></script>
```

あとはmarkdown形式で記述するだけです


機能
----------------------------------
* javascriptで変換するので、markdown用のビューワが必要ありません  
* ローカルで編集した場合、エディタで編集した内容をリアルタイムでブラウザに反映します  
  そのため、markdown用の特別なエディタを用意する必要がありません  
* 通常のmarkdownに加え、アウトラインを表示する機能を持っています  
* srcフォルダ内のstyle.cssを編集することでスタイルを拡張できます
* 画像をhtmlに埋め込むため、画像をbase64に変換するツールも付属しました  
  [trans_base64]:src/image2base64.html  
  ⇒[base64変換ツール][trans_base64]  
    
  <img height="48" src="data:image/jpeg;base64,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" />
  ＜変換したコードを張ることで画像を表示できます

* ついでにsvgで作図するツールも見つけたので、srcフォルダに一緒に置いておきました  
  [svg_edit]:src/svg-edit-2.6/svg-editor.html  
  ⇒[svg作図ツール][svg_edit]  

  <svg width="200" height="100" xmlns="http://www.w3.org/2000/svg">
   <g>
    <title>Layer 1</title>
    <path id="svg_1" d="m32.5,70.5c5,-17 -37,-55 1,-60c38,-5 101,17 123,14c22,-3 44,33 22,47c-22,14 -90,21 -112,16c-22,-5 -39,0 -34,-17z" stroke-linecap="null" stroke-linejoin="null" stroke-dasharray="null" stroke-width="5" stroke="#567bc4" fill="#8bceef"/>
   </g>
   <g>
    <title>Layer 2</title>
    <text transform="rotate(-8.53077 100.5 49.5)" font-weight="bold" xml:space="preserve" text-anchor="middle" font-family="serif" font-size="24" id="svg_2" y="58.5" x="100.5" stroke-linecap="null" stroke-linejoin="null" stroke-dasharray="null" stroke-width="0" stroke="#567bc4" fill="#000000">svg image</text>
   </g>
  </svg>
  
  svgの場合、コードを作図ツールに張り返すことで、再び編集できるようになるため便利です  
  ツール上部のEditSauceにコードを入れてApply Changesボタンを押すと再び編集できます  
  背景と文字が画面右側のレイヤーで分かれているのが確認できるかと思います  


ライセンス
----------------------------------
MIT ライセンス