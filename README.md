# my-first-repo
This is my awesome repo!!!

# 概要
リポ作って⇨クローンして⇨branch作って⇨ファイル修正して⇨addでstagingして⇨commitして
⇨(一応)pullして⇨pushして⇨pull request出して⇨mergeして⇨ローカルリポでpull

# コマンド
git --version  # gitのバージョンを確認

git clone {コピーしたリモートリポのURL}  # リモートリポからclone用のURLを取得してclone
※この際、リモートリポのフィルダに移動してREADME.mdファイルが存在するかの確認

subl .git  # gitフォルダの中身を見る

git config user.name '{USERNAME}'  # ローカルリポにユーザのセット
git config user.email '{EMAIL}'  # ローカルリポにEmailのセット
※--globalオプションをつければ、他のリポでもデフォルトでユーザがセットされる

git branch  # branch一覧の表示

git checkout {branch名}  # branchの切り替え(checkoutと呼ぶ)
※-bオプションをつければ新しいブランチを作成

git status  # 現在のリポの状態(commit待ちかcommit済か)	
※'working directory'＞add＞'Staging area'＞commit＞'Repository'
※addされた変更ではじめてcommit待ち状態、commitされてはじめて変更がrepo(ローカル)に反映

git add {ファイル名やフォルダ名}  # addしてstagingにあげる
※git add . とすればカレントディレクトリ以下の全ての変更をstagingにあげられる

git commit -m '{メッセージ}'  # 今stagingに上がっている全ての変更をcommitできる
※-mオプションでコミットメッセージを入れられる

git log  # commitの履歴を確認

git pull {repository} {branch}  # pull(リモートリポ⇨ローカルリポ)
※git remote -v で省略コードを確認(originのケースが多い)
※省略コード＞git pull origin main(共有ブランチ)

git push {repository} {branch}  # push(ローカルリポ⇨リモートリポ)
※pullと同じく{repository}はoriginで良い


