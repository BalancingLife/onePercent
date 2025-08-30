# onePercent

하루 1%의 꾸준한 성장을 기록하는 운동 루틴 관리 웹 애플리케이션

![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white)
![FSD](https://img.shields.io/badge/Architecture-FSD-blue?style=flat)

---

## 프로젝트 소개

**onePercent**는 취업 전 프론트엔드 지식을 다시 정립하며 한 단계 성장하기 위해 만든 개인 프로젝트입니다.  
실제로 사용할 운동 루틴 및 PR 기록 앱을 목표로 하며, *하루 1%의 꾸준한 성장*이라는 키워드를 담았습니다.  
AI는 개발 보조 도구로만 활용하고, 전체 코드는 직접 손코딩하는 것을 원칙으로 합니다.

## 프로젝트 목표와 원칙

- **목표**

  1. AI 활용을 최소화하고, 전체 코드를 직접 타이핑하며 프론트엔드 지식을 재정립하는 것
  2. 실제 내가 사용할 운동 루틴 관리 앱을 만드는 것

- **원칙**
  1. **폴더 구조(FSD)** – 기능 단위로 관심사 분리
  2. **타입스크립트 활용** – `strict` 모드, 제네릭/유틸리티 타입 적극 사용
  3. **컴포넌트 설계** – UI와 로직을 분리, 재사용성 확보
  4. **코드 퀄리티** – ESLint + Prettier, 단일 책임 원칙 유지

---

## 주요 기능 (예정 포함)

- 운동 루틴 등록 / 수정 / 삭제 (CRUD)
- 개인 기록(PR) 관리
- 주간·월간 기록 차트 시각화
- 운동별 세트 / 무게 / 횟수 기록
- 반응형 UI 지원

---

## 기술 스택

- **Frontend:** Vite, React, TypeScript
- **Architecture:** Feature-Sliced Design (FSD)
- **Styling:** Tailwind CSS
- (추가 예정: Zustand/Recoil, Recharts 등)

---

## 📂 폴더 구조 (초안)

```bash
src/
├── app/          # 루트 컴포넌트, providers, 글로벌 설정
├── processes/    # 사용자 플로우(인증 등)
├── features/     # 기능 단위 모듈 (ex. AddWorkoutForm)
├── entities/     # 핵심 도메인 (ex. Workout, User)
├── shared/       # 공용 라이브러리, UI, utils
├── widgets/      # 여러 엔티티/기능을 조합한 UI 블록
├── pages/        # 페이지 단위 컴포넌트
└── main.tsx      # 앱 실행 entrypoint
```
