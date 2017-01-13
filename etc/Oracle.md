### 계정 생성(이하 시스템/관리자 계정)
CREATE USER [유저아이디] IDENTIFIED BY [비밀번호];

\*비밀번호 생성시 특수문자가 입력이 안될때 비밀번호 앞뒤로 "비밀번호"라고 감싸주면 된다.

### 비밀번호 변경
ALTER USER [유저아이디] IDENTIFIED BY [새로운 비밀번호];

### 접속 및 객체에 대한 접근권한
GRANT CREATE SESSION TO [유저아이디];
GRANT SELECT ON [테이블소유자.테이블이름] TO [유저아이디];

### SELECT 확인(유저아이디로 로그인)
SELECT * FROM [테이블소유자.테이블이름]

### SYNONYM(별칭) 지정
CREATE SYNONYM [별칭.흔히 테이블명지정] FOR 테이블소유자.테이블이름
