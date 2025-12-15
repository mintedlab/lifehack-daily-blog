# 📦 GitHub & Vercel 연동 - 완전 초보자 가이드

> **목표**: AI에게 "글 써줘" 한 마디로 자동 발행되는 블로그 만들기  
> **소요 시간**: 5분  
> **비용**: 무료

---

## 🎬 **시작하기 전에**

### **필요한 것**
- [ ] 이메일 주소 (Gmail 등)
- [ ] 인터넷 브라우저 (Chrome 권장)
- [ ] 5분의 시간

### **얻게 될 것**
- ✅ 자동 배포되는 블로그
- ✅ 무료 호스팅 (https://your-blog.vercel.app)
- ✅ 버전 관리 (이전 버전 복구 가능)
- ✅ AI 자동 발행 시스템

---

## 📍 **Step 1: GitHub 계정 만들기 (1분)**

### **1-1. GitHub 접속**
🔗 **링크**: https://github.com/signup

### **1-2. 회원가입**
```
1. 이메일 입력 → Continue
2. 비밀번호 만들기 → Continue
3. 사용자 이름 입력 (예: lifehack-creator) → Continue
4. 이메일 인증 코드 입력
5. 완료! ✅
```

**💡 팁**: 사용자 이름은 나중에 블로그 URL에 포함됩니다
- 예: `github.com/lifehack-creator`

---

## 📍 **Step 2: 블로그 저장소 만들기 (2분)**

### **2-1. 새 저장소 생성**

로그인 후:

1. 우측 상단 **프로필 아이콘** 옆 **"+"** 클릭
2. **"New repository"** 선택

### **2-2. 저장소 정보 입력**

아래 내용을 **정확히** 입력하세요:

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📝 Repository name (필수)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
lifehack-daily-blog

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📄 Description (선택)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
LifeHack Daily - 생산성 & 디지털 라이프스타일 블로그

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🔓 Public / Private (필수)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
⚪ Public (이것 선택!) ← 무료 배포를 위해 필수

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📋 Initialize this repository with:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
☑️ Add a README file (체크!)

```

3. 하단 **"Create repository"** 버튼 클릭

### **2-3. 완료 화면**
```
✅ https://github.com/[당신아이디]/lifehack-daily-blog
```
이 주소를 **복사해두세요!** (나중에 사용)

---

## 📍 **Step 3: 블로그 파일 업로드 (1분)**

### **3-1. 파일 업로드 페이지 열기**

방금 만든 저장소 페이지에서:

1. **"Add file"** 버튼 클릭
2. **"Upload files"** 선택

### **3-2. 파일 준비**

**방법 A: ZIP 다운로드 (권장)**

이 대화창에서:
```
당신: "프로젝트 파일 ZIP으로 만들어줘"
AI: [다운로드 링크 제공]
```

**방법 B: 직접 선택**

다음 파일들을 선택:
```
📁 프로젝트 폴더
├── 📄 index.html
├── 📄 vercel.json (중요!)
├── 📄 .gitignore
├── 📁 css/
│   └── style.css
├── 📁 js/
│   └── main.js
├── 📁 posts/
│   ├── 2025-productivity-apps-top10.html
│   ├── remote-work-productivity-tips.html
│   ├── notion-vs-obsidian-2025.html
│   └── ai-automation-time-saving.html
└── 📁 pages/
    ├── about.html
    ├── contact.html
    ├── privacy.html
    └── terms.html
```

### **3-3. 업로드 실행**

1. 파일들을 드래그 앤 드롭 (또는 "choose your files" 클릭)
2. **Commit message** 입력:
   ```
   Initial commit: LifeHack Daily blog setup
   ```
3. **"Commit changes"** 버튼 클릭

### **3-4. 확인**

업로드 완료 후 저장소 메인 페이지에서:
```
✅ index.html
✅ vercel.json
✅ css/
✅ js/
✅ posts/
✅ pages/
```
이 파일들이 보이면 성공! 🎉

---

## 📍 **Step 4: Vercel 연동 (2분)**

### **4-1. Vercel 접속**
🔗 **링크**: https://vercel.com/signup

### **4-2. GitHub 계정으로 가입**

**중요!** GitHub 계정으로 연동해야 자동 배포가 됩니다.

1. **"Continue with GitHub"** 클릭
2. GitHub 로그인 (이미 로그인 되어있으면 스킵)
3. Vercel 접근 권한 승인:
   ```
   ✅ "Authorize Vercel" 클릭
   ```

### **4-3. 프로젝트 임포트**

Vercel 대시보드에서:

1. **"Add New..."** → **"Project"** 클릭
2. **"Import Git Repository"** 섹션 찾기
3. `lifehack-daily-blog` 저장소 찾기
   - 안 보이면 **"Adjust GitHub App Permissions"** 클릭 → 권한 추가
4. **"Import"** 버튼 클릭

### **4-4. 배포 설정**

아래처럼 **비워두세요** (정적 사이트라 빌드 불필요):

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Project Name
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
lifehack-daily-blog (자동 입력됨)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Framework Preset
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Other (선택)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Root Directory
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
./ (기본값 그대로)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Build and Output Settings
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Build Command:        (비워두기)
Output Directory:     (비워두기)
Install Command:      (비워두기)
```

5. **"Deploy"** 버튼 클릭! 🚀

### **4-5. 배포 진행 중...**

화면에 실시간 로그가 표시됩니다:
```
⏳ Building...
⏳ Deploying...
✅ Deployment Ready!
```

약 **30초~1분** 소요됩니다. ☕

### **4-6. 배포 완료! 🎉**

성공 화면:
```
✅ Congratulations!

Your project is now live:
🌐 https://lifehack-daily-blog.vercel.app
```

**"Visit"** 버튼 클릭 → 당신의 블로그가 보입니다!

---

## 🎯 **Step 5: 자동 배포 테스트 (1분)**

### **이제부터는 이렇게 작동합니다:**

```
┌─────────────────────────────────────┐
│  당신: "블로그 글 써줘: [주제]"      │
└─────────────────────────────────────┘
              ↓
┌─────────────────────────────────────┐
│  AI: 글 작성 + HTML 생성             │
│      + GitHub에 자동 Push            │
└─────────────────────────────────────┘
              ↓
┌─────────────────────────────────────┐
│  GitHub: 변경 감지                   │
└─────────────────────────────────────┘
              ↓
┌─────────────────────────────────────┐
│  Vercel: 자동 배포 시작 (30초)       │
└─────────────────────────────────────┘
              ↓
┌─────────────────────────────────────┐
│  ✅ 블로그에 새 글 발행 완료!         │
│  🌐 https://lifehack-daily-blog      │
│     .vercel.app                      │
└─────────────────────────────────────┘
```

### **테스트 해보기**

이 대화창에서 바로:

```
"블로그 글 써줘: 2025년 추천 무료 앱 5가지"
```

입력하시면 3분 후 자동 발행됩니다!

---

## 🔍 **배포 상태 확인 방법**

### **Vercel 대시보드**
👉 https://vercel.com/dashboard

- **Deployments** 탭: 실시간 배포 현황
- **Domains** 탭: 사이트 주소 확인
- **Analytics** 탭: 방문자 통계 (무료)

### **GitHub 저장소**
👉 https://github.com/[당신아이디]/lifehack-daily-blog

- **Commits**: 변경 이력 확인
- **Code**: 현재 파일 상태

---

## ✅ **완료 체크리스트**

설정이 완료되었는지 확인하세요:

- [ ] GitHub 계정 생성 완료
- [ ] `lifehack-daily-blog` 저장소 생성 완료
- [ ] 블로그 파일 업로드 완료
- [ ] Vercel 계정 연동 완료
- [ ] 첫 배포 성공 (https://...vercel.app 접속 가능)
- [ ] 자동 배포 작동 확인 (새 글 발행 테스트)

---

## 🎁 **보너스: 커스텀 도메인 연결 (선택)**

### **도메인이 있다면**

예: `lifehackdaily.com` 구매 후

1. Vercel 대시보드 → 프로젝트 선택
2. **Settings** → **Domains**
3. 도메인 입력 → **Add**
4. DNS 설정 안내 따라하기:
   ```
   A 레코드: 76.76.21.21
   ```
5. 10분 후 자동 SSL 인증서 발급 ✅

**추천 도메인 구매처:**
- Namecheap: $8.88/년
- GoDaddy: $11.99/년
- Cloudflare: $9.15/년

---

## 🆘 **문제 해결**

### **Q1: GitHub 저장소가 Vercel에 안 보여요**

**해결:**
1. Vercel → Settings → Git Integration
2. **"Adjust GitHub App Permissions"** 클릭
3. `lifehack-daily-blog` 저장소 체크
4. 저장 → 다시 Import 시도

### **Q2: 배포는 성공했는데 페이지가 안 떠요**

**원인**: `index.html` 파일이 루트에 없음

**해결:**
```
GitHub 저장소에서:
- index.html이 최상위에 있는지 확인
- 폴더 안에 있으면 밖으로 이동
```

### **Q3: CSS가 안 먹혀요 (스타일이 깨짐)**

**원인**: 파일 경로 문제

**해결:**
```html
<!-- index.html에서 경로 확인 -->
❌ <link rel="stylesheet" href="/css/style.css">
✅ <link rel="stylesheet" href="css/style.css">
```

### **Q4: GitHub Push 권한 오류**

**해결:**
1. GitHub → Settings → Developer settings
2. **Personal access tokens** → **Generate new token**
3. `repo` 권한 체크
4. 토큰 생성 → 복사
5. Push 시 비밀번호 대신 토큰 입력

---

## 🚀 **다음 단계**

### **1. 첫 블로그 글 발행하기**

이 대화창에서:
```
"블로그 글 써줘: 2025년 꼭 써봐야 할 무료 생산성 앱 TOP 10"
```

### **2. SEO 설정 (구글 검색 노출)**

- Google Search Console 등록
- Sitemap 제출
- Robots.txt 설정

### **3. 애드센스 준비**

```
목표 체크리스트:
□ 15-20개 이상 고품질 글
□ 일 100명 이상 방문자
□ 3개월 이상 운영
```

### **4. 수익화**

- 구글 애드센스 신청
- 제휴 마케팅 (쿠팡, 알리익스프레스)
- 디지털 제품 판매

---

## 🎊 **축하합니다!**

당신은 이제:

✅ **GitHub**에서 버전 관리  
✅ **Vercel**에서 자동 배포  
✅ **AI**로 콘텐츠 자동 생성  
✅ **무료** 호스팅  
✅ **HTTPS** 보안 연결  
✅ **무제한** 트래픽  

하는 **완전 자동화 블로그**를 가지게 되었습니다!

---

## 📞 **도움이 더 필요하신가요?**

이 대화창에서 언제든지:

```
"GitHub 연동이 안 돼요"
"배포 오류가 나요"
"블로그 글 써줘"
```

물어보세요! 즉시 도와드립니다. 😊

**Happy Blogging! 🎉**
