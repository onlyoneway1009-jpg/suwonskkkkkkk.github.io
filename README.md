# suwonskkkkkkk.github.io
sssssssssssssssssssdfa123123124

<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>수원 삼성 블루윙즈 2026 공식 사이트</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/orioncactus/pretendard@v1.3.8/dist/web/static/pretendard.css" />
    <style>
        :root {
            --suwon-blue: #074CA1;
            --suwon-red: #C8102E;
            --suwon-white: #FFFFFF;
            --suwon-gold: #B39759;
        }

        * { box-sizing: border-box; -webkit-font-smoothing: antialiased; }

        body {
            font-family: 'Pretendard', sans-serif;
            margin: 0; padding: 0;
            background: linear-gradient(rgba(0,0,0,0.85), rgba(0,0,0,0.85)), 
                        url('https://images.unsplash.com/photo-1574629810360-7efbbe195018?auto=format&fit=crop&q=80&w=2000') no-repeat center center fixed;
            background-size: cover;
            background-attachment: fixed;
            color: white;
        }

        nav {
            position: sticky; top: 0; z-index: 1000;
            background: rgba(7, 76, 161, 0.98);
            border-bottom: 4px solid var(--suwon-red);
            display: flex; justify-content: space-around; flex-wrap: wrap;
            padding: 15px 0;
            box-shadow: 0 4px 12px rgba(0,0,0,0.3);
        }

        .nav-item {
            color: white; font-weight: 700; font-size: 1rem;
            text-decoration: none; cursor: pointer;
            transition: 0.3s;
            padding: 8px 15px;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.5);
        }

        .nav-item:hover { 
            color: var(--suwon-gold);
            transform: scale(1.05);
            background: rgba(255,255,255,0.1);
            border-radius: 4px;
        }

        header {
            padding: 80px 20px; text-align: center;
            background: radial-gradient(circle, rgba(7, 76, 161, 0.5) 0%, transparent 70%);
        }

        .logo-main { width: 120px; margin-bottom: 20px; filter: drop-shadow(0 0 20px var(--suwon-blue)); }

        h1 { font-size: 3.5rem; margin: 10px 0; font-weight: 900; letter-spacing: -1px; }
        h1 span { color: var(--suwon-red); }

        .tagline { font-size: 1.2rem; color: var(--suwon-gold); font-weight: 500; margin-top: 15px; }

        section { 
            padding: 60px 20px; 
            max-width: 1400px; 
            margin: 0 auto; 
            display: none;
            animation: fadeIn 0.5s ease-in;
        }
        
        section.active { display: block; }

        @keyframes fadeIn { 
            from { opacity: 0; transform: translateY(20px); } 
            to { opacity: 1; transform: translateY(0); } 
        }

        .section-title {
            font-size: 2.5rem;
            border-left: 10px solid var(--suwon-red);
            padding-left: 20px;
            margin-bottom: 40px;
            color: white;
        }

        /* CARD GRID */
        .card-grid { 
            display: grid; 
            grid-template-columns: repeat(auto-fill, minmax(320px, 1fr)); 
            gap: 25px;
        }

        .card {
            height: 500px; 
            perspective: 1000px; 
            cursor: pointer;
        }

        .card-inner {
            position: relative; 
            width: 100%; 
            height: 100%;
            transition: transform 0.6s cubic-bezier(0.2, 0.8, 0.2, 1.2);
            transform-style: preserve-3d;
        }

        .card.flipped .card-inner { transform: rotateY(180deg); }

        .face {
            position: absolute; 
            width: 100%; 
            height: 100%;
            backface-visibility: hidden; 
            border-radius: 16px;
            overflow: hidden; 
            border: 3px solid var(--suwon-gold);
            box-shadow: 0 8px 25px rgba(7, 76, 161, 0.4), 
                        0 0 30px rgba(200, 16, 46, 0.2);
            background: #000;
        }

        /* CARD FRONT - SHINE EFFECT */
        .front { background: #000; }
        .front::after {
            content: ''; 
            position: absolute; 
            top: -100%; 
            left: -100%; 
            width: 300%; 
            height: 300%;
            background: linear-gradient(45deg, transparent, rgba(255,255,255,0.15), transparent);
            transform: rotate(45deg); 
            transition: 0.5s;
        }
        .card:hover .front::after { 
            top: 100%; 
            left: 100%; 
        }

        .player-img { 
            width: 100%; 
            height: 72%; 
            object-fit: cover;
            background: linear-gradient(135deg, #074CA1, #C8102E);
        }

        .p-info { 
            padding: 15px; 
            background: linear-gradient(to top, #074CA1, #1a0f2e);
            height: 28%;
        }

        .p-pos { 
            color: var(--suwon-gold); 
            font-size: 0.75rem; 
            font-weight: 700;
            letter-spacing: 1px;
        }

        .p-name { 
            font-size: 1.6rem; 
            font-weight: 900;
            margin-top: 5px;
            color: white;
        }

        .p-number {
            font-size: 0.85rem;
            color: rgba(255,255,255,0.7);
            margin-top: 2px;
        }

        /* CARD BACK - DETAIL */
        .back {
            background: linear-gradient(135deg, #074CA1, #C8102E);
            transform: rotateY(180deg); 
            padding: 20px; 
            font-size: 0.9rem;
            overflow-y: auto;
        }

        .back h3 {
            margin-top: 0;
            margin-bottom: 15px;
            font-size: 1.3rem;
            color: var(--suwon-gold);
        }

        .stat-row { 
            display: flex; 
            justify-content: space-between; 
            margin-bottom: 8px; 
            padding-bottom: 6px;
            border-bottom: 1px solid rgba(255,255,255,0.15);
        }

        .stat-label { 
            color: var(--suwon-gold); 
            font-weight: 700;
            font-size: 0.85rem;
        }

        .stat-value {
            color: white;
            font-weight: 500;
        }

        .ability-bar { 
            height: 5px; 
            background: rgba(255,255,255,0.2); 
            margin: 6px 0 12px 0; 
            border-radius: 3px; 
            overflow: hidden;
        }

        .ability-fill { 
            height: 100%; 
            background: linear-gradient(90deg, var(--suwon-gold), #FFD700);
            box-shadow: 0 0 8px var(--suwon-gold);
        }

        /* INFO CARDS */
        .info-card { 
            background: rgba(0,0,0,0.7); 
            padding: 30px; 
            border-radius: 12px; 
            border-left: 5px solid var(--suwon-blue); 
            line-height: 1.8; 
            margin-bottom: 25px;
            backdrop-filter: blur(5px);
        }

        .info-card h2 {
            color: var(--suwon-gold);
            margin-top: 0;
        }

        .info-card p {
            margin: 10px 0;
        }

        blockquote {
            font-style: italic;
            background: rgba(7, 76, 161, 0.15);
            padding: 20px;
            border-left: 4px solid var(--suwon-gold);
            margin: 20px 0;
        }

        .news-item { 
            padding: 18px;
            border-bottom: 1px solid #333; 
            transition: 0.3s;
            background: rgba(7, 76, 161, 0.1);
            margin-bottom: 10px;
            border-radius: 8px;
        }

        .news-item:hover { 
            background: rgba(7, 76, 161, 0.25);
            transform: translateX(5px);
        }

        .news-date {
            color: var(--suwon-gold);
            font-weight: 700;
            font-size: 0.9rem;
        }

        .news-title {
            margin-left: 15px;
            font-weight: 600;
            color: white;
        }

        .map-box { 
            background: rgba(7, 76, 161, 0.2);
            height: 280px; 
            display: flex; 
            align-items: center; 
            justify-content: center; 
            border-radius: 12px; 
            border: 2px solid var(--suwon-gold);
            font-size: 3rem;
        }

        /* RESPONSIVE */
        @media (max-width: 768px) {
            h1 { font-size: 2.5rem; }
            .section-title { font-size: 1.8rem; }
            .card-grid { grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); }
            nav { padding: 10px 0; }
            .nav-item { font-size: 0.9rem; padding: 6px 10px; }
            header { padding: 50px 20px; }
        }

        .sort-buttons {
            display: flex;
            gap: 10px;
            margin-bottom: 30px;
            flex-wrap: wrap;
        }

        .sort-btn {
            padding: 10px 20px;
            background: rgba(7, 76, 161, 0.7);
            color: white;
            border: 2px solid var(--suwon-gold);
            border-radius: 6px;
            cursor: pointer;
            font-weight: 600;
            transition: 0.3s;
        }

        .sort-btn:hover {
            background: var(--suwon-gold);
            color: #000;
        }

        .sort-btn.active {
            background: var(--suwon-gold);
            color: #000;
        }

        .coach-section {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
            margin-bottom: 40px;
        }

        .coach-card {
            background: rgba(7, 76, 161, 0.2);
            padding: 20px;
            border-radius: 12px;
            border: 2px solid var(--suwon-gold);
        }

        .coach-card h3 {
            color: var(--suwon-gold);
            margin-top: 0;
        }

    </style>
</head>
<body>

    <nav>
        <div class="nav-item" onclick="showSection('squad')">📋 선수단</div>
        <div class="nav-item" onclick="showSection('coach')">👨‍💼 코칭스태프</div>
        <div class="nav-item" onclick="showSection('club')">🏟️ 클럽정보</div>
        <div class="nav-item" onclick="showSection('news')">📰 뉴스</div>
        <div class="nav-item" onclick="showSection('map')">📍 위치</div>
    </nav>

    <header>
        <h1>수원 삼성 <span>블루윙즈</span></h1>
        <p class="tagline">🏆 이정효 감독 체제, 2026 K리그1 승격 도전 🏆</p>
    </header>

    <section id="squad" class="active">
        <h2 class="section-title">2026 시즌 선수단</h2>
        
        <div class="sort-buttons">
            <button class="sort-btn active" onclick="sortPlayers('all')">전체 선수</button>
            <button class="sort-btn" onclick="sortPlayers('GK')">골키퍼</button>
            <button class="sort-btn" onclick="sortPlayers('DF')">수비수</button>
            <button class="sort-btn" onclick="sortPlayers('MF')">미드필더</button>
            <button class="sort-btn" onclick="sortPlayers('FW')">공격수</button>
        </div>

        <div class="card-grid" id="playerGrid"></div>
    </section>

    <section id="coach">
        <h2 class="section-title">코칭 스태프</h2>
        
        <div class="coach-section" id="coachGrid"></div>
    </section>

    <section id="club">
        <h2 class="section-title">클럽 정보</h2>
        
        <div class="info-card">
            <h2>수원삼성 블루윙즈</h2>
            <img src="https://images.unsplash.com/photo-1574629810360-7efbbe195018?auto=format&fit=crop&q=80&w=800" style="width:100%; height:300px; object-fit:cover; border-radius:12px; margin-bottom:20px;">
            <p><strong>창단:</strong> 1995년 12월 15일</p>
            <p><strong>현재 감독:</strong> 이정효 (제11대)</p>
            <p><strong>홈구장:</strong> 수원 월드컵 경기장 (빅버드)</p>
            <p><strong>주요 성적:</strong></p>
            <ul>
                <li>K리그1 우승: 4회 (1997, 1998, 1999, 2001)</li>
                <li>FA컵 우승: 5회 (최다)</li>
                <li>AFC 챔피언스리그 우승: 2회 (2001, 2013)</li>
            </ul>
        </div>

        <div class="info-card">
            <h2>이정효 감독 인터뷰 (2026.01.02)</h2>
            <blockquote>
                "나의 축구는 명확하다. 수원은 이제 지지 않는 축구가 아니라, 상대를 압도하는 압박과 정확한 공격을 할 것이다. 팬들이 빅버드에서 전율을 느끼게 만드는 것이 나의 첫 번째 임무다. K리그2 승격은 필수가 아니라 당연한 결과가 되어야 한다."
            </blockquote>
        </div>

        <div class="info-card">
            <h2>2026 시즌 전망</h2>
            <p>
                <strong>이정효 감독 부임과 전폭적 전력 보강:</strong> 제일기획의 직접 지원으로 K리그 역대 최고 연봉의 감독 영입에 성공했으며, 광주 FC에서 함께 했던 코칭스태프 전원을 영입했습니다.
            </p>
            <p>
                <strong>외국인 무제한 보유:</strong> 2026 시즌부터 시행되는 새로운 규정에 따라 전략적 외국인 선수 구성으로 K리그2 다이렉트 승격을 노릴 준비가 완료되었습니다.
            </p>
            <p>
                <strong>승격 구조 개선:</strong> 최대 4팀까지 1부 승격이 가능한 2026 시즌은 수원삼성에게 최적의 기회입니다.
            </p>
        </div>
    </section>

    <section id="news">
        <h2 class="section-title">최신 뉴스</h2>
        <div id="newsGrid"></div>
    </section>

    <section id="map">
        <h2 class="section-title">경기장 및 위치</h2>
        
        <div class="info-card">
            <h3>🏟️ 홈 경기장: 수원 월드컵 경기장 (빅버드)</h3>
            <p><strong>위치:</strong> 경기도 수원시 팔달구 월드컵로 310 (우만동 228번지)</p>
            <p><strong>수용 인원:</strong> 43,959명</p>
            <p><strong>개장:</strong> 2001년 (2002 FIFA 월드컵 한국 경기장)</p>
            <p><strong>특징:</strong> 동·서쪽 관람석의 거대한 날개 모양 지붕이 특징이며, 새가 날개를 펼친 형상을 형상화한 "빅버드"라는 애칭으로 불림</p>
            <p><strong>대중교통:</strong> 신분당선 '수원월드컵경기장역' 인근</p>
            <div class="map-box">📍 경기도 수원시 팔달구 월드컵로 310</div>
        </div>

        <div class="info-card">
            <h3>🏠 클럽하우스: 삼성 트레이닝 센터</h3>
            <p><strong>위치:</strong> 경기도 용인시 기흥구 보정동 (삼성생명 휴먼센터 옆)</p>
            <p><strong>개장:</strong> 2007년 6월 15일</p>
            <p><strong>역할:</strong> 선수 훈련, 재활, 숙소 등 최고 수준의 스포츠 훈련 시설</p>
            <p><strong>특징:</strong> 국내 최초, 최대 규모의 사설 스포츠 훈련소 겸 재활 기관 / 건설비 800억 원 투입</p>
            <p><strong>시설:</strong> 체력 단련실(70종 140여 대 운동기구), 경기 분석실, 스포츠 과학 지원실, 물리치료실</p>
            <div class="map-box">📍 경기도 용인시 기흥구 보정동</div>
        </div>
    </section>

    <script>
        const playerData = [
            // 감독
            { type: 'Coach', name: '이정효', pos: 'HEAD COACH', pos_ko: '감독', number: '-', career: '광주 FC(2023~2025), 강원 FC(2019~2022)', stats: { '경력': '명장', '압박전술': 99, '공격성': 99 }, image: 'data:image/svg+xml,%3Csvg xmlns=%22http://www.w3.org/2000/svg%22 width=%22300%22 height=%22400%22%3E%3Crect fill=%22%23074CA1%22 width=%22300%22 height=%22400%22/%3E%3Ctext x=%2250%25%22 y=%2250%25%22 font-size=%2230%22 fill=%22white%22 text-anchor=%22middle%22 dominant-baseline=%22middle%22%3E이정효%3C/text%3E%3C/svg%3E' },

            // 골키퍼
            { type: 'GK', pos: 'GK', pos_ko: '골키퍼', name: '양형모', number: '21', career: '2019~ 수원삼성', stats: { '나이': 34, '신장': '185cm', '반사신경': 94, '안정감': 95, '킥': 88 } },
            { type: 'GK', pos: 'GK', pos_ko: '골키퍼', name: '김민준', number: '1', career: '2020~ 수원삼성', stats: { '나이': 26, '신장': '187cm', '반사신경': 88, '안정감': 90, '킥': 85 } },
            { type: 'GK', pos: 'GK', pos_ko: '골키퍼', name: '이경준', number: '31', career: '2024~ 수원삼성', stats: { '나이': 18, '신장': '189cm', '반사신경': 82, '안정감': 80, '킥': 79 } },

            // 수비수
            { type: 'DF', pos: 'CB', pos_ko: '센터백', name: '홍정호', number: '5', career: '전북→2026 수원삼성', stats: { '나이': 36, '신장': '186cm', '수비력': 96, '피지컬': 92, '리더십': 98 } },
            { type: 'DF', pos: 'CB', pos_ko: '센터백', name: '송주훈', number: '-', career: '경남→2026 수원삼성(FA)', stats: { '나이': 31, '신장': '190cm', '수비력': 94, '피지컬': 91, '빌드업': 87 } },
            { type: 'DF', pos: 'CB', pos_ko: '센터백', name: '고종현', number: '3', career: '2022~ 수원삼성', stats: { '나이': 17, '신장': '193cm', '수비력': 85, '피지컬': 88, '포지셔닝': 82 } },
            { type: 'DF', pos: 'CB', pos_ko: '센터백', name: '윤근영', number: '-', career: '2026 수원삼성(FA)', stats: { '나이': 20, '신장': '193cm', '수비력': 80, '피지컬': 87, '성장성': 92 } },
            { type: 'DF', pos: 'CB', pos_ko: '센터백', name: '모경빈', number: '-', career: '매탄고→2026 수원삼성', stats: { '나이': 17, '신장': '187cm', '수비력': 75, '피지컬': 85, '포지셔닝': 78 } },
            { type: 'DF', pos: 'CB', pos_ko: '센터백', name: '정성민', number: '-', career: '시흥 임대 중', stats: { '나이': 18, '신장': '189cm', '수비력': 76, '피지컬': 84, '공중볼': 80 } },
            { type: 'DF', pos: 'RB', pos_ko: '우측백', name: '장석환', number: '2', career: '2024~ 수원삼성', stats: { '나이': 19, '신장': '178cm', '수비력': 80, '크로스': 82, '체력': 88 } },
            { type: 'DF', pos: 'RB', pos_ko: '우측백', name: '이준재', number: '-', career: '경남→2026 수원삼성(FA)', stats: { '나이': 20, '신장': '180cm', '수비력': 78, '크로스': 85, '속도': 86 } },
            { type: 'DF', pos: 'LB', pos_ko: '좌측백', name: '최지묵', number: '18', career: '2023~ 수원삼성', stats: { '나이': 25, '신장': '178cm', '수비력': 82, '크로스': 80, '체력': 84 } },
            { type: 'DF', pos: 'LB', pos_ko: '좌측백', name: '박대원', number: '33', career: '2022~ 수원삼성', stats: { '나이': 25, '신장': '178cm', '수비력': 79, '크로스': 78, '침착성': 81 } },
            { type: 'DF', pos: 'LB', pos_ko: '좌측백', name: '이건희', number: '19', career: '2022~ 수원삼성', stats: { '나이': 18, '신장': '174cm', '수비력': 76, '크로스': 75, '성장성': 89 } },

            // 미드필더
            { type: 'MF', pos: 'CM', pos_ko: '중원', name: '박현빈', number: '-', career: '부천→2026 수원삼성', stats: { '나이': 20, '신장': '177cm', '패스': 87, '킬패스': 85, '시야': 88 } },
            { type: 'MF', pos: 'DM', pos_ko: '수비형 미드', name: '페신', number: '-', career: '2026 수원삼성(FA)', stats: { '나이': 25, '신장': '178cm', '수비': 82, '침착성': 86, '킥': 84 } },
            { type: 'MF', pos: 'CM', pos_ko: '중원', name: '홍원진', number: '14', career: '2020~ 수원삼성', stats: { '나이': 25, '신장': '183cm', '패스': 82, '지구력': 88, '리더십': 85 } },
            { type: 'MF', pos: 'CM', pos_ko: '중원', name: '이민혁', number: '17', career: '2019~ 수원삼성', stats: { '나이': 22, '신장': '179cm', '패스': 80, '드리블': 82, '체력': 86 } },
            { type: 'MF', pos: 'CM', pos_ko: '중원', name: '박우진', number: '15', career: '2023~ 수원삼성', stats: { '나이': 20, '신장': '183cm', '패스': 78, '킬패스': 80, '성장성': 88 } },
            { type: 'MF', pos: 'CM', pos_ko: '중원', name: '임지훈', number: '-', career: '2026 수원삼성(신입)', stats: { '나이': 18, '신장': '189cm', '패스': 75, '신체': 86, '성장성': 90 } },
            { type: 'MF', pos: 'CM', pos_ko: '중원', name: '강현묵', number: '10', career: '2021~ 수원삼성', stats: { '나이': 22, '신장': '173cm', '패스': 82, '민첩성': 88, '침착성': 85 } },
            { type: 'MF', pos: 'CM', pos_ko: '중원', name: '김민우', number: '-', career: '울산→2026 수원삼성(임대)', stats: { '나이': 21, '신장': '185cm', '패스': 81, '체력': 87, '킬패스': 83 } },

            // 공격수
            { type: 'FW', pos: 'LW/CAM', pos_ko: '윙어/공격수', name: '헤이스', number: '-', career: '광주 FC→2026 수원삼성', stats: { '나이': 31, '신장': '175cm', '슈팅': 92, '패스': 88, '드리블': 90 } },
            { type: 'FW', pos: 'ST', pos_ko: '스트라이커', name: '일류첸코', number: '9', career: '2021~ 수원삼성', stats: { '나이': 35, '신장': '187cm', '슈팅': 85, '파워': 88, '포스트플레이': 89 } },
            { type: 'FW', pos: 'ST', pos_ko: '스트라이커', name: '김지현', number: '77', career: '2019~ 수원삼성', stats: { '나이': 29, '신장': '183cm', '슈팅': 82, '침착성': 80, '결정력': 84 } },
            { type: 'FW', pos: 'LW', pos_ko: '좌윙', name: '브루노 실바', number: '74', career: '2022~ 수원삼성', stats: { '나이': 23, '신장': '176cm', '슈팅': 80, '드리블': 85, '속도': 86 } },
            { type: 'FW', pos: 'FW', pos_ko: '공격수', name: '강성진', number: '30', career: '2023~ 수원삼성(임대 복귀)', stats: { '나이': 22, '신장': '180cm', '슈팅': 78, '체력': 85, '성장성': 87 } },
            { type: 'FW', pos: 'FW', pos_ko: '공격수', name: '이상민', number: '29', career: '2023~ 수원삼성', stats: { '나이': 21, '신장': '175cm', '슈팅': 75, '속도': 88, '성장성': 89 } },
            { type: 'FW', pos: 'FW', pos_ko: '공격수', name: '김지호', number: '71', career: '2023~ 수원삼성', stats: { '나이': 22, '신장': '173cm', '슈팅': 73, '민첩성': 84, '성장성': 85 } },
            { type: 'FW', pos: 'FW', pos_ko: '공격수', name: '박지원', number: '91', career: '2022~ 수원삼성', stats: { '나이': 23, '신장': '166cm', '슈팅': 74, '속도': 87, '침착성': 78 } }
        ];

        const coachData = [
            { name: '이정효', pos: '감독', career: '광주FC(2022~2025) K리그2 우승·승격(2022년, 2024년)', role: '전술 총괄, 압박 시스템' },
            { name: '마철준', pos: '수석 코치', career: '광주FC(2025)·제주유나이티드·대구FC(2023)·성남FC(2018)', role: '전술 보좌 및 선수 평가' },
            { name: '조용태', pos: '공격 코치', career: '광주FC에서 이정효 감독과 함께 한 공격 전술 담당자', role: '공격 플레이 및 세트피스 설계' },
            { name: '조광수', pos: '골키퍼 코치', career: '울산HD(2024)·제주FC·성남FC(2018)', role: 'GK 전문 훈련 및 선수 개발' },
            { name: '신정환', pos: '골키퍼 코치', career: '광주FC 코칭스태프, 이정효 감독과 동반', role: '골키퍼 피지컬 및 기술' }
        ];

        const newsData = [
            { date: '2026.01.13', title: '헤이스 공식 영입 완료, 오늘부터 팀 훈련 합류' },
            { date: '2026.01.09', title: '김도연 콜업 발표, 2026 시즌 새로운 얼굴' },
            { date: '2026.01.07', title: '이준재·송주훈·페신·박현빈·홍정호·윤근영 완전 영입 발표' },
            { date: '2026.01.02', title: '이정효 감독 공식 취임, 100명 이상의 기자가 참석한 기자회견' },
            { date: '2025.12.24', title: '이정효 감독 제11대 수원 삼성 감독 공식 선임' },
            { date: '2025.12.21', title: '이정효 감독 광주 FC와 계약 해지 선언' }
        ];

        let currentFilter = 'all';

        function renderPlayers() {
            const grid = document.getElementById('playerGrid');
            grid.innerHTML = '';
            
            let filteredPlayers = currentFilter === 'all' ? 
                playerData : 
                playerData.filter(p => p.type === currentFilter);

            filteredPlayers.forEach((p, idx) => {
                let statsHtml = '';
                for (let [key, val] of Object.entries(p.stats)) {
                    const percentage = typeof val === 'number' && val <= 100 ? val : 50;
                    statsHtml += `
                        <div class="stat-row">
                            <span class="stat-label">${key}</span>
                            <span class="stat-value">${val}</span>
                        </div>
                        <div class="ability-bar"><div class="ability-fill" style="width:${percentage}%"></div></div>
                    `;
                }

                grid.innerHTML += `
                    <div class="card" onclick="this.classList.toggle('flipped')">
                        <div class="card-inner">
                            <div class="face front">
                                <svg class="player-img" viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg">
                                    <defs>
                                        <linearGradient id="grad${idx}" x1="0%" y1="0%" x2="100%" y2="100%">
                                            <stop offset="0%" style="stop-color:#074CA1;stop-opacity:1" />
                                            <stop offset="100%" style="stop-color:#C8102E;stop-opacity:1" />
                                        </linearGradient>
                                    </defs>
                                    <rect width="300" height="300" fill="url(#grad${idx})"/>
                                    <circle cx="150" cy="100" r="50" fill="white" opacity="0.8"/>
                                    <text x="150" y="200" font-size="48" fill="white" text-anchor="middle" font-weight="bold">${p.name}</text>
                                </svg>
                                <div class="p-info">
                                    <div class="p-pos">${p.pos_ko}</div>
                                    <div class="p-name">${p.name}</div>
                                    <div class="p-number">#${p.number}</div>
                                </div>
                            </div>
                            <div class="face back">
                                <h3>${p.name} - 능력 분석</h3>
                                <div class="stat-row">
                                    <span class="stat-label">포지션</span>
                                    <span class="stat-value">${p.pos_ko}</span>
                                </div>
                                <div class="stat-row">
                                    <span class="stat-label">경력</span>
                                    <span class="stat-value" style="font-size:0.75rem;">${p.career}</span>
                                </div>
                                <hr style="border: 1px solid rgba(255,255,255,0.2); margin: 12px 0;">
                                ${statsHtml}
                            </div>
                        </div>
                    </div>
                `;
            });
        }

        function renderCoaches() {
            const grid = document.getElementById('coachGrid');
            grid.innerHTML = '';
            
            coachData.forEach(coach => {
                grid.innerHTML += `
                    <div class="coach-card">
                        <h3>${coach.name}</h3>
                        <div class="stat-row">
                            <span class="stat-label">직책</span>
                            <span class="stat-value">${coach.pos}</span>
                        </div>
                        <div class="stat-row">
                            <span class="stat-label">경력</span>
                            <span class="stat-value" style="font-size:0.8rem;">${coach.career}</span>
                        </div>
                        <div class="stat-row">
                            <span class="stat-label">담당</span>
                            <span class="stat-value">${coach.role}</span>
                        </div>
                    </div>
                `;
            });
        }

        function renderNews() {
            const grid = document.getElementById('newsGrid');
            grid.innerHTML = '';
            
            newsData.forEach(news => {
                grid.innerHTML += `
                    <div class="news-item">
                        <span class="news-date">[${news.date}]</span>
                        <span class="news-title">${news.title}</span>
                    </div>
                `;
            });
        }

        function showSection(id) {
            document.querySelectorAll('section').forEach(s => s.classList.remove('active'));
            document.getElementById(id).classList.add('active');
            window.scrollTo(0, 200);
        }

        function sortPlayers(type) {
            currentFilter = type;
            
            document.querySelectorAll('.sort-btn').forEach(btn => btn.classList.remove('active'));
            event.target.classList.add('active');
            
            renderPlayers();
        }

        // 초기 렌더링
        renderPlayers();
        renderCoaches();
        renderNews();
    </script>
</body>
</html>

