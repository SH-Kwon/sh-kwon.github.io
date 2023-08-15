---
layout: post
title: Ruby 설치
subtitle: Ruby를 설치하는 법에 대하여 알아봅시다.
author: SH-Kwon
categories: [Setting Guide]
tags: [ruby, tool, setting_guide]
---
## Ruby에 대하여

## Ruby 인스톨러 받기
구글에 Ruby를 검색하여 [공식홈페이지][RubyPage]로 들어갑니다. 만약 본인이 Ruby를 설치하고자 하는 PC의 OS가 윈도우라면, 구글에 Ruby Installer를 검색해서 바로 [인스톨러 홈페이지][RubyInstallerPage]로 들어가도 무방합니다.

[RubyPage]: https://www.ruby-lang.org/en/
[RubyInstallerPage]: https://rubyinstaller.org/

![Ruby Installer download 1](/assets/images/posts/installtheme/1-1down_ru1.png)

Download Ruby를 누른 후, 나온 페이지에서 보면 알 수 있듯, 본인의 OS에 따라 RVM을 통해 Ruby를 통해 설치를 하거나  Installer를 다운로드 받아 설치해야 합니다. Windows OS 환경일 경우 앞서 언급했던 Ruby Installer 페이지로 이동하여 인스톨러를 받아줍시다.

![Ruby Installer download 2](/assets/images/posts/installtheme/1-1down_ru2.png)

Download를 누르면 버전별 Installer를 다운로드 받을 수 있는 사이트로 이동합니다.

![Ruby Installer download 3](/assets/images/posts/installtheme/1-1down_ru3.png)

제일 최신버전으로 받아줍니다.(Bold체로 강조되어 있음.)

![Ruby Installer download 4](/assets/images/posts/installtheme/1-1down_ru4.png)


## Ruby 인스톨러를 통해 설치 - Windows 환경
앞서 다운로드받은 Ruby 인스톨러를 통해 설치를 해봅시다.
인스톨러를 다운받은 뒤 실행해주면 라이센스에 동의하는 가에 대한 여부를 물어봅니다. 동의를 눌러 다음 단계로 넘어갑니다.

![Ruby Install 1](/assets/images/posts/installtheme/1-2install_r1.png)

원하는 설치 경로를 선택한 후 다음 단계로 넘어갑니다.
아래 옵션들에 대해서는 인스톨러 창의 TIP에서 볼 수 있듯, 마우스를 가져다대면 옵션에 대한 상세설명을 볼 수 있습니다.
'Add Ruby executables to your PATH'는 Ruby에 대한 환경변수를 추가할 것인지에 대한 옵션입니다.
'Assosciate .rb and rbw files with this Ruby installation'는 Ruby 인스톨러를 설치하고 나면 Ruby prompt를 실행할 수 있게 되는데, 해당 확장자 파일을 더블클릭하거나 Ruby prompt에서 실행할 수 있게 연동하는 것에 대한 옵션입니다.
현재는 없어진 옵션이지만, 간혹 다른 설치 가이드글 중에 오래된 글들을 보면 "Use UTF-8 as default external encoding' 옵션이 있는데, 이 옵션이 있었던 이유는 Ruby 2.0부터 default external encoding이 UTF-8로 되었기때문입니다.

![Ruby Install 2](/assets/images/posts/installtheme/1-2install_r2.png)

RI는 오프라인 기본 메뉴얼문서(man page)로, 인터넷이 연결되어 있지 않은 환경에서 참조할 수 있는 문서입니다.

[MSYS2][MSYS2Page]는 윈도우 소프트웨어를 실행하거나 설치, 개발하기에 좋은 환경을 구성해주는 일종의 도구 모음입니다.
Cygwin이라고 하는 오픈소스 툴을 바탕으로 만들어졌는데, 윈도우 환경에서 gcc, mingw-w64, CPython, CMake, OpenSSL, Rust, Ruby에 대한 네이티브 빌드(가상머신상에서가 아닌, 호스트 OS상에서 바로 직접적으로 실행되는 환경)를 제공합니다.
저는 default값 그대로 둔 채 다음 단계로 넘어갔습니다.

[MSYS2Page]: https://www.msys2.org/
![Ruby Install 3](/assets/images/posts/installtheme/1-2install_r3.png)

여기서 MSYS2를 설치위해 ridk 툴을 실행시키는 옵션이 default로 체크되어있는데 저는 기본값 그대로 하고 Ruby 인스톨러를 끝마쳤습니다.
ridk는 Ruby의 버전 2.4 이상의 런타임환경을 관리하는 툴입니다.

![Ruby Install 4](/assets/images/posts/installtheme/1-2install_r4.png)

1번을 선택한 뒤 Enter 키를 누르면 설치가 진행되는 것을 확인할 수 있으며, 'installed properly' 메세지가 뜨면 그냥 Enter 키를 눌러 종료합니다.
![Ruby Install 5](/assets/images/posts/installtheme/1-2install_r5.png)