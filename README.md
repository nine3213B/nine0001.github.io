<!DOCTYPE html>
<html lang="zh-Hant">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>我的個人首頁</title>
    <style>
        /* --- CSS 設定區域 (控制外觀) --- */

        /* 1. 全域設定：讓所有元素的邊距歸零，比較好排版 */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* 2. 背景與文字基礎設定 */
        body {
            /* 【關鍵】這裡設定深灰色背景 */
            background-color: #1a1a1a; 
            /* 設定主要文字顏色為淺灰，對比度才夠 */
            color: #e0e0e0;
            /* 使用無襯線字體，看起來比較乾淨現代 */
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            line-height: 1.6;
            padding: 20px;
        }

        /* 強制隱藏 GitHub 可能自動產生的頂部導覽列 */
        header, .header, #header { display: none !important; }

        /* 3. 主要容器：把所有內容包在中間，不要太寬 */
        .container {
            max-width: 800px; /* 最大寬度 800px */
            margin: 50px auto; /* 上下邊距 50px，左右自動置中 */
        }

        /* 4. 卡片樣式：讓內容區塊看起來像浮起來的卡片 */
        .card {
            background-color: #2d2d2d; /* 比背景稍亮的深灰色 */
            padding: 30px;
            border-radius: 15px; /* 圓角 */
            box-shadow: 0 10px 25px rgba(0,0,0,0.5); /* 陰影效果 */
            margin-bottom: 30px; /* 卡片之間的間距 */
        }

        /* 5. 標題顏色：用一個亮色系來點綴 (例如霓虹藍) */
        h1, h2 {
            color: #00d4ff;
            margin-bottom: 15px;
        }

        /* 6. 圖片樣式：確保圖片會自動縮放，不會破版 */
        .profile-image {
            width: 100%; /* 寬度佔滿卡片 */
            max-height: 400px; /* 限制最大高度，避免圖片太長 */
            object-fit: cover; /* 保持圖片比例裁切 */
            border-radius: 10px; /* 圖片也要圓角 */
            margin-bottom: 20px;
            border: 3px solid #333; /* 加個深色邊框更有質感 */
        }

        /* 7. 列表樣式 (用於硬體規格等) */
        ul.specs {
            list-style: none; /* 去掉預設的圓點 */
            padding-left: 0;
        }
        ul.specs li {
            margin-bottom: 10px;
            padding-left: 20px;
            border-left: 4px solid #00d4ff; /* 左側加一條亮線裝飾 */
            background-color: rgba(255, 255, 255, 0.05); /* 微微亮的背景條 */
            padding: 10px;
            border-radius: 0 5px 5px 0;
        }
        
        /* 連結樣式 */
        a {
            color: #00d4ff;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>

    <div class="container">

        <div class="card">
            <h1>歡迎來到我的領域</h1>
            <p>你好！這是一個熱愛 FPS 與節奏遊戲的玩家空間。這裡沒有廣告，只有我對遊戲和硬體的熱情。</p>
            <br>
            
            <img class="profile-image" src="https://via.placeholder.com/800x400/444444/00d4ff?text=Upload+Your+Image+Here" alt="我的封面圖">
            
            <p>目前正在鑽研 Python 開發，目標是寫出更強大的 Discord 機器人。</p>
        </div>

        <div class="card">
            <h2>⚙️ 裝備與戰績</h2>
            <p>工欲善其事，必先利其器。以下是我的目前配置：</p>
            <br>
            
            <ul class="specs">
                <li><strong>行動裝置：</strong>iPhone 17 Pro / Pixel 9a</li>
                <li><strong>PC 散熱：</strong>Noctua NH-D9L (貓頭鷹信仰!)</li>
                <li><strong>主力遊戲：</strong>Apex Legends, Valorant, 以及各類音樂遊戲</li>
                <li><strong>開發工具：</strong>VS Code, Python</li>
            </ul>
        </div>

        <p style="text-align: center; font-size: 0.9em; color: #888;">
            © 2026 Designed by Me. Hosted on GitHub Pages.
        </p>

    </div>

</body>
</html>
