1. node 프로젝트(application, library) 만들기
    1) 프로젝트 생성
        $ mkdir ex01
    2) 프로젝트 이동
        $ cd ex01
    3) 프로젝트 초기화: 프로젝트 매니페스트 파일(package.json)를 생성
        $ npm init -y
    
2. 패키지 
    1) 완전한 어플리케이션(babel, webpack, nodemon, Lint, ...)
    2) 프로젝트에서 사용하는 라이브러리 모듈(react, react-dom)

3. 의존성
    1) 개발하는 프로젝트에서 설치하는 패키지
    2) 일반 의존성: 개발하고 있는 프로젝트가 런타임 중 사용하는 패키지
    3) 개발 의존성: 개발시 필요할 때 도움이 되는 패키지로 빌드와 배포에는 포함x

4. 패키지 설치
    1) 전역 설치
    2) 지역 설치

==== 실습 ====
$ npm i ejs     [지역, 일반] <- default
$ npm i -D nodemon      [지역, 개발] <- default, 개발로 설치되기 때문에 배포판에는 넣으면 안됨
$ npm i -D -g gulp      [전역, 개발]

==== 실습 ====
$ npm un ejs     [지역]
$ npm un nodemon      [지역]
$ npm un -g gulp      [전역] -g는 전역이라는 표기

5. Modules
    1) 코어 모듈: node에서 제공하는 모듈(fs, os, process, http, ...)
    2) npm 모듈: npm을 통해서 node_module에 설치하고 사용하는 모듈
    3) 파일 모듈: 파일 경로로 불러온 모듈안에 함수나 객체를 사용한다.
    
