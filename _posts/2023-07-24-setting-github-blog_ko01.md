---
layout: post
title: Github Blog 만들기
subtitle: Github blog 세팅하는 법에 대해 알아봅시다.
author: SH-Kwon
categories: [Setting Guide]
tags: [githubblog, setting_guide]
---
## Github Blog용 Page 생성

### Page Repository 생성
먼저 Github에 들어가 우측 상단의 +버튼을 누르고 ‘New repository’를 선택하여 새 레포지토리를 생성하는 페이지로 넘어갑니다.
![createnewRepo1](/assets/images/posts/installtheme/0-1.make_newrepo1.png)


### Github desktop 설치


### PC에 local repository clone 해주기


### Git desktop 사용법




### Ruby 설치
Ruby 설치 방법은 [이 포스트][RubyinstallGuide]를 참조하여 설치하시면 됩니다.


[RubyinstallGuide]: (2023-07-28-install-ruby_ko.md)








### 루비 인코딩


### jekyll 설치


### Jekyll 사이트 레포지토리에 생성하기




새 사이트를 생성할 때 에러가 나는 경우가 왕왕 있습니다. 필자가 겪었던 에러에 대해 대처법을 알아봤는 데 대처법은 아래와 같습니다.
![createSiteError](/assets/images/posts/installtheme/1-6create_jsite-error.png)


Error : ~ new; is not empty
사이트를 생성하고자 하는 폴더에 파일이 존재할 경우 나타나는 메세지입니다.


따라서, 파일을 다른 곳에 저장하거나 삭제하여 사이트로 만들고자 하는 폴더를 비워준 뒤에 다시 명령어를 실행하면 문제없이 실행됩니다.


site를 생성하기 전에 앞서 각자의 Git desktop의 사용법을 익히기 위해 github.io폴더에 index.html을 작성하는 과정을 거쳤습니다. 이 과정상에서 site를 생성하고자 하는 github.io폴더에 파일이 존재하는 상태가 되었기 때문에 해당 가이드 문서에 따라 작성하신 것이라면 index.html 파일만 존재할 것이므로 해당 파일만 삭제한 후 다시 site 생성을 시도하시면 됩니다.


또 다른 해결 방법으로는 파일을 그대로 둔 채로 강제로 사이트를 생성하는 명령어를 실행하는 법이 있습니다.
실제로 실행해보면 각종 페이지용 파일들이 생성되는 한편, 사이트를 생성하고자 하는 폴더에 원래 있던 파일은 그대로 남아 있는 것을 확인할 수 있습니다.


![createSiteForce1](/assets/images/posts/installtheme/1-6create_jsite-force1.png)


이러한 경과를 봤을때 개인적인 추측으로는, 사전에 README.md라던가 기타 블로그에 필요한 파일들, 그 외 블로그와는 상관이 없으나 사이트를 생성하면서 생성될 파일들과 이름이 겹치는 파일들이 있을 때를 대비한 것 같습니다. 덮어쓰기가 되면서 기존 파일들의 데이터가 날라가기 때문에 백업을 해두라는 의미에서 이런 에러를 출력해주는 걸로 하지 않았나 싶습니다.




### Jekyll 서버를 로컬로 돌리기
아래 명령어를 입력합니다.
bundle install


아래 명령어를 입력하여 로컬 상에서 jekyll 서버를 구동시켜줍니다.
bundle exec jekyll serve


이후 인터넷 익스플로러, 크롬 등의 인터넷 프로그램을 실행시킨 뒤, 주소창에 'localhost:4000'을 입력시켜주면 테마를 적용시킨 블로그가 표시되는 것을 확인할 수 있습니다.


앞으로 블로그에 포스트를 올리거나, 수정, 삭제하기전 먼저 테스트할 때는 위 순서대로 돌려서 로컬에서 먼저 적용을 시킨 이후, git desktop을 이용해 branch에 commit, push해서 실제 블로그에 적용시키면 됩니다.






### Jekyll 테마 적용
[jekyll 테마 사이트][jekyllThemesSite]에서 마음에 드는 테마를 골라줍니다.


[jekyllThemsSite]:http://jekyllthemes.org/


## 로컬에서 블로그 테마 적용 테스트 해보기


![settingThemes1](/assets/images/posts/installtheme/1-3setting_themes1.png)


![settingThemes2](/assets/images/posts/installtheme/1-3setting_themes2.png)


![settingThemes3](/assets/images/posts/installtheme/1-3setting_themes3.png)


![settingThemes4](/assets/images/posts/installtheme/1-3setting_themes4.png)

0-1.make_newrepo1.png


노래 you know what to say
