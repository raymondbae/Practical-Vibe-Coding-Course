# 🚀 Practical Vibe Coding Course

> **Google DeepMind Antigravity AI** 코딩 어시스턴트와의 유기적인 협업을 위해 최적화된 **초경량 무장애 개발환경 규격** 및 **글로벌 프롬프트 룰 세팅 포맷** 저장소입니다.

---

## 🎨 1. 프로젝트 정체성 & 개요

이 프로젝트는 단순히 코드를 작성하는 것을 넘어, **인공지능 어시스턴트(Antigravity)와 인간 개발자 간의 극대화된 협업 효율성**을 보장하기 위해 설계된 표준 템플릿 저장소입니다. 

엄격하게 검증된 **서버리스 아키텍처 가이드라인**과 AI의 행동을 안전하게 제어하는 **글로벌 프로토콜**이 완벽하게 융합되어 있습니다.

---

## 💻 2. 초경량 무장애 개발환경 규격 (Development Environment)

서버리스 및 초경량 웹 애플리케이션 개발 시 발생할 수 있는 잠재적 500 에러 및 ESM 해석 버그를 근본적으로 예방하기 위한 아키텍처 규격입니다.

### 🛠️ 핵심 기술 스택
| 구분 | 기술 사양 | 비고 |
| :--- | :--- | :--- |
| **Frontend** | Vite + Vue 3 (Composition API) + TypeScript + Vanilla CSS | 시각적 극대화 및 고품격 UI 설계 지향 |
| **Backend** | Node.js ESM (Express) + Vercel Serverless Functions | 빠른 콜드 스타트 및 유연한 라우팅 |
| **Database** | Turso Cloud DB | 분산 Edge SQLite 기반 데이터베이스 |
| **Deployment**| Vercel | 글로벌 엣지 네트워크 배포 최적화 |

### 🚨 무장애 극복을 위한 세부 아키텍처 방안
1. **Turso DB REST HTTP 클라이언트 연동**
   - Vercel Serverless Function 환경에서 네이티브 C++ 바인딩 오류로 인한 500 에러를 방지하기 위해 **`@libsql/client/web`** 초경량 HTTP REST 전용 드라이버를 탑재하여 연동합니다.
2. **ESM 표준 확장자 생략 방지**
   - Node.js ESM 환경에서 빌드 시 임포트 경로 오류를 방지하기 위해 파일 임포트 구문 작성 시 반드시 **`.js` 확장자를 명시**합니다.
     ```typescript
     import { initDatabase } from './db.js';
     ```
3. **데이터베이스 동기화 보장 미들웨어 (Sync Lock)**
   - API 서버 콜드 스타트 시, DB 연결 및 초기화 연산이 끝나기 전에 요청이 유입되어 발생할 수 있는 쿼리 누락 문제를 방지하기 위해 **동기화 보장 미들웨어(Sync Lock Middleware)**를 도입하여 실행 안정성을 100% 확보합니다.

---

## 🔒 3. 구글 안티그래비티 글로벌 룰 세팅 포맷 (Antigravity Global Rules)

AI 코딩 어시스턴트(Antigravity)가 상시 준수해야 하는 최우선순위 협업 규정 프로토콜입니다.

### 1) 🎨 언어 및 주석 규정 (Language & Comments)
- AI가 생성하는 모든 대화, 실행 계획서, 보고서 등 의사소통은 **100% 한국어**로만 진행됩니다.
- 새로 작성하거나 수정하는 모든 소스코드 내부 설명 주석 역시 **한글**로 명확하게 추가하여 코드의 유지보수성을 극대화합니다.

### 2) 🔑 환경변수 및 보안 규정 (Security & Environment Variables)
- **`.env` 파일은 직접 읽거나 수정하지 않습니다.** 실서버 자격 증명의 유출을 미연에 방지하기 위함입니다.
- 필요한 환경변수 설정 가이드는 **`.env-sample`** 파일을 생성 및 수정하여 안전하게 보완 명세화합니다.

### 3) 📋 작업 계획 및 사전 승인 프로세스 (Process & Approval)
- 사용자의 모든 요청에 대해 항상 구체적인 실행 계획을 수립합니다.
- 단순 구두 설명에 그치지 않고, `implementation_plan.md` 계획 아티팩트 파일을 생성하여 사용자에게 시각적으로 먼저 승인을 요청합니다.
- 기존 파일 및 디렉토리의 삭제(`rm` 등) 작업은 **어떠한 경우에도 사전에 명시적 허가를 묻고 승인받은 후**에만 진행합니다.

### 4) ⚙️ 터미널 명령어 실행 정책 (Terminal Commands Policy)
- **자동 실행 허용**: 단순 파일 조회(`ls`, `find`, `grep`), 빌드 및 테스트(`npm run build`), 진단용 네트워크 상태 확인 등 안전한 명령어는 즉시 자체 실행합니다.
- **사전 승인 필수**: 파일의 삭제/파괴(`rm`), 형상 관리 이력 영구 기록(`git commit`, `git push`), 소스코드 영구 수정 등의 명령어는 **사전 계획 승인 후** 실행합니다.

### 5) 🐙 Git 협업 및 형상 관리 (Git Management)
- 작업 단위가 완료되면 **로컬 Git 커밋(`git commit`)은 AI가 자동으로 즉시 실행**하여 안전하게 코드를 백업합니다.
- 로컬 커밋 메시지는 반드시 한글로 품격 있고 유려하게 작성합니다.
- 원격 업로드(`git push`)는 절대로 독단적으로 실행하지 않고, **사용자가 명시적으로 푸시를 요청할 때만** 실행합니다.

### 6) 📝 작업 이력 로깅 (Work Logging)
- 매 작업이 마무리될 때마다 루트 디렉토리 아래의 `/doc/마지막작업-오늘날짜.md` 파일로 작성하여 추가 및 누적 관리합니다.
- 기존의 히스토리 기록을 훼손하거나 덮어쓰지 않고, **안전하게 기존 내용을 유지하면서 하단에 새로운 작업 내용을 지속 추가**하는 방식으로 누적 보관합니다.
- 본 파일들은 `.gitignore` 설정에 따라 자동으로 Git 추적에서 제외되어 개인 환경 로그로서 안전하게 로컬에 보존됩니다.

---

## 🚀 4. 바이브 코딩 실습 방법 (Vibe Coding Quick Start)

안티그래비티 AI 코딩 어시스턴트와 함께하는 고품격 바이브 코딩(Vibe Coding)의 실습 절차입니다. 아래 단계를 순서대로 진행하여 손쉽게 개발을 시작할 수 있습니다.

### 1️⃣ 안티그래비티 열기
- 사용 중인 IDE 환경에서 **Antigravity AI Assistant** 패널을 활성화하거나 실행합니다.

### 2️⃣ 저장소 클론 (Git Clone)
- 터미널을 열고 본 실습 프로젝트 저장소를 로컬 컴퓨터로 클론합니다.
  ```bash
  git clone https://github.com/raymondbae/Practical-Vibe-Coding-Course.git myfirst-vibe-coding
  ```


### 3️⃣ 개발 환경 명세 제공 (Drag & Drop)
- [doc/개발환경.md](file:///Users/bjhhmc/github.com/Practical-Vibe-Coding-Course/doc/개발환경.md) 파일을 안티그래비티 채팅창으로 드래그 앤 드롭(Drag & Drop)하여 프로젝트 기술 명세를 AI에게 전달합니다.

### 4️⃣ 기능 구현 명세 제공 (Drag & Drop)
- [doc/바이브코딩앱개발샘플/네이버뉴스정리앱.md](file:///Users/bjhhmc/github.com/Practical-Vibe-Coding-Course/doc/바이브코딩앱개발샘플/네이버뉴스정리앱.md) 파일을 안티그래비티 채팅창으로 드래그 앤 드롭(Drag & Drop)하여 구현하고자 하는 요구사항을 전달합니다.

### 5️⃣ 개발 지시 및 실행
- 안티그래비티 채팅창에 **`개발해줘`** 또는 **`다 개발 후 실행 해줘`**를 입력하고 엔터(Enter)를 누르면, AI가 요구사항을 분석하여 설계, 자동 개발 및 로컬 실행 작업을 주도적으로 시작합니다.

