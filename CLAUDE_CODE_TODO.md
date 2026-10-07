# Claude Code への依頼（このフォルダで実行）

このフォルダは、授業用の完成見本サイトです。次の2つをお願いします。

## 1. Unsplashの写真をダウンロードして anime03/images/ に保存する

下の表のとおりにダウンロードしてください。ダウンロードURLは `https://unsplash.com/photos/<ID>/download?force=true&w=1600` です（`curl -L` でリダイレクトを追う）。

| 保存名 | Unsplash ID | 内容 |
|---|---|---|
| hero.jpg | gKXKBY-C-Dk | 竹の椅子に寝そべる白黒の猫（室内） |
| block1.jpg | k6w8miMpfUI | 白い部屋の木のテーブルと椅子（カフェ店内） |
| block2.jpg | 7zow7-ZranQ | リーフ模様のカプチーノ |
| block3.jpg | Y3AqmbmtLQI | ラテとコーヒー豆の俯瞰写真 |
| block4.jpg | 75715CVEJhI | 茶色のテーブルの上のオレンジと白の猫 |
| mike.jpg | xadzcCQZ_Xc | 三毛猫 |
| tora.jpg | p6yH8VmGqxo | 黄色い背景のオレンジのトラ猫 |
| gin.jpg | 7AIDE8PrvA0 | 床の上のシルバータビーの子猫 |

- ダウンロード後、それぞれの画像を開いて内容が「内容」の列と合っているか確認する
- IDが無効だった、または内容が合わない場合は、Unsplashで同じ内容の**無料写真**（Unsplash+ ではないもの）を探して差し替える
- 1枚あたり500KB以下を目安に、横幅1600px以内・JPEGに縮小する（大きすぎると表示が遅い）

## 2. Netlify にデプロイする

- `npx netlify-cli` で、このフォルダ（index.html がある階層）を本番デプロイする
- 初回はブラウザでNetlifyへのログインが必要
- 新しいサイトとして作成し、サイト名は `aso-cg-anime-sample` を候補にする（使われていれば近い名前で）
- 完了したら、公開URL（https://〜.netlify.app）を表示する

確認：公開URLを開き、次の3ページが表示されること
- /anime03/（写真が全部表示され、スクロールで動く）
- /anime04/waves.html（3Dの波）
- /anime04/（3Dオープニング）
