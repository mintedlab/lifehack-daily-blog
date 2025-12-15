# 🚀 LifeHack Daily - GitHub & Vercel 자동 배포 가이드

## 📋 **전체 프로세스 (5분)**

```
1. GitHub 저장소 생성 (2분)
2. 파일 업로드 (1분)
3. Vercel 연동 (2분)
→ 완료! 이후 자동 배포 시작
```

---

## 1️⃣ **GitHub 저장소 생성**

### **1-1. GitHub 접속**
👉 https://github.com

### **1-2. 새 저장소 만들기**
1. 우측 상단 **"+"** → **"New repository"**
2. 설정:
   - **Repository name**: `lifehack-daily-blog`
   - **Description**: `LifeHack Daily - 생산성 & 디지털 라이프스타일 블로그`
   - **Public** 선택 ✅
   - **✅ Add a README file**
3. **"Create repository"** 클릭

### **1-3. 파일 업로드**
1. 생성된 저장소에서 **"Add file"** → **"Upload files"**
2. 프로젝트의 모든 파일을 드래그 앤 드롭:
   ```
   - index.html
   - css/ (폴더 전체)
   - js/ (폴더 전체)
   - posts/ (폴더 전체)
   - pages/ (폴더 전체)
   - vercel.json
   - README.md
   ```
3. Commit message: `Initial commit: LifeHack Daily blog`
4. **"Commit changes"** 클릭

---

## 2️⃣ **Vercel 연동 (무료 호스팅)**

### **2-1. Vercel 가입**
👉 https://vercel.com/signup

- **"Continue with GitHub"** 선택 (권장)
- GitHub 계정으로 로그인

### **2-2. 프로젝트 임포트**
1. Vercel 대시보드에서 **"Add New..."** → **"Project"**
2. **"Import Git Repository"** 섹션에서 `lifehack-daily-blog` 선택
3. **"Import"** 클릭

### **2-3. 배포 설정**
```
Framework Preset: Other
Root Directory: ./
Build Command: (비워두기)
Output Directory: (비워두기)
Install Command: (비워두기)
```

4. **"Deploy"** 클릭

### **2-4. 배포 완료! 🎉**
- 약 30초 후 배포 완료
- 주소: `https://lifehack-daily-blog.vercel.app`
- 커스텀 도메인 연결 가능 (선택)

---

## 3️⃣ **자동 배포 테스트**

### **새 블로그 글 발행 시나리오**

#### **AS-IS (이전 방식)**
```
1. AI에게 글 요청
2. HTML 파일 생성
3. [Publish 탭]에서 수동 Deploy 클릭
4. 전체 사이트 재배포
```

#### **TO-BE (GitHub 연동 후)**
```
1. AI에게 "블로그 글 써줘: [주제]" 요청
2. AI가 자동으로:
   - 글 작성 (2,500자)
   - HTML 파일 생성
   - index.html 업데이트
   - GitHub에 Push
3. Vercel이 자동 감지 → 30초 후 배포 완료! ✨
```

---

## 🎯 **실제 사용법**

### **예시 1: 새 글 발행**
```
당신: "블로그 글 써줘: ChatGPT 프롬프트 작성법 10가지"

AI (자동 처리):
✅ 글 작성 완료 (2,500자, SEO 최적화)
✅ posts/chatgpt-prompt-tips.html 생성
✅ index.html 업데이트 (최신 글 추가)
✅ GitHub Push 완료

Vercel (자동 처리):
🔄 변경 감지...
🚀 배포 시작...
✅ 배포 완료! (30초)

→ https://lifehack-daily-blog.vercel.app
```

**당신이 한 일**: 10초 (요청만)  
**시스템이 한 일**: 3분 30초 (전부 자동)

---

## 📊 **배포 확인 방법**

### **Vercel 대시보드**
👉 https://vercel.com/dashboard

- **Deployments** 탭에서 실시간 배포 상태 확인
- 각 배포마다 고유 URL 생성 (미리보기 가능)
- Production 배포는 메인 URL로 자동 연결

### **알림 설정 (선택)**
1. Vercel 대시보드 → **Settings** → **Notifications**
2. **Deploy Hooks** 활성화
3. 배포 성공/실패 시 이메일/Slack 알림

---

## 🔧 **고급 설정 (선택 사항)**

### **커스텀 도메인 연결**

1. 도메인 구매 (예: lifehackdaily.com)
2. Vercel 대시보드 → 프로젝트 → **Settings** → **Domains**
3. 도메인 추가 → DNS 설정 안내 따라하기
4. 자동 SSL 인증서 발급 ✅

### **환경 변수 설정**

만약 API 키 등이 필요하면:
1. Vercel 대시보드 → **Settings** → **Environment Variables**
2. 변수 추가 (예: `API_KEY`, `GA_TRACKING_ID`)
3. 자동으로 배포 시 적용

---

## ⚡ **문제 해결**

### **Q1: 배포가 실패했어요**
```bash
# Vercel 로그 확인
- 대시보드 → Deployments → 실패한 배포 클릭
- Build Logs 확인
```

**흔한 원인:**
- 파일 경로 오류 (대소문자 구분)
- 누락된 파일 (index.html 필수)

### **Q2: GitHub Push가 안 돼요**
```bash
# GitHub Personal Access Token 필요
1. GitHub → Settings → Developer settings
2. Personal access tokens → Generate new token
3. repo 권한 체크
4. 토큰 복사해서 비밀번호 대신 사용
```

### **Q3: 변경사항이 반영 안 돼요**
- 브라우저 캐시 문제: `Ctrl+Shift+R` (강력 새로고침)
- Vercel 배포 확인: 대시보드에서 최신 배포 완료 여부 체크

---

## 📈 **다음 단계**

### **1. 콘텐츠 확대 (1-2개월)**
```
목표: 15-20개 글 작성
방법: AI에게 "블로그 글 써줘" 요청
주기: 주 3-5회
```

### **2. SEO 최적화**
- Google Search Console 등록
- Sitemap.xml 생성 및 제출
- 내부 링크 강화

### **3. 애드센스 신청 (3개월 후)**
```
조건 체크:
✅ 20개 이상 고품질 글
✅ 일 100명 이상 방문자
✅ 3개월 이상 운영
✅ 독립 도메인 (선택)
```

### **4. 수익화 확대**
- 제휴 마케팅 (앱 추천 링크)
- 스폰서 콘텐츠
- 디지털 제품 판매 (전자책, 템플릿)

---

## 🎉 **완료!**

이제 당신의 블로그는:
- ✅ GitHub에서 버전 관리
- ✅ Vercel에서 자동 배포
- ✅ HTTPS 보안 연결
- ✅ 무료 호스팅
- ✅ 무제한 트래픽

**새 글 발행**: 이 대화창에서 "블로그 글 써줘" 한 마디면 끝!

---

## 📞 **추가 지원**

- GitHub 가이드: https://docs.github.com
- Vercel 문서: https://vercel.com/docs
- AI 글 요청: 이 대화창에서 언제든지!

**배포 성공을 축하합니다! 🎊**
