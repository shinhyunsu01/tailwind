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
