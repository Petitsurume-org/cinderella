# cinderella

<blockquote>
それは、女の子なら誰もがあこがれる物語。素敵な魔法にかけられて、綺麗なガラスの靴をはいて、大きなお城で舞踏会。
それまで見たこともなかった、夢のような世界。
だけど、12時の鐘が鳴ると、ガラスの靴も素敵なドレスも消えてしまって。

そこにいたのは、ごく普通の女の子。

魔法って、なんだろう。
魔法は、本当にあったのかな?

<cite>from: アニメ「アイドルマスター シンデレラガールズ」25話冒頭</cite>
</blockquote>

## これは何?

12時の鐘がなった時に、あなたのTwitterアカウント上のツイートをすべて削除するプログラムです。

## how to use

まず、Python3.xをインストールしたあと、依存ライブラリを`pip3 install -r requirements.txt`でインストールしてください。
次に、`cp .env.example .env`で`.env`ファイルをコピーしたあと、`お好みのエディタ .env`で.envファイルを編集してください。
そうしたら、お好みの方法(cron等)で、`python3 main.py`が毎日0時00分に実行されるようにしてください。

現在は、
- 自分でふぁぼったツイート
- `@`から始まるツイート
- 誰かにRTされたツイート

は削除されないようになっています(なお、RTしたツイートに対しては無条件でRT解除されます)。

この挙動が気にいらない場合は、コードを書きかえるか、もしくはIssueを立てていただければ挙動を.envで変更できるようにします。