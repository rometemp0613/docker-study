# Docker 학습 기록

**학습 방식**: Claude와 함께 실습 중심 학습
**학습 시작일**: -
**목표**: 컨테이너 기반 개발/배포 역량 확보 (예지보전 시스템 배포 포함)

**참고 도서**:
- "Docker Deep Dive" - Nigel Poulton (2025 개정판)
- "The Kubernetes Book" - Nigel Poulton (K8s 맛보기 참고)

---

## 진도 체크리스트

### Part 1: 큰 그림 (1주)

- [ ] **컨테이너 개념**
  - 핵심: 컨테이너 vs VM, OCI 표준, 컨테이너 런타임
- [ ] **Docker 설치 & 아키텍처**
  - 핵심: Docker Engine, 클라이언트-서버 모델, dockerd, containerd
- [ ] **Docker 첫 체험**
  - 핵심: docker run, pull, images, ps, stop, rm — 빅 픽처 실습

### Part 2: 이미지 & 컨테이너 (1-2주)

- [ ] **Docker 엔진 내부 구조**
  - 핵심: containerd, runc, shim, 프로세스 모델
- [ ] **이미지 심화**
  - 핵심: 레이어 구조, 레지스트리, 태그, 매니페스트, 다이제스트
- [ ] **컨테이너 심화**
  - 핵심: 라이프사이클, restart policy, exec, logs, inspect
- [ ] **이미지 & 컨테이너 종합 실습**
  - 핵심: 이미지 빌드 → 컨테이너 실행 → 로그 확인 → 정리

### Part 3: Dockerfile (1-2주)

- [ ] **Dockerfile 기초**
  - 핵심: FROM, RUN, COPY, WORKDIR, CMD, ENTRYPOINT
- [ ] **Dockerfile 심화**
  - 핵심: ARG, ENV, EXPOSE, LABEL, 멀티스테이지 빌드
- [ ] **이미지 최적화**
  - 핵심: .dockerignore, 레이어 캐싱, slim/alpine, 이미지 크기 줄이기
- [ ] **Python 앱 컨테이너화**
  - 핵심: Python 베이스 이미지, requirements.txt, uv in Docker, venv

### Part 4: Docker Compose (1-2주)

- [ ] **Docker Compose 기초**
  - 핵심: docker-compose.yml, services, up, down, build
- [ ] **Compose 서비스 구성**
  - 핵심: depends_on, environment, volumes, ports, networks, healthcheck
- [ ] **멀티 컨테이너 앱 구축**
  - 핵심: Python + PostgreSQL + Redis 구성, 서비스 연결

### Part 5: 네트워크 & 볼륨 (1-2주)

- [ ] **네트워크 기초**
  - 핵심: bridge, host, none, 컨테이너간 통신, 포트 매핑
- [ ] **오버레이 네트워크**
  - 핵심: 멀티호스트 통신, 서비스 디스커버리, DNS
- [ ] **볼륨과 영속 데이터**
  - 핵심: named volume, bind mount, tmpfs, 데이터 영속성
- [ ] **네트워크 & 볼륨 종합 실습**
  - 핵심: 커스텀 네트워크 + 볼륨으로 DB 컨테이너 구성

### Part 6: 보안 & 운영 (1주)

- [ ] **Docker 보안**
  - 핵심: 비루트 사용자, 시크릿 관리, 이미지 스캐닝, 최소 권한
- [ ] **로깅, 모니터링 & 디버깅**
  - 핵심: docker logs, 로그 드라이버, inspect, 리소스 모니터링, 트러블슈팅
- [ ] **레지스트리와 이미지 관리**
  - 핵심: Docker Hub, 프라이빗 레지스트리, 이미지 태깅 전략

### Part 7: CI/CD & 배포 (1-2주)

- [ ] **GitHub Actions + Docker**
  - 핵심: Docker 빌드 액션, 이미지 푸시, CI 파이프라인
- [ ] **개발 환경 Docker화**
  - 핵심: devcontainer, VS Code Remote Containers, 팀 개발 환경 통일
- [ ] **배포 전략**
  - 핵심: 롤링 업데이트, 블루-그린, 헬스체크, Watchtower

### Part 8: 고급 & 프로젝트 (1-2주)

- [ ] **쿠버네티스 맛보기**
  - 핵심: K8s 개념, Pod, Service, Deployment, 언제 필요한지
- [ ] **예지보전 앱 Docker화**
  - 핵심: ML 모델 서빙 컨테이너, 센서 데이터 파이프라인 구성
- [ ] **예지보전 Compose 스택**
  - 핵심: 데이터 수집 + 전처리 + 모델 서빙 + 대시보드 통합

---

## 학습 일지

| 날짜 | 주제 | 주요 내용 | 비고 |
|------|------|----------|------|

---

## 진행 현황

- **총 항목**: 27개
- **완료**: 0개
- **진행률**: 0%

---

## 디렉토리 구조

```
docker-study/
├── README.md              # 진도 체크리스트 (현재 파일)
├── CLAUDE.md              # Claude 학습 지침서
├── notes/                 # 주제별 학습 노트
├── logs/                  # 학습 일지
└── review/                # 3단계 복습 시스템
    ├── 1-new/terms.md
    ├── 2-practicing/terms.md
    └── 3-mastered/terms.md
```
