# Emolett ( » [Emolett Web Site](http://mayuco.github.com/emolett/) )

## Emolett について

### Emolettは、(　) と 漢字1文字での感情表現を絵文字で表すためのフォントです

Web Fontsとして利用されることを目的としてつくりました。

例えば (笑) に class="emo" と指定するだけで、絵文字になります。

日本語では(　) の中に漢字1文字で感情を表現をする文化があるので、絵に意味を持たせるのに適していると思いました。

Web Fonts が表示できないブラウザでも、単に(笑)と表示されるので、気持ちを伝えることができます。

## 使い方

### かんたんに試してみる

1. HTMLファイルのheadタグ内にCSSファイルへのリンクを書きます。

    &lt;link rel="stylesheet" href="http://mayuco.github.com/emolett/stylesheets/emolett.css"&gt;

2. 絵文字にしたい箇所で、以下のように class="emo" または class="emolett" を指定します。

    おもしろいね &lt;span class="emo"&gt;(笑)&lt;/span&gt;

### 実際に使ってみる

実際に使う場合は、フォントファイルを自分のサーバーへアップロードしましょう。

1. ダウンロードするか、cloneします。

    $ git clone git://github.com:mayuco/emolett.git

2. emolettフォルダの中にあるfontsフォルダを自分のWebサイトに置きます。

3. 例えば以下のようにCSSを書き、フォントのパスを指定します。

    @font-face {
        font-family: Emolett;
        src: url("/fonts/Emolett.woff") format("woff"),
        url("/fonts/Emolett.otf") format("opentype");
    }
    
    .emolett,
    .emo {
        font-family: Emolett;
    }

4. 絵文字にしたい箇所で、以下のように class="emo" または class="emolett" を指定します。

    おもしろいね &lt;span class="emo"&gt;(笑)&lt;/span&gt;

## バージョン

1.0.0

## ライセンス

Copyright (c) 2012 Mayuko Sekiya

[SIL Open Font License (OFL)](http://scripts.sil.org/cms/scripts/page.php?site_id=nrsi&id=OFL) を採用します。
