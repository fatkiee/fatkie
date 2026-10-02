# 1. 切換回主分支並拉取最新程式碼
git switch main
git pull

# 2. 建立並切換到新功能分支
git switch -c feature/user-profile

# 3. (進行程式碼修改與 Commit)
git add .
git commit -m "feat: 新增使用者個人頁面"

# 4. 完成後切換回主分支並合併
git switch main
git merge feature/user-profile

# 5. 清理已合併的臨時分支
git branch -d feature/user-profile