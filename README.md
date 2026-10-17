<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>لمسة من مرنونا | Lamsa Min Marnouna</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        body {
            background-color: #fcf6f8;
            color: #4a3b40;
            line-height: 1.6;
        }
        header {
            background-color: #ffffff;
            padding: 15px 40px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 10px rgba(214, 51, 132, 0.08);
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        .logo-container {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        .logo-container img {
            width: 75px;
            height: 75px;
            object-fit: contain;
            border-radius: 50%;
        }
        header h1 {
            color: #b0246b;
            font-size: 26px;
            font-weight: bold;
        }
        nav a {
            text-decoration: none;
            color: #6c5860;
            margin-left: 20px;
            font-weight: 600;
            cursor: pointer;
            transition: 0.2s;
        }
        nav a:hover {
            color: #d63384;
        }
        .hero {
            text-align: center;
            padding: 90px 20px;
            background: linear-gradient(rgba(0,0,0,0.45), rgba(0,0,0,0.45)), url('https://images.unsplash.com/photo-1519225421980-715cb0215aed?auto=format&fit=crop&w=1200&q=80') center/cover;
            color: white;
        }
        .hero h2 {
            font-size: 40px;
            margin-bottom: 15px;
            text-shadow: 2px 2px 6px rgba(0,0,0,0.6);
        }
        .hero p {
            font-size: 18px;
            margin-bottom: 30px;
            text-shadow: 1px 1px 4px rgba(0,0,0,0.6);
        }
        .btn {
            background-color: #d63384;
            color: white;
            padding: 12px 30px;
            border-radius: 25px;
            text-decoration: none;
            font-weight: bold;
            display: inline-block;
            transition: 0.3s;
            box-shadow: 0 4px 12px rgba(214, 51, 132, 0.3);
            border: none;
            cursor: pointer;
        }
        .btn:hover {
            background-color: #b0246b;
        }
        .container {
            max-width: 1100px;
            margin: auto;
            padding: 40px 20px;
        }
        .section-title {
            text-align: center;
            font-size: 32px;
            color: #b0246b;
            margin-bottom: 10px;
        }
        .section-subtitle {
            text-align: center;
            color: #777;
            margin-bottom: 40px;
        }
        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
        }
        .product-card {
            background: white;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            border: 1px solid #fce4ec;
            text-align: right;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }
        .product-card img {
            width: 100%;
            height: 250px;
            object-fit: cover;
        }
        .product-info {
            padding: 20px;
        }
        .product-card h4 {
            font-size: 20px;
            color: #333;
            margin-bottom: 8px;
        }
        .product-card p {
            color: #666;
            font-size: 14px;
            margin-bottom: 15px;
        }
        .price {
            font-weight: bold;
            color: #d63384;
            font-size: 18px;
            display: block;
            margin-bottom: 15px;
        }
        .card-actions {
            padding: 0 20px 20px;
            display: flex;
            flex-direction: column;
            gap: 10px;
        }
        .whatsapp-btn {
            background-color: #25d366;
            color: white;
            padding: 10px;
            border-radius: 20px;
            text-decoration: none;
            font-size: 14px;
            font-weight: bold;
            text-align: center;
            transition: 0.3s;
        }
        .whatsapp-btn:hover {
            background-color: #1ebe57;
        }
        .delete-btn {
            background-color: #dc3545;
            color: white;
            border: none;
            padding: 8px;
            border-radius: 6px;
            cursor: pointer;
            font-size: 13px;
            font-weight: bold;
            display: none;
        }
        .admin-box {
            max-width: 450px;
            margin: 60px auto;
            background: white;
            padding: 35px;
            border-radius: 15px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.08);
            text-align: right;
            display: none;
        }
        .admin-box h3 {
            color: #d63384;
            margin-bottom: 25px;
            text-align: center;
        }
        .form-group {
            margin-bottom: 20px;
        }
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
            color: #444;
        }
        .form-group input, .form-group textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 8px;
            font-size: 15px;
        }
        .contact-section {
            background-color: #fce4ec;
            border-radius: 15px;
            padding: 40px;
            margin: 50px auto;
            max-width: 900px;
            text-align: center;
        }
        .music-bar {
            background: #33292e;
            color: white;
            padding: 12px 20px;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 15px;
            font-size: 14px;
            flex-wrap: wrap;
        }
        footer {
            background-color: #33292e;
            color: white;
            text-align: center;
            padding: 25px;
            margin-top: 50px;
        }
    </style>
</head>
<body>

    <div class="music-bar">
        <span>🎻 استمع إلى موسيقى "From Pain to Peace" أثناء التصفح:</span>
        <audio controls loop style="height: 35px;">
            <source src="song.mp3" type="audio/mpeg">
            متصفحك لا يدعم تشغيل الملفات الصوتية.
        </audio>
    </div>

    <header>
        <div class="logo-container">
            <img src="logo_lamsa_marnona_1.png" alt="لمسة من مرنونا">
            <h1>لمسة من مرنونا</h1>
        </div>
        <nav>
            <a onclick="showSection('home')">الرئيسية</a>
            <a onclick="showSection('products')">المنتجات</a>
            <a onclick="showSection('admin-login')">لوحة التحكم (Admin)</a>
        </nav>
    </header>

    <div id="home-section">
        <section class="hero">
            <h2>أجمل بوكيهات الورد واكسسوارات الأفراح ✨</h2>
            <p>مصنوعة بأعلى جودة وبأدق التفاصيل عشان ليلة العمر تكون أسطورية.</p>
            <a onclick="showSection('products')" class="btn">تصفح المنتجات</a>
        </section>
    </div>

    <div class="container" id="products-section">
        <h3 class="section-title">تشكيلة لمسة من مرنونا المميزة</h3>
        <p class="section-subtitle">اختر اللحظة المناسبة، وسبقنا ننفذهالك بأجمل شكل</p>
        
        <div class="products-grid" id="products-container">
            <!-- المنتجات -->
        </div>
    </div>

    <div class="admin-box" id="admin-login">
        <h3>تسجيل دخول لوحة التحكم</h3>
        <div class="form-group">
            <label>اسم المستخدم</label>
            <input type="text" id="username" placeholder="اكتب اسم المستخدم">
        </div>
        <div class="form-group">
            <label>كلمة المرور</label>
            <input type="password" id="password" placeholder="اكتب كلمة المرور">
        </div>
        <button class="btn" style="width: 100%;" onclick="checkLogin()">دخول</button>
    </div>

    <div class="admin-box" id="admin-panel">
        <h3>إدارة منتجات لمسة من مرنونا 🛠️</h3>
        <div class="form-group">
            <label>اسم المنتج</label>
            <input type="text" id="p-title" placeholder="مثال: بوكيه ورد ملكي">
        </div>
        <div class="form-group">
            <label>وصف المنتج</label>
            <textarea id="p-desc" placeholder="تفاصيل المنتج..."></textarea>
        </div>
        <div class="form-group">
            <label>السعر (خانة واحدة)</label>
            <input type="text" id="p-price" placeholder="مثال: 500 جنيه">
        </div>
        <div class="form-group">
            <label>اختر صورة المنتج من جهازك</label>
            <input type="file" id="p-img-file" accept="image/*">
        </div>
        <button class="btn" style="width: 100%; margin-bottom: 10px;" onclick="addProduct()">إضافة المنتج للموقع</button>
        <button class="btn" style="width: 100%; background-color: #666;" onclick="logoutAdmin()">تسجيل خروج</button>
    </div>

    <div class="contact-section" id="contact">
        <h3>تواصل مع لمسة من مرنونا مباشرة</h3>
        <p>عندك تصميم معين في بالك؟ أو حابب تطلب بوكيه أو اكسسوار بمواصفات خاصة؟ كلمنا فوراً وهنساعدك!</p>
        <br>
        <a href="https://wa.me/201100329703" target="_blank" class="btn">تواصل معنا عبر واتساب</a>
    </div>

    <footer>
        <p>جميع الحقوق محفوظة © 2026 - لمسة من مرنونا (Lamsa Min Marnouna)</p>
    </footer>

    <script>
        let products = JSON.parse(localStorage.getItem('lamsa_marnouna_products')) || [
            {
                title: "بوكيه ورد عروسة فخم",
                desc: "تنسيق راقي من الورد بتصميم مميز لليلة العمر.",
                price: "750 جنيه",
                img: "https://images.unsplash.com/photo-1561181286-d3fee7d55364?auto=format&fit=crop&w=500&q=80"
            },
            {
                title: "طقم اكسسوارات خطوبة وأفراح",
                desc: "تشكيلة أنيقة من الإكسسوارات الخاصة بالعرائس والمناسبات.",
                price: "1200 جنيه",
                img: "https://images.unsplash.com/photo-1535254973040-607b474cb50d?auto=format&fit=crop&w=500&q=80"
            }
        ];

        let isAdmin = localStorage.getItem('lamsa_admin') === 'true';

        function renderProducts() {
            const container = document.getElementById('products-container');
            container.innerHTML = '';
            products.forEach((p, index) => {
                container.innerHTML += `
                    <div class="product-card">
                        <img src="${p.img}" alt="${p.title}">
                        <div class="product-info">
                            <h4>${p.title}</h4>
                            <p>${p.desc}</p>
                            <span class="price">${p.price}</span>
                        </div>
                        <div class="card-actions">
                            <a href="https://wa.me/201100329703?text=مرحباً، مهتم بالاستفسار عن ${p.title}" target="_blank" class="whatsapp-btn">اطلب عبر واتساب</a>
                            <button class="delete-btn" style="display: ${isAdmin ? 'block' : 'none'};" onclick="deleteProduct(${index})">حذف المنتج</button>
                        </div>
                    </div>
                `;
            });
        }

        function showSection(sectionId) {
            document.getElementById('home-section').style.display = 'none';
            document.getElementById('products-section').style.display = 'none';
            document.getElementById('admin-login').style.display = 'none';
            document.getElementById('admin-panel').style.display = 'none';

            if (sectionId === 'home') {
                document.getElementById('home-section').style.display = 'block';
                document.getElementById('products-section').style.display = 'block';
            } else if (sectionId === 'products') {
                document.getElementById('products-section').style.display = 'block';
            } else if (sectionId === 'admin-login') {
                if (isAdmin) {
                    document.getElementById('admin-panel').style.display = 'block';
                } else {
                    document.getElementById('admin-login').style.display = 'block';
                }
            }
        }

        function checkLogin() {
            let user = document.getElementById('username').value;
            let pass = document.getElementById('password').value;

            if (user === 'ميرنا' && pass === '112233') {
                isAdmin = true;
                localStorage.setItem('lamsa_admin', 'true');
                alert('أهلاً بك يا ميرنا في لوحة التحكم الخاصة بلمسة من مرنونا!');
                showSection('admin-login');
                renderProducts();
            } else {
                alert('اسم المستخدم أو كلمة المرور خطأ!');
            }
        }

        function logoutAdmin() {
            isAdmin = false;
            localStorage.setItem('lamsa_admin', 'false');
            alert('تم تسجيل الخروج بنجاح');
            showSection('home');
            renderProducts();
        }

        function addProduct() {
            let title = document.getElementById('p-title').value;
            let desc = document.getElementById('p-desc').value;
            let price = document.getElementById('p-price').value;
            let fileInput = document.getElementById('p-img-file');

            if (!title || !price) {
                alert('من فضلك اكتب اسم المنتج والسعر على الأقل!');
                return;
            }

            if (fileInput.files && fileInput.files[0]) {
                let reader = new FileReader();
                reader.onload = function(e) {
                    let base64Image = e.target.result;
                    
                    products.push({
                        title: title,
                        desc: desc || "تصميم راقي ومميز من لمسة من مرنونا",
                        price: price,
                        img: base64Image
                    });

                    localStorage.setItem('lamsa_marnouna_products', JSON.stringify(products));
                    alert('تم إضافة المنتج بالصورة بنجاح وتحديث الموقع!');
                    
                    document.getElementById('p-title').value = '';
                    document.getElementById('p-desc').value = '';
                    document.getElementById('p-price').value = '';
                    fileInput.value = '';

                    showSection('products');
                    renderProducts();
                }
                reader.readAsDataURL(fileInput.files[0]);
            } else {
                // لو مرفعش صوره، بنحط صورة افتراضية
                products.push({
                    title: title,
                    desc: desc || "تصميم راقي ومميز من لمسة من مرنونا",
                    price: price,
                    img: "https://images.unsplash.com/photo-1513519245088-0e12902e5a38?auto=format&fit=crop&w=500&q=80"
                });

                localStorage.setItem('lamsa_marnouna_products', JSON.stringify(products));
                alert('تم إضافة المنتج بنجاح وتحديث الموقع!');
                
                document.getElementById('p-title').value = '';
                document.getElementById('p-desc').value = '';
                document.getElementById('p-price').value = '';

                showSection('products');
                renderProducts();
            }
        }

        function deleteProduct(index) {
            if (confirm('هل أنت متأكد من حذف هذا المنتج؟')) {
                products.splice(index, 1);
                localStorage.setItem('lamsa_marnouna_products', JSON.stringify(products));
                renderProducts();
            }
        }

        renderProducts();
    </script>
</body>
</html>
