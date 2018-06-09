만일 크롬에서 (https://chrome.google.com/webstore/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd)[Vue.js devtools]를 사용하여 디버깅을 하려고하는데
```
Devtools inspection is not available because it's in production mode or explicitly disabled by the author.
```
라는 메시지가 뜨면서 안될때엔
vue 파일에
`Vue.config.devtools = true;` 를 넣으면 된다.
