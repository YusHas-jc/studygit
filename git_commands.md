+ `git init`
カレントディレクトリ配下をローカルリポジトリにする
.gitディレクトリにリポジトリ情報が保存管理される
+ `git add .`
カレントディレクトリの全ファイルを追加/ステージングする
+ `git commit -m 'message'`
ステージングしたファイルをコミットする
+ `git commit -a -m 'message'`
管理下のファイルをすべてステージングしてコミットする
+ `git push origin main`
ローカルの内容をリモートのmainブランチに反映する
+ `git pull origin main`
リモートのmainブランチの内容をローカルに反映する
+ `git checkout HEAD -- <file>`
\<file>で指定したファイルの変更を取り消して最新のコミットを反映する
+ `git status -s -u=no`
状態確認 -sで短縮表示
+ `git log --all --graph --oneline`
履歴確認 --allで全ブランチ表示、--graphでブランチ可視化、--onelineで短縮表示
+ `git reflog`
操作履歴を確認する。バージョンを間違って戻した操作など含めて辿れる
+ `git reset`
ステージングを取り消す
+ `git reset --hard <commit>`
\<commit>の状態に戻す
