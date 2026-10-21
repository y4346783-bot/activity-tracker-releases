# ActivityTracker のインストーラー

Windows 用アクティビティトラッカー ActivityTracker の配布用リポジトリです。ソースコードは置いていません。

## アプリ

- [最新の Release](../../releases/latest) から `ActivityTracker-Setup-<版>.exe` をダウンロードして実行してください（管理者権限は不要です）。
- 署名がないため、初回は「PC を保護しました」と出ます。「詳細情報」→「実行」で進めてください。
- インストール済みのアプリは、ここの最新の Release を 1 日に 1 回確認し、設定画面の「アップデート」から更新できます。
- `.sha256` は、インストーラーが壊れていないかをアプリが確かめるためのファイルです。

## ブラウザ拡張（見ているサイトの URL を記録する場合）

同じ Release に添付しています。拡張は URL とタイトルを、この PC で動いている ActivityTracker（127.0.0.1）にだけ送ります。

### Firefox / Zen

1. `activity-tracker-firefox-<版>.xpi` をダウンロードする。
2. ブラウザのアドレスバーに `about:addons` と入れて開き、歯車のメニューから「ファイルからアドオンをインストール」を選んで、ダウンロードした xpi を選ぶ。
3. 確認が出たら「追加」を押す。Mozilla の署名済みなので、再起動しても外れません。

### Chrome / Brave / Edge

1. `activity-tracker-chrome-<版>.zip` をダウンロードして、消さない場所に展開する（展開したフォルダを消すと拡張も動かなくなります）。
2. アドレスバーに `chrome://extensions`（Brave は `brave://extensions`、Edge は `edge://extensions`）と入れて開く。
3. 右上の「デベロッパー モード」をオンにして、「パッケージ化されていない拡張機能を読み込む」から展開したフォルダを選ぶ。
