##### 소개

Jekyll을 사용하려고 보니 아래와 같이 GUN/Linux, Unix, or macOS 에서 사용하라고 되어 있다.

하지만, 아래 추가적인 내용을 살펴보니. window에서도 충분히 사용 가능해 보인다.

즉 Requirements만 만족하면 window에서 구동 가능해 보인다.

그래서, window에서 Jekyll을 사용하는 방법을 살펴 보고 소개한다.

![](/assets/jekyll-requirements.png)

필요한 모듈들.. 아래 모듈을 차례대로 window에서 설치한다.

* Ruby
* Ruby development headers
* RubyGems \(Ruby 설치하면 같이 설치됨\)
* NodeJs
* Python 2.7

##### Ruby 설치

ruby window용 설치가 지원된다. 아래 사이트에서 다운 받아 설치한다.

[https://rubyinstaller.org/downloads/](https://rubyinstaller.org/downloads/)

![](/assets/window-ruby-install.png)

최신 버전으로 설치, 자신의 os 아키텍쳐에 맞는 버전으로 설치한다. 64bit쓰면 x64로

![](/assets/ruby-check.png)

정상 설치되었는지 'ruby --version' 으로 확인 가능하다.

만약 command에러가 나는 경우, window에 PATH 정보에 ruby PATH 정보를 추가한다.

기본적으로 설치시 PATH 옵션을 설정하였다면, 문제 없이 버전 정보를 볼 수 있다.

##### Ruby development headers 설치

ruby development headers는 ruby development kit을 설치하면 된다.

아래 사이트에서 다운 받아서 압축을 해제 한다.

[https://rubyinstaller.org/downloads/](https://www.gitbook.com/book/gseok/web-technology-introduction/edit#)

![](/assets/ruby-dev-kit-install.png)

설치위 위에서 설치한 ruby 버전에 맞는 버전으로 설치한다. ruby development kit의 설치 방법은

[https://github.com/oneclick/rubyinstaller/wiki/Development-Kit](https://github.com/oneclick/rubyinstaller/wiki/Development-Kit) 에 잘 설명되어 있다. Quick guide에 따라

압축 해제한 디렉토리에 가서 다음 명령어를 수행한다.

```ruby
ruby dk.rb init
ruby dk.rb install
```

아래와 같이 출력되면 정상 설치된 것이다.

![](/assets/ruby-dev-kit-install-success.png)

##### RubyGems 설치 확인

아래와 같이 `gem --version`  명령어를 사용해서 확인한다. ruby가 정상 설치되어있다면.

정상적으로 잘 나올 것이다.

![](/assets/rubyGems-check.png)

##### Node.js 설치

[https://nodejs.org/en/](https://nodejs.org/en/)

![](/assets/node.js-install.png)

사이트에서 최신 버전이나 LTS버전을 받아 설치한다.

아래와 같이 출력되면 정상 설치된 것이다.

![](/assets/node-js-install-check.png)

##### Python 2.7 설치

아래 사이트에서 받아서 설치하면 된다. 단 버전에 따라 동작이 다를 수 있음으로 2.7.xx 버전을 찾아서

설치한다.

[https://www.python.org/downloads/](https://www.python.org/downloads/)

![](/assets/python-install.png)

버전을 선택하고 나면 나오는 아래와 같은 화면에서, Window용 설치파일인 windows MSI Installer을 자신의 os

에 맞게 설치한다. 64bit면 x86-64 버전으로...

![](/assets/python-version-files.png)

python을 설치하고 나면, PATH을 설정해 주어야 한다.

```
C:\Python27;C:\Python27\Scripts;
```

제어판 &gt; 모든 제어판 항목 &gt; 시스템 &gt; 고급 시스템 설정 &gt; 환경변수 &gt; 시스템 변수 &gt; Path

을 찾아서, 위 값을 추가한다.

![](/assets/window-env-setting.png)

아래와 같이 출력되면 정상 설치된 것이다.

![](/assets/python-check.png)

##### Jekyll 설치하기

여기까지 진행했으면, Jekyll을 window에서 설치해서 사용하기 위한 기본 requirements에 대한 설정은 완료 되었다.

이제 실제 Jekyll을 window에서 설치 해보자

[https://jekyllrb.com/docs/installation/](https://jekyllrb.com/docs/installation/) 에 jekyll 의 설치 방법이 잘 나와 있다.

CMD에서 아래와 같이 gem을 이용해서 jekyll을 설치한다.

```
$ gem install jekyll
```

version을 확인했을때, 아래와 같이 출력되면 정상 설치된 것이다.

![](/assets/jeklly-check.png)

##### Jekyll 사용해보기

이제 마지막으로 window에서 Jekyll을 사용하는 부분만 남았다.

Jekyll을 사용하는 가장 간단한 방법은 Jekyll의 홈페이지의 [Quick-start guide](https://jekyllrb.com/docs/quickstart/)에 잘 나와 있다.

![](/assets/jekyll-start.png)

window의 cmd에서 위 명령어들을 수행시 시간이 약간 오래 걸릴 수 있다.

참을성 있게 기다리면 정상적으로 해당 명령어들이 잘 수행된다.

아래 그림은 실제 위 명령어 들을 window cmd에서 수행해본 결과이다.

```
$ gem install jekyll bundler
```

![](/assets/jekyll-bundler-install.png)

```
$ jekyll new blog
```

![](/assets/jekyll-new-blog.png)

```
bundle exec jekyll serve
```

![](/assets/jekyll-bundle-start.png)

이제 브라우저에서. `http://127.0.0.1:4000/` 에 접속해 보자..

아래와 같이 정상적으로 동작함을 볼 수 있다.![](/assets/window-run-jekyll.png)

이제 Window에서 즐거운 코딩을 하면 된다~!

Jekyll docs: [https://jekyllrb.com/docs/home/](https://jekyllrb.com/docs/home/)

Jekyll Themes: [https://jekyllthemes.io/](https://jekyllthemes.io/)

