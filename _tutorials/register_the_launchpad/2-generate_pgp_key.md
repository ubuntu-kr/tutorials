---
layout: tutorial
category: 런치패드에 가입하기
title: 2. PGP키를 생성하는 방법에 대해서 배웁니다.
order: 2
---

## 시작하기 전에
- PGP는 암호화 프로그램입니다.
- 이 튜토리얼에서는 오픈소스인 GnuPG를 사용할 예정입니다.
- LaunchPad에서 전자서명을 하기 위해 사용할 예정입니다.
- 암호화 방식, 키 길이, 유효시간을 담습니다.
- 사용자의 이름과 이메일 주소가 필요합니다.

## GPG 설치하기
- Ubuntu 사용자의 경우 이미 설치되어있기 때문에 따로 설치할 필요가 없습니다.

### MacOS
1. 다음을 터미널에 붙여넣어 brew를 설치합니다.

> /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

1. 다음을 터미널에 입력해 GPG를 설치합니다.

> brew install gpg

### Windows
1. [GnuPG 다운로드 사이트](https://gnupg.org/download/)에 가셔서 적절한 설치파일을 설치합니다.

---

## PGP키 생성하기

1. 다음을 입력하여 GPG가 제대로 설치되어있는지 확인합니다. 설치되어있지 않다면 위의 GPG설치하기를 진행합니다

> gpg --version

1. 다음을 입력하여 키를 만듭니다.

> gpg --gen-key #gpg1
> gpg --full-gen-key #gpg2

1. 다음 과 같은 설정이 나옵니다 기본값으로 설정하려면 엔터키를 누릅니다.
1. Is this correct? 라는 질문이 나오면 y키를 누릅니다.
1. 이제 기본설정이 완료 되었습니다.

![generate key](img/gen_key.PNG)

1. 다음 이미지를 참고하여 입력합니다.
2. Change (N)ame, (C)omment, (E)mail or (O)kay/(Q)uit? 가 나오면 제대로 입력했는지를 확인한 후 O를 누릅니다.
3. 비밀번호를 입력하면 랜덤바이트를 모읍니다.

![identify key](img/identify_key.PNG)

1. 다음을 입력하여 키 ID를 확인합니다.

> gpg --keyid-format short -k

1. 다음을 입력하여 키를 업로드 합니다.
2. [key-id]에는 방금 확인한 본인의 키 ID를 입력합니다.
1. 동기화 될때까지 기다립니다.

> gpg --send-key --keyserver keyserver.ubuntu.com [key-id]



