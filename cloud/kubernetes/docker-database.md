# MSSQL 설치
## 이미지 다운로드
docker pull microsoft/mssql-server-linux
## 이미지 실행
docker run -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=yourStrong(!)Password' -p 1700:1433 --name mssql -d microsoft/mssql-server-linux

## 확인
docker ps -a

## SA 암호변경
docker exec -it <컨테이너ID> /opt/mssql-tools/bin/sqlcmd -S localhost -U SA -P 'yourStrong(!)Password' -Q 'ALTER LOGIN SA WITH PASSWORD="<YourStrong!Passw0rd>"'


## container 접속
docker exec -it <컨테이너ID> "bash"

## sqlcmd 연결하기
/opt/mssql-tools/bin/sqlcmd -S localhost -U SA -P '<YourStrong!Passw0rd>'

## 데이터베이스 생성
CREATE DATABASE TestDB --데이터베이스 생성
SELECT Name from sys.Databases -- 데이터베이스 목록 보기
go -- 쿼리 실행하기

## 테이블 생성하여 데이터 insert 하기
USE TestDB -- TestDB 사용
CREATE TABLE CITY( id int IDENTITY (1,1) , name varchar(20) NOT NULL,  state varchar(20) NOT NULL,  country varchar(20) NOT NULL,  CONSTRAINT PK_CITY PRIMARY KEY(id) )
insert into city (name, state, country) values ('San Francisco', 'CA', 'US');
go

select * from information_schema.tables -- 테이블 목록보기


https://docs.microsoft.com/ko-kr/sql/linux/quickstart-install-connect-docker?view=sql-server-2017
docker로 MSSQL을 설치히는 법



# Oracle 설치

오라클 express edition 11g release 2
https://hub.docker.com/r/wnameless/oracle-xe-11g
