### 一般的な作業
+ `git init`  
カレントディレクトリ配下をローカルリポジトリにする  
.gitディレクトリにリポジトリ情報が保存管理される  
+ `git status -s`  
状態確認 -sで短縮表示 -u=noでアントラックを無視  
+ `git log --all --graph --oneline`  
履歴確認 --allで全ブランチ表示、--graphでブランチ可視化、--onelineで短縮表示  
+ `git reflog`  
操作履歴を確認する。バージョンを間違って戻した操作など含めて辿れる  

### コミット作業
+ `git add .`  
カレントディレクトリの全ファイルを追加/ステージングする  
+ `git commit -m 'message'`  
ステージングしたファイルをコミットする  
+ `git commit -a -m 'message'`  
管理下のファイルをすべてステージングしてコミットする  
+ `git reset`  
ステージングを取り消す  
+ `git reset --hard <commit>`  
\<commit>の状態に戻す  
+ `git checkout HEAD -- <file>`  
\<file>で指定したファイルの変更を取り消して最新のコミットを反映する  
### リモートとの同期
+ `git push origin main`  
ローカルの内容をリモートのmainブランチに反映する  
+ `git pull origin main`  
リモートのmainブランチの内容をローカルに反映する  
### ブランチ作業
+ `git checkout -b <branch> [<commit>]`  
ブランチを任意のコミットで切って移動  
+ `git merge -m 'message'`  
ブランチをマージ。コンフリクトが起きた場合には対象ファイルを修正してコミットすることでマージ完了する  
### タグ付作業
+ `git tag -m 'message' <tagname> [<commit>]`  
任意のコミットにタグをつける  
+ `git tag -l -n`  
タグ一覧を表示する  

