# WBUS DB
WBUS DB는 WBUS(http://play.google.com/store/apps/details?id=com.tarks.transport)에 사용되는 버스 DB 정보 저장소입니다.


##1. 구성

1. [index.html](https://github.com/jeonghunn/wbus_db/blob/master/index.html)
버스 DB를 이루는 JSON구조의 파일입니다. 버스 정류장 정보 등이 들어 있습니다.  참여하실 때 이 파일을 수정하신 후  pull request 하시면 됩니다.

“`
{"station_latitude":36.797163,"station_longitude":127.100359,"station_name":"펜타포트","country_srl":1,"route_srl":1,"station_srl":7,"way_srl":1}
“`

정류장 정보 형식은 위와 같습니다.

station_latitude : 정류장이 위치한 위도값입니다.
station_longitude : 정류장이 위치한 경도값입니다.
station_name : 정류장 이름값입니다.
country_srl : 지역 번호입니다. 약속된 지역 번호의 값은 [링크](https://github.com/jeonghunn/wbus_db/blob/master/country_srl.md)에서 확인하실 수 있습니다.
route_srl : 버스 노선 번호입니다.
way_srl : 방향 번호입니다. 한쪽 방향으로 가는 걸 1이라고 한다면 반대쪽 방향으로 가는걸 2라고 합니다. 양쪽 방향으로 가는거 외 다른 경우의 수가 있다면 3, 4 등 다른 숫자를 붙일 수 있습니다.
station_srl : 정류장 번호입니다. 방향에 따라 시작 지점에서 숫자 1을 시작으로 오름차순으로 매깁니다.

2. [country_srl](https://github.com/jeonghunn/wbus_db/blob/master/country_srl.md)

약속 된 지역 번호를 정리한 문서입니다.

3. [db_version](https://github.com/jeonghunn/wbus_db/blob/master/db_version.html)

DB 정보의 버전값이 있는 파일입니다. 클라이언트가 가지고 있는 값과 비교해서 다를경우 최신의 정보를 받는걸 요청합니다.

## 2. 참여하기

버스 정류장 DB 정보를 자신이 직접  추가하고, 개선하고 기여할 수 있습니다. 이는 보다 나은 사용자 경험을 제공합니다.
자신의 저장소로 fork한 뒤에 Pull request를 하여 변경한 사항 적용을 요청할 수 있습니다.

[Pull Request 하는 방법](https://www.xpressengine.com/devlog/22791272)

[DB 수정하기](https://github.com/jeonghunn/wbus_db/edit/master/index.html)

또는 Github 계정이 없거나, 어렵다면 wearbus@gmail.com으로 변경사항을 이메일로 보내주세요. 

감사합니다.
