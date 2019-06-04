# parcel-experiments

### 학습목표

> 실험용 front-end 학습을 위해 webpack은 너무 많은 설정을 해야 한다.
>
> (솔직히 공부를 안해서 잘 모른다. 지금 배우려면 너무 오래 걸려)
>
> front-end 여러 학습을 위해 parcel을 학습하고 간단한 프로젝트를 실험해 본다.
>
> [parcel 공식 홈페이지](https://parceljs.org/)



### Feature 파셀과 함께 만들고 싶은것

- React  :white_check_mark:
- ES6 with Babel :white_check_mark:
- SCSS :white_check_mark:
- CSS Modules :white_check_mark:
- Typography.js
- Build for production



### 프로젝트 설정

- yarn init 명령어를 통한 프로젝트 설정

  ``` bash
  $> yarn init
  ```

- parcel 글로벌 설치

  ```bash
  $> yarn global add parcel
  ```

- react-dom 설치

  ```bash
  $> yarn add react react-dom
  ```

- babel-preset 설치

  ```bash
  $> yarn add babel-preset-env babel-preset-react --dev
  ```
  
- post css modules 설치

  ```bash
  $> yarn add postcss-modules
  ```

  



### Parcel 실행

- parcel 실행

  ```bash
  $> parcel index.html
  Server running at http://localhost:1234 
  ✨  Built in 1.11s.
  ```

- package.json 실행 스크립트 추가 및 실행

  ```javascript
  ...
  scripts: {
  	start: parcel index.html;
  }
  ...
  
  $> yarn start
  ```



### scss지원을 위한 플러그인 설치 및 .postcssrc 설정

-  node에서 sass를 지원하기 위해 node-sass를 설치

  ```bash
  $> yarn global add node-sass
  ```

- auto prefixer를 지원하기 위한 autoprefixer 설치

  > 브라우저별로 따로 놀던 CSS3의 속성을 잡아주기 위해서 사용되기 시작된 프리픽스는 마크업시 css의 Class앞에 `-moz-`, `-webkit-`, `-o-`, `-ms-`라는 각 브라우저에서 판독이 가능한 접두어를 붙여서 해당 브라우저에서 인식할 수 있게 하는 것 -블로그 펌-
  >
  > 그걸 자동으로 붙여 주는 것

  ```bash
  $> yarn add autoprefixer
  ```

- autoprefixer 설정을 .postcssrc에 적용

  ```bash
  {
      "modules": true,
      "plugins": {
          "autoprefixer": {
              "browsers": [
                  "> 1%", // 글로벌 마켓 쉐어 시장에 1%이상인 브라우저를 지원하겠다
                  "Last 2 versions", // 해당 브라우저의 최근 두버전을 지원할거야
                  "IE 10", // 그리고 IE 10버전을 지원할 거야 (망해라 IE!!)
              ]
          }
      }
  }
  ```

  































