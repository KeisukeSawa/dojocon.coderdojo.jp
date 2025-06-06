# DojoCon Japan 公式サイト一覧

各年度の DojoCon Japan の概要 + テーマ + 実行委員長による開催に向けた思いなどを一覧できるページです。

これからの DojoCon Japan について考えたり、   
これまでの DojoCon Japan を一覧したい場面などでご参考になれば嬉しいです 😌💭 ✨

https://dojocon.coderdojo.jp/

[![DojoCon Japan 開催例](https://github.com/coderdojo-japan/dojocon.coderdojo.jp/blob/main/img/screenshot.jpg)](https://dojocon.coderdojo.jp/)

_※ 各サムネイル画像は、DojoCon Japan 実行委員会の著作物となります。_

-----

元々は初期に使っていた dojocon.coderdojo.jp ドメインへのリンクがすべてリンク切れになっていため、リンク切れを修正する目的でした。各 URL に対応するリダイレクトを追加するだけでも十分でしたが、せっかくなので DojoCon Japan を一覧できるサイトにリニューアルしてみた流れになります 🆙✨

なお、個別ページへのリンク切れにも気づき次第対応しています。例えば次のようなリンクも今までは 404 Page Not Found となっていましたが、2016年の DojoCon Japan の該当するページにリダイレクトされるようになっています ↩️ ✅

- リダイレクトの例: http://dojocon.coderdojo.jp/sponsor/
- リダイレクトの例: http://dojocon.coderdojo.jp/2016/09/04/coderdojo-japan-was-established.html

[![Google 検索 - "dojocon.coderdojo.jp"](https://github.com/coderdojo-japan/dojocon.coderdojo.jp/blob/main/img/google-search-result.jpg)](https://www.google.com/search?q=%22dojocon.coderdojo.jp%22)

<br>

## :yin_yang: DojoCon Japan とは? CoderDojo とは?

DojoCon Japan とは日本の [CoderDojo](https://github.com/coderdojo-japan) コミュニティメンバーが全国から集まるカンファレンスイベント (CoderDojo Conference) です。2016年に始まり、毎年１回のペースで開催しています。

CoderDojo は7〜17歳を対象とした非営利のプログラミング道場です。2011年にアイルランドで始まり、世界では100カ国・2,000の道場、[日本には220以上の道場](https://coderdojo.jp/)があります。

- DojoCon Japan の開催例を見る: https://dojocon.coderdojo.jp/
- 日本各地の CoderDojo を見る:  https://coderdojo.jp/

<br>

## :white_check_mark: ブラウザで情報修正を提案できます

情報を更新したい場合は **Webブラウザが一番簡単** だと思います...!! 😆

1. 下記の『更新方法』を参考に、修正を提案したい yml ファイルをクリックする
2. 画面右にある ✎ アイコン (Fork this project and edit this file) をクリックする
3. 気になる箇所を修正し、修正内容にタイトルと説明文を付け、Propose file change をクリックする
4. 修正内容を確認し、問題なければ Create pull request をクリックする

以上で完了です。提案された修正内容は運営チームによって再確認され、問題なければ提案された内容が反映されます。もし修正内容に不具合があっても運営側で気付いて修正するので、まずはお気軽に提案してみてください :wink:

<br>

## :up: 開催情報の更新方法

[`_data`](https://github.com/coderdojo-japan/dojocon.coderdojo.jp/tree/main/_data) ディレクトリ内に `events.yml` という YAML ファイルがあり、この YAML ファイルを修正すると情報を更新できます。

[`_data/events.yml`](https://github.com/coderdojo-japan/dojocon.coderdojo.jp/blob/main/_data/events.yml) ファイルの内容は以下の通りです。

```yml
# - url:   公式サイトへのURL
#   img:   サムネイル画像のファイル名 (画像は `img/events/` ディレクトリに置きます)
#   date:  開催日 (日付は `yyyy/mm/dd (曜日)` 形式で書きます)
#   venue: 開催地 (都道府県単位)
#   description: >-
#     ココに説明文を書きます。一部の Markdown や HTML にも対応しています。

# 例：「DojoCon Japan 2016」の場合
- url:   https://dojocon2016.coderdojo.jp/
  img:   2016.webp
  date:  2016/08/27 (土)
  venue: 大阪
  description: >-
    初開催の DojoCon Japan。THE MORE DOJOS, THE MORE COOL CODERS をテーマに開催。
      <ul style='list-style: inside;'>
        <li>国内での CoderDojo に携わるメンターの交流</li>
        <li>プログラミング教育、コミュニティー運営、アートなどの各分野に関するエキサイティングなスピーカーを揃えたセッション</li>
        <li>新しいテクノロジーやサービスに触れるショーケース</li>
      </ul>
    を中心に構成され、これから日本各地で CoderDojo が増え、それぞれがいっそう楽しく、より地域に根ざし、そしてクリエイティブなものになっていくことで次世代のテクノロジスト育成の促進を目指します。
```

\[[`_data/events.yml` ファイルを見る](https://github.com/coderdojo-japan/dojocon.coderdojo.jp/blob/main/_data/events.yml)\]

<br>


## :gem: ローカル環境で確認する方法

エラーなどで困ったら [Rails Girls インストール・レシピ](https://railsgirls.jp/install)を見るのがオススメです。  
Ruby がインストールできれば十分で、 **Rails のインストールは不要** です。

```shell
# macOS の場合: Homebrew ( https://brew.sh/index_ja ) 経由がオススメ
$ brew install rbenv ruby-build

# Linux の場合: https://github.com/rbenv/rbenv#readme に沿って rbenv をインストール
$ sudo apt install rbenv   # Debian, Ubuntu 系のディストリビューションの場合

# Windows の場合: 以下の Rails Girls インストール・レシピに沿ってインストール
# https://railsgirls.jp/install

# `.ruby-version` ファイルにあるバージョン番号を確認し、バージョン番号 x.y.z をメモする
# https://github.com/coderdojo-japan/dojocon.coderdojo.jp/blob/main/.ruby-version

# 上記でメモした Ruby のバージョン番号をインストールする
$ rbenv install x.y.z

# 上記のバージョンの Ruby がインストールされたことを確認する
$ ruby --version

# 必要なライブラリをインストールする
$ bundle install

# ローカルサーバーを立ち上げる
$ bundle exec jekyll server
```

無事にローカルサーバーが立ち上がったら、[http://localhost:4000/](http://localhost:4000/) にアクセスしてWebサイトを修正・確認します。

<br>


## :octocat: 関連リポジトリ

- [GitHub - DojoCon Japan リポジトリ一覧](https://github.com/search?q=org%3Acoderdojo-japan%20dojocon&type=repositories)
- [GitHub - decadojo.coderdojo.jp](https://github.com/coderdojo-japan/decadojo.coderdojo.jp)
- [GitHub - map.coderdojo.jp](https://github.com/coderdojo-japan/map.coderdojo.jp)
- [GitHub - coderdojo.jp](https://github.com/coderdojo-japan/coderdojo.jp)
- [GitHub - 一般社団法人 CoderDojo Japan](https://github.com/coderdojo-japan)

<br>

## :art: Design & Copyright

本サイトでは以下のテーマを購入し、使用しています。

- Theme:「ORION」(Version: 3.2.4)
- Author: [Design Plus](http://design-plus1.com/tcd-w/)
- 利用規約: [https://design-plus1.com/tcd-w/license_standard](https://design-plus1.com/tcd-w/license_standard)
- 購入記録: [coderdojo-japan/dojocon.coderdojo.jp/img/orion_purchase_license.png](https://github.com/coderdojo-japan/dojocon.coderdojo.jp/blob/main/img/orion_purchase_license.png)

-----

Copyright ©  DojoCon Japan 実行委員会 & 一般社団法人 CoderDojo Japan ([@coderdojo-japan](https://github.com/coderdojo-japan)).
