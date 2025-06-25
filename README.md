<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>周童装饰 - 您的理想家居设计专家</title>
    <style>
        * {margin:0;padding:0;box-sizing:border-box;}
        body {font-family:-apple-system,BlinkMacSystemFont,'Segoe UI','Microsoft YaHei',sans-serif;line-height:1.6;color:#333;background:#f4f5f7;}
        .container {max-width:1200px;margin:0 auto;padding:0 20px;}
        nav {background:#222c38;color:#fff;padding:1rem 0;position:fixed;width:100%;top:0;z-index:1000;box-shadow:0 2px 10px rgba(0,0,0,0.06);}
        nav .container {display:flex;justify-content:space-between;align-items:center;}
        .logo {font-size:1.7rem;font-weight:bold;letter-spacing:2px;}
        .nav-links {display:flex;list-style:none;gap:2rem;}
        .nav-links a {color:#fff;text-decoration:none;transition:color 0.3s;}
        .nav-links a:hover {color:#70b7ff;}
        .hero-bg {
            position: fixed; left:0; top:0; width:100vw; height:100vh; z-index:-1;
            background:linear-gradient(120deg,#5b86e5 0%,#36d1c4 100%);
        }
        .hero-canvas {position:absolute;left:0;top:0;width:100vw;height:100vh;z-index:0;}
        .hero {
            position:relative;
            min-height:60vh;
            display:flex;
            align-items:center;
            justify-content:center;
            flex-direction:column;
            text-align:center;
            color:#fff;
            padding:200px 0 120px;
            margin-top:60px;
        }
        .hero-content {
            background:rgba(30,40,60,0.48);
            border-radius:1.5rem;
            box-shadow:0 8px 40px 0 rgba(0,0,0,0.13);
            display:inline-block;
            padding:2.5rem 3rem 2rem 3rem;
            backdrop-filter:blur(2px);
        }
        .hero h1 {font-size:3.2rem;letter-spacing:1px;margin-bottom:1.2rem;font-weight:600;}
        .hero p {font-size:1.28rem;letter-spacing:1px;margin-bottom:2.2rem;}
        .cta-button {
            display:inline-block;background:#e74c3c;color:#fff;
            padding:14px 38px;font-size:1.08rem;
            text-decoration:none;border-radius:2rem;
            box-shadow:0 2px 18px rgba(231,76,60,0.15);
            transition:background 0.18s,transform 0.12s;
        }
        .cta-button:hover {background:#c0392b;transform:scale(1.05);}
        .services,.portfolio {padding:80px 0;}
        .section-title {text-align:center;font-size:2.5rem;margin-bottom:3rem;color:#274472;}
        .services-grid {
            display:grid;
            grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
            gap:2.5rem;
        }
        .service-card {
            background:#fff;padding:2.5rem 1.2rem;border-radius:1rem;
            box-shadow:0 2px 18px rgba(52,152,219,0.09);
            text-align:center;transition:transform 0.23s;
            border:1px solid #e9eef5;
        }
        .service-card:hover {transform:translateY(-6px) scale(1.03);}
        .service-icon {font-size:3rem;margin-bottom:1rem;}
        .service-card h3 {margin-bottom:1.3rem;color:#274472;font-size:1.25rem;}
        .portfolio-grid {
            display:grid;grid-template-columns:repeat(auto-fit,minmax(350px,1fr));
            gap:2rem;
        }
        .portfolio-item {
            position:relative;overflow:hidden;border-radius:1rem;
            box-shadow:0 4px 16px rgba(34,44,56,0.09);
        }
        .portfolio-item img {
            width:100%;height:280px;object-fit:cover;transition:transform 0.3s;
        }
        .portfolio-item:hover img {transform:scale(1.10);}
        .portfolio-overlay {
            position:absolute;bottom:0;left:0;right:0;
            background:linear-gradient(to top,rgba(0,0,0,0.85),transparent 75%);
            color:#fff;padding:1.7rem 2rem 2rem 1.7rem;
            transform:translateY(100%);transition:transform 0.3s;
        }
        .portfolio-item:hover .portfolio-overlay {transform:translateY(0);}
        .contact {background:#213043;color:#fff;padding:80px 0;}
        .contact-content {
            display:grid;grid-template-columns:repeat(auto-fit,minmax(320px,1fr));gap:3rem;
        }
        .contact-info h3 {margin-bottom:1.1rem;color:#48c6ef;}
        .contact-info p {margin-bottom:0.55rem;}
        footer {background:#1a252f;color:#fff;text-align:center;padding:2rem 0;}
        @media (max-width: 768px) {
            .nav-links {display:none;}
            .hero h1 {font-size:2.1rem;}
            .hero p {font-size:1rem;}
            .hero-content {padding:1.2rem;}
        }
    </style>
</head>
<body>
    <div class="hero-bg"></div>
    <canvas class="hero-canvas"></canvas>
    <nav>
        <div class="container">
            <div class="logo">周童装潢设计服务部</div>
            <ul class="nav-links">
                <li><a href="#home">首页</a></li>
                <li><a href="#services">服务项目</a></li>
                <li><a href="#portfolio">作品展示</a></li>
                <li><a href="#contact">联系我们</a></li>
            </ul>
        </div>
    </nav>
    <section class="hero" id="home">
        <div class="container">
            <div class="hero-content">
                <h1>打造您的理想家居空间</h1>
                <p>专业设计团队 | 精湛施工工艺 | 一站式装修服务</p>
                <a href="#contact" class="cta-button">立即咨询</a>
            </div>
        </div>
    </section>
    <section class="services" id="services">
        <div class="container">
            <h2 class="section-title">我们的服务</h2>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">🏠</div>
                    <h3>室内设计</h3>
                    <p>专业设计师团队，为您量身定制独特的室内设计方案，打造舒适美观的居住空间。</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🔨</div>
                    <h3>施工装修</h3>
                    <p>经验丰富的施工团队，严格把控质量，确保每一个细节都达到完美标准。</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🛋️</div>
                    <h3>软装搭配</h3>
                    <p>精选优质家具和装饰品，专业软装设计师为您搭配出和谐统一的居家环境。</p>
                </div>
            </div>
        </div>
    </section>
    <section class="portfolio" id="portfolio">
        <div class="container">
            <h2 class="section-title">精选案例</h2>
            <div class="portfolio-grid">
                <div class="portfolio-item">
                    <img src="https://picsum.photos/400/300?random=1" alt="现代简约客厅">
                    <div class="portfolio-overlay">
                        <h3>现代简约风格</h3>
                        <p>120㎡三室两厅，打造简洁大气的现代居住空间</p>
                    </div>
                </div>
                <div class="portfolio-item">
                    <img src="https://picsum.photos/400/300?random=2" alt="北欧风格卧室">
                    <div class="portfolio-overlay">
                        <h3>北欧风格</h3>
                        <p>90㎡两室一厅，营造温馨舒适的北欧风情</p>
                    </div>
                </div>
                <div class="portfolio-item">
                    <img src="https://picsum.photos/400/300?random=3" alt="新中式餐厅">
                    <div class="portfolio-overlay">
                        <h3>新中式风格</h3>
                        <p>150㎡四室两厅，融合传统与现代的东方美学</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <section class="contact" id="contact">
        <div class="container">
            <h2 class="section-title" style="color: white;">联系我们</h2>
            <div class="contact-content">
                <div class="contact-info">
                    <h3>公司信息</h3>
                    <p>📍 地址：江山市江电路16-5号周童装饰运营中心</p>
                    <p>📞 电话：13857007256</p>
                    <p>📧 邮箱：1113683543@qq.com</p>
                </div>
                <div class="contact-info">
                    <h3>营业时间</h3>
                    <p>周一至周五：9:00 - 18:00</p>
                    <p>周六至周日：10:00 - 17:00</p>
                    <p>节假日请提前预约</p>
                </div>
                <div class="contact-info">
                    <h3>关注我们</h3>
                    <p>微信公众号：周童装饰</p>
                    <p>官方网站：www.zhoutongzhuangshi.com</p>
                    <p>获取最新设计灵感和优惠信息</p>
                </div>
            </div>
        </div>
    </section>
    <footer>
        <div class="container">
            <p>&copy; 2024 周童装饰 版权所有 | 京ICP备88888888号</p>
        </div>
    </footer>
    <script>
        // 导航栏滚动渐变
        window.addEventListener('scroll', function() {
            const nav = document.querySelector('nav');
            if (window.scrollY > 100) {
                nav.style.background = 'rgba(44, 62, 80, 0.95)';
            } else {
                nav.style.background = '#222c38';
            }
        });
        // 平滑滚动
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
        // 英文首页动态背景（粒子流）
        const canvas = document.querySelector('.hero-canvas');
        if(canvas){
            let w = window.innerWidth, h = window.innerHeight;
            canvas.width = w;
            canvas.height = h;
            const ctx = canvas.getContext('2d');
            let particles = [];
            let num = Math.floor(w/28);
            for(let i=0;i<num;i++){
                particles.push({
                    x: Math.random()*w,
                    y: Math.random()*h*0.6,
                    r: 1.6+Math.random()*1.7,
                    alpha: 0.12+Math.random()*0.18,
                    dx: (Math.random()-0.5)*0.6,
                    dy: 0.15+Math.random()*0.6
                });
            }
            function draw(){
                ctx.clearRect(0,0,w,h);
                for(let p of particles){
                    ctx.save();
                    ctx.globalAlpha = p.alpha;
                    ctx.beginPath();
                    ctx.arc(p.x,p.y,p.r,0,2*Math.PI);
                    ctx.fillStyle = '#fff';
                    ctx.shadowColor = '#fff';
                    ctx.shadowBlur = 7;
                    ctx.fill();
                    ctx.restore();
                    p.x += p.dx;
                    p.y += p.dy;
                    if(p.x<0||p.x>w) p.x = Math.random()*w;
                    if(p.y>h*0.7){p.y=0;p.x=Math.random()*w;}
                }
                requestAnimationFrame(draw);
            }
            draw();
            window.addEventListener('resize',()=>{
                w=window.innerWidth;h=window.innerHeight;
                canvas.width=w;canvas.height=h;
            });
        }
    </script>
</body>
</html>
g
