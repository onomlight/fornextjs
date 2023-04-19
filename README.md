This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.js`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.js`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.

!! next.js 사용하는 ㅣㅇ유
ReactJS = > 풀스택 프레임워크라고 부르는걸 선호
React 는 사용자 인터페이스를 구축하기 위한 js 라이브러리

Next.js => 리액트상 구축된 프레임워크
프레임워크와 라이브러리의 차이점으로는 프레임워크 규모가 더욱 큼
안정적으로 리액트를 대규모 프로젝트를 위해 프로덕션용으로 사용하기위해! 라고 생각하면됨
Nextjs 역활
React 개발자의 업무를 수월해주기위함

!! Next js 추가하는 기능중 가장 중요한 기능은
내장된 기능인 서버 측 랜더링지원
React는 클라이언트 측 JavaScript 라이브러리이기 때문에 렌더링은 전부 클라이언트 측에서 처리

예를 들어, 일부 데이터를 화면에 '모임 약속' 같이 보여야 하는 데이터를 서버로부터 페칭하는 경우
데이터가 페칭되는 동안 즉, 요청이 전송될 때 잠깐 동안에 페이지가 깜빡이는 로딩 상태를 보게 됨

왜냐하면 클라이언트 측에서 JavaScript 코드가 실행된 뒤에 데이터 페칭이 시작
그래서 전송된 요청의 회신을 대기하느라 로딩이 생기죠 간단히 말해, 요청된 페이지가 아직 해당 데이터를 포함하지 않기 때문

!! Next JS가 추가해주는 또 다른 유용한 기능은 파일기반 라우팅

기존 React에는 라우터가 아예 없음

@라우팅이란 사용자에게 여러개의 페이지가 있는 듯한 착각을 불러 일으키는 것!

이렇게 탐색하며 페이지를 로드하는게 라우터의 역활

==> 일반적으로는 React Router를 사용!
라우터 URL을 확인해 URL이 변경될때 브라우저가 요청하는 서버로 보내는 기본 동작을 방지
대신 React를 통해 페이지 상에 다른 콘텐츠를 렌더링함
코드 내에서 라우트 설정을 모방함
페이지와 코드로 설정된 세개의 페이지가 있다면 페이지 컴포넌트 폴더에 페이지 컴포넌트가 여러개 있는건 당연한 결과

하지만 next.js로는 코드 내 라우트 정의를 사용할 필요가 없음
사용시에 파일과 폴더에 페이지와 라우트를 정의하게됨
NextJS는 필요한 중첩 라우트, 혹은 동적 매개변수를

사용하는 동적 라우트 등을 여전히 모두 지원

## next.js 생성법

1. npx create-next-app
   이후 엔터
2. 추가 패키지 설치 여부에 Y 설정

3. run npm install 실행

중요한 폴더 pages public styles 임

하지만 pages가 현재로서는 가장 중요한 폴더죠

styles 폴더는 당연히 스타일 파일을 포함하고 있는데

당장은 무시를 하고 이후에 작업해 주도록 하겠습니다

public 폴더는 우리 페이지가 사용할 수도 있는 공공 리소스인

이미지 파일 등을 포함하고 있습니다

public 폴더에서 아셔야 되는 건

create-react-app으로 생성한

일반적인 표준 React 앱의 내에는

public 폴더 내에 index.html 파일이 있는 반면

NextJS 앱 내에는 그 파일이 없다는 점입니다
이는 NextJS는 내장된 사전 렌더링이 포함되어 있기 때문인데요

요청이 서버로 도달할 때에 싱글 페이지 애플리케이션(SPA)의

단일 페이지가 동적으로 사전 렌더링이 되어

콘텐츠를 포함한 초기 페이지를 반환하는 것이라고 (정확히는 NextJS로 페이지가 언제 사전 렌더링될지 결정할 수 있게 됩니다. 나중에 단계별로 알아볼 거예요!)

4. 실행 단어 npm run dev
