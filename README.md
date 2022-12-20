일반상대론의 symbolic computation을 위한 package "xAct" 안내서 ver 0.1
=============

본 github 코드는 숭실대학교 우주물질연구소 15회차 정기 미팅 때 발표한 내용을 기반으로 만든 것입니다.

- 문의 이메일: cosmosapjw@soongsil.ac.kr
- 참고사항: 본 안내서의 많은 부분은 아래 Cyril Pitrou 교수님의 코드 모음집에서 내용을 가져오거나 참조하여 만들어진 것입니다.
추후 지속적 업데이트를 통하여 보다 독립적이고 상세한 내용의 안내서를 만들 계획입니다. 업데이트 알림은 내부 메일로 드릴 예정이니 참조 바랍니다.

https://github.com/xAct-contrib/examples/blob/master/README.md

xAct 및 Wolfram Engine 설치 방법
=============

I. Mathematica가 설치되어 있는 경우
-------------

1. http://www.xact.es/download.html 에서 Current Version 항목의 압축파일을 다운받는다.

2. 압축을 해제해서 나온 폴더를 다음의 경로에 옮긴다.
(주의: '압축 파일 명으로 폴더 만들어서 압축 풀기' 등의 옵션은 해제하고 압축을 풀어야 한다. 이미 폴더가 압축된 것이기 때문에 이중으로 폴더를 생성하면 설치가 되지 않는다.)


> 윈도우:
> - system-wide installation:
>
> C:\Program Files\Wolfram Research\Mathematica\<version>\AddOns\Applications\
>
> - single-user installation:
>
> C:\Users\<user>\AppData\Roaming\Mathematica\Applications\


> 맥:
> - system-wide installation:
>
>  /Library/Mathematica/Applications/
>
> - single-user installation:
>
>  /Users/<user>/Library/Mathematica/Applications/
 
> 리눅스:
>  - system-wide installation:
>
>  /usr/share/Mathematica/Applications/
>
>  - single-user installation:
>
> $HOME/.Mathematica/Applications/
 
3. xAct_intro.nb 파일을 열고 첫 줄을 실행한다. 에러가 발생하지 않으면 설치가 제대로 된 것이다.

II. Mathematica가 없는 경우
-------------

1. 다음 사이트에서 Wolfram Engine을 다운로드 받는다: 

https://www.wolfram.com/engine/

2. 사이트 안내사항을 따른다. 회원가입이 필요하며 설치 후에 등록 과정이 필요하다.

> - 윈도우 등록 방법: https://support.wolfram.com/46069
> - 맥 등록 방법: https://support.wolfram.com/46070
> - 리눅스 등록 방법: https://support.wolfram.com/46072

설치 과정 중 설치 경로를 기억해야 한다.

3. Jupyter notebook을 설치한다. (Anaconda를 사용한다면 이미 설치가 되어있을 것이다:

https://jupyter.org/install

4. 다음 사이트에 들어가서 안내사항을 따라 Wolfram Language kernel for Jupyter notebooks를 설치한다:

https://github.com/WolframResearch/WolframLanguageForJupyter

5. 2에서 설치된 경로 아래 Applications 폴더를 찾는다. (설치경로)/13.1/AddOns/Applications/와 같은 식으로 되어있을 것이다.

6. http://www.xact.es/download.html 에서 Current Version 항목의 압축파일을 다운받아 5에서 찾은 경로에 압축을 푼다.

(주의: '압축 파일 명으로 폴더 만들어서 압축 풀기' 등의 옵션은 해제하고 압축을 풀어야 한다. 이미 폴더가 압축된 것이기 때문에 이중으로 폴더를 생성하면 설치가 되지 않는다.)

7. jupyter notebook을 실행하여 xAct_intro.ipnyb 파일을 열고 첫 줄을 실행한다. 에러가 발생하지 않으면 설치가 제대로 된 것이다
(참고사항: vscode를 쓰는 경우 Wolfram language에 대한 extension이 있으니 설치해서 실행하는 것을 권장한다.)
