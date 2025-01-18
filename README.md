
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>صفحة مع رابط إنستجرام وصورة خلفية</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      height: 100vh;
      font-family: Arial, sans-serif;
      text-align: center;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      position: relative;
      transition: background-image 0.3s;
    }

    h1 {
      color: #fff;
    }

    .buttons-container {
      margin-top: 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
      z-index: 2;
    }

    .button {
      display: block;
      background-color: #094e00;
      color: #fff;
      border: none;
      width: 150px;
      height: 60px;
      margin: 10px 0;
      border-radius: 30px;
      font-size: 1rem;
      cursor: pointer;
      transition: background-color 0.3s, transform 0.2s;
    }

    .button:hover {
      background-color: #005700;
      transform: translateY(-5px) scale(1.05);
    }

    .gallery {
      display: none;
      flex-wrap: wrap;
      justify-content: center;
      align-items: center;
      background-color: #f0f0f0;
      width: 100%;
      height: 100%;
      position: absolute;
      top: 0;
      left: 0;
      overflow-y: auto;
      padding: 20px;
    }

    .image-container {
      margin: 10px;
    }

    .image-container img {
      width: 200px;
      height: auto;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      transition: transform 0.3s;
    }

    .image-container img:hover {
      transform: scale(1.1);
    }

    /* الغلاف */
    .cover-image {
      width: 100%;
      height: 100vh;
      object-fit: cover;
      position: absolute;
      top: 0;
      left: 0;
      z-index: 1;
    }

    /* الغلاف العازل الشفاف */
    .separator {
      width: 100%;
      height: 20px;
      background-color: rgba(0, 0, 0, 0.3); /* غلاف شفاف باللون الأسود */
      margin: 20px 0; /* التباعد */
    }

    /* استجابة للأجهزة الصغيرة */
    @media (max-width: 768px) {
      .button {
        width: 120px;
        height: 50px;
        font-size: 0.9rem;
      }

      .cover-image {
        height: 70vh; /* تقليل حجم الصورة في الأجهزة الصغيرة */
      }

      .image-container img {
        width: 150px; /* تصغير الصور في الأجهزة الصغيرة */
      }
    }

    /* استجابة للأجهزة الصغيرة جدًا مثل الهواتف */
    @media (max-width: 480px) {
      .button {
        width: 100px;
        height: 40px;
        font-size: 0.8rem;
      }

      .cover-image {
        height: 60vh; /* تقليل الحجم بشكل أكبر */
      }

      .image-container img {
        width: 130px; /* تقليل حجم الصور بشكل أكبر */
      }
    }
  </style>
</head>
<body>
  <!-- الغلاف -->
  <img src="/Users/mohamedahmed/Downloads/468476951_17902973115077430_8737714600511989503_n.jpg" class="cover-image" id="coverImage">

  <!-- الغلاف العازل الشفاف -->
  <div class="separator"></div>

  <div class="buttons-container">
    <a href="https://www.instagram.com/octa_cafe?utm_source=ig_web_button_share_sheet&igsh=ZDNlZDc0MzIxNw==" target="_blank">
      <button class="button">instagram</button>
    </a>
    <a href="https://l.instagram.com/?u=https%3A%2F%2Fwww.facebook.com%2Fprofile.php%3Fid%3D61550585673502%26mibextid%3DLQQJ4d&e=AT390MXtsyi6MtUFimz8oD7NgglfrROHBq1z7Ve2Oa7SCK5NFVtYXiQToex37wGg2I9aXe_J3vnmHjTFCCDy1o1y0hsjDbGM" target="_blank">
      <button class="button">facebook</button>
    </a>
    <button class="button" onclick="showGallery()">menu</button>
    <a href="https://l.instagram.com/?u=https%3A%2F%2Fmaps.app.goo.gl%2FqcjWLGviLjfsLmSXA%3Fg_st%3Diw&e=AT0jaJp4vaTCEAALi9b9QsPhtuJ5okngNucVRK90KCC2iu3cHFG9OwmEdxfqqZZC9d-m06yz3vnmHjTFCCDy1o1y0hsjDbGM" target="_blank">
      <button class="button">location</button>
    </a>
  </div>

  <!-- معرض الصور -->
  <div class="gallery" id="gallery">
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.09.06 AM.png" alt="صورة 1"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.08.20 AM.png" alt="صورة 2"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.09.48 AM.png" alt="صورة 3"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.10.03 AM.png" alt="صورة 4"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.10.32 AM.png" alt="صورة 5"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.10.52 AM.png" alt="صورة 6"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.11.18 AM.png" alt="صورة 7"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.11.35 AM.png" alt="صورة 8"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.11.50 AM.png" alt="صورة 9"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.12.08 AM.png" alt="صورة 10"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.12.25 AM.png" alt="صورة 11"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.12.37 AM.png" alt="صورة 12"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.12.52 AM.png" alt="صورة 13"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.13.07 AM.png" alt="صورة 14"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.13.26 AM.png" alt="صورة 15"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.13.39 AM.png" alt="صورة 16"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.13.55 AM.png" alt="صورة 17"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.14.09 AM.png" alt="صورة 18"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.14.24 AM.png" alt="صورة 19"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.14.42 AM.png" alt="صورة 20"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.15.01 AM.png" alt="صورة 21"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.15.18 AM.png" alt="صورة 22"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.15.32 AM.png" alt="صورة 23"></div>
    <div class="image-container"><img src="/Users/mohamedahmed/Desktop/Screenshot 2025-01-19 at 12.15.45 AM.png" alt="صورة 24"></div>
    <button class="button" onclick="hideGallery()">back</button>
  </div>

  <script>
    function showGallery() {
      document.querySelector('.buttons-container').style.display = 'none';
      document.getElementById('gallery').style.display = 'flex';
      document.getElementById('coverImage').style.display = 'none'; // إخفاء الغلاف عند فتح المعرض
    }

    function hideGallery() {
      document.querySelector('.buttons-container').style.display = 'flex';
      document.getElementById('gallery').style.display = 'none';
      document.getElementById('coverImage').style.display = 'block'; // إظهار الغلاف عند العودة
    }
  </script>
</body>
</html>
