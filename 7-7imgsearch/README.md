## 로컬에서 직접 수동 배포 (Netlify CLI)

npm install -g netlify-cli

# 초기 연결

netlify login
netlify init

# 배포

- build/ 폴더 기준으로 업로드
  npm run build
  netlify deploy --prod

# 확인

- 홈피에서
  netlify.com
