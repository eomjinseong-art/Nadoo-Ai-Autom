# AI Tools Atlas

> 50개 이상의 AI 도구와 6가지 자동화 워크플로우 Best Practice를 한 곳에

카테고리별로 정리된 AI 도구들을 탐색하고, 실제 자동화 프로젝트에서 검증된 워크플로우 패턴을 확인하세요.

## 🎯 특징

- **47개 도구 완전 정리**: 워크플로우 · LLM · 코드 어시스턴트 · 음성/영상 · 이미지 · 데이터 · 호스팅 등
- **6가지 Best Practice 아키텍처**: 실제 프로젝트에서 검증된 워크플로우 패턴
- **동적 렌더링**: JSON 기반 데이터, 실시간 검색 & 필터링
- **한국인 최적화**: Noto Sans KR 폰트, 한국어 완벽 지원
- **자동 배포**: GitHub Actions + Vercel 자동화
- **Formspree 연동**: 사용자 피드백 이메일 수집

## 📦 파일 구조

```
.
├── index.html                  # 메인 웹사이트
├── tools.json                  # 47개 도구 데이터
├── architecture.json           # 6개 Best Practice
├── package.json                # Node 설정
├── vercel.json                 # Vercel 배포 설정
├── .github/workflows/
│   └── deploy.yml              # GitHub Actions 배포
└── DEPLOYMENT_REPORT.md        # 배포 검수 보고서
```

## 🚀 빠른 시작

### 로컬 개발
```bash
# Python 간단 서버 (포트 3000)
python -m http.server 3000

# 브라우저에서 열기
# http://localhost:3000
```

### GitHub 배포
```bash
# 저장소 초기화
git init
git add .
git commit -m "Initial commit: AI Tools Atlas"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/ai-tools-atlas.git
git push -u origin main
```

### Vercel 배포
1. [https://vercel.com](https://vercel.com) 접속
2. GitHub 계정 연동
3. 프로젝트 import
4. Environment Variables 설정:
   - `VERCEL_TOKEN`: Vercel Personal Token
   - `VERCEL_ORG_ID`: Team ID
   - `VERCEL_PROJECT_ID`: Project ID

## 📝 도구 추가하는 방법

### 1. tools.json 편집
```json
{
  "id": "my-tool",
  "category": "LLM & 프롬프트",
  "categoryIcon": "brain",
  "name": "My Tool",
  "oneliner": "한줄 설명",
  "description": "상세 설명...",
  "useCases": "활용 사례...",
  "recommendation": "추천 근거...",
  "url": "https://example.com",
  "price": "free",
  "priceLabel": "무료",
  "logo": "🔧"
}
```

### 2. Git 커밋 & 푸시
```bash
git add tools.json
git commit -m "Add: My Tool"
git push origin main
```

### 3. 자동 배포 확인
- GitHub Actions 실행 (약 5-10분)
- Vercel 자동 배포
- 웹사이트에 새 도구 반영 ✅

## 🏗️ 데이터 구조

### tools.json
- **tools**: 47개 도구 배열
  - id: 고유 ID
  - category: 카테고리 (14개)
  - name: 도구명
  - oneliner: 한줄 설명
  - description: 상세 설명
  - useCases: 활용 사례
  - recommendation: 추천 근거
  - url: 공식 웹사이트
  - price: free / freemium / paid
  - logo: 이모지
- **meta**: 메타데이터
  - disclaimer: 법적 안내
  - lastUpdated: 업데이트 날짜
  - totalTools: 도구 수

### architecture.json
- **architectures**: 6개 Best Practice 배열
  - id: 고유 ID
  - title: 제목
  - subtitle: 부제
  - description: 설명
  - tools: 단계별 도구 정보
  - flow: 흐름도
  - useCase: 사용 사례

## 🔍 기능

### 검색 & 필터
- **실시간 검색**: 도구명/설명으로 검색
- **카테고리 필터**: 14개 카테고리 필터
- **통계**: 무료/유료 도구 자동 계산

### 인터랙션
- **도구 링크**: 공식 웹사이트 새 탭에서 열기
- **아키텍처 카드**: Best Practice 패턴 시각화
- **호버 효과**: 부드러운 트랜지션

### 이메일 문의
- **Formspree 연동**: 사용자 피드백 수집
- **폼 필드**: 이메일 + 메시지
- **자동 전송**: 제출 시 이메일 수신

## ⚠️ 중요 안내

- **요금제 변경**: AI 도구의 요금제는 예고 없이 변경될 수 있습니다. 사용 전 공식 웹사이트 확인 필수
- **정확성**: 본 정보는 참고용이며, 실제 사용 시 책임은 사용자에게 있습니다
- **법적 책임**: 본 사이트 정보로 인한 손해에 책임지지 않습니다

## 📊 통계

| 항목 | 수 |
|------|-----|
| 총 도구 | 47개 |
| 카테고리 | 14개 |
| Best Practice | 6개 |
| 무료 도구 | 11개 |
| 유료 도구 | 18개 |
| Freemium | 18개 |

## 🛠️ 기술 스택

- **Frontend**: Vanilla JavaScript (No Framework)
- **Data**: JSON
- **Styling**: CSS3 + Gradient
- **Hosting**: Vercel
- **Font**: Google Fonts (Noto Sans KR)
- **Automation**: GitHub Actions
- **Email**: Formspree

## 📄 라이센스

MIT License - 자유롭게 사용, 수정, 배포 가능

## 🤝 기여

도구 추가 또는 수정 제안:
1. tools.json 또는 architecture.json 편집
2. Git commit & push
3. 자동 배포 확인

또는 웹사이트의 **피드백 & 제안** 폼으로 직접 제안 가능 (Formspree 연동)

## 📧 연락

문의사항이 있으신가요? 웹사이트의 문의 폼으로 이메일을 보내주세요.

---

**Last Updated**: 2026-01-30
**Status**: ✅ Production Ready
