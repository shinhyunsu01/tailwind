## tailwind css install / Doc

```
  1. npm install -D tailwindcss postcss autoprefixer
     npx tailwindcsss init -p

  2. vscode -> extensions
  tailwind css intellisense install  <- auto color / 자동 완성

  3. create poscss.config + tailwind.config.js
     ex) content: [
        "./pages/**/*.{js,jsx,ts,tsx}" <- ** All folders / * All files
     ]
  4. styles/globals.css
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
```

## Learn

className

    border-dashed <- 점선
    shadow-xl <- 그림자,사이즈
    fonet-semibold <- 폰트 사이즈
    w-2/4 <- width 50%
    overflow-hidden
    relative <- position: relative
    focus:text-red-500
    ring-2 ring-offset-1 <- 링 생성
    aspect-square <- 정확한 사각형 생성 aspect-radiol 1/1;
    transition-colors <- 컬러 말고도 다른 요소 있음.
    first:bg-blue-50
    invalid:bg-red-500 <- form 경우 입력 되면 보이던 빨간색 사라짐

    list-decimal <- ul 태그에서 1. 2. 3. <-  이표시를 점으로 교체
    marker:text-teal-500 <- 1. 2.3. <- 색상 변경
    first-letter <- 첫번쨰 글자 선택.

```
<ul className="first:bg-blue-50 last:bg-red-50">
    <div /> <- 첫번째 요소만 blue로 변경
    <div />
    <div /> <- 마지막 요소만 red로 변경
</ul>
```

```
<div className="group">
    <div className="group-hover:bg-red-300 trnsition-colors" /> <-셀렉터 group 이밖에도 다양한 기능 있음.
    <div />
</div>
```

```
<form>
    <input className="peer"/> <- group
    <span className="peer-invalid:text-red-500"/> <- focust 되고 입력이 없으면 빨간색으로 표시.
</form>
```

```
클릭 되면 목차 보이는 기능 No JS
<details className="select-none open:text-white open:bg-indigo-400">
    <summary className="cursor-pointer">What is<summary/>
    <span>kimchi</span>
</details>
```
