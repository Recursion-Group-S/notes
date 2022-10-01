落書きツール(偏愛マップ) 
- 目的
話し手は自分の好きなものを最大限アピール・プレゼンし、相手に自身のことをわかってもらう
聞き手も共感できるところは話し手に伝えて、親睦を深める

- 概要
自己紹介の際に遠慮や忖度なく自身の好きなものを紹介することに重きを置く
つまり、文字だけでなく、画像、動画、絵などを埋め込み最大限アピールする

- ポイント
このプロジェクトだとデザインと使いやすいさと応答性がポイント
デザインはなるべく綺麗な落書きぽいデザイン (Font, Resources, UI/UX), フルカラーで手書き風な字とイラスト
Samples:
https://twitter.com/OTASM9/status/1198094562536742912
https://cdn.discordapp.com/attachments/710030107611365418/1025567409597321257/unknown.png
https://sheage.jp/article/83843
http://unpco.com/wp/images/henaimap2015.png

- Level 1(Webapp, Clicker Empire Gameと同等)
Flexboxをならべ、box内に画像、Iconを配置する
Flexboxの大きさはドラッグで大きさ変える
(Resources) StampとIconを提供する (https://www.flaticon.com/animated-icons)
参考：昔Jeffryが動画 (https://www.youtube.com/watch?v=Gq-6eYBRQ6E) で紹介したライブラリ
https://muuri.dev/

- Level 2 (Mobile/Desktop App) 
Level 2は下記フロント系のみ
App Release
- 使い方概要
  Level2は自分の偏愛マップを画面共有して使うので、フロントのみでも使用可能。
  画像出力機能でjpg jpeg png, resolutionをデバイスストレージに保存する
　自分のデータも利用できる
- 機能
　- フロント系
    文字、画像、動画（GIF）、Iconを自由に配置する
    文字色、線色、線種変えられるようにする
    配置などはhttps://lucid.co/みたいに、自由に変えられるのがベストだが、完成することを重視するならからのテンプレートに入力するでも可
    偏愛マップテンプレートの参考資料は、
      https://kanoba.jp/wp-content/uploads/2019/06/IMG_2779-768x1024.jpg
      http://tamkaism.com/wp-content/uploads/2014/06/seri.png
    結果をimgで出力できるようにする。

- Level3 (Mobile/Desktop App)
Level2 + バックエンド
App Release
- 使い方概要
    Level3は、Key Codeを共有して使う（MobileはQRコードで共有、Desktop AppはURLからアクセスすると自動的にAppを開く）
    話し手登録必須、聞き手登録必要ない（聞き手はURLアクセスするだけでOK）
    パスワード管理はユーザ登録が必要で気軽に利用できないので、URLにKey Code値いれて管理する
- 機能
    同じデータ（偏愛マップの）に対して、話し手と聞き手がアクセスできるようする
    話し手がアクセスしたときは、文字、画像が編集できるようにし、公開ボタンで聞き手側に見せるためのURL(Key code)を発行する
    聞き手側がアクセスしたときは、いいねボタン、エフェクトボタンを配置し、可能であればリアルタイムでエフェクトを共有できるようにする
    また画像が生成され、画像へアクセスも発行される
    Key codeアクセスでダウンロードできる
    ある程度でリアルタイムで編集見れるようにする
    動画など重いファイルはCDNとか使う
