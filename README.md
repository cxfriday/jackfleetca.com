<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jack Transport LLC | Premium Bay Area Travel & Transfers</title>
    <style>
        /* 导入高端英文字体 */
        @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&display=swap');

        /* 全局样式 - 黑金奢华风格 */
        body {
            font-family: 'Helvetica Neue', Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #0a0a0a;
            color: #f5f5f5;
            line-height: 1.8;
        }
        
        h1, h2, h3, .brand-name {
            font-family: 'Playfair Display', Georgia, serif;
            font-weight: 400;
            letter-spacing: 2px;
        }

        /* 导航栏 */
        header {
            background-color: rgba(10, 10, 10, 0.95);
            padding: 1.2rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 100;
            border-bottom: 1px solid #333;
        }
        .brand-name {
            color: #d4af37;
            font-size: 1.8rem;
            margin: 0;
            text-transform: uppercase;
        }
        .nav-links {
            display: flex;
            align-items: center;
        }
        nav a {
            color: #ffffff;
            margin-left: 30px;
            text-decoration: none;
            font-size: 0.9rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: color 0.3s;
        }
        nav a:hover {
            color: #d4af37;
        }
        /* 语言切换按钮样式 */
        .lang-btn {
            background: transparent;
            color: #d4af37;
            border: 1px solid #d4af37;
            padding: 5px 15px;
            margin-left: 30px;
            cursor: pointer;
            font-family: inherit;
            font-size: 0.85rem;
            text-transform: uppercase;
            transition: all 0.3s ease;
        }
        .lang-btn:hover {
            background: #d4af37;
            color: #0a0a0a;
        }

        /* 主视觉区 */
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.8)), url('https://images.unsplash.com/photo-1549317661-bd32c8ce0db2?auto=format&fit=crop&w=1920&q=80') no-repeat center center/cover;
            height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 0 20px;
        }
        .hero h1 {
            font-size: 3.5rem;
            color: #ffffff;
            margin-bottom: 1rem;
            text-transform: uppercase;
        }
        .hero p {
            font-size: 1.2rem;
            color: #cccccc;
            max-width: 800px;
            margin-bottom: 3rem;
            font-weight: 300;
        }
        .btn-gold {
            display: inline-block;
            background-color: transparent;
            color: #d4af37;
            padding: 15px 40px;
            text-decoration: none;
            border: 1px solid #d4af37;
            text-transform: uppercase;
            letter-spacing: 2px;
            transition: all 0.4s ease;
        }
        .btn-gold:hover {
            background-color: #d4af37;
            color: #0a0a0a;
        }

        /* 统一内容容器 */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 6rem 20px;
        }
        .section-title {
            text-align: center;
            color: #d4af37;
            font-size: 2.5rem;
            margin-bottom: 3rem;
        }
        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 2px;
            background-color: #d4af37;
            margin: 20px auto 0;
        }

        /* 业务卡片布局 */
        .services-grid {
            display: flex;
            justify-content: space-between;
            gap: 30px;
            flex-wrap: wrap;
        }
        .service-card {
            background-color: #151515;
            width: 31%;
            box-sizing: border-box;
            transition: transform 0.3s ease;
            border: 1px solid #222;
        }
        .service-card:hover {
            transform: translateY(-10px);
            border-color: #d4af37;
        }
        .service-image {
            width: 100%;
            height: 250px;
            object-fit: cover;
            display: block;
        }
        .service-content {
            padding: 30px;
            text-align: center;
        }
        .service-content h3 {
            color: #ffffff;
            font-size: 1.5rem;
            margin-top: 0;
            margin-bottom: 15px;
        }
        .service-content p {
            color: #999999;
            font-size: 0.95rem;
            margin-bottom: 0;
        }

        /* 车辆展示区 (新增) */
        .fleet-section {
            background-color: #050505;
            padding: 4rem 20px;
            text-align: center;
            border-top: 1px solid #222;
            border-bottom: 1px solid #222;
        }
        .fleet-container {
            max-width: 1000px;
            margin: 0 auto;
            display: flex;
            justify-content: center;
            gap: 40px;
            flex-wrap: wrap;
        }
        .fleet-item {
            width: 45%;
            background: #111;
            padding: 20px;
            border: 1px solid #333;
        }
        .fleet-item h4 {
            color: #d4af37;
            font-size: 1.3rem;
            margin-top: 0;
        }

        /* 底部信息 */
        footer {
            background-color: #050505;
            text-align: center;
            padding: 4rem 20px 2rem;
            color: #777;
        }
        .footer-info {
            margin-bottom: 2rem;
        }
        .footer-info p {
            margin: 5px 0;
            font-size: 1rem;
            color: #aaaaaa;
        }

        /* 响应式适配 */
        @media (max-width: 900px) {
            .service-card {
                width: 48%;
                margin-bottom: 30px;
            }
            .fleet-item {
                width: 100%;
            }
            .nav-links {
                display: none; 
            }
            .lang-btn {
                margin-left: 0;
            }
        }
        @media (max-width: 600px) {
            header {
                flex-direction: column;
                padding: 1rem;
            }
            .brand-name {
                margin-bottom: 15px;
            }
            .service-card {
                width: 100%;
            }
            .hero h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>

    <header>
        <h2 class="brand-name lang-text" data-zh="Jack Transport LLC" data-en="Jack Transport LLC">Jack Transport LLC</h2>
        <nav class="nav-links">
            <a href="#about" class="lang-text" data-zh="品牌简介" data-en="About Us">About Us</a>
            <a href="#services" class="lang-text" data-zh="核心业务" data-en="Our Services">Our Services</a>
            <a href="#fleet" class="lang-text" data-zh="专属车队" data-en="Our Fleet">Our Fleet</a>
            <a href="#contact" class="lang-text" data-zh="预约行程" data-en="Book Now">Book Now</a>
        </nav>
        <button class="lang-btn" id="lang-toggle" onclick="toggleLanguage()">中文</button>
    </header>

    <section class="hero">
        <h1 class="lang-text" data-zh="您的加州全能出行管家" data-en="Your Ultimate California Travel Partner">Your Ultimate California Travel Partner</h1>
        <p class="lang-text" data-zh="从宽敞舒适的 Minivan 包车旅游，到尊贵私密的豪华轿车商务接待。无论您去往何处，我们都以最高标准为您保驾护航。" data-en="From spacious Minivan charters for family tours to luxurious sedans for VIP executive travel. Wherever your destination, we ensure a premium journey tailored to your needs.">From spacious Minivan charters for family tours to luxurious sedans for VIP executive travel. Wherever your destination, we ensure a premium journey tailored to your needs.</p>
        <a href="#contact" class="btn-gold lang-text" data-zh="即刻预约报价" data-en="Get a Quote">Get a Quote</a>
    </section>

    <section id="fleet" class="fleet-section">
        <h2 class="section-title lang-text" data-zh="满足您一切需求的车队" data-en="A Fleet for Every Occasion">A Fleet for Every Occasion</h2>
        <div class="fleet-container">
            <div class="fleet-item">
                <h4 class="lang-text" data-zh="🚐 宽敞 Minivan (家庭与团队)" data-en="🚐 Spacious Minivan (Family & Groups)">🚐 Spacious Minivan (Family & Groups)</h4>
                <p class="lang-text" data-zh="空间宽敞，乘坐舒适。非常适合家庭出游、小团包车观光以及携带大量行李的机场往返。让您的集体出行轻松无忧。" data-en="Roomy and comfortable. Perfect for family vacations, small group sightseeing tours, and airport transfers with extensive luggage. Making group travel effortless.">Roomy and comfortable. Perfect for family vacations, small group sightseeing tours, and airport transfers with extensive luggage. Making group travel effortless.</p>
            </div>
            <div class="fleet-item">
                <h4 class="lang-text" data-zh="🚘 豪华轿车 (商务与 VIP)" data-en="🚘 Premium Sedans (Business & VIP)">🚘 Premium Sedans (Business & VIP)</h4>
                <p class="lang-text" data-zh="为您的高管通勤、重要会议和私人行程提供绝对私密、宁静且极具排面的旗舰座驾体验。配备专业白手套服务标准。" data-en="Providing a completely private, quiet, and prestigious flagship ride for executive commuting, important meetings, and VIP itineraries, complete with white-glove service standards.">Providing a completely private, quiet, and prestigious flagship ride for executive commuting, important meetings, and VIP itineraries, complete with white-glove service standards.</p>
            </div>
        </div>
    </section>

    <section id="services" style="background-color: #0f0f0f;">
        <div class="container">
            <h2 class="section-title lang-text" data-zh="我们的核心业务" data-en="Our Core Services">Our Core Services</h2>
            <div class="services-grid">
                
                <div class="service-card">
                    <img src="https://images.unsplash.com/photo-1501594907352-04cda38ebc29?auto=format&fit=crop&w=800&q=80" alt="Charter Tours" class="service-image">
                    <div class="service-content">
                        <h3 class="lang-text" data-zh="🗺️ 加州包车深度游" data-en="🗺️ California Charter Tours">🗺️ California Charter Tours</h3>
                        <p class="lang-text" data-zh="告别走马观花。搭乘我们的 Minivan，为您和家人定制专属的湾区、一号公路或优胜美地深度游路线，尽享沿途风景。" data-en="Say goodbye to rushed itineraries. Ride in our comfortable Minivans for customized, in-depth tours of the Bay Area, Highway 1, or Yosemite, and truly enjoy the scenery.">Say goodbye to rushed itineraries. Ride in our comfortable Minivans for customized, in-depth tours of the Bay Area, Highway 1, or Yosemite, and truly enjoy the scenery.</p>
                    </div>
                </div>

                <div class="service-card">
                    <img src="https://images.unsplash.com/photo-1436491865332-7a61a109cc05?auto=format&fit=crop&w=800&q=80" alt="Airport Transfer" class="service-image">
                    <div class="service-content">
                        <h3 class="lang-text" data-zh="✈️ 湾区机场接送" data-en="✈️ Bay Area Airport Transfers">✈️ Bay Area Airport Transfers</h3>
                        <p class="lang-text" data-zh="全面覆盖 SFO, SJC, OAK。我们的专职司机将提前守候，协助搬运大件行李。无论是商务出差还是全家旅行，起降皆从容。" data-en="Full coverage of SFO, SJC, and OAK. Our chauffeurs arrive early to assist with heavy luggage, ensuring a smooth departure or arrival for both business and family trips.">Full coverage of SFO, SJC, and OAK. Our chauffeurs arrive early to assist with heavy luggage, ensuring a smooth departure or arrival for both business and family trips.</p>
                    </div>
                </div>

                <div class="service-card">
                    <img src="https://images.unsplash.com/photo-1542282088-fe8426682b8f?auto=format&fit=crop&w=800&q=80" alt="Business Travel" class="service-image">
                    <div class="service-content">
                        <h3 class="lang-text" data-zh="💼 商务专车出行" data-en="💼 VIP Business Travel">💼 VIP Business Travel</h3>
                        <p class="lang-text" data-zh="专为高要求客户打造。乘坐我们的高级轿车，在繁忙的会议间隙享受宁静与高效。准点、安全、体面是我们永恒的承诺。" data-en="Designed for demanding clients. Enjoy tranquility and efficiency between busy meetings in our premium sedans. Punctuality, safety, and prestige are our eternal promises.">Designed for demanding clients. Enjoy tranquility and efficiency between busy meetings in our premium sedans. Punctuality, safety, and prestige are our eternal promises.</p>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <section id="about">
        <div class="container" style="text-align: center; max-width: 800px;">
            <h2 class="section-title lang-text" data-zh="专业牌照，安心首选" data-en="Licensed Professionals, Your Top Choice">Licensed Professionals, Your Top Choice</h2>
            <p class="lang-text" style="font-size: 1.2rem; color: #bbbbbb; font-weight: 300;" data-zh="Jack Transport LLC 是一家持有加州公用事业委员会 (CPUC) 正式营运许可的正规客运公司 (TCP 0050560-P)。立足 Fremont，辐射全加州，我们致力于为您提供合法、安全、高质量的包车与接送服务。选择我们，就是选择了信赖与专业。" data-en="Jack Transport LLC is a fully licensed passenger carrier holding a valid CPUC permit (TCP 0050560-P). Based in Fremont and serving all of California, we are committed to providing legal, safe, and high-quality charter and transfer services. Choosing us means choosing trust and professionalism.">
                Jack Transport LLC is a fully licensed passenger carrier holding a valid CPUC permit (TCP 0050560-P). Based in Fremont and serving all of California, we are committed to providing legal, safe, and high-quality charter and transfer services. Choosing us means choosing trust and professionalism.
            </p>
        </div>
    </section>

    <footer id="contact">
        <div class="container" style="padding: 2rem 20px;">
            <div class="footer-info">
                <h2 class="lang-text" style="color: #ffffff; margin-bottom: 20px;" data-zh="随时准备为您服务" data-en="Ready to Serve You">Ready to Serve You</h2>
                <p class="lang-text" data-zh="服务覆盖: Fremont, CA 及加州大湾区" data-en="Service Area: Fremont, CA and the Greater Bay Area">Service Area: Fremont, CA and the Greater Bay Area</p>
                <p class="lang-text" data-zh="联系电话: 请补充您的电话" data-en="Phone: [Your Phone Number]">Phone: [Your Phone Number]</p>
                <p class="lang-text" data-zh="预约电邮: 请补充您的邮箱" data-en="Email: [Your Email]">Email: [Your Email]</p>
            </div>
            <p class="lang-text" style="font-size: 0.85rem; color: #555; margin-top: 3rem;" data-zh="&copy; 2026 Jack Transport LLC (TCP 0050560-P). 保留所有权利。" data-en="&copy; 2026 Jack Transport LLC (TCP 0050560-P). All Rights Reserved.">&copy; 2026 Jack Transport LLC (TCP 0050560-P). All Rights Reserved.</p>
        </div>
    </footer>

    <script>
        let currentLang = 'en'; // 设定默认语言为英文

        function toggleLanguage() {
            // 切换语言状态
            currentLang = currentLang === 'en' ? 'zh' : 'en';
            
            // 更改按钮文字 (如果当前是英文，按钮显示'中文'；如果当前是中文，按钮显示'English')
            const langBtn = document.getElementById('lang-toggle');
            langBtn.innerText = currentLang === 'en' ? '中文' : 'English';
            
            // 遍历所有带有 lang-text 类的元素，替换对应文本
            const elements = document.querySelectorAll('.lang-text');
            elements.forEach(el => {
                el.innerHTML = el.getAttribute('data-' + currentLang);
            });
        }
    </script>

</body>
</html>
