# deeplink

제일 먼저 아이폰에서는 딥링크를 지원하지만 앱 설치 후 까지 데이터를 넘길 수 있는 방법이 없습니다.

유니버셜 링크라는게 있는데 이건 웹 페이지 작업까지해야 해서 개발 범위가 엄청 커집니다.

그외 여러 방안들에 대해서 확인했는데 딥링크 나 아래 설명한 링크 생성해서 호출하는 방식 입니다.

1. Firebase Dynamic Link :

	https://firebase.google.com/docs/dynamic-links/use-cases/web-to-app?hl=ko

	1. A 앱에서 딥링크 호출을 위한 웹 페이지 이동
		-  페이지 호출 시 key 값과 value값 전달

	2. 웹페이지에서 동적  링크 생성해서 바로 앱스토어 나 앱 호출

	3. B 앱에서 파이어베이스를 통해 데이터 전달 받음.


2. 브랜치 : https://branch.io/

	활용방안 : https://branch.io/how-branch-links-work/

	1.  Web SDK 활용하여 링크 생성
		- 페이지 호출 시 key 값과 value 값 전달

	2. 링크 호출 데이터 전달

	3. B 앱에서 데이터 파싱해서 사용

3. 에어브리치 : https://docs.airbridge.io

	1. 트래킹링크를 생성

	2. 트래킹링크를 A 앱에서 호출 : https://docs.airbridge.io/ko/advance/2-1-5.html

	3. B 앱에서 트래킹링크를 지연된 딥링크로 지원 : 
	https://docs.airbridge.io/ko/advance/2-6-2.html
