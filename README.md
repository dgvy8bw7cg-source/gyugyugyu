<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CampusFit - 대학생 식단 관리 및 건강 분석 서비스</title>
    <!-- Google Fonts: Outfit & Noto Sans KR -->
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700;800&family=Noto+Sans+KR:wght@300;400;500;700;900&display=swap" rel="stylesheet">
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    <!-- Chart.js CDN -->
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- ==================== LANDING PAGE (HOMEPAGE) ==================== -->
    <div id="landing-page" class="landing-page">
        <!-- Landing Header -->
        <header class="landing-header">
            <div class="landing-logo">
                <i data-lucide="leaf" class="logo-icon-green"></i>
                <span>CampusFit</span>
            </div>
            <nav class="landing-nav">
                <a href="#features-section">주요 기능</a>
                <a href="#how-section">이용 방법</a>
                <a href="#landing-tips-preview">건강 가이드</a>
            </nav>
            <button class="header-cta-btn" id="header-go-app-btn">대시보드 바로가기</button>
        </header>
        <!-- Landing Hero Section -->
        <section class="landing-hero">
            <div class="hero-bg-blobs">
                <div class="blob blob-1"></div>
                <div class="blob blob-2"></div>
            </div>
            
            <div class="hero-container">
                <div class="hero-text-content">
                    <span class="hero-tag"><i data-lucide="sparkles"></i> 대학생 맞춤형 웰니스 케어</span>
                    <h1>대학생을 위한<br><span class="highlight-green">똑똑한 식단 가이드</span></h1>
                    <p class="hero-subtitle">바쁜 전공 수업과 자취 생활 속에서 학식 및 편의점 프리셋을 활용해 식단을 관리하세요. 건강 점수 분석과 그래프 통계로 더 스마트한 캠퍼스 라이프를 지원합니다.</p>
                    <div class="hero-actions">
                        <button class="hero-primary-btn" id="start-app-btn">
                            <span>프로필 설정하고 시작하기</span>
                            <i data-lucide="arrow-right"></i>
                        </button>
                        <a href="#features-section" class="hero-secondary-link">더 알아보기</a>
                    </div>
                </div>
                <!-- CSS-based App Mockup Preview -->
                <div class="hero-mockup-wrapper">
                    <div class="mockup-card main-mockup">
                        <div class="mockup-header">
                            <span class="mockup-dot"></span>
                            <span class="mockup-title">오늘의 영양 대시보드</span>
                        </div>
                        <div class="mockup-body">
                            <!-- Circular Calorie Preview -->
                            <div class="mockup-radial-container">
                                <div class="mockup-circle">
                                    <span class="m-percent">68%</span>
                                    <span class="m-sub">1,560 / 2,300 kcal</span>
                                </div>
                            </div>
                            <!-- Food tag preview list -->
                            <div class="mockup-food-list">
                                <div class="m-food-item">
                                    <span class="m-emoji">🌅</span>
                                    <div class="m-food-info">
                                        <h4>참치마요 삼각김밥</h4>
                                        <p>아침 • 200 kcal</p>
                                    </div>
                                </div>
                                <div class="m-food-item">
                                    <span class="m-emoji">☀️</span>
                                    <div class="m-food-info">
                                        <h4>학식 제육덮밥</h4>
                                        <p>점심 • 650 kcal</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <!-- Floating Sub-card 1 -->
                    <div class="mockup-card floating-card-1">
                        <div class="f-header">
                            <i data-lucide="heart" class="heart-pulse text-red"></i>
                            <span>건강 점수</span>
                        </div>
                        <div class="f-value">88점</div>
                        <p class="f-desc">탄단지 비율이 훌륭해요!</p>
                    </div>
                    <!-- Floating Sub-card 2 -->
                    <div class="mockup-card floating-card-2">
                        <div class="f-header">
                            <i data-lucide="bar-chart-2" class="text-blue"></i>
                            <span>체질량지수(BMI)</span>
                        </div>
                        <div class="f-value">21.8 <span class="f-badge">정상</span></div>
                    </div>
                </div>
            </div>
        </section>
        <!-- Features Grid Section -->
        <section class="landing-features" id="features-section">
            <div class="section-header-centered">
                <span class="section-tag">FEATURES</span>
                <h2>CampusFit의 4가지 핵심 솔루션</h2>
                <p>대학생의 라이프스타일에 맞춘 실용적이고 직관적인 기능들을 소개합니다.</p>
            </div>
            
            <div class="features-grid">
                <div class="feature-box">
                    <div class="f-icon-container bg-green">
                        <i data-lucide="plus-circle"></i>
                    </div>
                    <h3>간편 식단 등록 프리셋</h3>
                    <p>학식 백반, 편의점 삼각김밥, 컵라면, 닭가슴살 샐러드 등 대학생 단골 메뉴가 영양 데이터와 함께 탑재되어 터치 한 번으로 쉽게 등록할 수 있습니다.</p>
                </div>
                <div class="feature-box">
                    <div class="f-icon-container bg-orange">
                        <i data-lucide="activity"></i>
                    </div>
                    <h3>실시간 건강 점수 산출</h3>
                    <p>단순 칼로리 계산을 넘어 탄수화물/단백질/지방의 비율, 규칙적인 식사 횟수, 신체 상태(BMI)를 계산하여 나만의 오늘 식단 건강 점수를 부여합니다.</p>
                </div>
                <div class="feature-box">
                    <div class="f-icon-container bg-blue">
                        <i data-lucide="bar-chart-3"></i>
                    </div>
                    <h3>주간/월간 통계 차트</h3>
                    <p>Chart.js 엔진을 탑재하여 주간 및 월간 권장 칼로리 달성 추이, 누적 탄단지 섭취 비중, 아침·점심·저녁 등 식사 종류별 기여도를 정교하게 시각화합니다.</p>
                </div>
                <div class="feature-box">
                    <div class="f-icon-container bg-pink">
                        <i data-lucide="lightbulb"></i>
                    </div>
                    <h3>대학생 식생활 밀착 가이드</h3>
                    <p>술자리에서 나트륨과 숙취를 줄이는 안주 매뉴얼, 편의점 가성비 다이어트 조합, 시험 기간 야식 추천 등 대학생 상황별 맞춤 팁을 상시 제공합니다.</p>
                </div>
            </div>
        </section>
        <!-- How It Works Section -->
        <section class="landing-how" id="how-section">
            <div class="section-header-centered">
                <span class="section-tag">HOW IT WORKS</span>
                <h2>이용 방법 안내</h2>
                <p>CampusFit을 통해 건강한 캠퍼스 다이어트를 시작하는 3단계 과정입니다.</p>
            </div>
            
            <div class="how-steps-grid">
                <div class="how-step">
                    <div class="step-num">01</div>
                    <h3>신체 정보 프로필 설정</h3>
                    <p>키, 몸무게, 활동 수준을 입력하면 맞춤형 일일 칼로리 권장량과 최적의 영양 밸런스 가이드라인을 바로 제안해 줍니다.</p>
                </div>
                <div class="how-step">
                    <div class="step-num">02</div>
                    <h3>매일의 식단 및 음료 입력</h3>
                    <p>학식이나 편의점 음식을 먹을 때마다 프리셋 또는 직접 입력을 통해 아침, 점심, 저녁, 간식의 식사 종류로 간편하게 추가합니다.</p>
                </div>
                <div class="how-step">
                    <div class="step-num">03</div>
                    <h3>건강 분석 리포트 확인</h3>
                    <p>대시보드에서 매일 갱신되는 피드백과 건강 점수를 확인하고, 통계 탭에서 균형 잡힌 습관이 형성되는 과정을 분석합니다.</p>
                </div>
            </div>
        </section>
        <!-- Tips Section Preview -->
        <section class="landing-tips-preview" id="landing-tips-preview">
            <div class="tips-preview-container">
                <div class="tips-preview-text">
                    <span class="section-tag">HEALTH TIPS</span>
                    <h2>대학 생활 속<br>식단 관리가 어려운가요?</h2>
                    <p>CampusFit에서는 대학생들이 마주하는 현실적인 식생활 고민들을 해결하기 위한 가이드를 상시 제공합니다. 지금 앱을 시작하여 더 많은 꿀팁들을 대시보드에서 확인해 보세요.</p>
                    <ul class="preview-tips-list">
                        <li><i data-lucide="check" class="check-icon"></i> 돈 없을 때 편의점 가성비 식단 꿀조합</li>
                        <li><i data-lucide="check" class="check-icon"></i> 학식 소스 따로 담기로 150kcal 절약 비법</li>
                        <li><i data-lucide="check" class="check-icon"></i> 전공 시험 기간 뇌 깨우는 견과류와 물 섭취 가이드</li>
                    </ul>
                </div>
                <div class="tips-preview-cards">
                    <div class="p-tip-card">
                        <div class="p-tip-header">
                            <span class="p-tip-tag"># 술자리 대처법</span>
                            <i data-lucide="beer" class="p-tip-icon"></i>
                        </div>
                        <h3>동아리 술자리 안주 스마트 선택법</h3>
                        <p>튀김이나 매운 탕 대신 두부김치, 계란말이, 먹태 같이 기름기가 적고 단백질이 풍부한 안주를 고르고 물을 1:1로 섭취하세요.</p>
                    </div>
                </div>
            </div>
        </section>
        <!-- CTA Section -->
        <section class="landing-cta">
            <div class="cta-card">
                <h2>오늘부터 더 건강한 나를 만나보세요</h2>
                <p>회원가입과 로그인 번거로움 없이 브라우저 로컬스토리지에 데이터가 안전하게 저장되어 즉시 무료로 이용 가능합니다.</p>
                <button class="cta-btn" id="cta-start-btn">지금 시작하기 <i data-lucide="arrow-right"></i></button>
            </div>
        </section>
        <!-- Landing Footer -->
        <footer class="landing-footer">
            <p>© 2026 CampusFit. All rights reserved.</p>
            <p class="disclaimer">본 서비스에서 제공하는 건강 정보 및 권장 권장량은 일반적인 계산식에 기반한 참고용 가이드라인이며, 전문 의학적 소견을 대체할 수 없습니다.</p>
        </footer>
    </div>
    // ==================== MAIN DASHBOARD APP ====================
    <div class="app-container hidden" id="app-container">
        <!-- Sidebar Navigation -->
        <aside class="sidebar">
            <div class="sidebar-header">
                <div class="logo" id="sidebar-logo-home" style="cursor: pointer;" title="홈페이지로 돌아가기">
                    <i data-lucide="leaf" class="logo-icon"></i>
                    <span>CampusFit</span>
                </div>
            </div>
            <!-- Profile Summary in Sidebar -->
            <div class="profile-summary-card">
                <div class="profile-avatar">
                    <span id="profile-emoji">🎓</span>
                </div>
                <div class="profile-info">
                    <h3 id="sidebar-user-name">게스트</h3>
                    <p class="profile-status" id="sidebar-user-bmi">프로필을 등록해주세요</p>
                </div>
                <button class="edit-profile-btn" id="open-profile-btn" title="프로필 설정">
                    <i data-lucide="settings"></i>
                </button>
            </div>
            <!-- Nav Items -->
            <nav class="nav-menu">
                <button class="nav-item active" data-tab="dashboard">
                    <i data-lucide="layout-dashboard"></i>
                    <span>대시보드</span>
                </button>
                <button class="nav-item" data-tab="meal-log">
                    <i data-lucide="calendar"></i>
                    <span>식단 기록</span>
                </button>
                <button class="nav-item" data-tab="statistics">
                    <i data-lucide="bar-chart-3"></i>
                    <span>영양 통계</span>
                </button>
                <button class="nav-item" data-tab="tips">
                    <i data-lucide="lightbulb"></i>
                    <span>꿀팁 & 가이드</span>
                </button>
            </nav>
            <div class="sidebar-footer">
                <p>© 2026 CampusFit</p>
                <p>For Healthy Campus Life</p>
            </div>
        </aside>
        <!-- Main Content Area -->
        <main class="main-content">
            <!-- Top Bar -->
            <header class="top-bar">
                <div class="header-title">
                    <h1 id="greeting-title">안녕하세요, 대학생 님!</h1>
                    <p id="today-date-str">2026년 6월 21일 일요일</p>
                </div>
                <div class="quick-stats-badge">
                    <i data-lucide="heart" class="heart-pulse"></i>
                    <span>오늘의 건강 점수: <strong id="top-health-score">0</strong>점</span>
                </div>
            </header>
            <!-- Content Tabs -->
            <!-- 1. DASHBOARD TAB -->
            <section class="tab-content active" id="dashboard-tab">
                <div class="dashboard-grid">
                    <!-- Progress Card: Calories -->
                    <div class="dashboard-card status-card">
                        <div class="card-header">
                            <h3>오늘의 칼로리</h3>
                            <i data-lucide="flame" class="icon-calorie"></i>
                        </div>
                        <div class="calorie-progress-container">
                            <div class="radial-progress">
                                <svg class="progress-ring" width="160" height="160">
                                    <circle class="progress-ring__circle-bg" stroke="#e2e8f0" stroke-width="12" fill="transparent" r="70" cx="80" cy="80"/>
                                    <circle class="progress-ring__circle" id="calorie-ring" stroke="#10b981" stroke-width="12" fill="transparent" r="70" cx="80" cy="80"/>
                                </svg>
                                <div class="radial-progress-text">
                                    <span class="progress-percent" id="calorie-percentage">0%</span>
                                    <span class="progress-sub" id="calorie-ratio">0 / 2300 kcal</span>
                                </div>
                            </div>
                        </div>
                        <div class="calorie-details">
                            <div class="detail-item">
                                <span>섭취량</span>
                                <strong id="eaten-calories">0 kcal</strong>
                            </div>
                            <div class="detail-item">
                                <span>남은 권장량</span>
                                <strong id="remaining-calories">2,300 kcal</strong>
                            </div>
                        </div>
                    </div>
                    <!-- Progress Card: Macros -->
                    <div class="dashboard-card status-card">
                        <div class="card-header">
                            <h3>3대 영양소 비율</h3>
                            <i data-lucide="pie-chart" class="icon-macro"></i>
                        </div>
                        <div class="macro-progress-list">
                            <!-- Carbs -->
                            <div class="macro-item">
                                <div class="macro-info">
                                    <span class="macro-label">탄수화물 (Carbs)</span>
                                    <span class="macro-value"><span id="eaten-carbs">0</span>g / <span id="target-carbs">287</span>g</span>
                                </div>
                                <div class="progress-bar-bg">
                                    <div class="progress-bar" id="carbs-bar" style="width: 0%; background-color: #3b82f6;"></div>
                                </div>
                            </div>
                            <!-- Protein -->
                            <div class="macro-item">
                                <div class="macro-info">
                                    <span class="macro-label">단백질 (Protein)</span>
                                    <span class="macro-value"><span id="eaten-protein">0</span>g / <span id="target-protein">115</span>g</span>
                                </div>
                                <div class="progress-bar-bg">
                                    <div class="progress-bar" id="protein-bar" style="width: 0%; background-color: #10b981;"></div>
                                </div>
                            </div>
                            <!-- Fat -->
                            <div class="macro-item">
                                <div class="macro-info">
                                    <span class="macro-label">지방 (Fat)</span>
                                    <span class="macro-value"><span id="eaten-fat">0</span>g / <span id="target-fat">76</span>g</span>
                                </div>
                                <div class="progress-bar-bg">
                                    <div class="progress-bar" id="fat-bar" style="width: 0%; background-color: #f59e0b;"></div>
                                </div>
                            </div>
                        </div>
                        <div class="macro-ratio-footer">
                            <span>권장 비율: 탄 50% | 단 25% | 지 25%</span>
                        </div>
                    </div>
                    <!-- Health Score Dial Card -->
                    <div class="dashboard-card status-card health-score-card">
                        <div class="card-header">
                            <h3>나의 건강 점수</h3>
                            <i data-lucide="activity" class="icon-health"></i>
                        </div>
                        <div class="health-score-container">
                            <div class="score-display">
                                <span class="score-number" id="dashboard-health-score">0</span>
                                <span class="score-max">/ 100 점</span>
                            </div>
                            <p class="health-score-feedback" id="health-score-feedback">프로필과 오늘의 첫 식단을 입력해 건강 분석을 시작하세요!</p>
                        </div>
                        <div class="health-meta-info">
                            <div class="meta-row">
                                <span>신체 질량 지수(BMI)</span>
                                <span class="badge" id="bmi-badge">--</span>
                            </div>
                            <div class="meta-row">
                                <span>일일 권장 칼로리</span>
                                <span class="badge badge-green" id="target-calories-badge">2,300 kcal</span>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- Quick Meal Log Section -->
                <div class="dashboard-section">
                    <div class="section-title-area">
                        <h2><i data-lucide="plus-circle"></i> 오늘 식단 간편 등록</h2>
                        <span class="section-subtitle">학식, 편의점 프리셋을 이용하면 터치 한 번으로 등록됩니다.</span>
                    </div>
                    <div class="meal-log-card">
                        <!-- Meal Type Selector -->
                        <div class="meal-type-selector">
                            <label class="meal-type-btn">
                                <input type="radio" name="meal-type" value="아침" checked>
                                <span>🌅 아침</span>
                            </label>
                            <label class="meal-type-btn">
                                <input type="radio" name="meal-type" value="점심">
                                <span>☀️ 점심</span>
                            </label>
                            <label class="meal-type-btn">
                                <input type="radio" name="meal-type" value="저녁">
                                <span>🌙 저녁</span>
                            </label>
                            <label class="meal-type-btn">
                                <input type="radio" name="meal-type" value="간식">
                                <span>🧁 간식</span>
                            </label>
                        </div>
                        <div class="log-form-container">
                            <!-- Preset Dropdown -->
                            <div class="form-group preset-group">
                                <label for="preset-select"><i data-lucide="search"></i> 대학생 맞춤 인기 메뉴 검색/선택</label>
                                <div class="select-wrapper">
                                    <select id="preset-select">
                                        <option value="custom">-- 직접 입력 --</option>
                                        <optgroup label="🎒 캠퍼스 학식 & 가성비">
                                            <option value="학식_백반">학식 백반 (김치찌개/된장찌개 등) [550kcal]</option>
                                            <option value="학식_돈까스">학식 돈까스 정식 [850kcal]</option>
                                            <option value="제육덮밥">제육덮밥 [650kcal]</option>
                                            <option value="뼈다귀해장국">뼈다귀해장국 (밥 포함) [720kcal]</option>
                                        </optgroup>
                                        <optgroup label="🏪 편의점 꿀조합">
                                            <option value="참치마요_삼각김밥">참치마요 삼각김밥 (1개) [200kcal]</option>
                                            <option value="컵라면_소형">컵라면 소형 (육개장 등) [300kcal]</option>
                                            <option value="컵라면_대형">컵라면 대형 (불닭볶음면 등) [480kcal]</option>
                                            <option value="편의점_도시락">편의점 고기 가득 도시락 [750kcal]</option>
                                            <option value="훈제란">편의점 훈제란 (2알) [150kcal]</option>
                                        </optgroup>
                                        <optgroup label="🥗 헬스 & 다이어터">
                                            <option value="닭가슴살_샐러드">닭가슴살 샐러드 (오리엔탈 드레싱) [250kcal]</option>
                                            <option value="훈제닭가슴살">훈제 닭가슴살팩 (100g) [120kcal]</option>
                                            <option value="바나나">바나나 (1개) [90kcal]</option>
                                            <option value="고구마">찐 고구마 (1개, 120g) [150kcal]</option>
                                        </optgroup>
                                        <optgroup label="🍗 배달 & 외식">
                                            <option value="치킨_반마리">후라이드 치킨 (반마리, 4조각) [700kcal]</option>
                                            <option value="짜장면">짜장면 (1그릇) [780kcal]</option>
                                            <option value="엽떡_일인분">매운 국물떡볶이 (1인분 분량) [450kcal]</option>
                                            <option value="서브웨이_이탈리안">서브웨이 이탈리안 비엠티 (15cm) [410kcal]</option>
                                        </optgroup>
                                        <optgroup label="☕️ 대학생 수명 연장제 (음료/카페)">
                                            <option value="아메리카노">아이스 아메리카노 [10kcal]</option>
                                            <option value="바닐라라떼">바닐라 라떼 (시럽 포함) [220kcal]</option>
                                            <option value="에너지드링크">몬스터 에너지/핫식스 [100kcal]</option>
                                            <option value="소주">소주 (1병) [400kcal]</option>
                                        </optgroup>
                                    </select>
                                </div>
                            </div>
                            <!-- Manual Input Grid -->
                            <form id="meal-form" class="meal-form-grid">
                                <div class="form-group grid-col-2">
                                    <label for="food-name">음식명 <span class="required">*</span></label>
                                    <input type="text" id="food-name" required placeholder="예: 삼각김밥, 제육볶음">
                                </div>
                                <div class="form-group">
                                    <label for="food-amount">섭취량(g 또는 개/회) <span class="required">*</span></label>
                                    <input type="number" id="food-amount" required value="1" min="1" placeholder="예: 1">
                                </div>
                                <div class="form-group">
                                    <label for="food-calories">칼로리(kcal) <span class="required">*</span></label>
                                    <input type="number" id="food-calories" required min="0" placeholder="0">
                                </div>
                                <div class="form-group">
                                    <label for="food-carbs">탄수화물(g)</label>
                                    <input type="number" id="food-carbs" min="0" value="0" placeholder="0">
                                </div>
                                <div class="form-group">
                                    <label for="food-protein">단백질(g)</label>
                                    <input type="number" id="food-protein" min="0" value="0" placeholder="0">
                                </div>
                                <div class="form-group">
                                    <label for="food-fat">지방(g)</label>
                                    <input type="number" id="food-fat" min="0" value="0" placeholder="0">
                                </div>
                                <div class="form-group">
                                    <label for="meal-date">섭취 날짜</label>
                                    <input type="date" id="meal-date" required>
                                </div>
                                <div class="form-group grid-col-all flex-end">
                                    <button type="submit" class="submit-meal-btn">
                                        <i data-lucide="plus"></i> 식단 등록하기
                                    </button>
                                </div>
                            </form>
                        </div>
                    </div>
                </div>
            </section>
            <!-- 2. MEAL LOG TAB -->
            <section class="tab-content" id="meal-log-tab">
                <div class="meal-log-header-container">
                    <div class="section-title-area">
                        <h2>식단 일기</h2>
                        <p class="section-subtitle">언제든 지난 식단을 조회하고 관리할 수 있습니다.</p>
                    </div>
                    <div class="filter-controls">
                        <div class="filter-group">
                            <label for="log-date-filter"><i data-lucide="calendar"></i> 날짜 선택</label>
                            <input type="date" id="log-date-filter">
                        </div>
                        <div class="filter-group">
                            <label for="log-type-filter"><i data-lucide="filter"></i> 식사 종류</label>
                            <select id="log-type-filter">
                                <option value="all">전체 식사</option>
                                <option value="아침">🌅 아침</option>
                                <option value="점심">☀️ 점심</option>
                                <option value="저녁">🌙 저녁</option>
                                <option value="간식">🧁 간식</option>
                            </select>
                        </div>
                    </div>
                </div>
                <!-- Daily Summary Stats in Meal Log -->
                <div class="selected-day-summary" id="selected-day-summary-box">
                    <div class="summary-stat-box">
                        <span class="lbl">선택일 섭취 칼로리</span>
                        <strong id="log-day-calories">0 kcal</strong>
                    </div>
                    <div class="summary-stat-box">
                        <span class="lbl">탄수화물</span>
                        <span id="log-day-carbs">0g</span>
                    </div>
                    <div class="summary-stat-box">
                        <span class="lbl">단백질</span>
                        <span id="log-day-protein">0g</span>
                    </div>
                    <div class="summary-stat-box">
                        <span class="lbl">지방</span>
                        <span id="log-day-fat">0g</span>
                    </div>
                </div>
                <!-- Log List Grid -->
                <div class="meal-cards-container" id="meal-cards-list">
                    <!-- Cards will be dynamically inserted here -->
                    <div class="no-data-placeholder">
                        <i data-lucide="utensils-cross"></i>
                        <p>선택한 조건에 등록된 식단이 없습니다.</p>
                        <span>대시보드에서 오늘의 맛있는 식단을 기록해 보세요!</span>
                    </div>
                </div>
            </section>
            <!-- 3. STATISTICS TAB -->
            <section class="tab-content" id="statistics-tab">
                <div class="section-title-area">
                    <h2>영양 섭취 통계 분석</h2>
                    <p class="section-subtitle">주간 및 월간 단위로 칼로리와 영양 밸런스 추이를 한눈에 모니터링하세요.</p>
                </div>
                <div class="stats-period-selector">
                    <button class="period-btn active" data-period="weekly">최근 7일 (주간)</button>
                    <button class="period-btn" data-period="monthly">최근 30일 (월간)</button>
                </div>
                <div class="stats-charts-grid">
                    <!-- Chart 1: Calorie Trend -->
                    <div class="dashboard-card chart-card">
                        <div class="card-header">
                            <h3>칼로리 섭취량 추이</h3>
                            <span class="badge badge-outline">Line Chart</span>
                        </div>
                        <div class="chart-container">
                            <canvas id="calorieTrendChart"></canvas>
                        </div>
                        <div class="chart-desc">
                            <p>실제 섭취 칼로리(초록선)와 권장 칼로리 목표선(빨간 점선)의 대비를 보여줍니다.</p>
                        </div>
                    </div>
                    <!-- Chart 2: Nutrient Balance -->
                    <div class="dashboard-card chart-card">
                        <div class="card-header">
                            <h3>평균 영양 섭취 비율</h3>
                            <span class="badge badge-outline">Doughnut Chart</span>
                        </div>
                        <div class="chart-container flex-center">
                            <div class="chart-wrapper-small">
                                <canvas id="nutrientRatioChart"></canvas>
                            </div>
                        </div>
                        <div class="chart-desc">
                            <p>선택한 기간 동안의 탄수화물, 단백질, 지방 섭취 비중입니다. (권장 비율 탄:단:지 = 50%:25%:25%)</p>
                        </div>
                    </div>
                    <!-- Chart 3: Meal Type Contribution -->
                    <div class="dashboard-card chart-card grid-col-all">
                        <div class="card-header">
                            <h3>식사 종류별 섭취 기여도</h3>
                            <span class="badge badge-outline">Bar Chart</span>
                        </div>
                        <div class="chart-container">
                            <canvas id="mealTypeChart"></canvas>
                        </div>
                        <div class="chart-desc">
                            <p>아침, 점심, 저녁, 간식이 일일 전체 영양소 섭취에서 차지하는 칼로리 총량 비율을 비교합니다.</p>
                        </div>
                    </div>
                </div>
            </section>
            <!-- 4. TIPS TAB -->
            <section class="tab-content" id="tips-tab">
                <div class="section-title-area">
                    <h2>대학생 건강 식생활 가이드</h2>
                    <p class="section-subtitle">바쁜 대학 생활 속에서 가성비와 건강을 동시에 챙길 수 있는 알짜 꿀팁을 전해드립니다!</p>
                </div>
                <!-- Custom Tips Grid -->
                <div class="tips-grid" id="tips-cards-container">
                    <!-- Tips will be dynamically generated by JS -->
                </div>
            </section>
        </main>
    </div>
    <!-- Profile Edit Modal -->
    <div class="modal-overlay" id="profile-modal">
        <div class="modal-card">
            <div class="modal-header">
                <h2><i data-lucide="user"></i> 대학생 프로필 설정</h2>
                <button class="close-modal-btn" id="close-profile-btn">
                    <i data-lucide="x"></i>
                </button>
            </div>
            <form id="profile-form">
                <div class="modal-body">
                    <p class="modal-desc">키와 몸무게를 입력하시면 BMI 및 하루 영양소 권장량이 맞춤형으로 계산됩니다.</p>
                    
                    <div class="form-group">
                        <label for="user-name">이름 (닉네임) <span class="required">*</span></label>
                        <input type="text" id="user-name" required placeholder="예: 홍길동">
                    </div>
                    <div class="modal-form-grid">
                        <div class="form-group">
                            <label for="user-height">키 (cm) <span class="required">*</span></label>
                            <input type="number" id="user-height" required min="100" max="250" placeholder="예: 175">
                        </div>
                        <div class="form-group">
                            <label for="user-weight">몸무게 (kg) <span class="required">*</span></label>
                            <input type="number" id="user-weight" required min="30" max="200" placeholder="예: 70">
                        </div>
                    </div>
                    <div class="form-group">
                        <label for="user-gender">성별</label>
                        <div class="gender-selector">
                            <label class="gender-btn">
                                <input type="radio" name="user-gender" value="male" checked>
                                <span>🙋‍♂️ 남성</span>
                            </label>
                            <label class="gender-btn">
                                <input type="radio" name="user-gender" value="female">
                                <span>🙋‍♀️ 여성</span>
                            </label>
                        </div>
                    </div>
                    <div class="form-group">
                        <label for="user-activity">활동 수준</label>
                        <select id="user-activity">
                            <option value="sedentary">거의 앉아서 생활함 (대부분의 전공 수업, 공부)</option>
                            <option value="light">가벼운 활동 (통학, 걷기 위주 동아리)</option>
                            <option value="moderate">보통 활동 (주 3-4회 헬스, 활발한 신체활동)</option>
                            <option value="heavy">매우 활동적 (체육 전공, 강도 높은 스포츠 취미)</option>
                        </select>
                    </div>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" id="cancel-profile-btn">취소</button>
                    <button type="submit" class="btn btn-primary">저장 완료</button>
                </div>
            </form>
        </div>
    </div>
    <!-- Notification Toast -->
    <div id="toast" class="toast">
        <span id="toast-message">메시지</span>
    </div>
    <script src="script.js"></script>
</body>
</html>
