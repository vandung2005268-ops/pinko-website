# pinko-website
<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Pinko</title>

  <!-- GOOGLE FONT -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:'Poppins',sans-serif;
    }

    body{
      background:#111;
      color:white;
    }

    /* HEADER */
    header{
      background:#000;
      padding:15px 7%;
      display:flex;
      justify-content:space-between;
      align-items:center;
      position:sticky;
      top:0;
      z-index:1000;
      border-bottom:1px solid #ff4fa3;
    }

    .logo{
      font-size:28px;
      font-weight:700;
      color:#ff4fa3;
    }

    nav{
      display:flex;
      gap:25px;
    }

    nav a{
      color:white;
      text-decoration:none;
      transition:0.3s;
      font-weight:500;
    }

    nav a:hover{
      color:#ff4fa3;
    }

    .btn{
      background:#ff4fa3;
      color:white;
      padding:10px 18px;
      border:none;
      border-radius:30px;
      cursor:pointer;
      transition:0.3s;
      font-weight:600;
    }

    .btn:hover{
      background:#ff2f8d;
      transform:scale(1.05);
    }

    /* HERO */
    .hero{
      min-height:90vh;
      display:flex;
      justify-content:space-between;
      align-items:center;
      padding:50px 7%;
      flex-wrap:wrap;
      gap:40px;
    }

    .hero-text{
      flex:1;
      min-width:300px;
    }

    .hero-text h1{
      font-size:60px;
      line-height:1.2;
      margin-bottom:20px;
    }

    .hero-text span{
      color:#ff4fa3;
    }

    .hero-text p{
      color:#ccc;
      margin-bottom:30px;
      line-height:1.8;
    }

    .hero-image{
      flex:1;
      text-align:center;
      min-width:300px;
    }

    .hero-image img{
      width:90%;
      max-width:500px;
      border-radius:30px;
      box-shadow:0 0 30px rgba(255,79,163,0.4);
    }

    /* SECTION */
    section{
      padding:80px 7%;
    }

    .title{
      text-align:center;
      margin-bottom:50px;
    }

    .title h2{
      font-size:40px;
      color:#ff4fa3;
    }

    .products{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
      gap:30px;
    }

    .card{
      background:#1b1b1b;
      border-radius:20px;
      overflow:hidden;
      transition:0.3s;
      border:1px solid #2d2d2d;
    }

    .card:hover{
      transform:translateY(-10px);
      border-color:#ff4fa3;
    }

    .card img{
      width:100%;
      height:260px;
      object-fit:cover;
    }

    .card-content{
      padding:20px;
    }

    .card-content h3{
      margin-bottom:10px;
      font-size:22px;
    }

    .price{
      color:#ff4fa3;
      font-size:24px;
      font-weight:700;
      margin-bottom:15px;
    }

    .card-content p{
      color:#bbb;
      margin-bottom:20px;
      line-height:1.6;
    }

    /* ABOUT */
    .about{
      display:flex;
      gap:40px;
      align-items:center;
      flex-wrap:wrap;
    }

    .about img{
      width:100%;
      max-width:500px;
      border-radius:20px;
    }

    .about-text{
      flex:1;
      min-width:300px;
    }

    .about-text h2{
      color:#ff4fa3;
      margin-bottom:20px;
      font-size:40px;
    }

    .about-text p{
      line-height:1.9;
      color:#ccc;
    }

    /* CONTACT */
    .contact{
      text-align:center;
      background:#181818;
      border-radius:20px;
      padding:50px;
    }

    .contact h2{
      color:#ff4fa3;
      margin-bottom:20px;
      font-size:40px;
    }

    .contact p{
      color:#ccc;
      margin-bottom:15px;
    }

    footer{
      text-align:center;
      padding:30px;
      background:#000;
      border-top:1px solid #222;
      color:#888;
    }

    /* MOBILE */
    @media(max-width:768px){

      .hero-text h1{
        font-size:40px;
      }

      nav{
        display:none;
      }

      .hero{
        text-align:center;
      }

    }
  </style>
</head>

<body>

  <!-- HEADER -->
  <header>

    <div class="logo">
      Pink Moon Tea
    </div>

    <nav>
      <a href="#">Trang Chủ</a>
      <a href="#menu">Menu</a>
      <a href="#about">Giới Thiệu</a>
      <a href="#contact">Liên Hệ</a>
    </nav>

    <button class="btn">
      Đặt Hàng
    </button>

  </header>

  <!-- HERO -->
  <section class="hero">

    <div class="hero-text">

      <h1>
        Trà Sữa <span>Ngon</span>
        Cho Giới Trẻ
      </h1>

      <p>
        Không chỉ là trà sữa — đây là phong cách sống.
        Hương vị đậm chất Hàn Quốc với tone màu hồng đen hiện đại,
        trẻ trung và sang trọng.
      </p>

      <button class="btn">
        Xem Menu
      </button>

    </div>

    <div class="hero-image">

      <img src="https://images.unsplash.com/photo-1558857563-b371033873b8?q=80&w=1200" alt="Trà sữa">

    </div>

  </section>

  <!-- PRODUCTS -->
  <section id="menu">

    <div class="title">
      <h2>Best Seller</h2>
    </div>

    <div class="products">

      <!-- ITEM -->
      <div class="card">

        <img src="https://images.unsplash.com/photo-1525385133512-2f3bdd039054?q=80&w=1200">

        <div class="card-content">

          <h3>Trà Sữa Matcha</h3>

          <div class="price">
            49.000đ
          </div>

          <p>
            Matcha thơm béo kết hợp trân châu đường đen cực ngon.
          </p>

          <button class="btn">
            Mua Ngay
          </button>

        </div>

      </div>

      <!-- ITEM -->
      <div class="card">

        <img src="https://images.unsplash.com/photo-1515823064-d6e0c04616a7?q=80&w=1200">

        <div class="card-content">

          <h3>Trà Sữa bá vương </h3>

          <div class="price">
            45.000đ
          </div>

          <p>
            Vị dâu ngọt dịu kết hợp kem cheese béo mịn.
          </p>

          <button class="btn">
            Mua Ngay
          </button>

        </div>

      </div>

      <!-- ITEM -->
      <div class="card">

        <img src="https://images.unsplash.com/photo-1509042239860-f550ce710b93?q=80&w=1200">

        <div class="card-content">

          <h3>Trà Sữa Socola</h3>

          <div class="price">
            45.000đ
          </div>

          <p>
            Socola đậm vị dành cho tín đồ thích ngọt và béo.
          </p>

          <button class="btn">
            Mua Ngay
          </button>

        </div>

      </div>

    </div>

  </section>

  <!-- ABOUT -->
  <section id="about">

    <div class="about">

      <img src="https://images.unsplash.com/photo-1495474472287-4d71bcdd2085?q=80&w=1200">

      <div class="about-text">

        <h2>Về Chúng Tôi</h2>

        <p>
          PinkO là thương hiệu trà sữa mang phong cách hiện đại,
          trẻ trung với tone màu hồng đen đặc trưng.
          Chúng tôi tập trung vào trải nghiệm khách hàng,
          thiết kế không gian đẹp và đồ uống chất lượng cao.
        </p>

      </div>

    </div>

  </section>

  <!-- CONTACT -->
  <section id="contact">

    <div class="contact">

      <h2>Liên Hệ</h2>

      <p>📍 Trần Nguyên Hãn
      , Bắc Giang </p>

      <p>📞 0346564318</p>


      <button class="btn">
        Đặt Bàn Ngay
      </button>

    </div>

  </section>

  <!-- FOOTER -->
  <footer>
    © 2026 Pinko- All Rights Reserved
  </footer>

</body>
</html>
