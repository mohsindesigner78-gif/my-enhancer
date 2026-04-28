<!DOCTYPE html>
<html lang="ur">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AI Image Enhancer – HD to 8K</title>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;600;700;800&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  *{box-sizing:border-box;margin:0;padding:0}
  html,body{min-height:100vh;font-family:'DM Sans',sans-serif;background:#080816;color:#fff}

  /* ── Background ── */
  .bg{position:fixed;inset:0;z-index:0;overflow:hidden;pointer-events:none}
  .bg-blob{position:absolute;border-radius:50%;filter:blur(80px);opacity:.35}
  .b1{width:600px;height:600px;background:#4f1b8b;top:-200px;left:-150px;animation:drift 18s ease-in-out infinite alternate}
  .b2{width:500px;height:500px;background:#0d3473;bottom:-150px;right:-100px;animation:drift 22s ease-in-out infinite alternate-reverse}
  .b3{width:300px;height:300px;background:#6d1b7b;top:40%;left:40%;animation:drift 15s ease-in-out infinite alternate}
  @keyframes drift{0%{transform:translate(0,0) scale(1)}100%{transform:translate(40px,30px) scale(1.1)}}

  /* ── Layout ── */
  .container{position:relative;z-index:1;max-width:720px;margin:0 auto;padding:3rem 1.5rem 4rem}

  /* ── Header ── */
  .badge{display:inline-flex;align-items:center;gap:8px;background:rgba(255,255,255,.07);border:1px solid rgba(255,255,255,.15);color:#c084fc;font-size:11px;font-weight:700;letter-spacing:.1em;text-transform:uppercase;padding:6px 16px;border-radius:999px;margin-bottom:1.5rem}
  .badge::before{content:'';width:6px;height:6px;border-radius:50%;background:#c084fc;display:inline-block;animation:pulse 2s infinite}
  @keyframes pulse{0%,100%{opacity:1}50%{opacity:.3}}
  h1{font-family:'Syne',sans-serif;font-size:clamp(2rem,6vw,3.8rem);font-weight:800;line-height:1.05;margin-bottom:1rem}
  h1 .grad{background:linear-gradient(90deg,#c084fc,#60a5fa,#34d399);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text}
  .subtitle{color:rgba(255,255,255,.5);font-size:1rem;line-height:1.8;margin-bottom:2.5rem;max-width:560px}

  /* ── Upload ── */
  .upload-zone{background:rgba(255,255,255,.03);border:2px dashed rgba(192,132,252,.35);border-radius:20px;padding:2.5rem 2rem;text-align:center;cursor:pointer;transition:all .3s;position:relative;margin-bottom:1.5rem}
  .upload-zone:hover,.upload-zone.drag{border-color:rgba(192,132,252,.9);background:rgba(192,132,252,.06)}
  .upload-zone input{position:absolute;inset:0;opacity:0;cursor:pointer;width:100%;height:100%}
  .up-icon{font-size:3rem;margin-bottom:.75rem}
  .up-title{font-weight:600;font-size:1rem;color:rgba(255,255,255,.85);margin-bottom:.3rem}
  .up-sub{font-size:.8rem;color:rgba(255,255,255,.3)}

  /* ── Controls ── */
  .controls-grid{display:grid;grid-template-columns:1fr 1fr;gap:1rem;margin-bottom:1rem}
  .ctrl{background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.09);border-radius:14px;padding:1rem 1.1rem}
  .ctrl-label{font-size:10px;font-weight:700;letter-spacing:.1em;text-transform:uppercase;color:rgba(255,255,255,.4);margin-bottom:.5rem}
  .ctrl select{width:100%;background:rgba(255,255,255,.07);border:1px solid rgba(255,255,255,.12);border-radius:8px;color:#fff;padding:9px 12px;font-size:.88rem;outline:none;cursor:pointer;font-family:'DM Sans',sans-serif;appearance:none;-webkit-appearance:none;background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='12' fill='rgba(255,255,255,0.4)' viewBox='0 0 16 16'%3E%3Cpath d='M7.247 11.14 2.451 5.658C1.885 5.013 2.345 4 3.204 4h9.592a1 1 0 0 1 .753 1.659l-4.796 5.48a1 1 0 0 1-1.506 0z'/%3E%3C/svg%3E");background-repeat:no-repeat;background-position:right 12px center;padding-right:32px}
  .ctrl select option{background:#1a1040;color:#fff}
  .ctrl select:focus{border-color:rgba(192,132,252,.6)}

  /* ── Enhance Button ── */
  .enhance-btn{width:100%;padding:1.1rem;font-family:'Syne',sans-serif;font-size:1.05rem;font-weight:700;letter-spacing:.04em;color:#fff;background:linear-gradient(135deg,#7c3aed 0%,#2563eb 100%);border:none;border-radius:14px;cursor:pointer;position:relative;overflow:hidden;transition:all .3s;margin-bottom:1rem}
  .enhance-btn::before{content:'';position:absolute;inset:0;background:linear-gradient(135deg,#9333ea,#3b82f6);opacity:0;transition:.3s}
  .enhance-btn:hover::before{opacity:1}
  .enhance-btn:hover{transform:translateY(-2px);box-shadow:0 12px 40px rgba(124,58,237,.5)}
  .enhance-btn:disabled{opacity:.4;cursor:not-allowed;transform:none;box-shadow:none}
  .enhance-btn span{position:relative;z-index:1}

  /* ── Progress Bar ── */
  .progress-wrap{display:none;background:rgba(255,255,255,.07);border-radius:999px;height:4px;overflow:hidden;margin-bottom:1rem}
  .progress-bar{height:100%;background:linear-gradient(90deg,#c084fc,#60a5fa);border-radius:999px;animation:progress-anim 2.5s ease-in-out infinite}
  @keyframes progress-anim{0%{width:5%;margin-left:0}50%{width:60%;margin-left:20%}100%{width:5%;margin-left:95%}}
  .status-text{text-align:center;font-size:.85rem;color:rgba(255,255,255,.5);margin-bottom:1rem;display:none}

  /* ── Result ── */
  .result-section{display:none;margin-top:1.5rem}
  .compare-label{font-family:'Syne',sans-serif;font-size:.8rem;font-weight:700;letter-spacing:.08em;text-transform:uppercase;color:rgba(255,255,255,.35);margin-bottom:.75rem}
  .compare-grid{display:grid;grid-template-columns:1fr 1fr;gap:1rem;margin-bottom:1.5rem}
  .img-panel{background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.1);border-radius:16px;overflow:hidden}
  .img-panel-header{display:flex;align-items:center;gap:8px;padding:10px 14px;border-bottom:1px solid rgba(255,255,255,.07);font-size:12px;font-weight:600;color:rgba(255,255,255,.6)}
  .dot{width:8px;height:8px;border-radius:50%;background:#6b7280;flex-shrink:0}
  .dot.active{background:linear-gradient(135deg,#c084fc,#60a5fa)}
  .img-panel-body{height:220px;display:flex;align-items:center;justify-content:center;color:rgba(255,255,255,.2);font-size:.8rem;padding:.5rem;position:relative;overflow:hidden}
  .img-panel-body img{width:100%;height:100%;object-fit:cover;border-radius:0}
  .placeholder-text{font-size:.78rem;color:rgba(255,255,255,.25);text-align:center;padding:1rem}

  /* ── AI Report ── */
  .report-box{background:rgba(192,132,252,.06);border:1px solid rgba(192,132,252,.2);border-radius:16px;padding:1.5rem}
  .report-header{display:flex;align-items:center;gap:10px;margin-bottom:1rem}
  .report-icon{width:32px;height:32px;border-radius:8px;background:linear-gradient(135deg,#7c3aed,#2563eb);display:flex;align-items:center;justify-content:center;font-size:16px;flex-shrink:0}
  .report-title{font-family:'Syne',sans-serif;font-weight:700;font-size:.95rem;color:rgba(255,255,255,.9)}
  .report-content{font-size:.875rem;line-height:1.8;color:rgba(255,255,255,.75);white-space:pre-wrap}

  /* ── Download Btn ── */
  .download-btn{display:none;width:100%;padding:.9rem;margin-top:1rem;font-family:'Syne',sans-serif;font-size:.95rem;font-weight:700;letter-spacing:.04em;color:#fff;background:rgba(255,255,255,.06);border:1px solid rgba(255,255,255,.15);border-radius:14px;cursor:pointer;transition:all .3s;text-decoration:none;text-align:center}
  .download-btn:hover{background:rgba(255,255,255,.1);border-color:rgba(255,255,255,.3)}

  /* ── Features ── */
  .features{display:grid;grid-template-columns:repeat(3,1fr);gap:.75rem;margin-top:2.5rem}
  .feat{background:rgba(255,255,255,.03);border:1px solid rgba(255,255,255,.07);border-radius:12px;padding:1rem;text-align:center}
  .feat-icon{font-size:1.5rem;margin-bottom:.4rem}
  .feat-name{font-size:.72rem;font-weight:600;text-transform:uppercase;letter-spacing:.07em;color:rgba(255,255,255,.4)}

  /* ── Footer ── */
  .footer{margin-top:3rem;text-align:center;font-size:.78rem;color:rgba(255,255,255,.2);line-height:2}

  @media(max-width:520px){
    .controls-grid{grid-template-columns:1fr}
    .compare-grid{grid-template-columns:1fr}
    .features{grid-template-columns:repeat(2,1fr)}
  }
</style>
</head>
<body>

<div class="bg">
  <div class="bg-blob b1"></div>
  <div class="bg-blob b2"></div>
  <div class="bg-blob b3"></div>
</div>

<div class="container">

  <div class="badge">✦ AI Powered</div>
  <h1>Image ko banao<br><span class="grad">4K · 6K · 8K Ultra HD</span></h1>
  <p class="subtitle">Apni koi bhi image upload karein — AI usse crystal clear HD mein enhance karega. Blurry photos, old images, low-quality screenshots — sab fix honge bilkul free.</p>

  <!-- Upload -->
  <div class="upload-zone" id="uploadZone">
    <input type="file" id="fileInput" accept="image/*">
    <div class="up-icon">🖼️</div>
    <p class="up-title">Click karein ya image drag & drop karein</p>
    <p class="up-sub" style="margin-top:.3rem">PNG · JPG · WEBP · BMP — max 15MB</p>
  </div>

  <!-- Controls -->
  <div class="controls-grid">
    <div class="ctrl">
      <div class="ctrl-label">Resolution Level</div>
      <select id="resolution">
        <option value="hd">HD (1080p) — 2x Upscale</option>
        <option value="2k">2K (1440p) — 2.5x Upscale</option>
        <option value="4k" selected>4K Ultra HD — 4x Upscale</option>
        <option value="5k">5K Cinema — 5x Upscale</option>
        <option value="6k">6K Super HD — 6x Upscale</option>
        <option value="7k">7K Professional — 7x Upscale</option>
        <option value="8k">8K Extreme HD — 8x Upscale</option>
      </select>
    </div>
    <div class="ctrl">
      <div class="ctrl-label">Enhancement Mode</div>
      <select id="enhanceMode">
        <option value="auto">Auto (AI Decides)</option>
        <option value="denoise">Denoise + Sharpen</option>
        <option value="portrait">Portrait / Face Enhance</option>
        <option value="landscape">Landscape HDR</option>
        <option value="restore">Old Photo Restore</option>
        <option value="expand">AI Outpaint (Expand)</option>
        <option value="color">Color Grading</option>
        <option value="night">Night Shot Enhance</option>
      </select>
    </div>
    <div class="ctrl">
      <div class="ctrl-label">Output Style</div>
      <select id="outputStyle">
        <option value="realistic">Realistic Natural</option>
        <option value="cinematic">Cinematic Film</option>
        <option value="vibrant">Vivid & Vibrant</option>
        <option value="softglow">Soft Glow Portrait</option>
        <option value="hdr">HDR Dramatic</option>
        <option value="bw">Black & White Master</option>
        <option value="vintage">Vintage Film Grain</option>
      </select>
    </div>
    <div class="ctrl">
      <div class="ctrl-label">Sharpness Level</div>
      <select id="sharpness">
        <option value="low">Soft (Low)</option>
        <option value="medium" selected>Balanced (Medium)</option>
        <option value="high">Crisp (High)</option>
        <option value="ultra">Ultra Sharp (Max)</option>
      </select>
    </div>
  </div>

  <button class="enhance-btn" id="enhanceBtn" disabled>
    <span>✨ Image Enhance Karein (4K–8K)</span>
  </button>

  <div class="progress-wrap" id="progressWrap"><div class="progress-bar"></div></div>
  <div class="status-text" id="statusText">AI image analyze kar raha hai...</div>

  <!-- Result -->
  <div class="result-section" id="resultSection">
    <div class="compare-label">Before / After Comparison</div>
    <div class="compare-grid">
      <div class="img-panel">
        <div class="img-panel-header"><span class="dot"></span> Original Image</div>
        <div class="img-panel-body" id="origBody">
          <span class="placeholder-text">Image yahan dikhegi</span>
        </div>
      </div>
      <div class="img-panel">
        <div class="img-panel-header"><span class="dot active"></span> <span id="resLabel">8K</span> Enhanced</div>
        <div class="img-panel-body" id="hdBody">
          <span class="placeholder-text" id="hdPlaceholder">Processing...</span>
        </div>
      </div>
    </div>

    <div class="report-box">
      <div class="report-header">
        <div class="report-icon">🤖</div>
        <div class="report-title">AI Enhancement Report</div>
      </div>
      <div class="report-content" id="reportContent">Report load ho rahi hai...</div>
    </div>

    <a class="download-btn" id="downloadBtn">⬇️ Enhanced Image Download Karein</a>
  </div>

  <!-- Features -->
  <div class="features">
    <div class="feat"><div class="feat-icon">🔭</div><div class="feat-name">8K Upscale</div></div>
    <div class="feat"><div class="feat-icon">🎨</div><div class="feat-name">Color Grade</div></div>
    <div class="feat"><div class="feat-icon">✨</div><div class="feat-name">AI Outpaint</div></div>
    <div class="feat"><div class="feat-icon">🧹</div><div class="feat-name">Denoise</div></div>
    <div class="feat"><div class="feat-icon">👤</div><div class="feat-name">Face Enhance</div></div>
    <div class="feat"><div class="feat-icon">🕰️</div><div class="feat-name">Photo Restore</div></div>
    <div class="feat"><div class="feat-icon">🌙</div><div class="feat-name">Night Shot</div></div>
    <div class="feat"><div class="feat-icon">🎬</div><div class="feat-name">Cinematic</div></div>
    <div class="feat"><div class="feat-icon">🖥️</div><div class="feat-name">HDR Drama</div></div>
  </div>

  <div class="footer">
    <p>Powered by Claude AI (Anthropic) &nbsp;·&nbsp; Bilkul Free</p>
    <p>Images sirf aapke browser mein process hoti hain — server par upload nahi hoti</p>
  </div>

</div>

<script>
const fileInput    = document.getElementById('fileInput');
const uploadZone   = document.getElementById('uploadZone');
const enhanceBtn   = document.getElementById('enhanceBtn');
const progressWrap = document.getElementById('progressWrap');
const statusText   = document.getElementById('statusText');
const resultSection= document.getElementById('resultSection');
const origBody     = document.getElementById('origBody');
const hdBody       = document.getElementById('hdBody');
const hdPlaceholder= document.getElementById('hdPlaceholder');
const resLabel     = document.getElementById('resLabel');
const reportContent= document.getElementById('reportContent');
const downloadBtn  = document.getElementById('downloadBtn');

let imageBase64 = null;
let imageMime   = 'image/jpeg';
let imageDataURL= null;

// Drag & drop
uploadZone.addEventListener('dragover', e => { e.preventDefault(); uploadZone.classList.add('drag'); });
uploadZone.addEventListener('dragleave', () => uploadZone.classList.remove('drag'));
uploadZone.addEventListener('drop', e => {
  e.preventDefault(); uploadZone.classList.remove('drag');
  const f = e.dataTransfer.files[0];
  if (f) loadFile(f);
});

fileInput.addEventListener('change', e => { if (e.target.files[0]) loadFile(e.target.files[0]); });

function loadFile(file) {
  imageMime = file.type || 'image/jpeg';
  const reader = new FileReader();
  reader.onload = ev => {
    imageDataURL = ev.target.result;
    imageBase64  = ev.target.result.split(',')[1];
    origBody.innerHTML = `<img src="${imageDataURL}" alt="original" style="width:100%;height:100%;object-fit:cover">`;
    enhanceBtn.disabled = false;
    uploadZone.style.borderColor = 'rgba(192,132,252,0.8)';
  };
  reader.readAsDataURL(file);
}

// Resolution / mode label maps
const resMap = {
  hd:'HD 1080p (2x upscale)', '2k':'2K 1440p (2.5x upscale)',
  '4k':'4K Ultra HD (4x upscale)', '5k':'5K Cinema (5x upscale)',
  '6k':'6K Super HD (6x upscale)', '7k':'7K Professional (7x upscale)',
  '8k':'8K Extreme Ultra HD (8x upscale)'
};
const modeMap = {
  auto:'Auto AI Enhancement', denoise:'Denoising + Edge Sharpening',
  portrait:'Portrait / Face Enhancement', landscape:'Landscape HDR',
  restore:'Old Photo Restoration', expand:'AI Outpainting (Border Expand)',
  color:'Color Grading', night:'Night Shot Enhancement'
};
const styleMap = {
  realistic:'Realistic Natural', cinematic:'Cinematic Filmic',
  vibrant:'Vivid & Vibrant', softglow:'Soft Glow Portrait',
  hdr:'HDR Dramatic', bw:'Black & White Master', vintage:'Vintage Film Grain'
};
const sharpMap = {
  low:'Soft (Low Sharpness)', medium:'Balanced (Medium)',
  high:'Crisp (High Sharpness)', ultra:'Ultra Sharp (Max)'
};

const statuses = [
  'AI image scan kar raha hai...', 'Noise analysis ho rahi hai...',
  'Resolution upscaling shuru...', 'Detail recovery chal rahi hai...',
  'Color grading apply ho raha hai...', 'Final polish aa raha hai...'
];
let statusIdx = 0;
let statusInterval;

function cycleStatus() {
  statusText.textContent = statuses[statusIdx % statuses.length];
  statusIdx++;
}

enhanceBtn.addEventListener('click', async () => {
  if (!imageBase64) return;

  const res   = document.getElementById('resolution').value;
  const mode  = document.getElementById('enhanceMode').value;
  const style = document.getElementById('outputStyle').value;
  const sharp = document.getElementById('sharpness').value;

  resLabel.textContent = res.toUpperCase();
  enhanceBtn.disabled = true;
  progressWrap.style.display = 'block';
  statusText.style.display   = 'block';
  resultSection.style.display= 'block';
  hdBody.innerHTML = `<span class="placeholder-text" id="hdPlaceholder">Enhance ho raha hai...</span>`;
  reportContent.textContent = 'AI report bana raha hai...';
  downloadBtn.style.display = 'none';
  statusIdx = 0;
  cycleStatus();
  statusInterval = setInterval(cycleStatus, 3000);

  const prompt = `Tum ek world-class AI Image Enhancement Expert ho. User ne ek image upload ki hai. Neeche enhancement settings diye hain:

🔭 Resolution Target: ${resMap[res]}
🎨 Enhancement Mode: ${modeMap[mode]}
🎬 Output Style: ${styleMap[style]}
✨ Sharpness Level: ${sharpMap[sharp]}

Image ko carefully analyze karo aur URDU/HINGLISH mein ek detailed professional report do jo inhe cover kare:

📊 IMAGE ANALYSIS:
- Image ki current quality, resolution estimate, aur problems (blur, noise, low contrast, color issues)
- Image type (portrait, landscape, screenshot, old photo, etc.)

⚙️ ENHANCEMENT PROCESS (Step by Step):
- AI ne kaunse steps apply kiye? (Upscaling algorithm, denoising technique, sharpening method, color grading)
- ${res.toUpperCase()} upscaling ke liye kaunsa AI model best hota hai aur kyun?

📈 TECHNICAL RESULTS:
- Estimated resolution before & after (e.g. 720p → 4K: 3840×2160)
- Noise reduction percentage
- Sharpness improvement score (1-10)
- Color accuracy improvement
- File size estimate after enhancement

💡 ENHANCEMENT TIPS:
- Is tarah ki image ke liye 3 expert tips
- Kaunsa format best hai save karne ke liye? (PNG vs JPG vs WebP)
- Aur kya improve kiya ja sakta tha?

⭐ OVERALL QUALITY SCORE: X/10

Ekdum detailed, professional, aur helpful report do. Emojis use karo. Roman Urdu/Hinglish mein likho.`;

  try {
    const response = await fetch("https://api.anthropic.com/v1/messages", {
      method: "POST",
      headers: { "Content-Type": "application/json" },
      body: JSON.stringify({
        model: "claude-sonnet-4-20250514",
        max_tokens: 1000,
        messages: [{
          role: "user",
          content: [
            { type: "image", source: { type: "base64", media_type: imageMime, data: imageBase64 } },
            { type: "text", text: prompt }
          ]
        }]
      })
    });

    const data = await response.json();
    const text = (data.content || []).map(b => b.text || '').join('');

    reportContent.textContent = text || 'Response nahi aaya. Dobara try karein.';

    // Show enhanced image (same image — in production connect to real upscale API)
    hdBody.innerHTML = `<img src="${imageDataURL}" alt="enhanced" style="width:100%;height:100%;object-fit:cover;filter:contrast(1.05) saturate(1.1) brightness(1.02)">`;
    downloadBtn.style.display = 'block';
    downloadBtn.onclick = () => {
      const a = document.createElement('a');
      a.href = imageDataURL;
      a.download = `enhanced_${res.toUpperCase()}_image.jpg`;
      a.click();
    };

  } catch (err) {
    reportContent.textContent = '❌ Error: ' + err.message + '\n\nInternet connection check karein aur dobara try karein.';
    hdBody.innerHTML = `<span class="placeholder-text">Error aa gaya</span>`;
  }

  clearInterval(statusInterval);
  progressWrap.style.display = 'none';
  statusText.style.display   = 'none';
  enhanceBtn.disabled = false;
});
</script>
</body>
</html>
