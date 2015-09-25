# SocialLink_Kimsq1.2
소셜링크 kimsq v1.2용 / Facebook Login SDK V5로 수정

## SocialLink Facebook Login 연동에러 원인
- Facebook API V2.0까지만 FQL이 공식지원되고, 그 이후 버젼은 FQL를 사용할 수 없다.
> 자세한 사항은 [Facebook Platform Upgrade Guide v2.0 to v2.1](https://developers.facebook.com/docs/apps/upgrading#v2tov21)을 참고하기 바란다.
- 현재 킴스큐 마켓에 판매되는 SocialLink는 Facebook v2.0을 사용하고 있으며, Facebook App을 새로 생성할 경우 현재(2015.09.25 기준) 기본 Facebook API 버젼 2.4으로 셋팅된다.
- 따라서, Facebook API v2.1에서 사라진 FQL로의 로그인이 불가능하며, kimsq v1.2와 연동되지 않는 이유이다.

## SocialLink Facebook Login 연동에러 해결 방법
- SocialLink Module내에 사용하는 PHP SDK를 현재기준 최신 버젼인 v5.0으로 변경하고, 공식적으로 사용을 권장하는 Facebook Graph API를 사용한다.

## Facebook Graph API로 옮기면서 생기는 추가 문제
- SocialLink Facebook Login 진행시, Facebook의 정보를 끌어오는 필드가 총 

FACEBOOK LOGIN 연동이 문제가 되어왔지만, 유료 모듈임에도 불구하고 그에 대한 제작자의 대응이 없는 관계로 원본 파일 수정 및 OPEN SOURCE KIMSQ 개발 정신에 입각하여 수정된 파일을 공개함.

원본 : 킴스큐 유료 SOCIAL LINK : http://www.kimsq.co.kr/market/26/
제작자 : 레드블럭
