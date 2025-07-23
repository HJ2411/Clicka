<p align="left">
  <img src="https://github.com/HJ2411/Clicka/blob/6d482265624f383333e5f449e2392c221f03f740/Clicka_logo.png" alt="Click 로고" width="200px" />
</p>

간편한 출퇴근 기록 웹 서비스입니다.

---

## 🌐 배포 링크

👉 [https://click-and-go-time.lovable.app](https://click-and-go-time.lovable.app)

---

## 🛠️ 기술 스택

- [Vite](https://vitejs.dev/)
- [React](https://react.dev/)
- [TypeScript](https://www.typescriptlang.org/)
- [shadcn-ui](https://ui.shadcn.com/)
- [Tailwind CSS](https://tailwindcss.com/)

- [Google Studio AI](https://aistudio.google.com/)
- [Lovable](https://lovable.dev/)
- [Supabase](https://supabase.com/)

---

## ✨ 사용 방법

1. 상단 링크로 접속
2. 로그인 페이지 하단의 테스트 계정 클릭
3. 로그인해서 테스트하기
- Chrome에서 뜨는 비밀번호 유출 알림은 password를 단순한 "password"로 저장해서 나오는 알림입니다. (과거 유출된 조합이면 뜨는 알림)

---

## 📒 TODO LIST
👉 [구현내용 및 개선방향](https://github.com/HJ2411/Clicka/blob/6d482265624f383333e5f449e2392c221f03f740/TODOS.md)

---

## 회고
 이번 미니 프로젝트는 자연어 프롬프트를 입력하면 자동으로 웹 서비스를 구현하는 코드 툴의 도움을 받았습니다.
<br/>구현해보니 직접 구현하는 것과 도구의 도움을 받는 건 큰 차이가 있다는 것을 알 수 있었습니다.

제가 배운 DB는 MySQL 기반입니다. 그런데 이 프로젝트에서 사용한 Supabase는 PostgreSQL 기반입니다.
<br/>다른 기반의 DB를 사용했음에도 큰 장애 없이 DB를 연결할 수 있었습니다.
<br/>Supabase 자체에서 OAuth 인증이나 JWT, REST API 여러 기능을 지원해주고 DB 테이블 생성까지 도와주기 때문입니다.

다만, 백엔드 로직을 정석적으로 구현하다가 Supabase의 RSL 정책과 마주하면 약간 혼란스러웠습니다.
<br/>백엔드 구현 로직은 분리되어 있지만 Supabase는 DB에서 모든 걸 처리해서 결합도가 높아지기 때문입니다.
<br/>그래서 세부적인 성능 튜닝이나 조직단위나 계층적인 접근단위로 제어하는 작업이 복잡하다고 합니다.

또 프로젝트 규모가 커질 경우, Supabase에서 데이터를 이관해야 하는데 
<br/>(어떤 DB인지에 따라 다르겠지만) Supabase가 처리하던 백엔드 단의 작업들을 직접 구현하고 수정해야하니 복잡할 것입니다.

그럼에도 무료로 짧은 시간만에, MVP 기능을 구현한 웹 서비스를 완성할 수 있다는 점에서
<br/>노코드 + 디버깅의 조합은 매력적이라고 느꼈습니다.
