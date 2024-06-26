# ページを作成して HTML 要素を学ぼう！

以下に記載されているコードを貼り付けて実際にページを作成してみましょう。<br />
今回紹介する要素は代表的なごく一部の要素となりますが、各コードには使用されているタグの解説を記載しているので合わせて確認し、少しずつ意味を理解しましょう！

## タグとグルーピング

以下のコードをコピーして実際に表示を確認してみましょう！

```
<div>
  <h2>div タグを使って HTML 要素をグルーピングしよう</h2>
  <p>
    div タグを使用することで複数の HTML をグルーピングすることができます。
    <br />
    div を使用したグルーピングは文書的な意味は持ちませんが、複数の要素を 1 つの塊として扱うことができ見た目の装飾をする際に便利です。
  </p>
</div>
```

- `div` タグ: 区分を意味する `division` の略で、複数の HTML をグルーピングして区分する際に使用します。見た目の装飾するために複数の要素をまとめたり、ページを区分するためのコンテナのような使い方ができます。<br>
  [詳細はこちら](https://developer.mozilla.org/ja/docs/Web/HTML/Element/div)
- `h1~6` タグ: 見出しを表現する `heading` の略で、 1~6 の数字で見出しのレベルを表現して使用します。<br>
  [詳細はこちら](https://developer.mozilla.org/ja/docs/Web/HTML/Element/Heading_Elements)
- `p` タグ: 文章を意味する `paragraph` の略で、その名の通り文章を意味する際に使用します。テキストを囲うタグ ≠ p タグというわけではなく、文章として表現したい場合に使用するようにしましょう。<br>
  [詳細はこちら](https://developer.mozilla.org/ja/docs/Web/HTML/Element/p)
- `br` タグ: 開業を意味する `break` の略で、画面上で改行させたい場合に使用します。 HTML コード内の改行はあくまで**コード内での改行**となるため、画面上で改行をさせたい場合は明示的に br タグを使用しましょう。<br>
  [詳細はこちら](https://developer.mozilla.org/ja/docs/Web/HTML/Element/br)

## セクションと見出しを理解しよう

以下のコードをコピーして実際に表示を確認してみましょう！

```
<section>
  <h2>section を使って文章の構造をより明確に作成しよう</h2>
  <p>
    section タグを使用することで「見出し」と「その見出しに紐づくコンテンツ」をグルーピングすることができます。
    <br />
    このときグルーピングされたコンテンツは、1つの章や節としてまとめられ、階層構造で表現することができます。
  </p>
  <section>
    <h3>セクションの階層</h3>
    <p>
      section タグの中に section タグを使用することで「見出し3」は「見出し2」に紐づく小さな章 (節)
      として表現できます。
      <br />
      このように、見出しタグと section を仕様することで文章の構造を明確にすることができます。
      <br />
      構造を明確にすることで検索エンジンがコンテンツを理解しやすくなり、ユーザーが情報を見つけやすくなります。
    </p>
  </section>
</section>
```

- `section` タグ: ページ内のコンテンツを章分けして、意味をもたせる際に使用します。グルーピングをするという点では div タグと似ていますが、ページを構成する章や節として区分したい場合にはこちらを使用しましょう。<br>
  [詳細はこちら](https://developer.mozilla.org/ja/docs/Web/HTML/Element/section)

## テキストを箇条書きとして表現しよう

以下のコードをコピーして実際に表示を確認してみましょう！

```
<section>
  <h2>箇条書きを表現する ul と ol を理解しよう</h2>
  <p>
    文字を文章としてではなく、箇条書きで表現したい場合は p タグではなく ul または ol を使用します。<br />
  </p>
  <ul>
    <li>順番に意味がない箇条書き</li>
    <li>順番に意味がない箇条書き</li>
    <li>順番に意味がない箇条書き</li>
  </ul>
  <ol>
    <li>順番に意味がある箇条書き</li>
    <li>順番に意味がある箇条書き</li>
    <li>順番に意味がある箇条書き</li>
  </ol>
</section>
```

- `ul` タグ: 順不同を意味する `unordered list` の略で順番に意味がない箇条書きを表現する際に使用します。<br>
  [詳細はこちら](https://developer.mozilla.org/ja/docs/Web/HTML/Element/ul)

- `ol` タグ: 順番を意味する `ordered list` の略で、料理の作成手順などのように順番に意味がある箇条書きを表現する際に使用します。<br>
  [詳細はこちら](https://developer.mozilla.org/ja/docs/Web/HTML/Element/ol)

- `li` タグ: 箇条書きの内容を意味する `list item` の略で `ul` タグと `ol` タグの内容を表現する際に使用します。 `ul` タグと `ol` タグの直下は**必ずこのタグを使用する**決まりとなっており、逆にそれ以外の場面では使用してはいけません。<br>
  [詳細はこちら](https://developer.mozilla.org/ja/docs/Web/HTML/Element/li)

## 画像を表示する img タグと図表として意味を追加する figure タグ

以下のコードをコピーして実際に表示を確認してみましょう！

```
<section>
  <h2>画像を表示しよう</h2>
  <p>
    画像を表示させたい場合は img タグを使用します。
    <br />
    img
    タグは単体だけでは何も表示はしてくれませんが、「src="画像のURL"」のように表示したい画像の場所を示すことで画像を表示してくれます。
  </p>
  <div>
    <img src="https://placehold.jp/150x150.png" alt="150x150 の画像" />
  </div>
  <p>ただの画像としてではなく何かを示すための図表として使用する際は figure タグで強調することができます。</p>
  <figure>
    <img src="https://placehold.jp/150x150.png" alt="図表" />
    <figcaption>図表の説明文</figcaption>
  </figure>
</section>
```

- `img` タグ: 画像を表示する際に使用します。 `src` 属性に画像の場所を示すパスか URL を入力し、 `alt` 属性にはその画像の説明文を入れます。<br>
  [詳細はこちら](https://developer.mozilla.org/ja/docs/Web/HTML/Element/img)

- `figure` タグ: img タグなどの画像に対して図表である意味を追加する際に使用します。任意で子要素に `figcaption` 要素を配置することで画像の説明文を表示することもできます。<br>
  [詳細はこちら](https://developer.mozilla.org/ja/docs/Web/HTML/Element/figure)

## 終わりに

今回紹介したタグは代表的なものの中でもごく一部となりますが、HTMLタグは文章や要素の意味を表現するために非常に重要な役割を持っていることを感じていただけたかと思います。<br />
以下ページに HTML で使用できるタグの一覧が乗っていますが、その数は膨大で、正直使用されることのないマイナーなタグも多くあります。<br />
https://developer.mozilla.org/ja/docs/Web/HTML/Element

これらを一つ一つを英単語のように覚えるのは非常に効率が悪いです。<br />
今後学習していく中で様々なタグを見ることになるので、初めての見るタグが出てきたら都度調べて用途を少しずつ覚えていくようにしていきましょう！
