### Javascript location 객체의 프로퍼티와 메서드 정리

#### location 객체의 프로퍼티와 메서드

**프로퍼티**

`hash`: URL 중에서 #로 싲가하는 해시 부분의 정보를 담고 있다.

`host`: URL의 호스트 이름과 포트 번호를 담고 있다.

`hostname`: URL의 호스트 이름이 저장된다.

`href`: 전체 URL이다. 이 값을 변경하면 해당 주소로 이동할 수 있다.

`pathname`: URL 경로가 저장된다.

`port`: URL의 포트 번호를 담고 있다.

`protocol`: URL의 프로토콜을 저장한다.

`password`: 도메인 이름 앞에 `username` 과 `password` 를 함께 입력해서 접속하는 URL일 경우에 `password` 정보를 저장한다.

`search`: URL 중에서 ?로 시작하는 검색 내용을 저장한다.

`username`: 도메인 이름 앞에 `username` 을 함께 입력해서 접속하는 사이트의 URL일 경우에 `username` 정보를 저장한다.



**메서드**

`assign()`: 현재 문서에 새 문서 주소를 할당해서 새 문서를 가져온다.

`reload()`: 현재 문서를 다시 불러온다.

`replace()`: 현재 문서의 URL을 지우고 다른 URL의 문서로 교체한다.

`toString()`: 현재 문서의 URL을 문자열로 반환한다.