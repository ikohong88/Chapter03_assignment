# 항해99_3주차 개인 과제
------------
## 요구사항
>  `서비스 완성`, `AWS 배포` 두 가지를 모두 완수해야 합니다.
### `서비스 완성`
1. 전체 게시글 목록 조회 API
    - 제목, 작성자명, 작성 날짜를 조회하기
    - 작성 날짜 기준으로 내림차순 정렬하기
2. 게시글 작성 API
    - 제목, 작성자명, 비밀번호, 작성 내용을 입력하기
3. 게시글 조회 API
    - 제목, 작성자명, 작성 날짜, 작성 내용을 조회하기 
    (검색 기능이 아닙니다. 간단한 게시글 조회만 구현해주세요.)
4. 게시글 수정 API
    - API를 호출할 때 입력된 비밀번호를 비교하여 동일할 때만 글이 수정되게 하기
5. 게시글 삭제 API
    - API를 호출할 때 입력된 비밀번호를 비교하여 동일할 때만 글이 삭제되게 하기

### `AWS 배포`
1. RDS 연결
    - MySQL을 이용하기
2. EC2 배포
    - Ubuntu EC2 를 구매한 뒤, 8080 포트와 80번 포트를 연결하여 포트 번호 없이도 서비스에 접속 가능하게 하기
------------
## 개발 툴
> - IntelliJ Ultimate

## 서버 환경
> - AWS (Ubuntu Server 22.04 LTS)

## 데이터베이스 환경
> - AWS (RDS - MySQL)

## 종속성
> - Lombok
> - JPA
> - SpringWeb
> - MySQL

## API 설계
![API 설계 - 3주차 과제](https://user-images.githubusercontent.com/85264446/177257347-4bd8c265-be3f-4118-be89-8815bfa4db7e.PNG)

## 데이터베이스 설계
![데이터베이스 설계](https://user-images.githubusercontent.com/85264446/177257260-c2975d60-5216-44d7-a8ea-8a9f3aeec5e2.PNG)
> - title : 게시글 제목
> - name : 작성자 이름
> - password : 게시글 비밀번호
> - post : 게시글 내용
> - created_at : 게시글 생성일자
> - modified_at : 게시글 수정일자
