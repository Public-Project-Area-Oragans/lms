# LearnFlow AI v5.0

AI 기반 적응형 학습 관리 시스템 + 개인 학습 인프라.

## 🔗 링크

- 🎮 **인터랙티브 스토리보드**: https://public-project-area-oragans.github.io/lms/storyboard.html
- 📖 **문서 Wiki**: https://github.com/Public-Project-Area-Oragans/lms/wiki

## 📦 구성

| 영역 | 링크 |
|------|------|
| 프로젝트 계획 · ERD · 아키텍처 | [Wiki 01~04](https://github.com/Public-Project-Area-Oragans/lms/wiki) |
| 화면 설계 · 요구사항 · 스토리보드 | [Wiki 05~08](https://github.com/Public-Project-Area-Oragans/lms/wiki) |
| Git · 환경 · 테스트 · 리뷰 | [Wiki 09~13](https://github.com/Public-Project-Area-Oragans/lms/wiki) |
| 배포 · 매뉴얼 · 운영 · 스케줄 | [Wiki 14~17](https://github.com/Public-Project-Area-Oragans/lms/wiki) |

## 🛠 기술 스택

**Backend**: Spring Boot 4 · Java 21 · JPA + QueryDSL · Spring Security 7
**Data**: MySQL 8 · pgvector · Redis 7 · Elasticsearch 8 · Kafka
**AI/LLM**: Claude API · OpenAI GPT (fallback) · RAGAS · DeepEval
**Frontend**: React 18 · TypeScript · Flutter 3.x · Tailwind
**Infra**: Docker · Kubernetes · Prometheus + Grafana · OTel

## 📑 문서 구조

`docs/`는 GitHub Pages 배포용 정적 자산을 담습니다. 개발 문서 원본은 Wiki에서 관리됩니다.

```
docs/
├── index.html       # Pages 랜딩 (storyboard로 자동 이동)
└── storyboard.html  # 인터랙티브 화면 스토리보드 (27 화면)
```

## 🗓 마일스톤

- **M6** (Week 24): LMS 코어 완성
- **M7** (Week 28): SRS MVP (SM-2 + Bloom)
- **M8** (Week 33): Notes MVP (위키링크 + 그래프)
- **M9** (Week 36): v5.0 정식 릴리즈
