### 재귀 DNS 확인자
- 클라이언트 재귀 요청에 응답
- DNS 레코드를 추적하는데 시간을 투자
- 요청한 레코드에 대해 권한 있는 DNS 네임서버에 도달 할 때 까지 일련의 요청을 하는 방식(또는 시간 초과나 오류 반환)
- 클라이언트에 응답하는데 필요한 레코드를 추적하기 위해 여러요청 필요X
- 캐싱은 DNS 조회 초기에 요청한 리소스 레코드를 제공하여 필요한 요청을 단락 시키는데 도움이 되는 데이터 지속성 프로세스

### 권한 있는 네임서버
- 실제로 DNS 리소스 레코드를 보유, 담당하는 서버
- 쿼리한 리소스 레코드로 응답하는 DNS 조회 체인의 맨 아래 있는 서버
- 웹 브라우저가 웹 사이트 또는 웹 리소스에 엑세스하는데 필요한 IP 주소에 도달하도록 요청
- 자체 데이터의 쿼리 충족
 
### DNS 레코드
- 권한 있는 DNS 서버에 존재
- 해당 도메인과 연결된 IP 주소 및 해당 도메인에 대한 요청을 처리하는 방법을 포함한 도메인에 대한 정보를 제공하는 지침
- [DNS구문]1)으로 알려진 일련의 텍스트 파일로 구성
- TTL: Time-To-Live. DNS 서버가 해당 레코드를 새로 고치는 빈도.


// 1) DNS 서버에 수행할 작업을 알려주는 명령으로 사용되는 명령어
