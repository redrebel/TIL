npm install 옵션
-D: --save-dev

1. 초기화  
`npm init --yes`

- lite-server 설치  
`npm install lite-server --save-dev`

- bs-config.js 파일생1.
```JavaScript
// bs-config.js
{
    "server": {
      // 홈 디렉토리 경로
        "baseDir": "./public"
    },
    "open":false
}
```

- package.json 파일수정
```JavaScript
// package.json
{
  "name": "jq-to-vue",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    // 아래부분으로 수정
    "dev": "lite-server"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "lite-server": "^2.3.0"
  }
}
```
- 적당한 html / js 파일을 작성하여 저장한다.
- 웹서버를 실행한다.  
```npm run dev```
