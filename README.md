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

- React
- ES6 with Babel
- SCSS
- CSS Modules
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
  $> yarn add  babel-preset-env babel-preset-react --dev
  ```



### Parcel 실행

- parcel 실행

  ```bash
  $> parcel index.html
  Server running at http://localhost:1234 
  ✨  Built in 1.11s.
  ```

  