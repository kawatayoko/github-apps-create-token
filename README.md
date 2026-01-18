# github-apps-create-token
## 環境変数設定
export APP_ID="2679467"
export PRIVATE_KEY=$(cat [秘密鍵ファイルのpath])
export GITHUB_REPOSITORY_OWNER=$(gh config get -h github.com user)
export TARGET_REPO="github-apps-test1"
export GITHUB_API_URL="https://api.github.com"
export GITHUB_OUTPUT="./token.txt"

## 環境変数設定（github workflows）
gh secret set APP_ID --body "2679467"
gh secret set PRIVATE_KEY < [秘密鍵ファイルのpath]