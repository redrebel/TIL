

### How to clear / delete the content of StringBuffer or StringBuilder. (StringBuffer 나 StringBuilder 를 초기화하는 방법)

there are 3 way.
(3가지 방법이 있습니다.)

1. stringBuilder.setLength(0);
2. stringBuilder.delete(0, StringBuilder.size());
3. stringBuilder = new StringBuilder();

I think, 1st way is the best way.  
Because ...

1번 방법이 가장 좋아보인다.  
이유는 코드리딩에 이해하기 편하고 성능도 좋아보이기 때문이다.

코드리딩때 이해하기 편한 것만 따지자면 3번이 가장 좋아 보이지만,  
웬지 loop 문을 돌면서 사용해야되는 경우  
매번 StringBuilder를 생성하는게 안좋아보여서이다.  
물론 제가 틀렸거나 다른 의견들이 있을 수 있다.

각 경우에 따라서 성능 이슈등 여러가지 의견들이 있다.

http://stackoverflow.com/questions/2242471/java-clearing-the-string-buffer-after-loop  
http://stackoverflow.com/questions/5192512/how-can-i-clear-or-empty-a-stringbuilder  
http://stackoverflow.com/questions/18766780/stringbuilder-reset-or-create-a-new  
https://blog.outsider.ne.kr/265

### Object의 타입이 확실히 String 인걸 보장할때 .toString() 보다 (String) 캐스팅이 2배이상 빠르다.
참고로 String.valueOf() 는 비추한다.   
만일 Object 가 null 일 경우 to.String() 이나 (String) 은 null 에러를 발생시키지만
String.valueOf() 은 "null" 을 반환하므로 잠재적인 장애의 원인이 될 수 있다.

http://www.cowtowncoder.com/blog/archives/2008/12/entry_119.html
http://stackoverflow.com/questions/676363/string-or-tostring
