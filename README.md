# 서예은 변호사 홈페이지

대한변호사협회 대의원 서예은 변호사의 공식 웹사이트입니다.

## 📋 프로젝트 개요

미니멀하고 세련된 디자인의 변호사 개인 홈페이지로, 변호사 소개, 활동사항, 칼럼, 성공사례, 상담문의 등의 정보를 제공합니다.

## ✨ 주요 기능

### 완료된 기능

1. **홈 (Hero Section)**
   - 미니멀한 디자인
   - 전문적인 법률 사무실 배경 이미지
   - 깔끔한 타이포그래피
   - 상담 문의 CTA 버튼

2. **변호사 소개**
   - 프로필 사진 및 경력사항
   - 2025 - 현재: 대한변호사협회 대의원
   - 2025 - 2025: 법무법인 가람 대표변호사
   - 2024 - 2025: 법무법인 수림 소속변호사
   - 2023 - 2024: 법무법인 율앤 소속변호사
   - 2023 - 2023: 경찰청 본청 범죄분석관실 법률사무종사 변호사
   - 자격사항: 2023년 변호사 자격 취득

3. **활동사항**
   - 언론보도: 2025.06 - 같은 아파트 사는 스토킹범 풀어준 경찰
   - 학회 및 단체 활동
   - 공익 활동
   - 위원회 활동

4. **칼럼**
   - 네이버 블로그 (https://blog.naver.com/lawyeryenny) 연동
   - 조회수 높은 인기 칼럼 3개 표시
   - 클릭 시 블로그로 이동
   - "더 많은 칼럼 보기" 버튼으로 블로그 직접 방문 가능

5. **성공사례**
   - 6가지 주요 성공사례 소개
   - 특수폭행 무죄, 성범죄 불기소, 횡령 집행유예 등

6. **상담문의**
   - 카카오톡 오픈채팅 연결 (https://open.kakao.com/o/slAyrTfi)
   - 이메일: lawyer.yenny.s@gmail.com
   - 사무실 정보 (서울 서초구 법원로 16, 정곡빌딩 동관 509호)
   - 카카오맵 연동 (길찾기 기능)
   - 지하철 안내 포함

7. **반응형 디자인**
   - 데스크톱, 태블릿, 모바일 완벽 대응

## 🎨 디자인 특징

- **미니멀한 히어로 섹션**: 전문적인 법률 사무실 배경 이미지
- **깔끔한 타이포그래피**: 대형 타이틀, 간결한 텍스트
- **고급스러운 컬러**: 다크 블루 + 골드
- **완벽한 반응형**: 모든 기기 최적화

## 🔧 홈페이지 내용 수정 방법

### 📝 텍스트 수정

#### 1. 메인 타이틀 변경
**파일**: `index.html` (52번째 줄)
```html
<h2 class="hero-title">서예은 변호사</h2>
```
→ "서예은 변호사"를 원하는 텍스트로 변경

#### 2. 서브타이틀 변경
**파일**: `index.html` (53번째 줄)
```html
<p class="hero-subtitle">형사변호 전문</p>
```
→ "형사변호 전문"을 원하는 텍스트로 변경

#### 3. 경력사항 수정
**파일**: `index.html` (97-120번째 줄)
```html
<li>
    <span class="timeline-year">2025 - 현재</span>
    <span class="timeline-content">대한변호사협회 대의원</span>
</li>
```
- 연도와 내용을 수정하거나
- `<li>...</li>` 블록 전체를 복사하여 추가 가능

#### 4. 연락처 정보 수정
**파일**: `index.html` (364, 374번째 줄)
- 이메일: "lawyer.yenny.s@gmail.com"

**Footer 이메일**: `index.html` (446번째 줄)

### 🖼️ 이미지 수정

#### 1. 메인 배경 이미지 변경
**파일**: `css/style.css` (176번째 줄)
```css
background-image: url('현재이미지URL');
```
→ URL을 새 이미지 URL로 교체

#### 2. 프로필 사진 변경
**파일**: `index.html` (87번째 줄)
```html
<img src="https://www.genspark.ai/api/files/s/t4VCcQZ1" alt="서예은 변호사">
```
→ src 속성을 새 이미지 URL로 교체

### 📝 블로그 칼럼 수정 (네이버 블로그 연동)

칼럼 섹션은 네이버 블로그 (https://blog.naver.com/lawyeryenny)와 연동되어 있습니다.

#### 칼럼 게시글 변경 방법

**파일**: `index.html` (약 200-240번째 줄)

각 칼럼 카드는 다음과 같은 구조입니다:

```html
<a href="블로그URL" target="_blank" class="column-card" rel="noopener noreferrer">
    <div class="column-image">
        <img src="이미지URL" alt="설명">
    </div>
    <div class="column-content">
        <span class="column-category">카테고리</span>
        <h3>게시글 제목</h3>
        <p>게시글 요약 설명</p>
        <div class="column-meta">
            <span><i class="far fa-calendar"></i> 날짜</span>
            <span class="column-link"><i class="fas fa-external-link-alt"></i> 블로그에서 읽기</span>
        </div>
    </div>
</a>
```

**수정할 부분:**
1. `href="블로그URL"` - 블로그 게시글 전체 URL
2. `<span class="column-category">카테고리</span>` - 카테고리명
3. `<h3>게시글 제목</h3>` - 실제 제목
4. `<p>게시글 요약 설명</p>` - 간단한 요약
5. `<span>날짜</span>` - 게시 날짜 (YYYY.MM.DD)

**예시:**
```html
<a href="https://blog.naver.com/lawyeryenny/224172806194" target="_blank" class="column-card">
    <div class="column-content">
        <span class="column-category">형사변호</span>
        <h3>피해액 수억 원 횡령 혐의였지만, 영장 기각으로 불구속 수사로 전환된 사례</h3>
        <p>수억 원 횡령 혐의로 구속영장이 청구되었으나...</p>
        <div class="column-meta">
            <span><i class="far fa-calendar"></i> 2025.02.05</span>
        </div>
    </div>
</a>
```

### 🎨 색상 변경

**파일**: `css/style.css` (7-15번째 줄)
```css
--primary-color: #1a3a5c;      /* 메인 다크 블루 */
--secondary-color: #c9a961;     /* 골드 */
--accent-color: #2c5f8d;        /* 액센트 블루 */
```
→ 색상 코드를 원하는 색으로 변경

### 📱 카카오톡 연동 (완료)

**파일**: `js/main.js` (225번째 줄)

카카오톡 오픈채팅이 이미 연동되어 있습니다:
```javascript
const kakaoChannelUrl = 'https://open.kakao.com/o/slAyrTfi';
```

**변경 방법:**
- 다른 카카오톡 채널/오픈채팅으로 변경하려면 URL만 교체하세요.

### 🗺️ 사무실 위치 (완료)

**현재 주소**: 서울 서초구 법원로 16, 정곡빌딩 동관 509호

**변경 방법:**

1. **연락처 섹션 주소** (`index.html` 354번째 줄)
```html
<p>서울 서초구 법원로 16<br>정곡빌딩 동관 509호</p>
```

2. **Footer 주소** (`index.html` 438번째 줄)
```html
<li><i class="fas fa-map-marker-alt"></i> 서울 서초구 법원로 16, 정곡빌딩 동관 509호</li>
```

3. **지도 링크** (`index.html` 415번째 줄)
```html
<a href="https://map.kakao.com/link/search/주소입력" ...>
```
→ 주소 부분만 변경

## 🚀 기능 엔트리 포인트

### 주요 URL 구조

- `/` (index.html): 메인 페이지
  - `#home`: 히어로 섹션
  - `#about`: 변호사 소개
  - `#activities`: 활동사항
  - `#columns`: 칼럼
  - `#cases`: 성공사례
  - `#contact`: 상담문의

## 📂 프로젝트 구조

```
.
├── index.html              # 메인 HTML 파일
├── css/
│   └── style.css          # 메인 스타일시트
├── js/
│   └── main.js            # JavaScript 기능
└── README.md              # 프로젝트 문서
```

## 🔧 추가 설정이 필요한 항목

### 1. 칼럼 업데이트
- 새 블로그 글 작성 시 칼럼 카드 내용 업데이트
- 제목, 날짜, URL만 변경하면 됨

### 2. 성공사례 수정
- 실제 사례로 교체 가능
- `index.html`의 250-334번째 줄

## 📱 반응형 브레이크포인트

- **Desktop**: 1024px 이상
- **Tablet**: 768px - 1023px
- **Mobile**: 767px 이하

## 🌐 SEO 최적화

- 메타 태그 설정 완료
- 시맨틱 HTML 구조
- 접근성 고려 (ARIA 레이블)
- 빠른 로딩 속도를 위한 최적화

## 🎯 향후 개발 추천 사항

### 우선순위 높음
1. ✅ ~~카카오톡 채널 연동 완료~~
2. ✅ ~~지도 연동 완료 (카카오맵)~~
3. ✅ ~~이메일 주소 설정 완료~~
4. 인기 칼럼 업데이트 (블로그에서 새 글 발행 시)

### 우선순위 중간
5. 성공사례 상세 페이지 추가
6. 관리자 페이지 (칼럼/사례 관리)
7. 칼럼 이미지 최적화 (각 게시글에 맞는 썸네일)

### 우선순위 낮음
8. 다국어 지원 (영어)
9. 법률 상담 예약 시스템
10. 고객 후기/리뷰 섹션

## 💡 빠른 수정 팁

1. **텍스트 수정**: `index.html` 파일에서 Ctrl+F로 검색 후 수정
2. **색상 변경**: `css/style.css` 상단의 `:root` 변수 수정
3. **이미지 교체**: 이미지 URL만 찾아서 교체
4. **섹션 숨기기**: 해당 `<section>` 태그에 `style="display:none"` 추가

## 🔒 보안 고려사항

- HTTPS 사용 필수
- 개인정보 처리방침 페이지 추가 필요

## 📄 라이선스

Copyright © 2025 서예은 변호사. All rights reserved.

---

**제작일**: 2025년 2월  
**최종 업데이트**: 2025년 2월  
**버전**: 2.0.0