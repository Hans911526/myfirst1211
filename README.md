快速總結 (懶人包)
下次開新專案，依序執行這 6 行指令即可：

Bash

git init                      # 1. 初始化
git add .                     # 2. 加入所有檔案 (記得先創檔案!)
git commit -m "first commit"  # 3. 提交
git branch -M main            # 4. 改名分支
git remote add origin <URL>   # 5. 連線 (只有第一次需要)
git push -u origin main       # 6. 上傳
您現在可以試著建立一個全新的資料夾，從頭跑一次這個流程看看嗎？這樣印象會最深刻！
====================================================
更新 GitHub 的標準三步驟
請在 VSCode 終端機依序輸入以下指令：

1. 打包變更 (git add)
告訴 Git 哪些檔案被修改了，要準備送出。

Bash

git add .
解釋：. 代表「當前資料夾下的所有變更」。如果你只想上傳特定檔案，可以把 . 換成檔名。

2. 存檔確認 (git commit)
把剛剛打包好的東西存成一個版本，並寫下這次改了什麼。

Bash

git commit -m "這裡寫你改了什麼，例如：修正登入按鈕顏色"
解釋：-m 後面的文字很重要，建議寫清楚，以後回頭看紀錄才知道這一次改動是為了什麼。

3. 上傳推送 (git push)
把本地做好的這個新版本，推送到 GitHub 上。

Bash

git push
解釋：注意到了嗎？第二次以後，我們只需要打 git push 就好，不用再打 -u origin main 那一長串了，因為 Git 已經記住預設路徑了。