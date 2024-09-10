# 동찬 노드 서버 (Node.js with TypeScript)

이 프로젝트는 Node.js와 TypeScript를 기반으로 한 서버 애플리케이션.
이 프로젝트는 타입 안정성과 최신 JavaScript 기능을 사용하기 위해 TypeScript를 적용했으며, `src` 폴더에 TypeScript로 작성된 소스 파일이 포함되어 있고, `dist` 폴더에는 컴파일된 JavaScript 파일이 저장됩니다.

## 프로젝트 구조

```
/ 동찬 노드 서버
│
├── /src           # TypeScript 소스 파일들이 위치한 디렉터리
│   └── index.ts   # 메인 서버 파일
│
├── /dist          # TypeScript가 컴파일된 JavaScript 파일들이 위치한 디렉터리
│   └── index.js   # 컴파일된 메인 서버 파일
│
├── package.json   # 프로젝트 설정 및 의존성 정보
├── tsconfig.json  # TypeScript 설정 파일
├── .prettierrc    # Prettier 코드 포맷팅 설정 파일
├── .eslint.json   # ESLint 설정 파일 (선택 사항)
└── README.md      # 프로젝트 설명 파일 (현재 파일)
```

## 사용 기술

- **Node.js**: 백엔드 애플리케이션을 위한 JavaScript 런타임
- **TypeScript**: 정적 타입을 지원하는 JavaScript의 상위 집합
- **Express.js**: 웹 서버 프레임워크
- **Prettier**: 코드 포맷터
- **ESLint**: 코드 린팅 도구 (선택 사항)

## 프로젝트 설정 및 실행 방법

### 1. 패키지 설치

먼저, 프로젝트의 의존성을 설치합니다.

```bash
npm install
```

### 2. 개발 모드에서 서버 실행

개발 중일 때는 `ts-node`와 `nodemon`을 사용하여 TypeScript 파일을 직접 실행하고, 파일 변경 시 자동으로 서버를 재시작할 수 있습니다.

```bash
npm run dev
```

### 3. TypeScript 파일 컴파일

TypeScript 파일을 JavaScript로 컴파일하려면 다음 명령어를 사용합니다.

```bash
npm run build
```

컴파일된 파일들은 `dist` 폴더에 저장됩니다.

### 4. 프로덕션 모드에서 서버 실행

프로덕션 환경에서는 컴파일된 JavaScript 파일을 실행합니다.

```bash
npm start
```

### 5. 코드 포맷팅

코드 포맷팅은 Prettier를 사용합니다. 아래 명령어로 전체 코드를 Prettier 설정에 맞게 포맷할 수 있습니다.

```bash
npm run format
```

### 6. ESLint로 코드 린팅 (선택 사항)

ESLint를 사용하여 코드 스타일과 규칙을 검사할 수 있습니다.

```bash
npm run lint
```

## 주요 명령어 정리

- `npm install`: 프로젝트 의존성 설치
- `npm run dev`: 개발 모드로 서버 실행 (자동 재시작 및 TypeScript 파일 실행)
- `npm run build`: TypeScript 파일을 JavaScript로 컴파일
- `npm start`: 프로덕션 모드에서 서버 실행 (컴파일된 JavaScript 파일 실행)
- `npm run format`: Prettier를 사용하여 코드 포맷팅
- `npm run lint`: ESLint를 사용하여 코드 린팅 (선택 사항)
