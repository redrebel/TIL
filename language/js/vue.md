만일 크롬에서 [Vue.js devtools](https://chrome.google.com/webstore/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd)를 사용하여 디버깅을 하려고하는데
```
Devtools inspection is not available because it's in production mode or explicitly disabled by the author.
```
라는 메시지가 뜨면서 안될때엔
vue 파일에
`Vue.config.devtools = true;` 를 넣으면 된다.


Vue.js 필수 라이브러리
1. Vue-router
2. vuex
3. vueloader

추가적인 라이브러리
1. Vee-validate : 폼유효성 검사
2. Vue-auth : 인증
3. axios : api호출
4. Vue-resource (X비추, axios 를 사용)
