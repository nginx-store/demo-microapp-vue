# Webpack Module Federation을 사용한 Vue.js 마이크로프론트엔드 구현

## 프로젝트 구조

```
micro-frontend-app/
├── container/                 # 호스트 애플리케이션 (셸)
│   ├── public/
│   ├── src/
│   │   ├── App.vue            # 메인 앱 컴포넌트
│   │   ├── bootstrap.js       # 애플리케이션 초기화
│   │   ├── components/        # 공통 컴포넌트
│   │   ├── main.js            # 진입점
│   │   └── router.js          # 라우터 설정
│   ├── package.json
│   ├── vue.config.js
│   └── webpack.config.js
│
├── todo-app/                  # 할 일 관리 마이크로앱
│   ├── public/
│   ├── src/
│   │   ├── App.vue
│   │   ├── bootstrap.js
│   │   ├── components/
│   │   │   └── TodoList.vue
│   │   └── main.js
│   ├── package.json
│   ├── vue.config.js
│   └── webpack.config.js
│
├── weather-app/               # 날씨 마이크로앱
│   ├── public/
│   ├── src/
│   │   ├── App.vue
│   │   ├── bootstrap.js
│   │   ├── components/
│   │   │   └── WeatherWidget.vue
│   │   └── main.js
│   ├── package.json
│   ├── vue.config.js
│   └── webpack.config.js
│
└── currency-app/              # 환율 변환기 마이크로앱
    ├── public/
    ├── src/
    │   ├── App.vue
    │   ├── bootstrap.js
    │   ├── components/
    │   │   └── CurrencyConverter.vue
    │   └── main.js
    ├── package.json
    ├── vue.config.js
    └── webpack.config.js
```
