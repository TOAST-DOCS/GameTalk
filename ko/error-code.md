## Game > GameTalk > 오류 코드

## Client SDK

| Platform           | Error                                    | Error Code | Description                              |
| ------------------ | ---------------------------------------- | ---------- | ---------------------------------------- |
| Android, iOS | NOT_INITIALIZED | 1 | GameTalk SDK가 초기화되어 있지 않습니다. |
| Android, iOS | NOT_LOGGED_IN | 2 | 로그인이 되어 있지 않습니다. |
| Android, iOS | ALREADY_INITIALIZED | 3 | GameTalk SDK가 이미 초기화되어 있습니다.  |
| Android, iOS | ALREADY_LOGGED_IN | 4 | 이미 로그인이 되어 있습니다. |
| Android, iOS | INVALID_PARAMETER | 5 | 잘못된 파라미터입니다. |
| Android, iOS | RESPONSE_TIMEOUT | 11 | 네트워크 상태가 불안정하여 응답이 없습니다. |
| Android, iOS | NOT_SUPPORTED | 91 | 지원하지 않는 기능입니다. |
| Android, iOS | NOT_SUPPORTED_ANDROID | 92 | Android에서 지원하지 않는 기능입니다. |
| Android, iOS | NOT_SUPPORTED_IOS | 93 | iOS에서 지원하지 않는 기능입니다. |
| Android, iOS | SOCKET_CONNECTION_FAILED | 101 | 소켓 연결에 실패했습니다. |
| Android, iOS | SOCKET_CONNECTION_TIMEOUT | 102 | 소켓 연결 중 시간 초과가 발생했습니다. |
| Android, iOS | SERVER_INTERNAL_ERROR | 201 | 서버 오류가 발생했습니다. |
| Android, iOS | INVALID_SERVER_RESPONSE | 202 | 서버에서 잘못된 응답이 전달되었습니다. |
| Android, iOS | API_ID_IS_EMPTY | 203 | 서버 응답에 API ID가 누락되어 있습니다. |
| Android, iOS | HEADER_IS_NULL | 204 | 서버 응답에 Header가 누락되어 있습니다. |
| Android, iOS | TRANSACTION_ID_IS_EMPTY | 205 | 서버 응답에 Transaction ID가 누락되어 있습니다. |
| Android, iOS | MESSAGE_LIMIT_EXCEEDED | 301 | 메시지의 길이가 한도를 초과하였습니다.  |
| Android, iOS | UNKNOWN_ERROR | 999 | 알 수 없는 오류가 발생했습니다. |

## Server
| Module  | Error Code            | Description                              |
| ------- | --------------------- | ---------------------------------------- |
| Common  | -4000001<br/>-4000006 | 잘못된 파라미터 유형으로 API 호출 <br/>- 예) 파라미터는 int형으로 선언돼 있는데, string형 데이터로 API가 호출됨 |
|         | -4000002<br/>-4000004<br>-4000005 | 필수 파라미터가 생략되었거나 값이 없을 때, 부적절한 값으로 호출될 때 <br> |
|         | -4000003              | Request body에 정의되지 않은 값이 전달된 경우 |
|         | -4000007              | 더 이상 지원되지 않는 API 버전을 호출 |
|         | -4000008              | 파라미터 길이가 초과됨 |
|         | -4010002              | 잘못된 AppKey가 호출됨 |
|         | -4010003              | 인증되지 않은 클라이언트에서 인증이 필요한 API를 호출한 경우 |
|         | -4010004              | 잘못된 비밀 키(secret key)가 호출됨 |
|         | -4060001              | HTTP 헤더에 Content-Type을 잘못 설정 |
|         | -4060002              | Deprecated API 버전을 호출 |
|         | -4060003              | 잘못된 API 버전을 호출 했거나, 잘못된 URI로 호출한 경우 |
|         | -4090001 ~ 4          | 내부 DB 관련 오류 |
|         | -4150001              | 잘못된 형식의 JSON 데이터 전달 |
|         | -5000001 ~ 15         | 내부 시스템 오류 |
| Front   | -4150102              | 요청 타임 아웃 |
|         | -5000101<br/>-5000102<br/>-5040102 | 내부 시스템 오류 |
| Back    | -4000201              | 지원되지 않는 IdP로 인증 요청한 경우 |
|         | -4000202<br/>-4000203 | 지원되지 않는 API를 호출 |
|         | -4000204              | 지원되지 않는 LanguageCode로 호출 |
|         | -4010201<br/>-4010202<br/>-4040201<br/>-4040203 | 내부 오류. 계속 발생시 고객센터를 통해 문의 필요 |
|         | -4040202              | 채널 없음 |
|         | -4040204              | 인증 정보가 등록되지 않은 경우 |
|         | -4290201              | 채널 생성 한도 초과 |
|         | -4290202              | 태그 생성 한도 초과 |
|         | -4290203              | 채널의 구독 한도 초과 |
|         | -4290204              | 채널의 태그 한도 초과 |
|         | -4290206<br/>-4290207 | 채널 관련 오류 |
|         | -4290208              | 메시지 전송 관련 오류 |
|         | -4290209              | 메시지 조회 관련 오류 |
|         | -4290210              | 채널 구독 관련 오류 |
|         | -4290211<br/>-4290212 | 태그 관련 오류 |
|         | -4290213<br/>-4290214 | 메시지 전송자 관련 오류 |
|         | -4290215              | 금칙어에 의한 전송 메시지 차단 |
|         | -4290216              | 인증 관련 오류 |
|         | -5000201 ~ 5<br/>-5040201<br/>-5040202<br/>-5100201 | 내부 시스템 오류 |

