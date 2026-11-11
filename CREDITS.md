# 出典・利用条件

GitHub Pagesで動作するブラウザゲームです。元データをゲーム用に簡略化・正規化・着色しています。境界の正確さや現行住所を保証しません。

- 町丁字等：総務省統計局「令和2年国勢調査 町丁・字等境界データ」、e-Stat。https://www.e-stat.go.jp/gis/statmap-search 、https://www.e-stat.go.jp/terms-of-use 。加工：ゲーム制作者。
- 行政区域：国土交通省「国土数値情報 行政区域データ」。https://nlftp.mlit.go.jp/ksj/ 。
- 過去の市区町村境界：国土交通省、筑波大学大学院生命環境科学研究科空間情報科学分野・村山祐司研究室「行政界変遷データベース」を基にNIIが加工、Geoshapeが配布。https://geoshape.ex.nii.ac.jp/city/choropleth/ 。ゲーム用の加工境界はCC BY-SA 4.0を継承。https://creativecommons.org/licenses/by-sa/4.0/ 。
- 地名・存続期間：CODH「Geoshape市区町村IDデータセット」「歴史的行政区域データセットβ版」、doi:10.20676/00000447、CC BY 4.0。https://geoshape.ex.nii.ac.jp/city/ 。
- 旧国・藩：CODH・本田謙一「幕末期近世村領域データセット」の村域を集約した復元領域。https://geoshape.ex.nii.ac.jp/av/ 、CC BY-SA 4.0。2015年集落境界による推定復元で、厳密な当時の法定境界ではありません。藩の参照資料：CODH「江戸時代の藩データ」、https://codh.rois.ac.jp/han/ 、CC BY 4.0。
- 追加の日本の島2,926体：© OpenStreetMap contributors、Open Data Commons Open Database License 1.0（ODbL 1.0）。https://www.openstreetmap.org/copyright 、https://opendatacommons.org/licenses/odbl/1-0/ 。加工元：kamataryo「日本の島クイズ」公開データ、https://github.com/kamataryo/japan-island-quiz （参照commit 1f42ab7d429136fe114b463c44b74024cd0bdabe、原資料2026-09-24、取得2026-11-07）。元の公開DBもODbL、リポジトリのコードはMITですがゲームコードは流用していません。Wikidata由来の補足情報はCC0。取得資料から選別し、輪郭を結合・簡略化・ゲーム座標へ等比変換、名称表記を統一しました。加工DBはODbL 1.0を継承し、ゲーム内の島の「出典」→「収録島データを保存」からJSONを提供します。詳しくはSOURCE-NOTES.mdを参照。
- 湖：© OpenStreetMap contributors、ODbL。https://www.openstreetmap.org/copyright 。ゲーム内図鑑に個別資料を維持。
- 世界地図・海外の使者の地形：Natural Earth, Admin 0 – Countries, 1:50m。パブリックドメイン。https://www.naturalearthdata.com/about/terms-of-use/ 。ゲーム用に簡略化・正規化。国・地域と境界の区分は原資料に準拠し、政治的な立場を示しません。Made with Natural Earth.
- 同梱ライブラリー：three.js MIT License © three.js authors、fflate MIT License © 2023 Arjun Barrett。各ライセンス全文はゲーム内および同梱ファイルに保持。

ゲーム内のクレジット・図鑑出典も参照してください。元データ・加工境界に関する条件を、ゲームプログラム全体へ一括適用するものではありません。


## 青函トンネル施設

名称・接続地域・全長の参考：今別町「青函トンネル入口広場」 https://www.town.imabetsu.lg.jp/sightseeing/tourist/tonneru.html 。北海道知内町と青森県今別町を結ぶ施設として、既存の市区町村中心座標にゲーム用の入口を配置。建物・経路・通過時間は独自の簡略表現で、実際のトンネル線形・坑口位置・乗降施設・運行を再現するものではありません。新たな地形キャラクターや収録IDは追加していません。

## Ver1.1 市区町村統計・アイコン

- 市区町村統計：総務省統計局「令和2年国勢調査 人口等基本集計 第1-1表」。https://www.stat.go.jp/data/kokusei/2020/kekka.html 、原表 https://www.e-stat.go.jp/stat-search/file-download?statInfId=000032142402&fileKind=0 。人口・世帯数・面積・人口密度は2020年10月1日基準。面積は同表の国土地理院「令和2年全国都道府県市区町村別面積調」参照値。e-Stat利用規約 https://www.e-stat.go.jp/terms-of-use 。ゲーム用に1,916地域を抽出・名前に照合して再配置。現在値や現在の境界を保証せず、能力・排出確率には使用しません。行政区再編前の浜松市旧6区を含む既存の収録境域を維持しています。
- A・B・Cコイン、コイン箱の画像：ユーザー提供、2026年11月5日。画像生成は不使用。周囲の連結した白背景のみ透明化し、輪郭と描画内容を維持したまま縮小しています。画像そのものの権利を地理資料のライセンスへ移すものではありません。

## 東京23区専用マップと東京スカイツリー

- 境界：総務省統計局 e-Stat「令和2年国勢調査 町丁・字等別境界データ 東京都」、2020年10月1日基準。https://www.e-stat.go.jp/gis
- 元データを東京周辺の局所平面へ投影し、20mをゲーム地図の1単位に縮尺化・簡略化しました。23区・町丁の相対位置は実際の境界から構成しています。町丁キャラは既存の3,139件を使用し、既存の除外・IDを維持しています。
- e-Stat利用規約：https://www.e-stat.go.jp/terms-of-use 。原ZIPのSHA-256は `0e63cf86074450f248df666788070aeea20c668f9f47020f8e3017cbaabc1d1f`。この配布物には制作原本や編集元を含みません。
- 東京スカイツリーの高さ634m・天望デッキ350m・天望回廊450mは公式フロアガイド・スペックを参照。https://www.tokyo-skytree.jp/about/spec/ ／ https://www.tokyo-skytree.jp/floor/
- タワーは独自に作成したゲーム用の概形です。公式の画像・ロゴ・3Dモデルは使用していません。展望は写真やパノラマではなく、ゲーム内の同じマップを一人称カメラで描画しています。現実の建物・道路景観を再現するものではありません。公式施設との提携・公認を示すものではありません。

## 23区の川・橋・主要道路・鉄道・駅

© OpenStreetMap contributors。Open Database License 1.0に基づくデータです。
https://www.openstreetmap.org/copyright
https://opendatacommons.org/licenses/odbl/1-0/

Overpass取得データの基準時刻は2026-07-15T15:22:01Zです。23区内で切り出し・平面投影・簡略化を行った加工データはODbL-1.0で利用できます。ソフトウェアや独立した統計・国勢調査の境界データ全体をODbLに変更するものではありません。加工データは公開用の `game.bin` 内の extras に非暗号化で収録しています。取り出し方法をSOURCE-NOTES.mdに記載しています。

OpenStreetMapの実座標を使っていますが、道路幅、橋の高さ、駅・塔の建物形状、地下鉄の表示はゲーム用の概形で、現実の通行可否・運行状況を保証するものではありません。

## JR・地下鉄の駅順と接続

JR東日本「路線図」 https://www.jreast.co.jp/map/ 、東京メトロ「路線・駅の情報」 https://www.tokyometro.jp/station/index.html 、東京都交通局「各駅情報」 https://www.kotsu.metro.tokyo.jp/subway/stations/ を参照し、駅順・路線名をゲーム用データとして編集しました。公式路線図の画像・ロゴ・時刻表は転載していません。駅座標は既存のOpenStreetMap由来の地図データを使います。

23区内の収録駅のみを対象とする簡略な移動機能で、現実の運賃・所要時間・直通運転・列車種別・運行状況・正確な走行軌跡を示すものではありません。各鉄道会社との提携・公認を示すものではありません。

## 追加の私鉄・その他路線

駅順・路線名という事実情報を、各社の路線・駅案内を参照してゲーム用に編集しています。公式の路線図画像・ロゴ・時刻表は転載していません。駅座標は従来のOpenStreetMap由来データを再利用します。

東急 https://www.tokyu.co.jp/ ／京王 https://www.keio.co.jp/ ／小田急 https://www.odakyu.jp/ ／西武 https://www.seiburailway.jp/ ／東武 https://www.tobu.co.jp/ ／京成 https://www.keisei.co.jp/ ／京急 https://www.keikyu.co.jp/ ／北総 https://www.hokuso-railway.co.jp/ ／東京臨海高速鉄道 https://www.twr.co.jp/ ／ゆりかもめ https://www.yurikamome.co.jp/ ／東京モノレール https://www.tokyo-monorail.co.jp/ ／首都圏新都市鉄道 https://www.mir.co.jp/ ／東京都交通局 https://www.kotsu.metro.tokyo.jp/ 。

「その先」は路線が続く方向の全国地図へ出るゲーム用の処理です。実際の区境通過点や線路形状を正確に再現するものではありません。各社による公認・提携を示しません。

## 大阪市24区の専用マップ

区境・町丁の位置は、総務省統計局 e-Stat「令和2年国勢調査 町丁・字等境界」大阪府の世界測地系データを加工しています。基準日は2020年10月1日です。町丁を統合した区境は描画用に簡略化し、登場位置は町丁内の代表点を使っています。

取得元 https://www.e-stat.go.jp/gis/statmap-search/data?dlserveyId=A002005212020&code=27&coordSys=1&format=shape&downloadType=5&datum=2000

利用条件 https://www.e-stat.go.jp/terms-of-use

道路・河川・橋・鉄道は、国土地理院「最適化ベクトルタイル」従来版を加工して使用しています。2023年10月1日時点のタイルで、2026年11月5日に取得しました。地物ごとの実際の更新日や現在の状態を保証しません。道路は国道・都道府県道・高速道路などを選別しています。公式の地図画像や地図ライブラリーは同梱せず、加工した座標を独自描画します。

国土地理院 最適化ベクトルタイル https://github.com/gsi-cyberjapan/optimal_bvmap

国土地理院コンテンツ利用規約 https://www.gsi.go.jp/kikakuchousei/kikakuchousei40182.html

駅は地理院の駅注記と駅部の形状による概略位置です。新大阪の新幹線発着点・夢洲などを補完しました。同名の複数駅・乗換駅はゲーム用にまとめている場合があります。大阪のデータはOpenStreetMap由来と表示しません。東京側の従来のOpenStreetMap由来データとそのODbL表示・条件は維持します。

大阪の路線・駅名の参照先：Osaka Metro https://subway.osakametro.co.jp/guide/routemap.php ／JR西日本 https://www.jr-odekake.net/railroad/ ／阪急 https://www.hankyu.co.jp/ ／阪神 https://www.hanshin.co.jp/ ／京阪 https://www.keihan.co.jp/ ／近鉄 https://www.kintetsu.co.jp/ ／南海 https://www.nankai.co.jp/ ／阪堺 https://www.hankai.co.jp/ 。

## 新幹線

路線・駅名という事実情報をゲーム用に編集し、65の主要駅を概略位置で収録しています。JR東日本 https://www.jreast.co.jp/map/ ／JR東海 https://railway.jr-central.co.jp/route-map/ ／JR西日本 https://www.jr-odekake.net/railroad/ ／JR北海道 https://www.jrhokkaido.co.jp/ 。

公式路線図画像・ロゴ・時刻表を転載したものではなく、各社の公認・提携を示しません。座標・停車パターン・所要時間・走行軌跡・乗換は現実の運行案内には使えません。


## Ver1.13 追加データ

- 線路形状・駅位置：国土交通省「国土数値情報 鉄道データ」2025年度版、2025年12月31日基準、CC BY 4.0。経路抽出・簡略化・ゲーム座標への変換を実施。https://nlftp.mlit.go.jp/ksj/gml/datalist/KsjTmplt-N02-2025.html
- 地図表示用の歴史境界：「歴史的行政区域データセットβ版」ROIS-DS人文学オープンデータ共同利用センター、CC BY 4.0。原典には国土交通省「行政区域データ」、筑波大学「行政界変遷データベース」等を使用。境界の抽出・結合・簡略化・面積の概算を実施。https://geoshape.ex.nii.ac.jp/city/

新しい地図表示用の加工境界はCC BY 4.0です。従来収録の戦闘用地形など、別の利用条件を持つデータはその表記を維持します。詳しくはSOURCE-NOTES.mdを参照してください。

## Ver1.13 修正版の救助施設

新潟市の「緊急救助システム」は、既存のThree.jsと基本図形・文字ラベルによる独自のゲーム用モデルです。建物・敷地・復帰地点は架空の簡略表現で、実在の公的救助施設ではありません。新規の外部画像・3D素材・ライブラリーは使用していません。既存の市区町村モデル、歴史境界資料、鉄道データの出典・利用条件は上記のとおりで変更ありません。

## 証の間の勲章表示

金属の縁・月桂樹・リボン・刻印・名札は、本ゲーム用のSVGとCSSによるプログラム描画です。中央の地形輪郭には従来の各地理資料を引き続き用いており、各資料の出典・利用条件は上記とSOURCE-NOTES.mdに従います。新しい外部画像・ライブラリー・フォントは追加していません。

## 遊び方PDFのフォント

別配布の「遊び方.pdf」の100勝表記の更新部分には、Noto Sans JP Regularの埋め込みサブセットを使用しています。Noto Project、SIL Open Font License 1.1。元フォント：https://github.com/google/fonts/tree/main/ofl/notosansjp 。ゲーム画面へ外部フォントの通信を追加する変更ではありません。利用条件はLICENSES.txtにも記載しています。
