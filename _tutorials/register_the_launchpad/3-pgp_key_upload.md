---
layout: tutorial
category: 런치패드에 가입하기
title: 3. PGP키를 LaunchPad에 등록하는 방법에 대해 배웁니다.
order: 3
---

1. 좌측 상단의 Log in / Register를 클릭합니다

![main page](img/LaunchPad_main-page.PNG)

1. I am a returning user and my password is:를 체크하면 비밀번호 입력 양식이 보입니다.
2. 이메일과 비밀번호를 입력하고 로그인 버튼을 누릅니다.
1. 이름과 이메일을 확인하고 **Yes, log me in**을 누릅니다.

![login page](img/login_page.PNG)

1. 좌측 상단의 본인 닉네임을 클릭합니다.

![main page](img/main_page.PNG)

1. 아래와 같은 페이지가 열립니다.
1. 프로필 화면의 우측에 있는 Change details, Change branding을 눌러 유저 정보를 꾸밀 수 있습니다.
1. Languages와 Time zone을 설정하여 본인의 시간대와 언어를 설정할 수 있습니다.
1. OpenPGP keys의 연필 아이콘을 클릭하여 PGP키를 등록합니다.
1. 다시한번 로그인합니다.

![user page](img/user_page.PNG)

1. Fingerprint 박스에 예제와 같이 Fingerprint를 입력합니다.
2. Import Key를 누르면 잠시후 이메일로 인증 메일이 도착합니다.

![PGP page](img/PGP_key.PNG)

1. 다음과 같이 온 메일의 PGP MESSAGE 부분을 복사하여 새 파일에 저장합니다.

![email](img/email.PNG)

1. 다음과 같이 입력하여 암호를 해제합니다.

> gpg --decrypt [FILE NAME]

1. 맨 하단의 링크로 들어가 키 등록을 끝냅니다.


