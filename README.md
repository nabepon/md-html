# md-html

渡辺 貴明 <siokosyo@gmail.com>


## 概要

* htmlに3行追加するだけで、markdown形式のhmtlが表示可能になります
* markdown用ビューワ、エディタが不要になります  
* 編集をリアルタイム反映します  
* アウトライン機能付き  

## 使い方

htmlの上部に次の3行を書き足し、通常のmd形式で書くだけです。

```
<meta http-equiv="X-UA-Compatible" content="IE=10,chrome=1"><meta charset="UTF-8">
<script src="http://cdn.rawgit.com/nabepon/md-html/1.0.0/src/md-html.js"></script>
<!-- 使い方：https://github.com/nabepon/md-html -->
```

## 画像

### 画像表示  
  htmlのimgタグを使用して画像を表示できます  
```
<img src="画像パス">
```
  
### 画像埋め込み  
  画像を以下のツールで変換し、コードをhtmlに貼り付けます  
  [http://cdn.rawgit.com/nabepon/md-html/1.0.0/src/image2base64.html](http://cdn.rawgit.com/nabepon/md-html/1.0.0/src/image2base64.html)  
  
### 作図する  

  作図には以下を使用します  
  [http://svg-edit.googlecode.com/svn/branches/stable/editor/svg-editor.html](http://svg-edit.googlecode.com/svn/branches/stable/editor/svg-editor.html)  
  
  画面上部の「svgボタン」を押し、表示されたコードをhtmlに貼り付けます  
  コードを作図ツールに読み込ませることで、再編集が可能です  


ライセンス
----------------------------------
MIT ライセンス