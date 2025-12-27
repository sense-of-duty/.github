# GDGOC 통합 페이지

GDG On Campus 커뮤니티 운영을 위한 통합 웹 플랫폼입니다.  
공지/강의자료/출석/알림/자유게시판/관리자 기능을 한 곳에서 제공해, 운영 흐름을 단순화하고 멤버 경험을 개선합니다.

---

## Key Features

### 인증/계정
- 이메일/비밀번호 회원가입 & 로그인
- Google OAuth2 로그인
- JWT 기반 인증
  - Access Token: Authorization Bearer
  - Refresh Token: HttpOnly Secure Cookie + DB 저장 + Rotation
- 로그아웃 / 토큰 재발급(reissue)

### 커뮤니티 기능
- 공지사항 & 댓글
- 강의자료 목록/검색
- 출석 세션 오픈/체크
- 내 알림 조회 / 읽음 처리 / 미확인 알림 개수
- 자유게시판

### 관리자(ORGANIZER)
- 유저 목록/요청 관리
- 역할/파트 변경
- 유저 승인/거절/비활성화

---

## Tech Stack

### Backend
- Java 17 / Spring Boot
- Spring Security (Stateless)
- JWT (JJWT)
- Validation (Jakarta Validation)
- Swagger / OpenAPI
- Storage: AWS S3 (프로필 이미지)

### Frontend
- React + Vite
- Axios
- React Router

### Infrastructure / DevOps
- Docker Compose
- CI/CD: GitHub Actions
- Deploy: EC2
