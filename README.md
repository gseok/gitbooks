![](/assets/gitbook-main.png)

#### GitBook

Gitbook은 web상에서 곧바로 문서를 만들수 있는 서비스다.

오픈소스 프로젝트이고, 무료로 사용가능하다. 사용 가입 역시, github이나 google+ 계정을 통한 Single Sign On을 지원한다.

Gitbook의 open source project 참고: [https://github.com/GitbookIO/gitbook](https://github.com/GitbookIO/gitbook)

기본적으로, GitBook으로 만든 document는 곧바로 web상에 publish 되어, 여러 사람들이 볼 수 있는 구조로 되어 있다.

꼭 Book의 형태가 아니어도, API Document의 형식이나, Q&A와 같은 knowledge기반의 문서 역시 생성 가능히다.

![](/assets/gitbook-selfhosting.png)[https://toolchain.gitbook.com/](https://toolchain.gitbook.com/)

위 그림은, gitbook 에서 gitbook으로 gitbook에 대한 toolchain document을 작성한 모습이다. 기본적인 web book의 형태를 취하고 있다.

GitBook을 이용해서, 자신만의 Web Book을 손쉽게 작성 가능하고, 소규모 프로젝트에서의 API Document등의 작성도 아주 쉽게 작성 가능하다.

GitBook에 가입을 하고나면, 사용자들이 쉽게 문서를 작성 할 수 있도록 아래 그림과 같은 book template을 제공한다.![](/assets/gitbook-newbook.png)

템플릿을 선택하고, Create Book을 만들고 나면, 자신만의 하나의 web book이 바로 생성된다. \(멋지다!!!!\)

GitBook에서 문서를 작성하는 문서 작성 툴 역시 기본적으로 제공되고 있다.

일단 Web 서비스이다보니, web에서 곧바로 edting하여 저장\(publish\)할 수 있는 기능을 제공한다.

게다가, markdown\(md\)을 지원해서, wiki나 confluence사용자들이, 기존에 작성하던 방식 그대로 문서 작성을 할 수 있도록 한다.

거기에 더하여, 아래 그림과 같이, 기존 문서들\(pdf, docx, xml, ...\)을 import하거나, github, 또는 git\(bitbucket\)을 연동하는 것 또한 가능하다.![](/assets/gitbook-newbook-add.png)

또한 offline에서 사용가능한 editor 역시 제공하고 있다.![](/assets/gitbook-offline-editor.png)

Gitbook의 매커니즘은 git의 기술을 사용하여,  version 컨트롤이 된다. 즉, 문서를 작성하고 저장하면, git의 하나의 commit와 같이 되고, 이전 작성 이력이나 이전 버전의 문서를 볼 수 도 있다. git의 기술을 사용한 만큼, 협업\(collaboration\)으로 하나의 문서를 여러명이 작업 가능한 구조 역시 가지고 있다. 

그냥 전체적으로, source code에서 사용하는 부분을 문서 작성의 영역으로 가져왔다.

기본적으로 작성한 문서들은 public으로 공개되지만, 유료 사용을 하면, private한 문서도 작성 가능하다..\(일기라던가, 팀 내부의 문서\)



끝으로...

쉽게 작성가능하고, web에 바로 publish 되는 이 매력적인 서비스를 한번 사용해보자.

나만의 책을 만드는 재미에 빠져 볼 수 있을듯 하다.



