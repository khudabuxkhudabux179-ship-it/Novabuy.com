<!DOCTYPE html>
<html lang="ur">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PUBG UC Shop - پاکستان | UC فروخت</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        :root {
            --pubg-orange: #FF8C00;
            --pubg-dark: #1a1a1a;
            --pubg-light: #f8f9fa;
        }
        
        body {
            background-color: #f5f5f5;
            color: #333;
            direction: rtl;
        }
        
        /* ہیڈر سٹائل */
        header {
            background: linear-gradient(135deg, var(--pubg-dark) 0%, #333 100%);
            color: white;
            padding: 1rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
        }
        
        .logo {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        
        .logo h1 {
            font-size: 1.8rem;
            color: var(--pubg-orange);
        }
        
        .logo span {
            font-size: 1rem;
            color: #ccc;
        }
        
        nav ul {
            display: flex;
            list-style: none;
            gap: 30px;
        }
        
        nav a {
            color: white;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s;
            font-size: 1.1rem;
        }
        
        nav a:hover {
            color: var(--pubg-orange);
        }
        
        /* ہیرو سیکشن */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.8), rgba(0,0,0,0.8)), 
                        url('https://images.unsplash.com/photo-1550745165-9bc0b252726f?auto=format&fit=crop&w=1350');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 100px 20px;
            margin-bottom: 50px;
        }
        
        .hero h2 {
            font-size: 3rem;
            margin-bottom: 20px;
            color: var(--pubg-orange);
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 30px;
            line-height: 1.6;
        }
        
        .cta-button {
            background-color: var(--pubg-orange);
            color: white;
            padding: 15px 40px;
            border: none;
            border-radius: 50px;
            font-size: 1.2rem;
            font-weight: bold;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
            display: inline-block;
            text-decoration: none;
        }
        
        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(255,140,0,0.3);
        }
        
        /* UC پیکیجز */
        .packages {
            padding: 50px 5%;
            max-width: 1400px;
            margin: 0 auto;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
            color: var(--pubg-dark);
        }
        
        .section-title h2 {
            font-size: 2.5rem;
            color: var(--pubg-orange);
            margin-bottom: 15px;
        }
        
        .section-title p {
            font-size: 1.1rem;
            color: #666;
        }
        
        .package-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-bottom: 60px;
        }
        
        .package-card {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.08);
            transition: transform 0.3s, box-shadow 0.3s;
            border: 2px solid #eee;
        }
        
        .package-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
            border-color: var(--pubg-orange);
        }
        
        .package-header {
            background: linear-gradient(135deg, var(--pubg-dark) 0%, #444 100%);
            color: white;
            padding: 25px;
            text-align: center;
        }
        
        .package-amount {
            font-size: 2.5rem;
            font-weight: bold;
            color: var(--pubg-orange);
            margin-bottom: 10px;
        }
        
        .package-price {
            font-size: 2rem;
            font-weight: bold;
            color: white;
        }
        
        .package-body {
            padding: 25px;
        }
        
        .package-features {
            list-style: none;
            margin-bottom: 25px;
        }
        
        .package-features li {
            padding: 10px 0;
            border-bottom: 1px solid #eee;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .buy-btn {
            width: 100%;
            padding: 15px;
            background: linear-gradient(135deg, var(--pubg-orange) 0%, #FFA500 100%);
            color: white;
            border: none;
            border-radius: 10px;
            font-size: 1.1rem;
            font-weight: bold;
            cursor: pointer;
            transition: opacity 0.3s;
        }
        
        .buy-btn:hover {
            opacity: 0.9;
        }
        
        /* ادائیگی طریقے */
        .payment-methods {
            background-color: white;
            padding: 40px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.05);
            margin-bottom: 50px;
        }
        
        .payment-icons {
            display: flex;
            justify-content: center;
            gap: 30px;
            flex-wrap: wrap;
            margin-top: 30px;
        }
        
        .payment-icon {
            background-color: #f8f9fa;
            padding: 20px;
            border-radius: 10px;
            width: 120px;
            text-align: center;
            transition: transform 0.3s;
        }
        
        .payment-icon:hover {
            transform: scale(1.05);
        }
        
        /* فوٹر */
        footer {
            background-color: var(--pubg-dark);
            color: white;
            padding: 60px 5% 30px;
            margin-top: 80px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }
        
        .footer-column h3 {
            color: var(--pubg-orange);
            margin-bottom: 25px;
            font-size: 1.3rem;
        }
        
        .footer-column ul {
            list-style: none;
        }
        
        .footer-column ul li {
            margin-bottom: 15px;
        }
        
        .footer-column ul li a {
            color: #ccc;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-column ul li a:hover {
            color: var(--pubg-orange);
        }
        
        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid #444;
            color: #aaa;
            font-size: 0.9rem;
        }
        
        /* رسپانسیو ڈیزائن */
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                gap: 20px;
                text-align: center;
            }
            
            nav ul {
                flex-wrap: wrap;
                justify-content: center;
                gap: 20px;
            }
            
            .hero h2 {
                font-size: 2rem;
            }
            
            .section-title h2 {
                font-size: 2rem;
            }
            
            .package-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- ہیڈر -->
    <header>
        <div class="logo">
            <h1>🔥 PUBG UC Shop</h1>
            <span>پاکستان کا معتبر UC سٹور</span>
        </div>
        <nav>
            <ul>
                <li><a href="#home">ہوم</a></li>
                <li><a href="#packages">پیکیجز</a></li>
                <li><a href="#how-to">خریدیں کیسے</a></li>
                <li><a href="#contact">رابطہ</a></li>
            </ul>
        </nav>
    </header>

    <!-- ہیرو سیکشن -->
    <section class="hero" id="home">
        <h2>PUBG UC خریدیں پاکستان سے</h2>
        <p>تیز ترین ڈیلیوری، کم ترین قیمتیں، اور 100% محفوظ ادائیگی۔ ہمارے ہزاروں گاہک ہمارے ساتھ مطمئن ہیں۔</p>
        <a href="#packages" class="cta-button">ابھی UC خریدیں</a>
    </section>

    <!-- UC پیکیجز -->
    <section class="packages" id="packages">
        <div class="section-title">
            <h2>UC پیکیجز</h2>
            <p>اپنی پسند کا UC پیکیج منتخب کریں</p>
        </div>
        
        <div class="package-grid">
            <!-- پیکیج 1 -->
            <div class="package-card">
                <div class="package-header">
                    <div class="package-amount">60 UC</div>
                    <div class="package-price">روپے 200</div>
                </div>
                <div class="package-body">
                    <ul class="package-features">
                        <li>✅ فوری ڈیلیوری (5 منٹ)</li>
                        <li>✅ 100% سیف</li>
                        <li>✅ 24/7 سپورٹ</li>
                        <li>✅ PUBG Mobile</li>
                    </ul>
                    <button class="buy-btn">ابھی خریدیں</button>
                </div>
            </div>

            <!-- پیکیج 2 -->
            <div class="package-card">
                <div class="package-header">
                    <div class="package-amount">325 UC</div>
                    <div class="package-price">روپے 1,000</div>
                </div>
                <div class="package-body">
                    <ul class="package-features">
                        <li>✅ فوری ڈیلیوری (10 منٹ)</li>
                        <li>✅ 100% سیف</li>
                        <li>✅ 24/7 سپورٹ</li>
                        <li>✅ سب سے مشہور پیکیج</li>
                    </ul>
                    <button class="buy-btn">ابھی خریدیں</button>
                </div>
            </div>

            <!-- پیکیج 3 -->
            <div class="package-card">
                <div class="package-header">
                    <div class="package-amount">660 UC</div>
                    <div class="package-price">روپے 2,000</div>
                </div>
                <div class="package-body">
                    <ul class="package-features">
                        <li>✅ فوری ڈیلیوری (15 منٹ)</li>
                        <li>✅ 100% سیف</li>
                        <li>✅ 24/7 سپورٹ</li>
                        <li>✅ بہترین ویلیو</li>
                    </ul>
                    <button class="buy-btn">ابھی خریدیں</button>
                </div>
            </div>
        </div>

        <!-- ادائیگی طریقے -->
        <div class="payment-methods">
            <div class="section-title">
                <h2>ادائیگی کے طریقے</h2>
                <p>محفوظ اور آسان ادائیگی کے آپشنز</p>
            </div>
            <div class="payment-icons">
                <div class="payment-icon">💳 JazzCash</div>
                <div class="payment-icon">📱 EasyPaisa</div>
                <div class="payment-icon">🏦 بینک ٹرانسفر</div>
                <div class="payment-icon">🛡️ PayPal</div>
            </div>
        </div>
    </section>

    <!-- فوٹر -->
    <footer id="contact">
        <div class="footer-content">
            <div class="footer-column">
                <h3>ہمارے بارے میں</h3>
                <p>PUBG UC Shop پاکستان کا نمبر 1 UC فراہم کنندہ ہے۔ تیز ترین سروس اور صارفین کی تسلی ہماری پہچان ہے۔</p>
            </div>
            <div class="footer-column">
                <h3>تیز لنکس</h3>
                <ul>
                    <li><a href="#home">ہوم</a></li>
                    <li><a href="#packages">پیکیجز</a></li>
                    <li><a href="#how-to">خریدیں کیسے</a></li>
                    <li><a href="#contact">رابطہ</a></li>
                </ul>
            </div>
            <div class="footer-column">
                <h3>رابطہ کریں</h3>
                <ul>
                    <li>📞: 0300-1234567</li>
                    <li>📧: info@pubgucshop.pk</li>
                    <li>📍: لاہور، پاکستان</li>
                    <li>⏰: 24 گھنٹے</li>
                </ul>
            </div>
        </div>
        <div class="copyright">
            <p>© 2024 PUBG UC Shop - پاکستان. تمام حقوق محفوظ ہیں۔</p>
            <p style="margin-top: 10px; font-size: 0.8rem;">یہ سائٹ PUBG Mobile کے ساتھ وابستہ نہیں ہے۔</p>
        </div>
    </footer>

    <!-- جاوا اسکرپٹ -->
    <script>
        // خریدنے کے بٹن کے لیے
        document.querySelectorAll('.buy-btn').forEach(button => {
            button.addEventListener('click', function() {
                const packageCard = this.closest('.package-card');
                const amount = packageCard.querySelector('.package-amount').textContent;
                const price = packageCard.querySelector('.package-price').textContent;
                
                alert(`شکریہ! آپ نے ${amount} پیکیج (${price}) منتخب کیا ہے۔\n\nادائیگی کی معلومات آپکو واٹس ایپ پر بھیج دی جائیں گی۔`);
            });
        });

        // نیویگیشن سموتھ سکرول
        document.querySelectorAll('nav a').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                const targetSection = document.querySelector(targetId);
                
                window.scrollTo({
                    top: targetSection.offsetTop - 80,
                    behavior: 'smooth'
                });
            });
        });

        // CTA بٹن کے لیے
        document.querySelector('.cta-button').addEventListener('click', function(e) {
            e.preventDefault();
            document.querySelector('#packages').scrollIntoView({
                behavior: 'smooth'
            });
        });

        // چھوٹا اینیمیشن
        window.addEventListener('load', () => {
            document.querySelector('.hero').style.opacity = '0';
            document.querySelector('.hero').style.transform = 'translateY(20px)';
            
            setTimeout(() => {
                document.querySelector('.hero').style.transition = 'opacity 1s, transform 1s';
                document.querySelector('.hero').style.opacity = '1';
                document.querySelector('.hero').style.transform = 'translateY(0)';
            }, 300);
        });
    </script>
</body>
</html>
