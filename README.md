<!DOCTYPE html>
<html lang="zh-TW" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>馬煜駿 Peter & 熊郁雯 Wendy 婚禮邀請函</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        morandi: {
                            gold: '#d4a373',
                            sage: '#8da399',
                            bg: '#FAF8F5',
                            card: '#FFFFFF',
                            text: '#333333',
                            muted: '#7A7A7A',
                            border: '#E8E2D9'
                        }
                    },
                    fontFamily: {
                        garamond: ['"Cormorant Garamond"', 'serif'],
                        serifTC: ['"Noto Serif TC"', 'serif'],
                    }
                }
            }
        }
    </script>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,600;0,700;1,400&family=Noto+Serif+TC:wght@300;400;600;700&display=swap" rel="stylesheet">
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        body {
            font-family: 'Noto Serif TC', serif;
            background-color: #FAF8F5;
            color: #333333;
            overflow-x: hidden;
        }

        /* 1. 頂端毛玻璃質感導覽列 */
        .glass-nav {
            background: rgba(250, 248, 245, 0.75);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border-bottom: 1px solid rgba(212, 163, 115, 0.15);
        }

        /* 2. 倒數計時器白色微光卡片與柔和陰影 */
        .glow-card {
            background: #ffffff;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05), 0 2px 10px rgba(212, 163, 115, 0.08);
            border: 1px solid rgba(255, 255, 255, 0.8);
            position: relative;
        }
        .glow-card::after {
            content: '';
            position: absolute;
            top: 0; left: 0; right: 0; bottom: 0;
            border-radius: inherit;
            pointer-events: none;
            box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.9);
        }

        /* 6. 手機版視覺優化：強制 key words 不自動斷行跑版 */
        .no-wrap {
            white-space: nowrap !important;
            word-break: keep-all !important;
        }

        /* 淡入視覺效果 */
        .fade-in-up {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.8s ease-out, transform 0.8s ease-out;
        }
        .fade-in-up.visible {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body class="antialiased selection:bg-morandi-gold/20 selection:text-morandi-gold">

    <!-- 1. 頂端固定毛玻璃質感導航列 -->
    <header class="fixed top-0 left-0 right-0 z-50 glass-nav transition-all duration-300">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            <a href="#" class="font-garamond text-2xl font-bold tracking-widest text-morandi-gold">P & W</a>
            
            <nav class="hidden md:flex space-x-8 text-sm tracking-wider font-medium">
                <a href="#about" class="hover:text-morandi-gold transition-colors duration-200">關於我們 <span class="font-garamond text-xs text-morandi-sage block text-center">About</span></a>
                <a href="#details" class="hover:text-morandi-gold transition-colors duration-200">婚禮詳情 <span class="font-garamond text-xs text-morandi-sage block text-center">Details</span></a>
                <a href="#rsvp" class="hover:text-morandi-gold transition-colors duration-200">出席回函 <span class="font-garamond text-xs text-morandi-sage block text-center">RSVP</span></a>
            </nav>

            <!-- 手機選單按鈕 -->
            <button id="mobile-menu-btn" class="md:hidden text-morandi-text p-2 focus:outline-none" aria-label="Toggle Menu">
                <i class="fa-solid fa-bars text-xl"></i>
            </button>
        </div>

        <!-- 手機版下拉菜單 -->
        <div id="mobile-menu" class="hidden md:hidden glass-nav border-t border-morandi-border px-6 py-4 space-y-4 text-center">
            <a href="#about" class="mobile-link block text-sm tracking-wider hover:text-morandi-gold">關於我們 About</a>
            <a href="#details" class="mobile-link block text-sm tracking-wider hover:text-morandi-gold">婚禮詳情 Details</a>
            <a href="#rsvp" class="mobile-link block text-sm tracking-wider hover:text-morandi-gold">出席回函 RSVP</a>
        </div>
    </header>

    <!-- 3. 全螢幕封面背景 Hero Section -->
    <section class="relative h-screen w-full flex items-center justify-center overflow-hidden">
        <!-- 封面背景圖片 -->
        <div class="absolute inset-0 bg-cover bg-center bg-no-repeat transform scale-105 transition-transform duration-1000"
             style="background-image: url('https://i.postimg.cc/rF3zfVJ6/IMG-4802.jpg');">
            <!-- 優雅漸層遮罩 -->
            <div class="absolute inset-0 bg-gradient-to-b from-black/40 via-black/20 to-black/60"></div>
        </div>

        <!-- 封面文字資訊 -->
        <div class="relative z-10 text-center text-white px-4 max-w-3xl mx-auto space-y-6">
            <p class="font-garamond tracking-widest text-lg sm:text-xl uppercase text-amber-100/90 font-light">We Are Getting Married</p>
            <h1 class="font-serifTC text-3xl sm:text-5xl lg:text-6xl font-light tracking-wide leading-tight">
                馬煜駿 <span class="font-garamond italic text-morandi-gold font-normal">Peter</span>
                <span class="inline-block mx-2 text-2xl font-light text-amber-200/80">&</span>
                熊郁雯 <span class="font-garamond italic text-morandi-gold font-normal">Wendy</span>
            </h1>
            <div class="w-16 h-[1px] bg-amber-200/60 mx-auto my-4"></div>
            <p class="font-serifTC text-lg sm:text-xl font-light tracking-widest text-slate-100">
                <span class="font-medium text-amber-100">馬熊聯姻</span>
            </p>
            <p class="font-garamond text-sm sm:text-base tracking-widest text-slate-200 pt-2">
                2027 . 04 . 10 — SATURDAY 19:00
            </p>
            <div class="pt-8">
                <a href="#rsvp" class="inline-block px-8 py-3 rounded-full border border-white/60 bg-white/10 backdrop-blur-md text-white font-serifTC text-sm tracking-widest hover:bg-white hover:text-morandi-text transition-all duration-300 shadow-lg hover:shadow-xl">
                    出席回函 RSVP
                </a>
            </div>
        </div>

        <!-- 向下捲動引導 -->
        <a href="#about" class="absolute bottom-8 left-1/2 -translate-x-1/2 z-10 text-white/80 hover:text-white transition-colors animate-bounce">
            <i class="fa-solid fa-angle-down text-2xl"></i>
        </a>
    </section>

    <!-- 2. 藝術感倒數計時器專區 -->
    <section id="countdown-section" class="py-16 sm:py-24 bg-morandi-bg px-4">
        <div class="max-w-4xl mx-auto text-center fade-in-up">
            <p class="font-garamond text-morandi-gold text-lg tracking-widest uppercase mb-2">Countdown to Our Special Day</p>
            <h2 class="font-serifTC text-2xl sm:text-3xl text-morandi-text font-normal tracking-wider mb-10">婚禮倒數計時</h2>

            <!-- 獨立白色微光卡片，搭配柔和陰影與優雅垂直細線分隔 -->
            <div class="flex items-center justify-center space-x-2 sm:space-x-4 max-w-2xl mx-auto">
                <!-- 天數 DAYS -->
                <div class="glow-card flex-1 p-3 sm:p-6 rounded-2xl text-center">
                    <span id="cd-days" class="font-garamond text-3xl sm:text-5xl font-bold text-morandi-gold block leading-none">00</span>
                    <span class="font-garamond text-[10px] sm:text-xs tracking-widest text-morandi-sage uppercase mt-2 block">Days</span>
                    <span class="font-serifTC text-[10px] text-morandi-muted block">天</span>
                </div>

                <!-- 垂直細線分隔 -->
                <div class="h-12 sm:h-16 w-[1px] bg-morandi-gold/30"></div>

                <!-- 時 HOURS -->
                <div class="glow-card flex-1 p-3 sm:p-6 rounded-2xl text-center">
                    <span id="cd-hours" class="font-garamond text-3xl sm:text-5xl font-bold text-morandi-gold block leading-none">00</span>
                    <span class="font-garamond text-[10px] sm:text-xs tracking-widest text-morandi-sage uppercase mt-2 block">Hours</span>
                    <span class="font-serifTC text-[10px] text-morandi-muted block">時</span>
                </div>

                <!-- 垂直細線分隔 -->
                <div class="h-12 sm:h-16 w-[1px] bg-morandi-gold/30"></div>

                <!-- 分 MINUTES -->
                <div class="glow-card flex-1 p-3 sm:p-6 rounded-2xl text-center">
                    <span id="cd-minutes" class="font-garamond text-3xl sm:text-5xl font-bold text-morandi-gold block leading-none">00</span>
                    <span class="font-garamond text-[10px] sm:text-xs tracking-widest text-morandi-sage uppercase mt-2 block">Mins</span>
                    <span class="font-serifTC text-[10px] text-morandi-muted block">分</span>
                </div>

                <!-- 垂直細線分隔 -->
                <div class="h-12 sm:h-16 w-[1px] bg-morandi-gold/30"></div>

                <!-- 秒 SECONDS -->
                <div class="glow-card flex-1 p-3 sm:p-6 rounded-2xl text-center">
                    <span id="cd-seconds" class="font-garamond text-3xl sm:text-5xl font-bold text-morandi-gold block leading-none">00</span>
                    <span class="font-garamond text-[10px] sm:text-xs tracking-widest text-morandi-sage uppercase mt-2 block">Secs</span>
                    <span class="font-serifTC text-[10px] text-morandi-muted block">秒</span>
                </div>
            </div>
        </div>
    </section>

    <!-- 關於我們 ABOUT -->
    <section id="about" class="py-16 sm:py-24 bg-white px-4">
        <div class="max-w-3xl mx-auto text-center space-y-6 fade-in-up">
            <p class="font-garamond text-morandi-gold text-lg tracking-widest uppercase">About Us</p>
            <h2 class="font-serifTC text-2xl sm:text-3xl text-morandi-text font-normal tracking-wider">關於我們</h2>
            <div class="w-12 h-[1px] bg-morandi-gold/50 mx-auto my-4"></div>
            <p class="font-serifTC text-morandi-text leading-relaxed text-base sm:text-lg font-light max-w-2xl mx-auto">
                誠摯邀請您見證我們的幸福時刻。<br>
                在這個充滿愛與溫暖的日子裡，期待與最珍惜的親朋好友共享這份喜悅與浪漫。
            </p>
            <div class="pt-4 flex justify-center space-x-6 text-morandi-sage">
                <i class="fa-solid fa-heart text-morandi-gold text-sm"></i>
                <i class="fa-solid fa-ring text-morandi-gold text-sm"></i>
                <i class="fa-solid fa-heart text-morandi-gold text-sm"></i>
            </div>
        </div>
    </section>

    <!-- 3. 婚禮詳情：垂直 V-Card 設計 -->
    <section id="details" class="py-16 sm:py-24 bg-morandi-bg px-4">
        <div class="max-w-4xl mx-auto fade-in-up">
            <div class="text-center mb-12">
                <p class="font-garamond text-morandi-gold text-lg tracking-widest uppercase">Wedding Details</p>
                <h2 class="font-serifTC text-2xl sm:text-3xl text-morandi-text font-normal tracking-wider">婚禮資訊</h2>
            </div>

            <!-- 垂直 V-Card 設計三欄位 -->
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6 sm:gap-8">
                <!-- 時間卡片 -->
                <div class="bg-white p-8 rounded-2xl shadow-sm border border-morandi-border/60 text-center hover:shadow-md transition-shadow">
                    <div class="w-12 h-12 rounded-full bg-morandi-gold/10 text-morandi-gold flex items-center justify-center mx-auto mb-4">
                        <i class="fa-regular fa-calendar-check text-xl"></i>
                    </div>
                    <h3 class="font-serifTC font-semibold text-lg text-morandi-text mb-2">日期與時間</h3>
                    <p class="font-serifTC text-sm text-morandi-muted leading-relaxed">
                        116年 (2027年) 4月10日<br>
                        <span class="font-garamond text-morandi-gold font-bold">19:00</span> 晚宴開始
                    </p>
                </div>

                <!-- 地點卡片 (套用 no-wrap 保護關鍵地點) -->
                <div class="bg-white p-8 rounded-2xl shadow-sm border border-morandi-border/60 text-center hover:shadow-md transition-shadow">
                    <div class="w-12 h-12 rounded-full bg-morandi-sage/10 text-morandi-sage flex items-center justify-center mx-auto mb-4">
                        <i class="fa-solid fa-location-dot text-xl"></i>
                    </div>
                    <h3 class="font-serifTC font-semibold text-lg text-morandi-text mb-2">宴客地點</h3>
                    <p class="font-serifTC text-sm text-morandi-muted leading-relaxed">
                        <span class="no-wrap font-medium text-morandi-text">青青食尚花園會館</span><br>
                        <span class="no-wrap text-xs">台北市士林區至善路2段266巷32號</span>
                    </p>
                </div>

                <!-- Dress Code 卡片 -->
                <div class="bg-white p-8 rounded-2xl shadow-sm border border-morandi-border/60 text-center hover:shadow-md transition-shadow">
                    <div class="w-12 h-12 rounded-full bg-morandi-gold/10 text-morandi-gold flex items-center justify-center mx-auto mb-4">
                        <i class="fa-solid fa-user-tie text-xl"></i>
                    </div>
                    <h3 class="font-serifTC font-semibold text-lg text-morandi-text mb-2">著裝建議</h3>
                    <p class="font-serifTC text-sm text-morandi-muted leading-relaxed">
                        Dress Code<br>
                        <span class="text-morandi-gold font-medium">請正裝出席</span>
                    </p>
                </div>
            </div>

            <!-- 7. & 6. 交通指引：隱藏式摺疊面板 (Accordion) 且包含 no-wrap 技術處理 -->
            <div class="mt-12 bg-white rounded-2xl shadow-sm border border-morandi-border/60 overflow-hidden">
                <button id="accordion-toggle" class="w-full px-6 py-5 text-left flex justify-between items-center bg-white hover:bg-morandi-bg/50 transition-colors focus:outline-none">
                    <span class="font-serifTC font-medium text-morandi-text flex items-center">
                        <i class="fa-solid fa-compass text-morandi-gold mr-3"></i>
                        交通指引與位置指南 Transportation Guide
                    </span>
                    <i id="accordion-icon" class="fa-solid fa-chevron-down text-morandi-sage transition-transform duration-300"></i>
                </button>

                <div id="accordion-content" class="hidden px-6 py-6 border-t border-morandi-border/40 bg-morandi-bg/20 text-sm text-morandi-text space-y-4">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                        <!-- 大眾運輸 -->
                        <div class="space-y-2">
                            <h4 class="font-semibold text-morandi-gold flex items-center">
                                <i class="fa-solid fa-bus mr-2"></i>捷運與公車
                            </h4>
                            <p class="text-morandi-muted leading-relaxed">
                                搭乘捷運至 <span class="no-wrap font-medium text-morandi-text">捷運士林站</span> 1號出口，轉乘公車 <span class="no-wrap font-medium text-morandi-text">255</span>、<span class="no-wrap font-medium text-morandi-text">304</span> 或 <span class="no-wrap font-medium text-morandi-text">小18</span> 至 <span class="no-wrap font-medium text-morandi-text">故宮博物院站</span> 下車，步行約 3-5 分鐘即可抵達 <span class="no-wrap font-medium text-morandi-text">青青食尚花園會館</span>。
                            </p>
                        </div>

                        <!-- 自行開車 -->
                        <div class="space-y-2">
                            <h4 class="font-semibold text-morandi-gold flex items-center">
                                <i class="fa-solid fa-car mr-2"></i>自行開車 / 停車資訊
                            </h4>
                            <p class="text-morandi-muted leading-relaxed">
                                導航設定至 <span class="no-wrap font-medium text-morandi-text">台北市士林區至善路2段266巷32號</span>。會館備有專屬賓客停車場，提供免費停車服務。
                            </p>
                        </div>
                    </div>

                    <!-- 地圖連結 -->
                    <div class="pt-4 text-center border-t border-morandi-border/30">
                        <a href="https://maps.google.com/?q=青青食尚花園會館" target="_blank" rel="noopener noreferrer" 
                           class="inline-flex items-center text-xs font-serifTC text-morandi-gold hover:underline">
                            <i class="fa-solid fa-map-location-dot mr-1.5"></i> 開啟 Google 地圖導航
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 4. & 5. & 8. 出席回函 RSVP：中英雙語標籤、隱藏 Iframe 技術、智能動態顯示 -->
    <section id="rsvp" class="py-16 sm:py-24 bg-white px-4">
        <div class="max-w-2xl mx-auto fade-in-up">
            <div class="text-center mb-10">
                <p class="font-garamond text-morandi-gold text-lg tracking-widest uppercase">Rsvp Form</p>
                <h2 class="font-serifTC text-2xl sm:text-3xl text-morandi-text font-normal tracking-wider">出席回函</h2>
                <p class="text-xs text-morandi-muted mt-2 font-serifTC">請於婚禮前協助填寫回函，方便我們為您安排座位與餐點</p>
            </div>

            <!-- 5. 隱藏式 Iframe 提交技術 Target (防止頁面跳轉) -->
            <iframe name="hidden_iframe" id="hidden_iframe" style="display:none;" onload="if(submitted){showSuccessModal();}"></iframe>

            <!-- Google Form 提交表單（僅提取 entry ID，預設值為空） -->
            <form action="https://docs.google.com/forms/d/e/1FAIpQLSefXUTyeD55QE6mZVYw6f85dy--i3LtTU8Bik51ifR5HMtUmA/formResponse" 
                  method="POST" 
                  target="hidden_iframe" 
                  id="wedding-rsvp-form"
                  class="space-y-6 bg-morandi-bg/40 p-6 sm:p-10 rounded-2xl border border-morandi-border/60 shadow-sm">

                <!-- 4. 中英雙語標籤：姓名 NAME -->
                <div>
                    <label class="block font-serifTC text-sm font-medium text-morandi-text mb-1">
                        姓名 <span class="font-garamond text-xs text-morandi-sage uppercase">NAME</span> <span class="text-rose-400">*</span>
                    </label>
                    <input type="text" 
                           name="entry.1028388764" 
                           required 
                           value="" 
                           placeholder="請輸入您的姓名"
                           class="w-full px-4 py-3 rounded-lg border border-morandi-border bg-white text-morandi-text focus:outline-none focus:ring-2 focus:ring-morandi-gold/50 text-sm">
                </div>

                <!-- 4. 中英雙語標籤：電子郵件 EMAIL -->
                <div>
                    <label class="block font-serifTC text-sm font-medium text-morandi-text mb-1">
                        電子郵件 <span class="font-garamond text-xs text-morandi-sage uppercase">EMAIL</span> <span class="text-rose-400">*</span>
                    </label>
                    <input type="email" 
                           name="entry.1399570734" 
                           required 
                           value="" 
                           placeholder="example@mail.com"
                           class="w-full px-4 py-3 rounded-lg border border-morandi-border bg-white text-morandi-text focus:outline-none focus:ring-2 focus:ring-morandi-gold/50 text-sm">
                </div>

                <!-- 4. 中英雙語標籤：與新人的關係 RELATIONSHIP (下拉選單為純中文) -->
                <div>
                    <label class="block font-serifTC text-sm font-medium text-morandi-text mb-1">
                        與新人的關係 <span class="font-garamond text-xs text-morandi-sage uppercase">RELATIONSHIP</span> <span class="text-rose-400">*</span>
                    </label>
                    <select name="entry.214106935" 
                            required 
                            class="w-full px-4 py-3 rounded-lg border border-morandi-border bg-white text-morandi-text focus:outline-none focus:ring-2 focus:ring-morandi-gold/50 text-sm">
                        <option value="" disabled selected>請選擇關係</option>
                        <option value="男方好友">男方好友</option>
                        <option value="女方好友">女方好友</option>
                        <option value="男方親戚">男方親戚</option>
                        <option value="女方親戚">女方親戚</option>
                    </select>
                </div>

                <!-- 4. 中英雙語標籤：參加人數 ATTENDANCE -->
                <div>
                    <label class="block font-serifTC text-sm font-medium text-morandi-text mb-1">
                        參加晚宴人數 <span class="font-garamond text-xs text-morandi-sage uppercase">ATTENDANCE</span> <span class="text-rose-400">*</span>
                    </label>
                    <input type="number" 
                           id="attendance-input"
                           name="entry.375192929" 
                           min="0" 
                           max="10" 
                           required 
                           value="" 
                           placeholder="若無法出席請填 0"
                           class="w-full px-4 py-3 rounded-lg border border-morandi-border bg-white text-morandi-text focus:outline-none focus:ring-2 focus:ring-morandi-gold/50 text-sm">
                </div>

                <!-- 8. 智能表單邏輯區塊：只有在『參加晚宴人數』大於 0 時才顯示 -->
                <div id="dynamic-rsvp-fields" class="space-y-6 hidden border-t border-morandi-border/60 pt-6">
                    <!-- 飲食需求 DIETARY (下拉選單為純中文) -->
                    <div>
                        <label class="block font-serifTC text-sm font-medium text-morandi-text mb-1">
                            飲食需求 <span class="font-garamond text-xs text-morandi-sage uppercase">DIETARY</span>
                        </label>
                        <select name="entry.1454076875" 
                                class="w-full px-4 py-3 rounded-lg border border-morandi-border bg-white text-morandi-text focus:outline-none focus:ring-2 focus:ring-morandi-gold/50 text-sm">
                            <option value="葷食" selected>葷食</option>
                            <option value="全素">全素</option>
                            <option value="蛋奶素">蛋奶素</option>
                        </select>
                    </div>

                    <!-- 兒童座椅 BABY CHAIR (下拉選單為純中文) -->
                    <div>
                        <label class="block font-serifTC text-sm font-medium text-morandi-text mb-1">
                            是否需要兒童椅 <span class="font-garamond text-xs text-morandi-sage uppercase">BABY CHAIR</span>
                        </label>
                        <select name="entry.2104263428" 
                                class="w-full px-4 py-3 rounded-lg border border-morandi-border bg-white text-morandi-text focus:outline-none focus:ring-2 focus:ring-morandi-gold/50 text-sm">
                            <option value="不需要" selected>不需要</option>
                            <option value="需要">需要</option>
                        </select>
                    </div>
                </div>

                <!-- 備註 NOTE -->
                <div>
                    <label class="block font-serifTC text-sm font-medium text-morandi-text mb-1">
                        給新人的祝福與備註 <span class="font-garamond text-xs text-morandi-sage uppercase">NOTE</span>
                    </label>
                    <textarea name="entry.2014287893" 
                              rows="3" 
                              placeholder="請寫下您想對 Peter & Wendy 說的話..."
                              class="w-full px-4 py-3 rounded-lg border border-morandi-border bg-white text-morandi-text focus:outline-none focus:ring-2 focus:ring-morandi-gold/50 text-sm"></textarea>
                </div>

                <!-- 提交按鈕 -->
                <div class="pt-2">
                    <button type="submit" 
                            class="w-full py-3.5 px-6 rounded-full bg-morandi-gold hover:bg-[#c39262] text-white font-serifTC text-sm tracking-widest shadow-md hover:shadow-lg transition-all duration-300">
                        確認送出 SUBMIT
                    </button>
                </div>
            </form>
        </div>
    </section>

    <!-- 頁尾 Footer -->
    <footer class="py-8 bg-morandi-bg text-center text-xs text-morandi-muted border-t border-morandi-border/40 font-garamond tracking-widest">
        <p>© 2027 PETER & WENDY'S WEDDING. ALL RIGHTS RESERVED.</p>
    </footer>

    <!-- 提交成功提示 Modal -->
    <div id="success-modal" class="fixed inset-0 z-50 flex items-center justify-center bg-black/50 backdrop-blur-sm hidden px-4">
        <div class="bg-white rounded-2xl p-8 max-w-sm w-full text-center space-y-4 shadow-2xl border border-morandi-border transform transition-all">
            <div class="w-14 h-14 bg-morandi-gold/10 text-morandi-gold rounded-full flex items-center justify-center mx-auto text-2xl">
                <i class="fa-solid fa-heart"></i>
            </div>
            <h3 class="font-serifTC text-xl font-medium text-morandi-text">完成回函填寫</h3>
            <p class="font-serifTC text-sm text-morandi-muted leading-relaxed">
                非常感謝您的回覆！<br>Peter & Wendy 期待在婚禮當天與您相見。
            </p>
            <button onclick="closeSuccessModal()" class="w-full py-2.5 bg-morandi-gold text-white rounded-full text-xs font-serifTC tracking-wider hover:bg-[#c39262] transition-colors">
                關閉視窗
            </button>
        </div>
    </div>

    <!-- JavaScript 互動邏輯 -->
    <script>
        // 全域變數追蹤表單提交狀態
        var submitted = false;

        // 1. 手機版選單開關
        const mobileBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        const mobileLinks = document.querySelectorAll('.mobile-link');

        mobileBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        mobileLinks.forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });

        // 2. 婚禮藝術倒數計時器 Logic (目標日期：116年/2027年4月10日 19:00:00)
        const targetDate = new Date('2027-04-10T19:00:00').getTime();

        function updateCountdown() {
            const now = new Date().getTime();
            const distance = targetDate - now;

            if (distance < 0) {
                document.getElementById('cd-days').innerText = "00";
                document.getElementById('cd-hours').innerText = "00";
                document.getElementById('cd-minutes').innerText = "00";
                document.getElementById('cd-seconds').innerText = "00";
                return;
            }

            const days = Math.floor(distance / (1000 * 60 * 60 * 24));
            const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((distance % (1000 * 60)) / 1000);

            document.getElementById('cd-days').innerText = days < 10 ? '0' + days : days;
            document.getElementById('cd-hours').innerText = hours < 10 ? '0' + hours : hours;
            document.getElementById('cd-minutes').innerText = minutes < 10 ? '0' + minutes : minutes;
            document.getElementById('cd-seconds').innerText = seconds < 10 ? '0' + seconds : seconds;
        }

        setInterval(updateCountdown, 1000);
        updateCountdown();

        // 7. Accordion 交通資訊摺疊面板開關
        const accordionToggle = document.getElementById('accordion-toggle');
        const accordionContent = document.getElementById('accordion-content');
        const accordionIcon = document.getElementById('accordion-icon');

        accordionToggle.addEventListener('click', () => {
            accordionContent.classList.toggle('hidden');
            accordionIcon.classList.toggle('rotate-180');
        });

        // 8. 智能表單動態邏輯：只有在『參加人數』 > 0 時才展開飲食與座椅選項
        const attendanceInput = document.getElementById('attendance-input');
        const dynamicFields = document.getElementById('dynamic-rsvp-fields');

        attendanceInput.addEventListener('input', function() {
            const val = parseInt(this.value, 10);
            if (!isNaN(val) && val > 0) {
                dynamicFields.classList.remove('hidden');
            } else {
                dynamicFields.classList.add('hidden');
            }
        });

        // 5. 表單提交狀態與彈窗邏輯
        const rsvpForm = document.getElementById('wedding-rsvp-form');
        rsvpForm.addEventListener('submit', function() {
            submitted = true;
        });

        function showSuccessModal() {
            document.getElementById('success-modal').classList.remove('hidden');
            rsvpForm.reset();
            dynamicFields.classList.add('hidden');
            submitted = false;
        }

        function closeSuccessModal() {
            document.getElementById('success-modal').classList.add('hidden');
        }

        // 頁面捲動淡入動畫
        const observerOptions = { threshold: 0.1 };
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.fade-in-up').forEach(el => {
            observer.observe(el);
        });
    </script>
</body>
</html>
