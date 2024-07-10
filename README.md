# elibrary 영원한 도서관

## 1. 프로젝트 내용
elibrary(영원한도서관)는 전자도서관을 구축하고 사용자가 대출한 도서데이터를 기반으로 해당 사용자 및 사용자의 나이와 비슷한 사용자들이 선호할만한 도서 혹은 최근에 대출한 도서와 비슷한 줄거리를 가지거나 유사한 장르의 도서를 추천해주는 기능을 가지고 있습니다.

2023.02.27 ~ 2023.03.26(28일)


## 2. 개발환경
- **운영체제**: Windows
- **IDE**: VScode, Oracle SQL Developer
- **서버**: Apache Tomcat 9.0
- **저장소 관리**: GitHub, Maven

### Front-end
- **Language**: HTML5, CSS3, JavaScript
- **Framework**: jQuery, Bootstrap
- **Methodology**: Ajax

### Back-end
- **Language**: Java 11, JSP, Python
- **Framework**: Spring, MyBatis, Tiles

### 데이터베이스
- **Database**: Oracle Database
- **Tool**: Oracle SQL Developer

### API
- **API 사용**:
  - 국립중앙도서관 ISBN 서지정보 API
  - 도서관정보나루 인기대출도서 API
  - Kakao Developers API


## 3. 주요기능
- 회원가입, 로그인, 회원탈퇴
- 관리자 회원가입, 로그인, 회원관리, 도서관리
- 도서명, 저자명, 출판사별 검색기능
- KDC 분류에 따른 분류별 도서 조회
- 도서 대출, 반납, 대출연장 기능
- 대출받은 사용자만 가능한 별점, 리뷰기능
- 대출도서 데이터 기반 도서추천 기능
- 사용자 주소지 인근 도서관 안내 기능


## 4. 기여내용
- ERD 다이어그램 작성, 프로젝트 테이블 구성 계획
![elibrary_ERD](https://github.com/EastCanyon/elibrary/blob/main/elibrary_ERD.png)

- 일반회원 회원가입, 로그인, 회원탈퇴 기능 구현
![elibrary_signup](https://github.com/EastCanyon/elibrary/blob/main/elibrary_signup.png)
![elibrary_login](https://github.com/EastCanyon/elibrary/blob/main/elibrary_login.png)
![elibrary_delete](https://github.com/EastCanyon/elibrary/blob/main/elibrary_delete.png)

- 도서 대출연장 및 자동 반납 기능 구현
![elibrary_borrow1](https://github.com/EastCanyon/elibrary/blob/main/elibrary_borrow1.png)
![elibrary_borrow2](https://github.com/EastCanyon/elibrary/blob/main/elibrary_borrow2.png)
![elibrary_borrow3](https://github.com/EastCanyon/elibrary/blob/main/elibrary_borrow3.png)

- KDC 분류별 도서 조회 기능
![elibrary_KDC](https://github.com/EastCanyon/elibrary/blob/main/elibrary_KDC.png)


## 신경쓴 부분

- **맞춤도서추천 기능**: 파이썬 Flask를 이용하여 카카오도서 API에 저장되어 있는 줄거리의 형태소를 분리 후 상관관계를 분석해 가장 높은 상관관계를 가진 도서를 추천하여 추천기능의 정확도를 높이기 위해 노력했습니다.
- **RESTful API 설계**: 클린 아키텍처를 유지하고, 각 API의 책임을 명확히 하기 위해 노력했습니다.
- **보안**: 사용자 인증 및 권한 부여를 강화하고, 데이터베이스에 저장되는 정보를 안전하게 보호하기 위해 노력했습니다.
