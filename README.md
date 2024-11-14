<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Website with Sliding Welcome Animation</title>
    <style>
        /* تنسيق شاشة الترحيب */
        #welcomeScreen {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: #8b5e3c; /* لون كافيه */
            color: #f7ffb2;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 2.5em;
            font-family: 'Arial', sans-serif;
            z-index: 10;
        }
    
        /* حركة النص */
        #welcomeText {
            position: relative;
            animation: slideInFromRight 3s ease-out forwards;
        }
    
        /* تأثير الحركة من اليمين إلى اليسار */
        @keyframes slideInFromRight {
            from {
                transform: translateX(100%);
            }
            to {
                transform: translateX(0);
            }
        }

        /* خلفية متحركة */
        body {
            background: linear-gradient(270deg, #8b5e3c, #f5e6d8);
            background-size: 400% 400%;
            animation: gradientAnimation 10s ease infinite;
            color: #4d3a2f;
            font-family: Arial, sans-serif;
            margin: 0;
            padding-top: 50px;
        }

        @keyframes gradientAnimation {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
    
        /* تنسيق المحتوى الرئيسي */
        #mainContent {
            display: none;
            text-align: center;
            background-color: #ffffff;
            color: #4d3a2f;
            padding: 20px;
            min-height: 100vh;
        }
    
        /* تنسيق الصورة الرئيسية */
        .main-image {
            display: block;
            margin: 0 auto;
            width: 1000px;
            height: 680px;
            margin-bottom: 50px; /* إضافة مسافة بين الصورة الرئيسية والصور الإضافية */
        }
    
        /* تنسيق شبكة الصور الإضافية */
        .image-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr); /* 4 صور لكل صف */
            gap: 10px; /* مسافة بين كل صورة وصورة */
            margin-top: 20px;
        }
    
        .image-grid img {
            width: 100%;
            height: auto;
            border-radius: 8px;
            border: 2px solid #8b5e3c; /* إضافة حد بين الصور */
        }
    </style>
</head>
<body>
    <!-- شاشة الترحيب -->
    <div id="welcomeScreen">
        <h1 id="welcomeText">WELCOME TO QAF</h1>
    </div>
    

        <!-- الصورة الرئيسية -->
        <img src="/Users/mohamedahmed/Library/Containers/com.apple.Photos/Data/tmp/TemporaryItems/PasteboardItemExports/C5AE067C-5509-465C-B3EF-ABD05F48DE4D_1_102_o.jpeg" alt="Main Pastry Coffee" class="main-image">
        
  
        
    <!-- المحتوى الرئيسي للصفحة -->
    <div id="mainContent">
        <h1>MENU</h1>
        <p>This is a coffee and pastry </p>
        <!-- أيقونة الإنستجرام -->
<div style="text-align: center; margin-top: 20px;">
    <a href="https://www.instagram.com/qaf.eg?utm_source=ig_web_button_share_sheet&igsh=ZDNlZDc0MzIxNw==" target="_blank" style="text-decoration: none; color: #000000;">
        <img src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Instagram_icon.png" alt="Instagram" style="width: 40px; height: 40px;"><!-- أيقونة الفيسبوك -->
        <div style="text-align: center; margin-top: 20px;">
            <a href="https://www.facebook.com/Qafcafe?mibextid=LQQJ4d" target="_blank" style="text-decoration: none; color: #3b5998;">
                <img src="https://upload.wikimedia.org/wikipedia/commons/5/51/Facebook_f_logo_%282019%29.svg" alt="Facebook" style="width: 40px; height: 40px;">
                
            </a>
        
    </a>
</div>

</div>
📍 15 May City - Downtown mall Down Cairo Lab
📍 Helwan - Next to Bazooka and KFC
        <!-- شبكة الصور الإضافية -->
        <div class="image-grid">
            <img src="/Users/mohamedahmed/Downloads/untitled folder/Untitled-1.jpg" alt="Additional Image 1">
            <img src="/Users/mohamedahmed/Library/Containers/com.apple.Photos/Data/tmp/TemporaryItems/PasteboardItemExports/69497E35-ED41-47A8-9113-E6D8CCA86E6A_1_105_c.jpeg" alt="Additional Image 2">
            <img src="/Users/mohamedahmed/Library/Containers/com.apple.Photos/Data/tmp/TemporaryItems/PasteboardItemExports/CE33C3B7-40D3-4EE2-B72A-66762BFB253D_1_105_c.jpeg" alt="Additional Image 3">
            <img src="/Users/mohamedahmed/Library/Containers/com.apple.Photos/Data/tmp/TemporaryItems/PasteboardItemExports/65F53C78-5C34-451C-851D-692C1E80D321_1_105_c.jpeg" alt="Additional Image 4">
            <img src="/Users/mohamedahmed/Library/Containers/com.apple.Photos/Data/tmp/TemporaryItems/PasteboardItemExports/66554982-C14F-42B4-A065-8B0BC86FF5B5_1_105_c.jpeg" alt="Additional Image 5">
            <img src="/Users/mohamedahmed/Library/Containers/com.apple.Photos/Data/tmp/TemporaryItems/PasteboardItemExports/05FC7B2F-757A-4FD0-9531-23C818DE11BE_1_105_c.jpeg" alt="Additional Image 6">
            <img src="/Users/mohamedahmed/Library/Containers/com.apple.Photos/Data/tmp/TemporaryItems/PasteboardItemExports/7458679A-0B14-4413-B288-901D270C7D94_1_105_c.jpeg" alt="Additional Image 7">
            <img src="/Users/mohamedahmed/Library/Containers/com.apple.Photos/Data/tmp/TemporaryItems/PasteboardItemExports/10A7BEA3-ED02-4098-88FF-52902437A5B7_1_105_c.jpeg" alt="Additional Image 8">
            <img src="/Users/mohamedahmed/Library/Containers/com.apple.Photos/Data/tmp/TemporaryItems/PasteboardItemExports/61566987-3AD6-42F5-80AD-D560D811F5FB_1_105_c.jpeg" alt="Additional Image 9">
            <img src="/Users/mohamedahmed/Library/Containers/com.apple.Photos/Data/tmp/TemporaryItems/PasteboardItemExports/0967678B-3C71-4E6D-960C-0521ADAAC9BF_1_105_c.jpeg" alt="Additional Image 10">
            <img src="/Users/mohamedahmed/Library/Containers/com.apple.Photos/Data/tmp/TemporaryItems/PasteboardItemExports/C9FD31D4-BF36-4565-9872-E07686A9BDF5_1_105_c.jpeg" alt="Additional Image 11">
            <img src="/Users/mohamedahmed/Library/Containers/com.apple.Photos/Data/tmp/TemporaryItems/PasteboardItemExports/A510B4F7-3F64-411E-B815-68F8E6BDEC5D_1_105_c.jpeg" alt="Additional Image 12">
            <img src="/Users/mohamedahmed/Library/Containers/com.apple.Photos/Data/tmp/TemporaryItems/PasteboardItemExports/125944DB-90DB-474B-84B1-52EACD0EA40C_1_105_c.jpeg" alt="Additional Image 13">
            <img src="/Users/mohamedahmed/Library/Containers/com.apple.Photos/Data/tmp/TemporaryItems/PasteboardItemExports/A4750B4D-A0AF-4D9D-8E4E-D81072C319CF_1_105_c.jpeg" alt="Additional Image 14">
            <img src="/Users/mohamedahmed/Library/Containers/com.apple.Photos/Data/tmp/TemporaryItems/PasteboardItemExports/9777018C-F0FB-4D2E-9FC8-EAB4BF9A99FE_1_105_c.jpeg" alt="Additional Image 15">
            <img src="/Users/mohamedahmed/Library/Containers/com.apple.Photos/Data/tmp/TemporaryItems/PasteboardItemExports/42C9458B-924B-45A2-BB2F-3F54BEC0187E_1_105_c.jpeg" alt="Additional Image 16">
            <!-- أضف المزيد من الصور هنا --> 
             
        </div>
    </div>![Premium Photo | Chocolate milk twister whirlwind or tornado realistic splash coffee and cocoa brown swirl](https://github.com/user-attachments/assets/77816ca3-a3a3-4476-bc86-2a2af4a8ffc4)

    <script>
        // إخفاء شاشة الترحيب بعد 4 ثواني وإظهار المحتوى الرئيسي
        setTimeout(function() {
            document.getElementById("welcomeScreen").style.display = "none"; // إخفاء شاشة الترحيب
            document.getElementById("mainContent").style.display = "block"; // إظهار المحتوى الرئيسي
        }, 4000); // 4000 ميلي ثانية (4 ثواني)
    </script>
</body>
</html>
