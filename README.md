<!DOCTYPE html>
<html lang="en" class="h-full bg-slate-950 text-slate-100">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Razan Alsunaidi - Custom Profile README Banner Generator</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;600&family=Plus+Jakarta+Sans:wght@400;600;700;800&display=swap" rel="stylesheet">
  <script src="https://unpkg.com/lucide@latest"></script>
  <style>
    body {
      font-family: 'Plus Jakarta Sans', sans-serif;
    }
    .font-mono {
      font-family: 'Fira Code', monospace;
    }
    
    /* Custom Violet & Cream Glows */
    .bg-violet-cream-gradient {
      background: linear-gradient(135deg, #1f102e 0%, #2a1b3d 40%, #150921 100%);
    }
    .text-cream {
      color: #F5F5DC;
    }
    .text-cream-light {
      color: #FDFBF7;
    }
    .border-violet-accent {
      border-color: rgba(138, 43, 226, 0.4);
    }
    .bg-violet-primary {
      background-color: #8A2BE2;
    }
    
    /* Canvas Glow Effects */
    .glow-purple {
      box-shadow: 0 0 35px rgba(138, 43, 226, 0.35);
    }
    .glow-cream {
      box-shadow: 0 0 20px rgba(245, 245, 220, 0.2);
    }

    /* Ambient Particle Canvas */
    #ambientCanvas {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
    }
  </style>
</head>
<body class="h-full flex flex-col overflow-x-hidden bg-slate-950">

  <!-- Top Navigation Header -->
  <header class="border-b border-purple-900/40 bg-slate-900/80 backdrop-blur-md sticky top-0 z-50">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-16 flex items-center justify-between">
      <div class="flex items-center gap-3">
        <div class="w-9 h-9 rounded-xl bg-gradient-to-tr from-purple-600 to-amber-200 flex items-center justify-center text-slate-950 font-bold shadow-lg shadow-purple-900/30">
          RA
        </div>
        <div>
          <h1 class="text-base font-bold text-slate-100 flex items-center gap-2">
            Razan Alsunaidi <span class="text-xs px-2 py-0.5 rounded-full bg-purple-900/60 text-amber-200 border border-purple-500/30">README Suite</span>
          </h1>
          <p class="text-xs text-slate-400">Violet & Cream (#8A2BE2 & #F5F5DC) Game-Dev Aesthetic</p>
        </div>
      </div>
      
      <div class="flex items-center gap-2">
        <button id="copyMdBtn" class="flex items-center gap-2 px-4 py-2 text-xs font-semibold rounded-lg bg-purple-600 hover:bg-purple-500 text-white transition-all shadow-md glow-purple">
          <i data-lucide="copy" class="w-4 h-4"></i>
          <span>Copy Full README Code</span>
        </button>
      </div>
    </div>
  </header>

  <main class="flex-1 max-w-7xl w-full mx-auto px-4 sm:px-6 lg:px-8 py-8 space-y-8">
    
    <!-- Hero / Live Interactive SVG Banner Canvas -->
    <section class="space-y-4">
      <div class="flex items-center justify-between">
        <h2 class="text-lg font-semibold text-slate-200 flex items-center gap-2">
          <i data-lucide="sparkles" class="w-5 h-5 text-amber-200"></i>
          Live Interactive Banner Preview (Violet & Cream HUD)
        </h2>
        <span class="text-xs text-slate-400 font-mono">Native Responsive SVG / HTML Vector Header</span>
      </div>

      <div class="relative rounded-2xl overflow-hidden border border-purple-800/40 bg-violet-cream-gradient p-8 md:p-12 shadow-2xl transition-all">
        <canvas id="ambientCanvas"></canvas>

        <div class="relative z-10 space-y-6">
          <!-- Top Tag HUD -->
          <div class="flex flex-wrap items-center justify-between gap-4">
            <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-purple-950/80 border border-purple-500/40 text-amber-100 text-xs font-mono shadow-inner">
              <span class="w-2 h-2 rounded-full bg-amber-200 animate-pulse"></span>
              SYSTEM.GAME_DEV // XR & AI ACTIVE
            </div>
            <div class="text-xs font-mono text-purple-300/70 tracking-widest uppercase">
              Riyadh, SA • First-Class Honors
            </div>
          </div>

          <!-- Main Title Block -->
          <div class="space-y-2">
            <h1 class="text-4xl sm:text-5xl md:text-6xl font-extrabold tracking-tight text-cream-light drop-shadow-md">
              Razan Alsunaidi
            </h1>
            <p class="text-base sm:text-lg text-purple-200 font-medium max-w-2xl leading-relaxed">
              Crafting Immersive Interactive Worlds, Extended Realities, Intelligent AI Systems, and Game QA Frameworks.
            </p>
          </div>

          <!-- Live Dynamic Typing HUD -->
          <div class="p-4 rounded-xl bg-slate-950/60 border border-purple-500/30 backdrop-blur-md font-mono text-sm flex items-center gap-3">
            <span class="text-amber-200 font-bold">></span>
            <span id="typingEffectText" class="text-purple-200"></span>
            <span class="w-2 h-5 bg-amber-200 animate-ping inline-block"></span>
          </div>

          <!-- Specialized Badges Strip -->
          <div class="flex flex-wrap gap-2 pt-2">
            <span class="px-3 py-1.5 rounded-lg bg-purple-900/60 text-amber-100 text-xs font-semibold border border-purple-400/30 flex items-center gap-1.5">
              <i data-lucide="gamepad-2" class="w-4 h-4 text-amber-200"></i> Game Dev & XR
            </span>
            <span class="px-3 py-1.5 rounded-lg bg-purple-900/60 text-amber-100 text-xs font-semibold border border-purple-400/30 flex items-center gap-1.5">
              <i data-lucide="shield-check" class="w-4 h-4 text-amber-200"></i> QA & Software Testing
            </span>
            <span class="px-3 py-1.5 rounded-lg bg-purple-900/60 text-amber-100 text-xs font-semibold border border-purple-400/30 flex items-center gap-1.5">
              <i data-lucide="cpu" class="w-4 h-4 text-amber-200"></i> AI & Computer Vision
            </span>
          </div>
        </div>
      </div>
    </section>

    <!-- Content Section: GitHub Profile Layout Preview & Source Code Editor -->
    <section class="grid grid-cols-1 lg:grid-cols-2 gap-8">
      
      <!-- Left Column: Markdown Code Block -->
      <div class="space-y-4">
        <div class="flex items-center justify-between">
          <h3 class="text-sm font-semibold text-slate-300 flex items-center gap-2">
            <i data-lucide="code-2" class="w-4 h-4 text-purple-400"></i>
            GitHub README Markdown Code (Violet & Cream Theme)
          </h3>
          <button id="copyBannerOnlyBtn" class="text-xs text-purple-300 hover:text-amber-200 flex items-center gap-1">
            <i data-lucide="copy" class="w-3.5 h-3.5"></i> Copy snippet
          </button>
        </div>

        <div class="relative rounded-xl border border-slate-800 bg-slate-900 overflow-hidden font-mono text-xs">
          <pre id="readmeCodeText" class="p-4 text-purple-200/90 overflow-x-auto leading-relaxed max-h-[500px] scrollbar-thin scrollbar-thumb-purple-800"></pre>
        </div>
      </div>

      <!-- Right Column: Interactive Profile Component Showcase -->
      <div class="space-y-6">
        <h3 class="text-sm font-semibold text-slate-300 flex items-center gap-2">
          <i data-lucide="layout-grid" class="w-4 h-4 text-purple-400"></i>
          GitHub Component Showcase
        </h3>

        <!-- Tech Stack Badge Showcase -->
        <div class="p-5 rounded-xl border border-purple-900/30 bg-slate-900/60 space-y-3">
          <h4 class="text-xs font-bold uppercase tracking-wider text-amber-200 font-mono">1. Tech Stack Matrix</h4>
          <div class="flex flex-wrap gap-2">
            <span class="px-3 py-1 rounded bg-purple-950 text-amber-100 text-xs border border-purple-700/50">Unity</span>
            <span class="px-3 py-1 rounded bg-purple-950 text-amber-100 text-xs border border-purple-700/50">Unreal Engine</span>
            <span class="px-3 py-1 rounded bg-purple-950 text-amber-100 text-xs border border-purple-700/50">C# / C++</span>
            <span class="px-3 py-1 rounded bg-purple-950 text-amber-100 text-xs border border-purple-700/50">Python</span>
            <span class="px-3 py-1 rounded bg-purple-950 text-amber-100 text-xs border border-purple-700/50">VR / AR / XR</span>
            <span class="px-3 py-1 rounded bg-purple-950 text-amber-100 text-xs border border-purple-700/50">Game QA Automation</span>
            <span class="px-3 py-1 rounded bg-purple-950 text-amber-100 text-xs border border-purple-700/50">AI & Computer Vision</span>
          </div>
        </div>

        <!-- Featured Projects Table Preview -->
        <div class="p-5 rounded-xl border border-purple-900/30 bg-slate-900/60 space-y-3">
          <h4 class="text-xs font-bold uppercase tracking-wider text-amber-200 font-mono">2. Structured Project Highlights</h4>
          <div class="overflow-x-auto">
            <table class="w-full text-left text-xs border-collapse">
              <thead>
                <tr class="border-b border-purple-900/50 text-purple-300 font-mono">
                  <th class="py-2 px-3">Domain</th>
                  <th class="py-2 px-3">Featured Projects</th>
                </tr>
              </thead>
              <tbody class="divide-y divide-purple-950/60 text-slate-300">
                <tr>
                  <td class="py-2.5 px-3 font-semibold text-amber-100">🎮 Game Dev & XR</td>
                  <td class="py-2.5 px-3">Factory Shift, Maze of Echoes, Mental Wellness VR</td>
                </tr>
                <tr>
                  <td class="py-2.5 px-3 font-semibold text-amber-100">🧪 Quality Assurance</td>
                  <td class="py-2.5 px-3">Automated Test Suites, Bug Tracking Pipelines</td>
                </tr>
                <tr>
                  <td class="py-2.5 px-3 font-semibold text-amber-100">🤖 AI & Vision</td>
                  <td class="py-2.5 px-3">XrayDiagnosis (CNN), Celestiy (GenAI Companion)</td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>

        <!-- Connect Buttons Preview -->
        <div class="p-5 rounded-xl border border-purple-900/30 bg-slate-900/60 space-y-3">
          <h4 class="text-xs font-bold uppercase tracking-wider text-amber-200 font-mono">3. Custom Styled Badges</h4>
          <div class="flex flex-wrap gap-3">
            <a href="https://www.linkedin.com/in/razan-alsunaidi/" font-bold inline-flex class="px-4 py-2 rounded-lg bg-purple-700 text-amber-100 text-xs font-semibold hover:bg-purple-600 transition-colors shadow">
              LinkedIn
            </a>
            <a href="https://razanalsunaidi.itch.io/" class="px-4 py-2 rounded-lg bg-amber-100 text-purple-950 text-xs font-bold hover:bg-amber-200 transition-colors shadow">
              itch.io
            </a>
            <a href="https://glitter-snowman-845.notion.site/Razan-Alsunaidi-35bd843cc00680b2b428daf954c2e520?pvs=143" class="px-4 py-2 rounded-lg bg-slate-800 text-purple-200 border border-purple-700/50 text-xs font-semibold hover:bg-slate-700 transition-colors">
              Portfolio
            </a>
          </div>
        </div>

      </div>
    </section>
  </main>

  <!-- Notification Toast -->
  <div id="toast" class="fixed bottom-6 right-6 bg-purple-600 text-white px-5 py-3 rounded-xl shadow-2xl flex items-center gap-3 transform translate-y-20 opacity-0 transition-all duration-300 pointer-events-none z-50">
    <i data-lucide="check-circle-2" class="w-5 h-5 text-amber-200"></i>
    <span id="toastMessage" class="text-xs font-semibold">README Code copied to clipboard!</span>
  </div>

  <script>
    // Initialize Lucide Icons
    lucide.createIcons();

    // Canvas Ambient Glow & Particle Effect
    const canvas = document.getElementById('ambientCanvas');
    const ctx = canvas.getContext('2d');

    function resizeCanvas() {
      canvas.width = canvas.parentElement.clientWidth;
      canvas.height = canvas.parentElement.clientHeight;
    }
    resizeCanvas();
    window.addEventListener('resize', resizeCanvas);

    // Particle class for violet/cream nodes
    class Particle {
      constructor() {
        this.reset();
      }
      reset() {
        this.x = Math.random() * canvas.width;
        this.y = Math.random() * canvas.height;
        this.size = Math.random() * 2 + 1;
        this.speedX = (Math.random() - 0.5) * 0.4;
        this.speedY = (Math.random() - 0.5) * 0.4;
        this.color = Math.random() > 0.3 ? 'rgba(138, 43, 226, ' : 'rgba(245, 245, 220, ';
        this.alpha = Math.random() * 0.5 + 0.2;
      }
      update() {
        this.x += this.speedX;
        this.y += this.speedY;
        if (this.x < 0 || this.x > canvas.width || this.y < 0 || this.y > canvas.height) {
          this.reset();
        }
      }
      draw() {
        ctx.fillStyle = this.color + this.alpha + ')';
        ctx.beginPath();
        ctx.arc(this.x, this.y, this.size, 0, Math.PI * 2);
        ctx.fill();
      }
    }

    const particles = Array.from({ length: 45 }, () => new Particle());

    function animateParticles() {
      ctx.clearRect(0, 0, canvas.width, canvas.height);
      particles.forEach(p => {
        p.update();
        p.draw();
      });
      requestAnimationFrame(animateParticles);
    }
    animateParticles();

    // Typing Effect Logic
    const typingPhrases = [
      "Building Immersive XR & Unity Experiences...",
      "Designing Game QA Automation & Test Suites...",
      "Developing Computer Vision & AI Systems...",
      "Crafting Interactive Games & Mobile Apps..."
    ];
    let phraseIdx = 0;
    let charIdx = 0;
    let isDeleting = false;
    const typingEl = document.getElementById('typingEffectText');

    function typeEffect() {
      const currentPhrase = typingPhrases[phraseIdx];
      
      if (isDeleting) {
        charIdx--;
      } else {
        charIdx++;
      }

      typingEl.textContent = currentPhrase.substring(0, charIdx);

      let speed = isDeleting ? 40 : 80;

      if (!isDeleting && charIdx === currentPhrase.length) {
        speed = 2000;
        isDeleting = true;
      } else if (isDeleting && charIdx === 0) {
        isDeleting = false;
        phraseIdx = (phraseIdx + 1) % typingPhrases.length;
        speed = 500;
      }

      setTimeout(typeEffect, speed);
    }
    typeEffect();

    // Markdown Template String
    const rawMarkdownCode = `<!-- Custom Violet (#8A2BE2) & Cream (#F5F5DC) Banner -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=24&duration=2500&pause=1000&color=8A2BE2&background=F5F5DC00&center=true&vCenter=true&width=650&lines=Razan+Alsunaidi;Game+%26+XR+Developer;QA+%26+Game+Testing+Specialist;AI+%26+Computer+Vision+Engineer;" alt="Razan Alsunaidi Header" />
</p>

<p align="center">
  🎮 <b>Game Dev & XR</b> • 🧪 <b>QA & Software Testing</b> • 🤖 <b>AI & Computer Vision</b>
</p>

---

### 🕹️ Tech Stack & Tools

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=unity,unreal,cs,py,cpp,git,github,figma&theme=dark" />
  </a>
</p>

<p align="center">
  <code>Unity</code> • <code>Unreal Engine</code> • <code>C# / C++</code> • <code>VR / AR / XR</code><br>
  <code>Game QA & Automated Testing</code> • <code>Bug Tracking & Test Cases</code><br>
  <code>Python</code> • <code>AI / ML / Computer Vision</code>
</p>

---

### 🚀 Featured Highlights

| Domain | Projects & Focus |
| :--- | :--- |
| 🎮 **Game Dev & XR** | **Factory Shift** & **Maze of Echoes** (Survival Horror), Mental Wellness VR |
| 🧪 **Quality Assurance** | Test Case Design, Game Testing & Bug Tracking Pipelines |
| 🤖 **AI & Vision** | **XrayDiagnosis** (Deep Learning CNN), Generative AI Companion (**Celestiy**) |
| 📱 **Mobile Apps** | **MothLight** (Gamified Social Skills App) |

---

### 📬 Connect & Portfolio

<p align="center">
  <a href="https://www.linkedin.com/in/razan-alsunaidi/">
    <img src="https://img.shields.io/badge/LinkedIn-8A2BE2?style=for-the-badge&logo=linkedin&logoColor=F5F5DC" />
  </a>
  <a href="https://razanalsunaidi.itch.io/">
    <img src="https://img.shields.io/badge/itch.io-F5F5DC?style=for-the-badge&logo=itch.io&logoColor=8A2BE2" />
  </a>
  <a href="https://glitter-snowman-845.notion.site/Razan-Alsunaidi-35bd843cc00680b2b428daf954c2e520?pvs=143">
    <img src="https://img.shields.io/badge/Portfolio-2A1B3D?style=for-the-badge&logo=notion&logoColor=F5F5DC" />
  </a>
</p>`;

    // Display Markdown Code
    document.getElementById('readmeCodeText').textContent = rawMarkdownCode;

    // Toast Notification helper
    function showToast(msg) {
      const toast = document.getElementById('toast');
      const toastMsg = document.getElementById('toastMessage');
      toastMsg.textContent = msg;
      toast.classList.remove('translate-y-20', 'opacity-0');
      toast.classList.add('translate-y-0', 'opacity-100');

      setTimeout(() => {
        toast.classList.add('translate-y-20', 'opacity-0');
        toast.classList.remove('translate-y-0', 'opacity-100');
      }, 3000);
    }

    // Copy handlers
    document.getElementById('copyMdBtn').addEventListener('click', () => {
      const tempArea = document.createElement('textarea');
      tempArea.value = rawMarkdownCode;
      document.body.appendChild(tempArea);
      tempArea.select();
      document.execCommand('copy');
      document.body.removeChild(tempArea);
      showToast('Full README Code copied successfully!');
    });

    document.getElementById('copyBannerOnlyBtn').addEventListener('click', () => {
      const tempArea = document.createElement('textarea');
      tempArea.value = rawMarkdownCode;
      document.body.appendChild(tempArea);
      tempArea.select();
      document.execCommand('copy');
      document.body.removeChild(tempArea);
      showToast('Markdown code copied!');
    });
  </script>
</body>
</html>
