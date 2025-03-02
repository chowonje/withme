# Instagram 스타일 앱

React Native와 Express를 사용한 인스타그램 스타일 앱입니다.

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
npm start
```

Expo 앱을 사용하여 QR 코드를 스캔하거나 다음 명령어로 실행할 수 있습니다:

```bash
npm run android  # 안드로이드 에뮬레이터 실행
# 또는
npm run ios      # iOS 시뮬레이터 실행 (Mac 필요)
# 또는
npm run web      # 웹 브라우저에서 실행
```

## 주요 기능

- 인스타그램 스타일 로그인 페이지
- 사용자 인증
- 메인 화면 (개발 중)

## 기술 스택

- **프론트엔드**: React Native, Expo
- **백엔드**: Node.js, Express
- **데이터베이스**: MongoDB (mongoose) 