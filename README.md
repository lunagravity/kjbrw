
사용법
------

프로젝트 소스코드를 가져옵니다:

    $ git clone https://lunagravity@bitbucket.org/lugr/kjbrw.git


프로젝트폴더로 이동합니다:

    $ cd kjbrw 


의존성 패키지를 설치합니다:

    $ npm install
    

Pre Requirements
---------------
* Git
* Node.js >= 8
* Graphviz
* SQL Server
* SQL Management Studio
* Webstorm
* Webstorm Plugins: .ignore, CMD Support, Markdown support, plantuml


개발환경
--------
* Webstorm 설정: safe write 설정 OFF
    ![예](assets/safe-write.png)
    
* SQL Server 의 1433 포트 오픈
    * 실행: Sql Server 2016 구성 관리자    
    * SQL Server 네트워크 구성 -> MSSQLSERVER에 대한 프로토콜 -> TCP/IP -> 사용
    
* SQL Server: "localhost"에 "GC_KJBRW_MES" Database 추가

* SQL Server: "localhost"에 "DZICUBE" Database 추가

* SQL Server: sa 사용자 사용 가능하도록 설정 (암호 1234로 설정)
    * 실행: SQL Server Management
    * sa 사용 설정: localhost,1433 접속 -> 보안 -> 로그인 > sa(우클릭) -> 속성 -> 상태 -> 로그인: 사용체크
    * sa 암호 지정: 위 화면의 좌측메뉴의 "일반" -> 암호정책 체크해제 -> 암호: 1234로 지정
    * DB 로그인 사용 체크: DB선택(우클릭) -> 속성 -> 보안 -> "SQL Server 및 Windows 인증 모드" 선택
    * DB 재시작: DB선택(우클릭) -> 다시시작
