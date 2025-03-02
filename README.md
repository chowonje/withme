# React Native + Express 앱 프로젝트

이 프로젝트는 React Native 모바일 앱과 Express 백엔드 서버로 구성된 풀스택 애플리케이션입니다.

## 프로젝트 구조

```
/
├── mobile-app/         # React Native 앱
│   └── MobileApp/      # Expo로 생성된 React Native 프로젝트
└── backend/            # Express 백엔드 서버
    ├── index.js        # 메인 서버 파일
    ├── package.json    # 백엔드 의존성
    └── .env            # 환경 변수
```

## 시작하기

### 백엔드 서버 실행

```bash
cd backend
npm install
npm run dev
```

서버는 기본적으로 http://localhost:5000 에서 실행됩니다.

### 모바일 앱 실행

```bash
cd mobile-app/MobileApp
npm install
npm run android  # 안드로이드 에뮬레이터 실행
# 또는
npm run ios      # iOS 시뮬레이터 실행 (Mac 필요)
# 또는
npm run web      # 웹 브라우저에서 실행
```

## API 연결

모바일 앱에서 백엔드 API에 연결하려면 `App.js` 파일에서 API URL을 수정해야 할 수 있습니다:

- 안드로이드 에뮬레이터: `http://10.0.2.2:5000`
- iOS 시뮬레이터: `http://localhost:5000`
- 실제 기기: 컴퓨터의 로컬 IP 주소 (예: `http://192.168.1.100:5000`)

## 기술 스택

- **프론트엔드**: React Native, Expo
- **백엔드**: Node.js, Express
- **데이터베이스**: MongoDB (mongoose) 