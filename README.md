## npm 패키지 제작 후 사용 프로젝트
verdaccio 버다치오
Verdaccio는 프라이빗 NPM 레지스트리 서버입니다.
내부에서만 NPM 패키지를 배포하거나 테스트할 때 유용.
예: 회사 팀원들끼리만 쓰는 공용 패키지를 배포할 때 사용.

# 실행방법
npx verdaccio 

# 배포 방법 
- 터미널 하나더 띄워서 명령어 입력
npm publish --access=public --registry=http://localhost:4873


# 캐시삭제 후 재 배포
rm -rf node_modules package-lock.json
npm version patch
npm publish --access=public --registry http://localhost:4873


