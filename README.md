[index.html](https://github.com/user-attachments/files/27400947/index.html)
<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>王振宇 · 文字探訪與內容企劃</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', sans-serif;
      background-color: #f4f7fc;
      color: #1e2a3e;
      line-height: 1.5;
      scroll-behavior: smooth;
    }

    .container {
      max-width: 1100px;
      margin: 0 auto;
      padding: 2rem 1.5rem;
    }

    .card {
      background: white;
      border-radius: 28px;
      box-shadow: 0 12px 30px rgba(0, 0, 0, 0.05);
      padding: 2rem 2.2rem;
      margin-bottom: 2rem;
      transition: transform 0.2s ease, box-shadow 0.2s ease;
    }

    .card:hover {
      box-shadow: 0 20px 35px rgba(0, 0, 0, 0.08);
    }

    .hero {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      align-items: center;
      gap: 2rem;
    }

    .hero-left {
      flex: 1;
      min-width: 280px;
    }

    .profile-header {
      display: flex;
      align-items: center;
      gap: 1.5rem;
      margin-bottom: 1rem;
      flex-wrap: wrap;
    }

    .profile-photo {
      width: 110px;
      height: 130px;
      object-fit: cover;
      border-radius: 16px;
      border: 3px solid #f0f4f8;
      box-shadow: 0 4px 10px rgba(0,0,0,0.05);
    }

    .hero-left h1 {
      font-size: 2.8rem;
      font-weight: 700;
      letter-spacing: -0.02em;
      background: linear-gradient(135deg, #1e2a3e, #2c4c6c);
      background-clip: text;
      -webkit-background-clip: text;
      color: transparent;
      margin: 0;
    }

    .hero-left .title-tag {
      font-size: 1.2rem;
      font-weight: 500;
      color: #2c6e9e;
      border-left: 4px solid #2c6e9e;
      padding-left: 0.75rem;
      margin: 0.5rem 0 0 0;
    }

    .badge-group {
      display: flex;
      flex-wrap: wrap;
      gap: 0.6rem;
      margin-top: 1rem;
    }

    .badge {
      background: #eef2f5;
      padding: 0.25rem 1rem;
      border-radius: 40px;
      font-size: 0.8rem;
      font-weight: 500;
      color: #1e4a6e;
    }

    .hero-right {
      background: #eaf2f8;
      border-radius: 2rem;
      padding: 1rem 1.8rem;
      text-align: center;
      min-width: 240px;
    }

    .contact-item {
      display: flex;
      align-items: center;
      gap: 0.6rem;
      font-size: 0.9rem;
      margin: 0.6rem 0;
      color: #1f3b4c;
    }

    .contact-item i {
      width: 1.6rem;
      color: #2c6e9e;
      font-size: 1.1rem;
    }

    .section-title {
      font-size: 1.6rem;
      font-weight: 700;
      margin-bottom: 1.25rem;
      letter-spacing: -0.3px;
      display: flex;
      align-items: center;
      gap: 0.6rem;
      border-bottom: 3px solid #dce7ef;
      padding-bottom: 0.5rem;
    }

    .section-title i {
      color: #2c6e9e;
      font-size: 1.5rem;
    }

    .bio-text p {
      margin-bottom: 1rem;
      font-size: 1rem;
      color: #2c3f4f;
    }

    .highlight {
      background: #eef3fc;
      border-left: 4px solid #2c6e9e;
      padding: 0.2rem 0.8rem;
      font-weight: 500;
      border-radius: 0 12px 12px 0;
    }

    .exp-item {
      margin-bottom: 2rem;
    }

    .exp-header {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      font-weight: 700;
      font-size: 1.15rem;
      margin-bottom: 0.4rem;
    }

    .exp-company {
      color: #0f3b5c;
    }

    .exp-date {
      font-weight: 400;
      color: #5a6e7c;
      font-size: 0.85rem;
    }

    .exp-title {
      font-weight: 600;
      color: #2c6e9e;
      margin-bottom: 0.75rem;
      font-size: 0.95rem;
    }

    .exp-desc {
      padding-left: 0.5rem;
      list-style-type: none;
    }

    .exp-desc li {
      margin-bottom: 0.5rem;
      display: flex;
      gap: 0.6rem;
      font-size: 0.94rem;
    }

    .exp-desc li i {
      color: #2c6e9e;
      font-size: 0.85rem;
      margin-top: 0.2rem;
      width: 1.2rem;
    }

    .skills-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 0.8rem;
      margin-top: 0.5rem;
    }

    .skill-chip {
      background: #eef2f5;
      padding: 0.4rem 1rem;
      border-radius: 30px;
      font-size: 0.85rem;
      font-weight: 500;
    }

    .work-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 1.2rem;
      margin-top: 1rem;
    }

    .work-card {
      background: #f9fbfd;
      border-radius: 1.2rem;
      padding: 1rem 1.2rem;
      flex: 1 1 200px;
      border: 1px solid #e2edf2;
      transition: all 0.2s;
    }

    .work-card i {
      font-size: 1.8rem;
      color: #2c6e9e;
      margin-bottom: 0.4rem;
    }

    .work-card h4 {
      font-weight: 700;
      margin: 0.5rem 0 0.2rem;
    }

    /* 汽車攝影作品區 - 縮小圖片尺寸 */
    .photo-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 1.2rem;
      margin-top: 1rem;
      justify-content: center;
    }

    .photo-item {
      max-width: 400px;  /* 限制最大寬度 */
      width: 100%;
      background: #f9fbfd;
      border-radius: 1.2rem;
      padding: 0.8rem;
      border: 1px solid #e2edf2;
      text-align: center;
    }

    .photo-item img {
      width: 100%;
      height: auto;
      max-width: 100%;
      border-radius: 0.8rem;
      display: block;
      object-fit: contain;  /* 保持原圖比例，不裁切 */
    }

    .photo-caption {
      font-size: 0.75rem;
      color: #5a6e7c;
      margin-top: 0.4rem;
    }

    .footer {
      text-align: center;
      padding: 1.5rem 0 1rem;
      font-size: 0.8rem;
      color: #67829c;
      border-top: 1px solid #d4e2ec;
      margin-top: 1rem;
    }

    @media (max-width: 700px) {
      .container {
        padding: 1rem;
      }
      .card {
        padding: 1.5rem;
      }
      .hero-left h1 {
        font-size: 2rem;
      }
      .section-title {
        font-size: 1.4rem;
      }
      .profile-header {
        flex-direction: column;
        align-items: flex-start;
        gap: 1rem;
      }
      .photo-item {
        max-width: 100%;  /* 手機上改為滿版 */
      }
    }
  </style>
</head>
<body>
<div class="container">
  <!-- 頁首：姓名 + 照片 + 聯絡資訊 -->
  <div class="card">
    <div class="hero">
      <div class="hero-left">
        <div class="profile-header">
          <img src="https://i.ibb.co/5h6V8cWh/image.jpg" alt="王振宇" class="profile-photo" onerror="this.style.display='none'">
          <div>
            <h1>王振宇</h1>
            <div class="title-tag">文字採訪 · 內容企劃 · 學術轉譯</div>
          </div>
        </div>
        <div class="badge-group">
          <span class="badge"><i class="fas fa-pen-nib"></i> 採訪編輯</span>
          <span class="badge"><i class="fas fa-graduation-cap"></i> 宗教研究所 (輔大)</span>
          <span class="badge"><i class="fas fa-book-open"></i> 《臺灣宗教研究》發表</span>
          <span class="badge"><i class="fas fa-car"></i> 汽車雜誌撰稿</span>
        </div>
      </div>
      <div class="hero-right">
        <div class="contact-item"><i class="fas fa-phone-alt"></i> 0939-732-318</div>
        <div class="contact-item"><i class="fas fa-envelope"></i> aia5566aia@gmail.com</div>
        <div class="contact-item"><i class="fas fa-map-marker-alt"></i> 新北市樹林區 · 台北市</div>
        <div class="contact-item"><i class="fas fa-clock"></i> 隨時可上班</div>
      </div>
    </div>
  </div>

  <!-- 專業摘要 -->
  <div class="card">
    <div class="section-title">
      <i class="fas fa-user-pen"></i>
      <span>專業摘要</span>
    </div>
    <div class="bio-text">
      <p>具備文字採訪、內容編輯與研究型寫作能力。曾於輔仁大學宗教研究所進修，鑽研龍樹中觀哲學，並在台灣宗教領域頂尖期刊《臺灣宗教研究》發表論文〈宗教時間中的綿延與斷裂〉。過去任雜誌採訪編輯兩年餘，擅長將高度複雜的資訊 — 無論是宗教思想、文化現象或汽車機械技術 — 重新拆解、整理為清晰、有邏輯且貼近讀者的內容。</p>
      <p>我的文字具備學術深度與傳播效益，能在不同讀者群之間切換語氣與敘事策略。期待投入內容產製、品牌敘事、文史整理或媒體企劃，讓艱澀的知識轉譯為可被信賴的報導與論述。</p>
      <p class="highlight"><i class="fas fa-arrow-right"></i> 核心使命：將複雜變成透明，將資訊淬鍊為觀點。</p>
    </div>
  </div>

  <!-- 工作經歷 -->
  <div class="card">
    <div class="section-title">
      <i class="fas fa-briefcase"></i>
      <span>工作經歷</span>
    </div>
    <div class="exp-item">
      <div class="exp-header">
        <span class="exp-company">雨生文化出版事業有限公司</span>
        <span class="exp-date">2019.06 – 2021.06</span>
      </div>
      <div class="exp-title">文字採訪編輯｜汽車生活誌</div>
      <ul class="exp-desc">
        <li><i class="fas fa-caret-right"></i> <strong>企劃與執行</strong>：獨立負責每期汽車單元企劃，從主題發想、車輛聯繫、實拍試駕到撰稿完成，每月穩定產出2-3篇深度報導。</li>
        <li><i class="fas fa-caret-right"></i> <strong>跨部門溝通</strong>：與廣告主、公關公司及受訪者協調採訪細節，成功完成多次新車發表會與試駕現場報導。</li>
        <li><i class="fas fa-caret-right"></i> <strong>文案與編排</strong>：撰寫高吸引力的標題與內文，使用軟體進行初步圖文排版，確保閱讀動線與資訊清晰度。</li>
        <li><i class="fas fa-caret-right"></i> <strong>視覺產出</strong>：具備基礎汽車攝影能力，獨立拍攝雜誌配圖並篩選編輯，強化文字論述。</li>
      </ul>
    </div>
    <div class="exp-item">
      <div class="exp-header">
        <span class="exp-company">語果作文 · 才藝教室</span>
        <span class="exp-date">2017.01 – 2018.01</span>
      </div>
      <div class="exp-title">作文老師／寫作引導</div>
      <ul class="exp-desc">
        <li><i class="fas fa-caret-right"></i> 設計寫作架構課程，引導不同年齡層學生將抽象想法轉化為邏輯清晰的文字。</li>
        <li><i class="fas fa-caret-right"></i> 訓練對於「讀者理解障礙」的敏感度，預判敘事盲點並調整教學／書寫策略。</li>
      </ul>
    </div>
  </div>

  <!-- 學術與人文專業 -->
  <div class="card">
    <div class="section-title">
      <i class="fas fa-landmark"></i>
      <span>學術與人文專業</span>
    </div>
    <div style="display: flex; flex-wrap: wrap; gap: 1.5rem;">
      <div style="flex: 2; min-width: 180px;">
        <p><strong><i class="fas fa-university"></i> 輔仁大學 · 宗教研究所</strong> (碩士班進修 2021–2025)<br>研究領域：龍樹中觀哲學、宗教時間理論、當代宗教轉譯</p>
        <p style="margin-top: 0.5rem;"><strong><i class="fas fa-file-alt"></i> 期刊發表</strong><br>〈宗教時間中的綿延與斷裂〉，刊登於《臺灣宗教研究》—— 台灣宗教學門最具指標性的THCI核心期刊。</p>
        <p><strong><i class="fas fa-graduation-cap"></i> 學士背景</strong><br>國立東華大學 華文文學系／銘傳大學 應用中國文學系，奠定文本分析、修辭及寫作結構訓練。</p>
      </div>
      <div style="flex: 1.2; background: #f0f6fa; border-radius: 20px; padding: 1rem 1.2rem;">
        <i class="fas fa-chalkboard-user" style="font-size: 1.4rem; color: #1f6390;"></i>
        <p style="font-weight: 600; margin-top: 0.3rem;">儒釋道經典×現代敘事</p>
        <p style="font-size: 0.85rem;">能夠進行經典思想之譯註、文史資料彙整，將傳統智慧重新詮釋為現代文案、刊物或簡報。</p>
      </div>
    </div>
  </div>

  <!-- 核心職能 -->
  <div class="card">
    <div class="section-title">
      <i class="fas fa-code-branch"></i>
      <span>核心職能</span>
    </div>
    <div style="display: flex; flex-wrap: wrap; gap: 2rem;">
      <div style="flex: 1;">
        <h4 style="margin-bottom: 0.8rem;"><i class="fas fa-pen-fancy"></i> 編輯企劃力</h4>
        <ul style="list-style: none;">
          <li>✓ 採訪寫作、審稿校對、下標改稿</li>
          <li>✓ 內容轉譯 · 複雜資訊架構重建</li>
          <li>✓ 簡報邏輯設計 / 企劃提案能力</li>
          <li>✓ 刊物編撰、出版流程管理</li>
        </ul>
      </div>
      <div style="flex: 1;">
        <h4 style="margin-bottom: 0.8rem;"><i class="fas fa-laptop-code"></i> 數位工具</h4>
        <div class="skills-grid">
          <span class="skill-chip">Word / Excel / PPT</span>
          <span class="skill-chip">Photoshop / Lightroom</span>
          <span class="skill-chip">Canva / 簡報設計</span>
          <span class="skill-chip">Director / 多媒體基礎</span>
          <span class="skill-chip">中文60字/分｜英文40字/分</span>
        </div>
        <h4 style="margin: 1.2rem 0 0.6rem 0;"><i class="fas fa-language"></i> 語言能力</h4>
        <p>英文 聽/讀 中等 · 台語 中等</p>
      </div>
    </div>
  </div>

  <!-- 代表作品 -->
  <div class="card">
    <div class="section-title">
      <i class="fas fa-folder-open"></i>
      <span>代表作品</span>
    </div>
    <div class="work-grid">
      <div class="work-card">
        <i class="fas fa-newspaper"></i>
        <h4>汽車雜誌試乘文章</h4>
        <p style="font-size: 0.8rem; margin-top: 6px;">實車拍攝＋專業試駕報導，含圖文編排、規格轉譯，每月穩定刊出。</p>
        <p style="margin-top: 8px;">
          <a href="https://motormag.com.tw/2020/05/02/land-rover-discovery-sport-p250-r-dynamic-se/" target="_blank" rel="noopener noreferrer" style="color: #2c6e9e; text-decoration: none; font-weight: 500;">🔗 閱讀文章 →</a>
        </p>
      </div>
      <div class="work-card">
        <i class="fas fa-scroll"></i>
        <h4>學術論文 · 臺灣宗教研究</h4>
        <p style="font-size: 0.8rem;">〈宗教時間中的綿延與斷裂〉— 展現抽象理論與哲學架構之寫作能力。</p>
        <p style="margin-top: 8px;">
          <a href="https://www.airitilibrary.com/Article/Detail/a0000594-N202501070006-00004" target="_blank" rel="noopener noreferrer" style="color: #2c6e9e; text-decoration: none; font-weight: 500;">🔗 閱讀論文 →</a>
        </p>
      </div>
      <div class="work-card">
        <i class="fas fa-microphone-alt"></i>
        <h4>採訪實錄與專題報導</h4>
        <p style="font-size: 0.8rem;">車界人物專訪、活動紀實，擅長將專業術語改寫為高親和力內容。</p>
      </div>
    </div>

    <!-- 汽車攝影作品區（車輛動態實拍）- 已縮小尺寸 -->
    <div style="margin-top: 2rem;">
      <h4 style="margin-bottom: 0.5rem;"><i class="fas fa-camera"></i> 汽車攝影作品</h4>
      <p style="font-size: 0.85rem; color: #4a627a;">實際拍攝之汽車專業照片，展現構圖、光影運用與動態捕捉能力。</p>
      <div class="photo-grid">
        <div class="photo-item">
          <a href="https://i.ibb.co/Z6nfx8Gf/IMG-0360.jpg" target="_blank" rel="noopener noreferrer">
            <img src="https://i.ibb.co/Z6nfx8Gf/IMG-0360.jpg" alt="車輛動態實拍">
          </a>
          <div class="photo-caption">車輛動態實拍</div>
        </div>
      </div>
    </div>
    <div style="margin-top: 1rem; background: #e3f0f5; border-radius: 40px; padding: 0.6rem 1rem; text-align: center; font-size: 0.85rem;">
      <i class="fas fa-paperclip"></i> 完整作品集（期刊PDF、試車文章樣本）可依面試需求提供
    </div>
  </div>

  <!-- 職涯目標與合作價值 -->
  <div class="card">
    <div class="section-title">
      <i class="fas fa-chart-line"></i>
      <span>職涯目標 & 合作價值</span>
    </div>
    <div style="display: flex; flex-wrap: wrap; gap: 1.2rem;">
      <div style="flex: 2;">
        <p><i class="fas fa-check-circle" style="color:#2c6e9e;"></i> <strong>期待職稱：</strong>文字編輯／採訪企劃／內容專員／文史整理與編輯</p>
        <p><i class="fas fa-check-circle" style="color:#2c6e9e;"></i> <strong>工作地點：</strong>台北市、新北市</p>
        <p><i class="fas fa-check-circle" style="color:#2c6e9e;"></i> <strong>全職 · 日班/彈性 · 薪資面議 (期待與專業匹配)</strong></p>
        <p style="margin-top: 0.8rem;">具備從資訊採集、內容企劃到精準校稿的完整閉環能力，能獨立作業，亦擅長跨團隊溝通，在時程壓力下維持高品質產出。同時擁有學術訓練帶來的「論證嚴謹性」與媒體實務的「讀者思維」。</p>
      </div>
      <div style="flex: 1; background: #eef3fc; border-radius: 18px; padding: 1rem;">
        <i class="fas fa-lightbulb"></i>
        <p style="font-weight: bold; margin-top: 0.3rem;">轉譯者的優勢</p>
        <p style="font-size: 0.85rem;">將艱澀概念（宗教、技術）轉變為每個人都能共感的故事與知識。</p>
      </div>
    </div>
  </div>

  <div class="footer">
    <p><i class="fas fa-envelope-open-text"></i> 歡迎來信或致電 0939-732-318 ｜ 電子履歷與作品備索 · 願景：讓好內容被看見，讓複雜被理解</p>
    <p style="margin-top: 0.4rem;">© 2026 王振宇 · 線上商務履歷</p>
  </div>
</div>
</body>
</html>
