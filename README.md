# What switch pressed?

## What is?

「このキーを押したら」「このスイッチについての情報を表示する」ができるwebアプリケーション。

## Why use?

ご家庭で余っているキーボードをスイッチテスターとして活用したい。

また、一般的な単にスイッチテスターは樹脂製のハコにスイッチを固定しているだけのものが多い。  
このアプリを使うことで、任意のキーボードで打鍵感を試す行為が楽しくなる。

## What can?

## Memo…

* キー配置をどこまでカスタマイズできるようにすべきか？
    * remapみたいに対応するのはつらすぎるな…
    * 一般的なレイアウトに対応する案
        * ℹ️**キーコードに対してマッピング**するにはキーボード個体ごとの情報を定義しておかなければならない。
            * それは現実的ではないので**文字コードに対してマッピング**する。
        * メインのレイアウトと、自由に追加できるキー情報リストを持つ。
            * 主要な幾つかのレイアウトはデフォルでサポートする。
                * 左ctrl,右ctrl、とか単一の文字コードで複数キー持ってる箇所はどうしよう？
                    * 利用者の方でなんとかしてください。とする。
            * プラス、自由に追加できる[カードorリスト]エリアを用意してカスタムできるようにする。
* 初回リリース（v0.1.xとする）はミニマムで行きたい。
    * 押下されたkeycode(「C」なのか？「x004x0」みたいなやつで取得できるのか？)とスイッチをマッピングする
    * スイッチはシステムユニークである必要はない
        * まずはユーザが自由に定義できるようにする案
            * 次のフェーズでユーザ間で共有のDBを開発する。
                * その場合は自分で入力したやつらをスムーズに移行できるように考慮が必要。
                    * 最低限の項目定義
* ゆくゆくは [Switches DB](https://www.prominence.tv/keyswitch/) アプリ（[Discord ch](https://discord.com/channels/777912889344393216/1060801088967671808) ）と合流したい。
    * [プロダクトコード](https://discord.com/channels/777912889344393216/1060801088967671808/1061144535167684688)をユニークキーとして
* ソース公開/ライセンス/収益性はどうするか
    * 個人的に無償にはしたくない。そのうち広告入れられるようにはしたい。
    * とはいえissueとか上げてもらえる仕組みにはしたい。
        * issueや要望上げられる場所だけ公開すればいいか？
* 

