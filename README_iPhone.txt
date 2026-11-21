HIROKI AI AGENCY Pixel Office PWA v1 — iPhone設定・公開手順

【現在の状態】
・パッケージ準備済み、ローカル検証済み
・まだホスティングされていません。公開URLは未作成です。
・本体はローカルの模擬オフィスです。AI API呼び出し、投稿、外部操作は行いません。

【無料ホスト候補：GitHub Pages（手動設定）】
注意：FreeプランではGitHub Pagesを利用するため、通常はPublicリポジトリが必要です。Publicにするとファイルが誰でも見られる状態になるため、公開前に内容を確認し、明示的に承認してください。

【iPhoneのみで準備する手順】
1. ZIPをダウンロードし、「ファイル」アプリのダウンロードまたはiCloud Driveに保存。
2. Safariで github.com を開き、自分でログイン。
3. 新規リポジトリ名を hiroki-ai-office にして作成。
4. 公開範囲を決める前にファイルを確認。公開には明示的な承認が必要です。秘密情報・個人情報は含めないでください。
5. Public公開を承認した場合のみPublicで作成。
6. ZIP内フォルダの中身（index.html、manifest.webmanifest、sw.js、icon-192.png、icon-512.png）をリポジトリ直下にアップロード。ZIP自体だけをアップロードしない。
7. リポジトリ Settings > Pages。
8. Build and deploymentで Deploy from a branch、Branch=main、Folder=/(root) を選び Save。
9. PagesのURLが表示されるまで待つ。
10. HTTPSのPages URLをSafariで開き、読み込み完了を待つ。
11. Safariの共有（□↑）> ホーム画面に追加。名前を HIROKI OFFICE にし、表示されたら「Web Appとして開く」を有効にして追加。
12. ホーム画面アイコンから起動。初回はネット接続が必要。以後キャッシュされたファイルはオフラインでも一部利用可能。

【iPhoneで複数ファイルを選べない場合】
GitHubのWeb Upload files画面でファイルを個別に追加してください。index.htmlは必ずリポジトリ直下に置き、余分なフォルダ階層にしないでください。

【トラブル】
・404：Pagesの設定と公開完了状態、root配置を確認。
・アイコンが出ない：ファイル名の大文字小文字と配置を確認。
・オフライン動作しない：HTTPSサイトを一度オンラインで開いてから再読み込み。Service Worker登録には時間がかかることがあります。
・ホーム画面追加が出ない：SafariでHTTPS URLを直接開く（アプリ内ブラウザではなくSafari）。

【承認ゲート】
GitHubリポジトリ作成、Public化、Web公開はまだ行っていません。これらは明示的な承認が必要です。
