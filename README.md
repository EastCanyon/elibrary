# elibrary

## 1. 프로젝트 내용
elibrary(영원한도서관)은 전자도서관을 구축하고 사용자가 대출한 도서데이터를 기반으로 해당 사용자 및 사용자의 나이와 비슷한 사용자들이 선호할만한 도서를 추천해주는 기능을 가지고 있습니다.


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

## 신경쓴 부분

- **RESTful API 설계**: 클린 아키텍처를 유지하고, 각 API의 책임을 명확히 하기 위해 노력했습니다.
- **테스트 커버리지**: 주요 비즈니스 로직에 대해 단위 테스트와 통합 테스트를 작성하여 안정성을 높였습니다.
- **보안**: 사용자 인증 및 권한 부여를 강화하고, 데이터베이스에 저장되는 정보를 안전하게 보호하기 위해 노력했습니다.
