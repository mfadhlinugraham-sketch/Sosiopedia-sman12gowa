# Sosiopedia-sman12gowa
Aplikaai belajar sosiologi
```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>SOSIOPEDIA - SMAN 12 GOWA | Portal Edukasi Sosiologi</title>
  
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            brand: {
              50: '#f0fdf4',
              100: '#dcfce7',
              500: '#16a34a',
              600: '#15803d',
              700: '#166534',
              800: '#14532d',
              900: '#052e16',
            },
            navy: {
              800: '#1e293b',
              900: '#0f172a'
            }
          },
          fontFamily: {
            sans: ['Inter', 'sans-serif']
          }
        }
      }
    }
  </script>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

  <style>
    body { font-family: 'Inter', sans-serif; background-color: #f8fafc; color: #1e293b; }
    .custom-scroll::-webkit-scrollbar { width: 6px; height: 6px; }
    .custom-scroll::-webkit-scrollbar-track { background: #f1f5f9; }
    .custom-scroll::-webkit-scrollbar-thumb { background: #cbd5e1; border-radius: 9999px; }
    .custom-scroll::-webkit-scrollbar-thumb:hover { background: #94a3b8; }
    .hero-glow {
      background: radial-gradient(circle at 50% 30%, rgba(22, 163, 74, 0.12) 0%, rgba(248, 250, 252, 0) 70%);
    }
  </style>
</head>
<body class="min-h-screen flex flex-col bg-slate-50 antialiased selection:bg-brand-500 selection:text-white">

  <!-- HEADER UTAMA -->
  <header class="sticky top-0 z-40 bg-white/95 backdrop-blur-md border-b border-slate-200 shadow-sm">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
      
      <!-- Identitas Sekolah & Logo -->
      <div onclick="switchTab('home')" class="flex items-center space-x-3.5 cursor-pointer group">
        <div class="w-14 h-14 flex-shrink-0 bg-slate-100 rounded-full p-1 border-2 border-brand-500 shadow-sm flex items-center justify-center overflow-hidden group-hover:scale-105 transition-transform">
          <!-- Vektor Logo Presisi SMAN 12 Gowa -->
          <svg viewBox="0 0 500 500" class="w-full h-full" xmlns="http://www.w3.org/2000/svg">
            <circle cx="250" cy="250" r="240" fill="#c0c0c0" stroke="#dc2626" stroke-width="18" />
            <circle cx="250" cy="250" r="226" fill="#c7c7c7" stroke="#ffffff" stroke-width="6" />
            <path d="M 250,330 A 130,130 0 0,1 250,70 A 130,130 0 0,1 250,330 Z" fill="#facc15" />
            <g stroke="#eab308" stroke-width="7" stroke-linecap="round">
              <line x1="250" y1="200" x2="250" y2="100" />
              <line x1="250" y1="200" x2="280" y2="105" /><line x1="250" y1="200" x2="220" y2="105" />
              <line x1="250" y1="200" x2="310" y2="120" /><line x1="250" y1="200" x2="190" y2="120" />
              <line x1="250" y1="200" x2="335" y2="145" /><line x1="250" y1="200" x2="165" y2="145" />
              <line x1="250" y1="200" x2="350" y2="180" /><line x1="250" y1="200" x2="150" y2="180" />
              <line x1="250" y1="200" x2="355" y2="215" /><line x1="250" y1="200" x2="145" y2="215" />
            </g>
            <path d="M 210,130 Q 240,65 270,115 Q 285,150 250,165 Q 215,160 210,130 Z" fill="#dc2626" />
            <path d="M 205,145 L 190,160 L 220,155 Z" fill="#991b1b" />
            <path d="M 110,315 Q 240,270 380,320 L 370,330 Q 240,290 120,335 Z" fill="#1e293b" />
            <path d="M 125,310 Q 245,268 375,313 Q 250,290 125,310 Z" fill="#ffffff" />
            <text x="250" y="303" font-size="20" font-weight="900" fill="#0f172a" text-anchor="middle" font-family="sans-serif">2008</text>
            <path d="M 345,200 L 320,295 L 305,300 L 325,200 Z" fill="#0f172a" />
            <g fill="#eab308" stroke="#ca8a04" stroke-width="2">
              <ellipse cx="65" cy="240" rx="14" ry="24" transform="rotate(-30 65 240)" />
              <ellipse cx="80" cy="190" rx="14" ry="24" transform="rotate(-20 80 190)" />
              <ellipse cx="105" cy="145" rx="14" ry="24" transform="rotate(-10 105 145)" />
              <ellipse cx="140" cy="110" rx="14" ry="24" transform="rotate(5 140 110)" />
              <ellipse cx="180" cy="85" rx="14" ry="24" transform="rotate(20 180 85)" />
              <ellipse cx="65" cy="295" rx="14" ry="24" transform="rotate(-45 65 295)" />
              <ellipse cx="80" cy="350" rx="14" ry="24" transform="rotate(-60 80 350)" />
              <ellipse cx="115" cy="395" rx="14" ry="24" transform="rotate(-75 115 395)" />
            </g>
            <g fill="#ffffff" stroke="#15803d" stroke-width="4">
              <circle cx="430" cy="240" r="15" /><circle cx="415" cy="190" r="15" />
              <circle cx="390" cy="145" r="15" /><circle cx="355" cy="110" r="15" />
              <circle cx="310" cy="85" r="15" /><circle cx="430" cy="295" r="15" />
              <circle cx="410" cy="350" r="15" /><circle cx="375" cy="395" r="15" />
            </g>
            <text x="250" y="365" font-size="34" font-weight="900" fill="#0f172a" text-anchor="middle" font-family="sans-serif">SMA NEGERI 12</text>
            <text x="250" y="405" font-size="32" font-weight="900" fill="#0f172a" text-anchor="middle" font-family="sans-serif">GOWA</text>
            <path d="M 120,410 Q 250,470 380,410 Q 250,490 120,410 Z" fill="#0f172a" />
            <text x="250" y="450" font-size="20" font-weight="800" fill="#ffffff" text-anchor="middle" font-family="sans-serif" letter-spacing="4">SULAWESI SELATAN</text>
          </svg>
        </div>
        <div>
          <div class="flex items-center space-x-2">
            <span class="text-xs font-black tracking-widest text-brand-600 bg-brand-50 px-2.5 py-0.5 rounded-full border border-brand-200">SOSIOPEDIA</span>
            <span class="text-[11px] font-semibold text-slate-400">SMAN 12 GOWA</span>
          </div>
          <h1 class="text-base sm:text-lg font-black text-slate-800 tracking-tight leading-snug">SMA NEGERI 12 GOWA</h1>
          <p class="text-[11px] text-slate-500 font-medium">Created by: <span class="font-bold text-slate-700">MUH. FADHLI NUGRAHA M</span></p>
        </div>
      </div>

      <!-- Navigasi Menu Desktop & Tombol Admin -->
      <div class="flex items-center space-x-2">
        <nav class="hidden md:flex items-center bg-slate-100 p-1.5 rounded-2xl border border-slate-200 space-x-1">
          <button onclick="switchTab('home')" id="nav-home" class="tab-btn px-4 py-2 rounded-xl text-xs font-bold transition flex items-center space-x-2 bg-brand-600 text-white shadow-sm">
            <i class="fa-solid fa-house"></i>
            <span>Beranda</span>
          </button>
          <button onclick="switchTab('simulasi')" id="nav-simulasi" class="tab-btn px-4 py-2 rounded-xl text-xs font-bold transition flex items-center space-x-2 text-slate-600 hover:text-slate-900 hover:bg-white">
            <i class="fa-solid fa-graduation-cap"></i>
            <span>Simulasi TKA</span>
          </button>
          <button onclick="switchTab('materi')" id="nav-materi" class="tab-btn px-4 py-2 rounded-xl text-xs font-bold transition flex items-center space-x-2 text-slate-600 hover:text-slate-900 hover:bg-white">
            <i class="fa-solid fa-book-open"></i>
            <span>Materi</span>
          </button>
          <button onclick="switchTab('assessment')" id="nav-assessment" class="tab-btn px-4 py-2 rounded-xl text-xs font-bold transition flex items-center space-x-2 text-slate-600 hover:text-slate-900 hover:bg-white">
            <i class="fa-solid fa-file-signature text-amber-500"></i>
            <span>Assessment</span>
          </button>
          <button onclick="switchTab('quiz')" id="nav-quiz" class="tab-btn px-4 py-2 rounded-xl text-xs font-bold transition flex items-center space-x-2 text-slate-600 hover:text-slate-900 hover:bg-white">
            <i class="fa-solid fa-gamepad"></i>
            <span>Kuis & Game</span>
          </button>
          <button onclick="switchTab('siswa')" id="nav-siswa" class="tab-btn px-4 py-2 rounded-xl text-xs font-bold transition flex items-center space-x-2 text-slate-600 hover:text-slate-900 hover:bg-white">
            <i class="fa-solid fa-users"></i>
            <span>Data Siswa</span>
          </button>
        </nav>

        <!-- Tombol Admin Guru (PIN Protected: 2202) -->
        <button onclick="requireTeacherAccess('adminPanel')" title="Akses Pengaturan Guru" class="p-2.5 sm:px-3 sm:py-2 bg-slate-100 hover:bg-slate-200 text-slate-700 rounded-xl border border-slate-300 font-bold text-xs flex items-center space-x-1.5 transition">
          <i class="fa-solid fa-lock text-slate-500"></i>
          <span class="hidden sm:inline">Panel Guru</span>
        </button>
      </div>
    </div>

    <!-- Navigasi Mobile Bawah Header -->
    <div class="md:hidden flex items-center justify-around border-t border-slate-200 bg-white px-2 py-2 overflow-x-auto">
      <button onclick="switchTab('home')" id="mob-home" class="flex-1 py-1.5 px-2 text-center text-xs font-bold text-brand-600 border-b-2 border-brand-600 whitespace-nowrap">
        <i class="fa-solid fa-house block text-sm mb-0.5"></i>Beranda
      </button>
      <button onclick="switchTab('simulasi')" id="mob-simulasi" class="flex-1 py-1.5 px-2 text-center text-xs font-bold text-slate-500 hover:text-slate-800 whitespace-nowrap">
        <i class="fa-solid fa-graduation-cap block text-sm mb-0.5"></i>Simulasi
      </button>
      <button onclick="switchTab('materi')" id="mob-materi" class="flex-1 py-1.5 px-2 text-center text-xs font-bold text-slate-500 hover:text-slate-800 whitespace-nowrap">
        <i class="fa-solid fa-book-open block text-sm mb-0.5"></i>Materi
      </button>
      <button onclick="switchTab('assessment')" id="mob-assessment" class="flex-1 py-1.5 px-2 text-center text-xs font-bold text-slate-500 hover:text-slate-800 whitespace-nowrap">
        <i class="fa-solid fa-file-signature block text-sm mb-0.5 text-amber-500"></i>Asesmen
      </button>
      <button onclick="switchTab('quiz')" id="mob-quiz" class="flex-1 py-1.5 px-2 text-center text-xs font-bold text-slate-500 hover:text-slate-800 whitespace-nowrap">
        <i class="fa-solid fa-gamepad block text-sm mb-0.5"></i>Kuis
      </button>
      <button onclick="switchTab('siswa')" id="mob-siswa" class="flex-1 py-1.5 px-2 text-center text-xs font-bold text-slate-500 hover:text-slate-800 whitespace-nowrap">
        <i class="fa-solid fa-users block text-sm mb-0.5"></i>Siswa
      </button>
    </div>
  </header>

  <!-- KONTEN UTAMA -->
  <main class="flex-1 max-w-7xl w-full mx-auto p-4 sm:p-6 lg:p-8">

    <!-- TAB 0: BERANDA -->
    <section id="tab-home-content" class="tab-pane block space-y-10 hero-glow py-4 sm:py-8">
      <div class="max-w-4xl mx-auto text-center space-y-6">
        <div class="w-32 h-32 sm:w-40 sm:h-40 mx-auto bg-white rounded-full p-2.5 shadow-xl border-4 border-brand-500 flex items-center justify-center transform hover:scale-105 transition duration-300">
          <svg viewBox="0 0 500 500" class="w-full h-full" xmlns="http://www.w3.org/2000/svg">
            <circle cx="250" cy="250" r="240" fill="#c0c0c0" stroke="#dc2626" stroke-width="18" />
            <circle cx="250" cy="250" r="226" fill="#c7c7c7" stroke="#ffffff" stroke-width="6" />
            <path d="M 250,330 A 130,130 0 0,1 250,70 A 130,130 0 0,1 250,330 Z" fill="#facc15" />
            <g stroke="#eab308" stroke-width="7" stroke-linecap="round">
              <line x1="250" y1="200" x2="250" y2="100" /><line x1="250" y1="200" x2="280" y2="105" /><line x1="250" y1="200" x2="220" y2="105" />
              <line x1="250" y1="200" x2="310" y2="120" /><line x1="250" y1="200" x2="190" y2="120" />
              <line x1="250" y1="200" x2="335" y2="145" /><line x1="250" y1="200" x2="165" y2="145" />
              <line x1="250" y1="200" x2="350" y2="180" /><line x1="250" y1="200" x2="150" y2="180" />
              <line x1="250" y1="200" x2="355" y2="215" /><line x1="250" y1="200" x2="145" y2="215" />
            </g>
            <path d="M 210,130 Q 240,65 270,115 Q 285,150 250,165 Q 215,160 210,130 Z" fill="#dc2626" />
            <path d="M 205,145 L 190,160 L 220,155 Z" fill="#991b1b" />
            <path d="M 110,315 Q 240,270 380,320 L 370,330 Q 240,290 120,335 Z" fill="#1e293b" />
            <path d="M 125,310 Q 245,268 375,313 Q 250,290 125,310 Z" fill="#ffffff" />
            <text x="250" y="303" font-size="20" font-weight="900" fill="#0f172a" text-anchor="middle" font-family="sans-serif">2008</text>
            <path d="M 345,200 L 320,295 L 305,300 L 325,200 Z" fill="#0f172a" />
            <g fill="#eab308" stroke="#ca8a04" stroke-width="2">
              <ellipse cx="65" cy="240" rx="14" ry="24" transform="rotate(-30 65 240)" />
              <ellipse cx="80" cy="190" rx="14" ry="24" transform="rotate(-20 80 190)" />
              <ellipse cx="105" cy="145" rx="14" ry="24" transform="rotate(-10 105 145)" />
              <ellipse cx="140" cy="110" rx="14" ry="24" transform="rotate(5 140 110)" />
              <ellipse cx="180" cy="85" rx="14" ry="24" transform="rotate(20 180 85)" />
              <ellipse cx="65" cy="295" rx="14" ry="24" transform="rotate(-45 65 295)" />
              <ellipse cx="80" cy="350" rx="14" ry="24" transform="rotate(-60 80 350)" />
              <ellipse cx="115" cy="395" rx="14" ry="24" transform="rotate(-75 115 395)" />
            </g>
            <g fill="#ffffff" stroke="#15803d" stroke-width="4">
              <circle cx="430" cy="240" r="15" /><circle cx="415" cy="190" r="15" />
              <circle cx="390" cy="145" r="15" /><circle cx="355" cy="110" r="15" />
              <circle cx="310" cy="85" r="15" /><circle cx="430" cy="295" r="15" />
              <circle cx="410" cy="350" r="15" /><circle cx="375" cy="395" r="15" />
            </g>
            <text x="250" y="365" font-size="34" font-weight="900" fill="#0f172a" text-anchor="middle" font-family="sans-serif">SMA NEGERI 12</text>
            <text x="250" y="405" font-size="32" font-weight="900" fill="#0f172a" text-anchor="middle" font-family="sans-serif">GOWA</text>
            <path d="M 120,410 Q 250,470 380,410 Q 250,490 120,410 Z" fill="#0f172a" />
            <text x="250" y="450" font-size="20" font-weight="800" fill="#ffffff" text-anchor="middle" font-family="sans-serif" letter-spacing="4">SULAWESI SELATAN</text>
          </svg>
        </div>

        <div class="space-y-3">
          <div class="inline-flex items-center space-x-2 px-3.5 py-1.5 rounded-full bg-brand-100/80 border border-brand-300 text-brand-800 text-xs font-black tracking-wide">
            <i class="fa-solid fa-graduation-cap text-brand-700"></i>
            <span>PORTAL RESMI PEMBELAJARAN SOSIOLOGI</span>
          </div>
          <h2 class="text-4xl sm:text-6xl font-black text-slate-900 tracking-tight">
            <span class="bg-gradient-to-r from-brand-600 via-emerald-600 to-teal-700 bg-clip-text text-transparent">SOSIOPEDIA</span>
          </h2>
          <h3 class="text-xl sm:text-2xl font-extrabold text-slate-800">SMA NEGERI 12 GOWA</h3>
          <p class="text-xs sm:text-sm font-semibold text-slate-600 uppercase tracking-widest">
            Created by: <span class="text-brand-700 font-black">MUH. FADHLI NUGRAHA M</span>
          </p>
          <p class="text-slate-600 text-sm sm:text-base max-w-2xl mx-auto leading-relaxed pt-2">
            Selamat datang di media pembelajaran interaktif sosiologi. Tingkatkan pemahaman konsep masyarakat, hadapi simulasi Tes Kemampuan Akademik (TKA) 2026, dan uji nalar kritis melalui studi kasus terstruktur.
          </p>
        </div>

        <div class="flex flex-wrap items-center justify-center gap-3 pt-2">
          <button onclick="switchTab('simulasi')" class="px-7 py-3.5 bg-brand-600 hover:bg-brand-700 text-white font-extrabold rounded-2xl text-sm shadow-lg shadow-brand-600/25 transition transform active:scale-95 flex items-center space-x-2">
            <i class="fa-solid fa-play"></i>
            <span>Mulai Simulasi TKA 2026</span>
          </button>
          <button onclick="switchTab('materi')" class="px-7 py-3.5 bg-white hover:bg-slate-100 text-slate-800 font-extrabold rounded-2xl text-sm border-2 border-slate-300 shadow-sm transition flex items-center space-x-2">
            <i class="fa-solid fa-book-open text-brand-600"></i>
            <span>Jelajahi Modul Materi</span>
          </button>
          <button onclick="switchTab('assessment')" class="px-7 py-3.5 bg-amber-500 hover:bg-amber-600 text-white font-extrabold rounded-2xl text-sm shadow-md transition flex items-center space-x-2">
            <i class="fa-solid fa-file-signature"></i>
            <span>Menu Assessment</span>
          </button>
        </div>
      </div>

      <!-- KARTU MENU NAVIGASI UTAMA (5 Kolom Seimbang) -->
      <div class="pt-6 max-w-6xl mx-auto">
        <div class="text-center mb-6">
          <h4 class="text-xs font-black uppercase tracking-widest text-slate-400">PILIHAN MENU SOSIOPEDIA</h4>
          <p class="text-lg font-black text-slate-800">Akses Cepat Fitur Pembelajaran</p>
        </div>

        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-5 gap-4">
          <div onclick="switchTab('simulasi')" class="group cursor-pointer bg-white rounded-3xl p-5 border-2 border-slate-200 hover:border-brand-500 shadow-sm hover:shadow-xl transition-all duration-300 flex flex-col justify-between space-y-4">
            <div class="w-12 h-12 rounded-2xl bg-brand-50 border border-brand-200 flex items-center justify-center text-brand-600 text-xl font-black group-hover:bg-brand-600 group-hover:text-white transition">
              <i class="fa-solid fa-graduation-cap"></i>
            </div>
            <div>
              <span class="text-[10px] font-black uppercase text-brand-600 tracking-wider">Ujian Mandiri</span>
              <h5 class="text-base font-black text-slate-800 group-hover:text-brand-700 transition">Simulasi TKA</h5>
              <p class="text-xs text-slate-500 mt-1.5 leading-relaxed">40 Butir soal TKA 2026 resmi, opsi teracak otomatis, skor instan, dan pembahasan.</p>
            </div>
            <div class="pt-2 flex items-center text-xs font-bold text-brand-600 space-x-1 group-hover:translate-x-1 transition-transform">
              <span>Buka Simulasi</span>
              <i class="fa-solid fa-arrow-right text-[10px]"></i>
            </div>
          </div>

          <div onclick="switchTab('materi')" class="group cursor-pointer bg-white rounded-3xl p-5 border-2 border-slate-200 hover:border-emerald-500 shadow-sm hover:shadow-xl transition-all duration-300 flex flex-col justify-between space-y-4">
            <div class="w-12 h-12 rounded-2xl bg-emerald-50 border border-emerald-200 flex items-center justify-center text-emerald-600 text-xl font-black group-hover:bg-emerald-600 group-hover:text-white transition">
              <i class="fa-solid fa-book-open"></i>
            </div>
            <div>
              <span class="text-[10px] font-black uppercase text-emerald-600 tracking-wider">Materi Pokok</span>
              <h5 class="text-base font-black text-slate-800 group-hover:text-emerald-700 transition">Materi Pelajaran</h5>
              <p class="text-xs text-slate-500 mt-1.5 leading-relaxed">3 Modul Pokok: Pengelompokan, Masalah Kelompok, & Kesetaraan Keberagaman.</p>
            </div>
            <div class="pt-2 flex items-center text-xs font-bold text-emerald-600 space-x-1 group-hover:translate-x-1 transition-transform">
              <span>Pelajari Modul</span>
              <i class="fa-solid fa-arrow-right text-[10px]"></i>
            </div>
          </div>

          <div onclick="switchTab('assessment')" class="group cursor-pointer bg-white rounded-3xl p-5 border-2 border-slate-200 hover:border-amber-500 shadow-sm hover:shadow-xl transition-all duration-300 flex flex-col justify-between space-y-4">
            <div class="w-12 h-12 rounded-2xl bg-amber-50 border border-amber-200 flex items-center justify-center text-amber-600 text-xl font-black group-hover:bg-amber-600 group-hover:text-white transition">
              <i class="fa-solid fa-file-signature"></i>
            </div>
            <div>
              <span class="text-[10px] font-black uppercase text-amber-600 tracking-wider">Evaluasi Guru</span>
              <h5 class="text-base font-black text-slate-800 group-hover:text-amber-700 transition">Assessment</h5>
              <p class="text-xs text-slate-500 mt-1.5 leading-relaxed">Gerbang asesmen terproteksi kode guru (SMAN12) untuk evaluasi berkala.</p>
            </div>
            <div class="pt-2 flex items-center text-xs font-bold text-amber-600 space-x-1 group-hover:translate-x-1 transition-transform">
              <span>Buka Asesmen</span>
              <i class="fa-solid fa-arrow-right text-[10px]"></i>
            </div>
          </div>

          <div onclick="switchTab('quiz')" class="group cursor-pointer bg-white rounded-3xl p-5 border-2 border-slate-200 hover:border-rose-500 shadow-sm hover:shadow-xl transition-all duration-300 flex flex-col justify-between space-y-4">
            <div class="w-12 h-12 rounded-2xl bg-rose-50 border border-rose-200 flex items-center justify-center text-rose-600 text-xl font-black group-hover:bg-rose-600 group-hover:text-white transition">
              <i class="fa-solid fa-gamepad"></i>
            </div>
            <div>
              <span class="text-[10px] font-black uppercase text-rose-600 tracking-wider">Asah Otak</span>
              <h5 class="text-base font-black text-slate-800 group-hover:text-rose-700 transition">Kuis & Game</h5>
              <p class="text-xs text-slate-500 mt-1.5 leading-relaxed">Pilihan ganda cepat, kuis benar/salah, serta TTS santai berkuota bantuan.</p>
            </div>
            <div class="pt-2 flex items-center text-xs font-bold text-rose-600 space-x-1 group-hover:translate-x-1 transition-transform">
              <span>Mainkan Game</span>
              <i class="fa-solid fa-arrow-right text-[10px]"></i>
            </div>
          </div>

          <div onclick="switchTab('siswa')" class="group cursor-pointer bg-white rounded-3xl p-5 border-2 border-slate-200 hover:border-blue-500 shadow-sm hover:shadow-xl transition-all duration-300 flex flex-col justify-between space-y-4">
            <div class="w-12 h-12 rounded-2xl bg-blue-50 border border-blue-200 flex items-center justify-center text-blue-600 text-xl font-black group-hover:bg-blue-600 group-hover:text-white transition">
              <i class="fa-solid fa-users"></i>
            </div>
            <div>
              <span class="text-[10px] font-black uppercase text-blue-600 tracking-wider">Direktori</span>
              <h5 class="text-base font-black text-slate-800 group-hover:text-blue-700 transition">Data Siswa</h5>
              <p class="text-xs text-slate-500 mt-1.5 leading-relaxed">Daftar kelas XII IPS 1-2 & IPA 1-3, pencarian NIS, dan ekspor rekap CSV.</p>
            </div>
            <div class="pt-2 flex items-center text-xs font-bold text-blue-600 space-x-1 group-hover:translate-x-1 transition-transform">
              <span>Lihat Siswa</span>
              <i class="fa-solid fa-arrow-right text-[10px]"></i>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- TAB ASSESSMENT: KODE AKSES TERPROTEKSI & SOAL KOSONG (STANDBY) -->
    <section id="tab-assessment-content" class="tab-pane hidden space-y-6">
      <div id="assessment-auth-pane" class="max-w-xl mx-auto bg-white rounded-3xl p-6 sm:p-8 border border-slate-200 shadow-md space-y-6">
        <div class="text-center space-y-2">
          <div class="w-14 h-14 mx-auto rounded-2xl bg-amber-50 border border-amber-200 flex items-center justify-center text-amber-600 text-2xl font-black">
            <i class="fa-solid fa-shield-halved"></i>
          </div>
          <span class="px-3 py-1 bg-amber-100 text-amber-800 text-[10px] font-black rounded-full uppercase tracking-wider">Evaluasi Belajar Terproteksi</span>
          <h3 class="text-xl font-black text-slate-800">ASSESSMENT SOSIOLOGI</h3>
          <p class="text-xs text-slate-500">Masukkan kode akses resmi dari Guru (SMAN12) untuk membuka sesi asesmen.</p>
        </div>

        <div class="space-y-4">
          <div>
            <label class="block text-xs font-bold text-slate-700 mb-1.5">
              <i class="fa-solid fa-key text-amber-500 mr-1"></i> Kode Akses dari Guru:
            </label>
            <input type="text" id="assessment-input-code" placeholder="Ketik kode akses (Contoh: SMAN12)" autocomplete="off"
              onkeydown="if(event.key === 'Enter') verifyAssessmentAccess();"
              class="w-full p-3.5 bg-slate-50 border-2 border-slate-300 focus:border-amber-500 rounded-2xl text-xs sm:text-sm font-black tracking-widest uppercase outline-none text-slate-800">
            <p id="assessment-code-error" class="hidden text-rose-600 text-[11px] font-bold mt-1.5 flex items-center space-x-1">
              <i class="fa-solid fa-circle-exclamation"></i>
              <span>Kode akses salah! Pastikan memasukkan kode resmi dari guru (SMAN12).</span>
            </p>
          </div>

          <div>
            <label class="block text-xs font-bold text-slate-700 mb-1.5">
              <i class="fa-solid fa-user text-slate-400 mr-1"></i> Nama Lengkap Siswa:
            </label>
            <input type="text" id="assessment-input-nama" placeholder="Ketik nama lengkap Anda..."
              class="w-full p-3.5 bg-slate-50 border border-slate-300 rounded-2xl text-xs sm:text-sm font-semibold outline-none focus:ring-2 focus:ring-amber-500 text-slate-800">
          </div>

          <div>
            <label class="block text-xs font-bold text-slate-700 mb-1.5">
              <i class="fa-solid fa-chalkboard-user text-slate-400 mr-1"></i> Pilih Rombongan Belajar (Kelas):
            </label>
            <select id="assessment-input-kelas" class="w-full p-3.5 bg-slate-50 border border-slate-300 rounded-2xl text-xs sm:text-sm font-semibold outline-none focus:ring-2 focus:ring-amber-500 text-slate-800">
              <option value="">-- Pilih Kelas --</option>
              <option value="XII IPS 1">XII IPS 1</option>
              <option value="XII IPS 2">XII IPS 2</option>
              <option value="XII IPA 1">XII IPA 1</option>
              <option value="XII IPA 2">XII IPA 2</option>
              <option value="XII IPA 3">XII IPA 3</option>
            </select>
          </div>

          <div class="p-4 bg-amber-50/70 border border-amber-200 rounded-2xl text-amber-900 text-xs space-y-1">
            <p class="font-bold flex items-center space-x-1.5">
              <i class="fa-solid fa-circle-info text-amber-600"></i>
              <span>Status Asesmen:</span>
            </p>
            <p class="text-[11px] text-amber-800 leading-relaxed">
              Ruang asesmen ini diproteksi oleh Guru pengampu mata pelajaran Sosiologi SMA Negeri 12 Gowa.
            </p>
          </div>

          <button onclick="verifyAssessmentAccess()" class="w-full py-3.5 bg-gradient-to-r from-amber-500 to-amber-600 hover:from-amber-600 hover:to-amber-700 text-white font-extrabold rounded-2xl text-sm shadow-md transition transform active:scale-95 flex items-center justify-center space-x-2">
            <span>Buka & Masuk Asesmen</span>
            <i class="fa-solid fa-arrow-right"></i>
          </button>
        </div>
      </div>

      <div id="assessment-exam-pane" class="hidden max-w-2xl mx-auto space-y-6">
        <div class="bg-white rounded-3xl p-8 border border-slate-200 shadow-sm text-center space-y-6">
          <div class="w-20 h-20 mx-auto rounded-3xl bg-amber-50 border-2 border-amber-300 flex items-center justify-center text-amber-600 text-3xl font-black">
            <i class="fa-regular fa-folder-open"></i>
          </div>

          <div class="space-y-2">
            <span class="px-3 py-1 bg-amber-100 text-amber-800 rounded-full text-xs font-black uppercase tracking-wider">
              Ruang Asesmen Aktif
            </span>
            <h3 class="text-xl sm:text-2xl font-black text-slate-800">Bank Soal Belum Dirilis Guru</h3>
            <p class="text-xs sm:text-sm text-slate-500 max-w-md mx-auto leading-relaxed">
              Halo, <b id="assessment-display-name" class="text-slate-800">-</b> (<span id="assessment-display-kelas" class="text-amber-700 font-bold">-</span>)! Kode akses <b>SMAN12</b> berhasil diverifikasi. Saat ini butir soal asesmen masih dalam tahap penyusunan oleh guru pengampu dan akan segera diaktifkan saat jam evaluasi dimulai.
            </p>
          </div>

          <div class="p-4 bg-slate-50 rounded-2xl border border-slate-200 text-slate-600 text-xs space-y-2 text-left max-w-md mx-auto">
            <div class="flex items-center space-x-2 font-bold text-slate-800">
              <i class="fa-solid fa-circle-check text-brand-600"></i>
              <span>Status Pendaftaran Terverifikasi</span>
            </div>
            <p class="text-[11px] text-slate-500">
              Sistem telah mendeteksi identitas Anda. Sembari menunggu guru mengunggah naskah soal asesmen, Anda dapat mempelajari kembali Modul Pembelajaran atau mencoba Simulasi TKA 2026.
            </p>
          </div>

          <div class="flex flex-wrap items-center justify-center gap-3 pt-2">
            <button onclick="switchTab('materi')" class="px-6 py-2.5 bg-brand-600 hover:bg-brand-700 text-white rounded-xl text-xs font-bold transition flex items-center space-x-2 shadow-sm">
              <i class="fa-solid fa-book-open"></i>
              <span>Baca Modul Materi</span>
            </button>
            <button onclick="resetAssessment()" class="px-6 py-2.5 bg-slate-100 hover:bg-slate-200 text-slate-700 rounded-xl text-xs font-bold transition flex items-center space-x-2">
              <i class="fa-solid fa-arrow-left"></i>
              <span>Kembali</span>
            </button>
          </div>
        </div>
      </div>
    </section>

    <!-- TAB 1: SIMULASI TKA 2026 -->
    <section id="tab-simulasi-content" class="tab-pane hidden space-y-6">
      <div id="simulasi-reg-pane" class="max-w-xl mx-auto bg-white rounded-3xl p-6 sm:p-8 border border-slate-200 shadow-md space-y-6">
        <div class="text-center space-y-2">
          <div class="w-14 h-14 mx-auto rounded-2xl bg-brand-50 border border-brand-200 flex items-center justify-center text-brand-600 text-2xl font-black">
            <i class="fa-solid fa-user-pen"></i>
          </div>
          <h3 class="text-xl font-black text-slate-800">Registrasi Simulasi TKA 2026</h3>
          <p class="text-xs text-slate-500">Silakan masukkan identitas diri sebelum memulai 40 butir soal sosiologi.</p>
        </div>

        <div class="space-y-4">
          <div>
            <label class="block text-xs font-bold text-slate-700 mb-1.5">Nama Lengkap Siswa:</label>
            <input type="text" id="sim-input-nama" placeholder="Ketik nama lengkap Anda..."
              class="w-full p-3.5 bg-slate-50 border border-slate-300 rounded-2xl text-xs sm:text-sm font-semibold outline-none focus:ring-2 focus:ring-brand-500 text-slate-800">
          </div>
          <div>
            <label class="block text-xs font-bold text-slate-700 mb-1.5">Pilih Rombongan Belajar (Kelas):</label>
            <select id="sim-input-kelas" class="w-full p-3.5 bg-slate-50 border border-slate-300 rounded-2xl text-xs sm:text-sm font-semibold outline-none focus:ring-2 focus:ring-brand-500 text-slate-800">
              <option value="">-- Pilih Kelas --</option>
              <option value="XII IPS 1">XII IPS 1</option>
              <option value="XII IPS 2">XII IPS 2</option>
              <option value="XII IPA 1">XII IPA 1</option>
              <option value="XII IPA 2">XII IPA 2</option>
              <option value="XII IPA 3">XII IPA 3</option>
            </select>
          </div>

          <div class="p-4 bg-amber-50 border border-amber-200 rounded-2xl text-amber-900 text-xs space-y-1">
            <p class="font-bold flex items-center space-x-1.5">
              <i class="fa-solid fa-circle-info text-amber-600"></i>
              <span>Petunjuk Simulasi TKA 2026:</span>
            </p>
            <ul class="list-disc list-inside space-y-0.5 text-[11px] text-amber-800">
              <li>Jumlah soal 40 butir pilihan ganda (A, B, C, D, E).</li>
              <li>Opsi jawaban teracak secara otomatis untuk setiap peserta.</li>
              <li>Skor akhir (0–100) dan lembar ulasan pembahasan tampil di akhir ujian.</li>
            </ul>
          </div>

          <button onclick="startSimulation()" class="w-full py-3.5 bg-brand-600 hover:bg-brand-700 text-white font-extrabold rounded-2xl text-sm shadow-md transition transform active:scale-95 flex items-center justify-center space-x-2">
            <span>Mulai Ujian Sekarang</span>
            <i class="fa-solid fa-arrow-right"></i>
          </button>
        </div>
      </div>

      <div id="simulasi-exam-pane" class="hidden space-y-6">
        <div class="bg-white rounded-2xl p-4 border border-slate-200 shadow-sm flex flex-wrap items-center justify-between gap-3">
          <div class="flex items-center space-x-3">
            <div class="w-10 h-10 rounded-xl bg-brand-50 border border-brand-200 flex items-center justify-center text-brand-600 font-black text-sm">
              <i class="fa-solid fa-user-graduate"></i>
            </div>
            <div>
              <p class="text-xs font-bold text-slate-800" id="exam-display-name">Peserta Ujian</p>
              <p class="text-[11px] font-semibold text-brand-600" id="exam-display-kelas">Kelas: -</p>
            </div>
          </div>
          <div class="flex items-center space-x-2">
            <span class="text-xs font-bold text-slate-500">Soal:</span>
            <span class="px-3 py-1 bg-slate-100 rounded-lg text-xs font-black text-slate-800" id="exam-progress-counter">1 / 40</span>
          </div>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-12 gap-6">
          <div class="lg:col-span-8 bg-white rounded-3xl p-6 sm:p-8 border border-slate-200 shadow-sm space-y-6">
            <div class="flex items-center justify-between border-b border-slate-100 pb-3">
              <span class="px-3 py-1 bg-brand-50 border border-brand-200 text-brand-700 rounded-full text-[11px] font-black uppercase tracking-wider" id="exam-question-category">
                Kategori Soal
              </span>
              <span class="text-xs font-bold text-slate-400" id="exam-question-num-tag">Nomor 1</span>
            </div>

            <p class="text-sm sm:text-base font-semibold text-slate-800 leading-relaxed" id="exam-question-text">
              Memuat naskah soal sosiologi...
            </p>

            <div class="space-y-3 pt-2" id="exam-options-container"></div>

            <div class="flex items-center justify-between pt-4 border-t border-slate-100">
              <button onclick="prevQuestion()" id="btn-prev-q" class="px-5 py-2.5 bg-slate-100 hover:bg-slate-200 text-slate-700 rounded-xl text-xs font-bold transition flex items-center space-x-1.5">
                <i class="fa-solid fa-arrow-left"></i>
                <span>Sebelumnya</span>
              </button>
              <button onclick="nextQuestion()" id="btn-next-q" class="px-6 py-2.5 bg-brand-600 hover:bg-brand-700 text-white rounded-xl text-xs font-bold transition flex items-center space-x-1.5">
                <span>Berikutnya</span>
                <i class="fa-solid fa-arrow-right"></i>
              </button>
            </div>
          </div>

          <div class="lg:col-span-4 bg-white rounded-3xl p-5 border border-slate-200 shadow-sm space-y-4">
            <div class="flex items-center justify-between pb-3 border-b border-slate-100">
              <h4 class="text-xs font-bold text-slate-800 uppercase tracking-wider">Palet Nomor Soal</h4>
              <span class="text-[11px] font-semibold text-slate-400">40 Butir</span>
            </div>

            <div class="grid grid-cols-5 sm:grid-cols-8 lg:grid-cols-5 gap-2" id="exam-palette-grid"></div>

            <div class="pt-3 border-t border-slate-100 space-y-2">
              <div class="flex items-center justify-between text-[11px] text-slate-500 font-medium">
                <span class="flex items-center space-x-1.5"><span class="w-3 h-3 rounded-full bg-brand-600 inline-block"></span><span>Sudah Terjawab</span></span>
                <span class="flex items-center space-x-1.5"><span class="w-3 h-3 rounded-full bg-slate-100 border border-slate-300 inline-block"></span><span>Belum</span></span>
              </div>
              <button onclick="finishExam()" class="w-full py-3 bg-rose-600 hover:bg-rose-700 text-white rounded-xl text-xs font-extrabold transition shadow-sm flex items-center justify-center space-x-2">
                <i class="fa-solid fa-check-double"></i>
                <span>Kumpulkan Jawaban</span>
              </button>
            </div>
          </div>
        </div>
      </div>

      <div id="simulasi-result-pane" class="hidden space-y-8">
        <div class="max-w-2xl mx-auto bg-white rounded-3xl p-6 sm:p-8 border border-slate-200 shadow-md text-center space-y-6">
          <div class="w-16 h-16 mx-auto rounded-full bg-brand-50 border-2 border-brand-500 flex items-center justify-center text-brand-600 text-3xl font-black">
            <i class="fa-solid fa-trophy"></i>
          </div>

          <div class="space-y-1">
            <span class="text-[11px] font-black uppercase text-brand-600 tracking-wider">HASIL AKHIR SIMULASI TKA 2026</span>
            <h3 class="text-2xl font-black text-slate-800" id="result-student-name">Nama Peserta</h3>
            <p class="text-xs font-bold text-slate-500" id="result-student-kelas">Kelas: -</p>
          </div>

          <div class="py-4 bg-slate-50 rounded-2xl border border-slate-200 max-w-sm mx-auto">
            <span class="text-xs font-bold text-slate-400 uppercase tracking-widest block">Skor Kemampuan Akademik</span>
            <span class="text-5xl font-black text-brand-600 tracking-tight" id="result-final-score">0</span>
            <span class="text-xs font-bold text-slate-400 block mt-1">Skala 0 - 100</span>
          </div>

          <div class="grid grid-cols-3 gap-3 max-w-md mx-auto text-center text-xs">
            <div class="p-3 bg-emerald-50 border border-emerald-200 rounded-xl">
              <span class="text-emerald-700 font-bold block">Benar</span>
              <span class="text-lg font-black text-emerald-800" id="result-correct-count">0</span>
            </div>
            <div class="p-3 bg-rose-50 border border-rose-200 rounded-xl">
              <span class="text-rose-700 font-bold block">Salah</span>
              <span class="text-lg font-black text-rose-800" id="result-wrong-count">0</span>
            </div>
            <div class="p-3 bg-slate-50 border border-slate-200 rounded-xl">
              <span class="text-slate-600 font-bold block">Kosong</span>
              <span class="text-lg font-black text-slate-700" id="result-empty-count">0</span>
            </div>
          </div>

          <div class="flex flex-wrap items-center justify-center gap-3 pt-2">
            <button onclick="resetSimulation()" class="px-6 py-2.5 bg-brand-600 hover:bg-brand-700 text-white rounded-xl text-xs font-bold transition flex items-center space-x-2">
              <i class="fa-solid fa-rotate-left"></i>
              <span>Ulangi Simulasi</span>
            </button>
            <button onclick="switchTab('home')" class="px-6 py-2.5 bg-slate-100 hover:bg-slate-200 text-slate-700 rounded-xl text-xs font-bold transition flex items-center space-x-2">
              <i class="fa-solid fa-house"></i>
              <span>Kembali ke Beranda</span>
            </button>
          </div>
        </div>

        <div class="max-w-4xl mx-auto space-y-4">
          <div class="flex items-center justify-between pb-2 border-b border-slate-200">
            <h4 class="text-base font-black text-slate-800 flex items-center space-x-2">
              <i class="fa-solid fa-book-open text-brand-600"></i>
              <span>Lembar Ulasan & Pembahasan Soal</span>
            </h4>
            <span class="text-xs font-semibold text-slate-400">40 Butir Soal</span>
          </div>
          <div class="space-y-4" id="review-items-container"></div>
        </div>
      </div>
    </section>

    <!-- TAB 2: MATERI -->
    <section id="tab-materi-content" class="tab-pane hidden space-y-6">
      <div class="flex flex-wrap items-center justify-between gap-3 border-b border-slate-200 pb-4">
        <div class="flex flex-wrap items-center gap-2">
          <button onclick="switchMateriSub('daftar')" id="subnav-daftar" class="px-4 py-2 rounded-xl text-xs font-bold transition bg-slate-800 text-white flex items-center space-x-2">
            <i class="fa-solid fa-list-check"></i>
            <span>Daftar Modul Pembelajaran</span>
          </button>
          <button onclick="switchMateriSub('pengelompokan')" id="subnav-pengelompokan" class="px-4 py-2 rounded-xl text-xs font-bold transition bg-white text-slate-700 border border-slate-200 hover:bg-slate-50 flex items-center space-x-1.5">
            <span class="w-2 h-2 rounded-full bg-brand-500"></span>
            <span>Pengelompokan Sosial</span>
          </button>
          <button onclick="switchMateriSub('permasalahan')" id="subnav-permasalahan" class="px-4 py-2 rounded-xl text-xs font-bold transition bg-white text-slate-700 border border-slate-200 hover:bg-slate-50 flex items-center space-x-1.5">
            <span class="w-2 h-2 rounded-full bg-rose-500"></span>
            <span>Permasalahan Sosial Kelompok</span>
          </button>
          <button onclick="switchMateriSub('kesetaraan')" id="subnav-kesetaraan" class="px-4 py-2 rounded-xl text-xs font-bold transition bg-white text-slate-700 border border-slate-200 hover:bg-slate-50 flex items-center space-x-1.5">
            <span class="w-2 h-2 rounded-full bg-indigo-500"></span>
            <span>Kesetaraan & Keberagaman</span>
          </button>
        </div>
      </div>

      <div id="view-materi-daftar" class="space-y-6">
        <div class="text-left space-y-1">
          <h3 class="text-lg font-black text-slate-800">Modul Pembelajaran Sosiologi</h3>
          <p class="text-xs text-slate-500">Pilih salah satu materi di bawah ini untuk mempelajari pokok bahasan dan mengerjakan studi kasusnya.</p>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
          <div onclick="switchMateriSub('pengelompokan')" class="group cursor-pointer bg-white rounded-3xl p-6 sm:p-7 border-2 border-slate-200 hover:border-brand-500 shadow-sm hover:shadow-xl transition-all duration-300 flex flex-col justify-between space-y-6">
            <div class="space-y-4">
              <div class="flex items-center justify-between">
                <span class="px-3 py-1 bg-brand-50 border border-brand-200 text-brand-700 text-[11px] font-extrabold rounded-full uppercase tracking-wider">Materi Pokok 1</span>
                <span class="text-xs font-bold text-slate-400">7 Pokok Bahasan</span>
              </div>
              <div>
                <h4 class="text-lg font-black text-slate-800 group-hover:text-brand-700 transition leading-snug">PENGELOMPOKAN SOSIAL DI MASYARAKAT</h4>
                <p class="text-xs text-slate-500 mt-2 leading-relaxed">Kajian dasar pembentukan kelompok, kriteria Soerjono Soekanto, teori propinquity & interaksi, paguyuban-patembayan, serta evolusi Bruce Tuckman.</p>
              </div>
            </div>
            <div class="pt-4 flex items-center justify-between border-t border-slate-100">
              <span class="text-xs font-bold text-brand-600 flex items-center space-x-1.5 group-hover:translate-x-1 transition-transform">
                <span>Pelajari Materi</span><i class="fa-solid fa-arrow-right text-xs"></i>
              </span>
              <div class="w-10 h-10 rounded-2xl bg-brand-50 border border-brand-200 flex items-center justify-center text-brand-600 group-hover:bg-brand-600 group-hover:text-white transition">
                <i class="fa-solid fa-book-open"></i>
              </div>
            </div>
          </div>

          <div onclick="switchMateriSub('permasalahan')" class="group cursor-pointer bg-white rounded-3xl p-6 sm:p-7 border-2 border-slate-200 hover:border-rose-500 shadow-sm hover:shadow-xl transition-all duration-300 flex flex-col justify-between space-y-6">
            <div class="space-y-4">
              <div class="flex items-center justify-between">
                <span class="px-3 py-1 bg-rose-50 border border-rose-200 text-rose-700 text-[11px] font-extrabold rounded-full uppercase tracking-wider">Materi Pokok 2</span>
                <span class="text-xs font-bold text-slate-400">7 Pokok Masalah</span>
              </div>
              <div>
                <h4 class="text-lg font-black text-slate-800 group-hover:text-rose-700 transition leading-snug">PERMASALAHAN SOSIAL DALAM LINGKUP KELOMPOK SOSIAL</h4>
                <p class="text-xs text-slate-500 mt-2 leading-relaxed">Analisis patologi sosial, 4 faktor determinan, kemiskinan, segitiga kekerasan Johan Galtung, ketenagakerjaan, hingga ketidakadilan struktural.</p>
              </div>
            </div>
            <div class="pt-4 flex items-center justify-between border-t border-slate-100">
              <span class="text-xs font-bold text-rose-600 flex items-center space-x-1.5 group-hover:translate-x-1 transition-transform">
                <span>Pelajari Materi</span><i class="fa-solid fa-arrow-right text-xs"></i>
              </span>
              <div class="w-10 h-10 rounded-2xl bg-rose-50 border border-rose-200 flex items-center justify-center text-rose-600 group-hover:bg-rose-600 group-hover:text-white transition">
                <i class="fa-solid fa-triangle-exclamation"></i>
              </div>
            </div>
          </div>

          <div onclick="switchMateriSub('kesetaraan')" class="group cursor-pointer bg-white rounded-3xl p-6 sm:p-7 border-2 border-slate-200 hover:border-indigo-500 shadow-sm hover:shadow-xl transition-all duration-300 flex flex-col justify-between space-y-6">
            <div class="space-y-4">
              <div class="flex items-center justify-between">
                <span class="px-3 py-1 bg-indigo-50 border border-indigo-200 text-indigo-700 text-[11px] font-extrabold rounded-full uppercase tracking-wider">Materi Pokok 3</span>
                <span class="text-xs font-bold text-slate-400">6 Pokok Bahasan</span>
              </div>
              <div>
                <h4 class="text-lg font-black text-slate-800 group-hover:text-indigo-700 transition leading-snug">KESETARAAN DALAM PERBEDAAN SOSIAL DI MASYARAKAT</h4>
                <p class="text-xs text-slate-500 mt-2 leading-relaxed">Hakikat keberagaman, masyarakat multikultural Furnivall & Geertz, faktor maritim-ekologis, problematika etnosentrisme, dan kesetaraan hakiki.</p>
              </div>
            </div>
            <div class="pt-4 flex items-center justify-between border-t border-slate-100">
              <span class="text-xs font-bold text-indigo-600 flex items-center space-x-1.5 group-hover:translate-x-1 transition-transform">
                <span>Pelajari Materi</span><i class="fa-solid fa-arrow-right text-xs"></i>
              </span>
              <div class="w-10 h-10 rounded-2xl bg-indigo-50 border border-indigo-200 flex items-center justify-center text-indigo-600 group-hover:bg-indigo-600 group-hover:text-white transition">
                <i class="fa-solid fa-scale-balanced"></i>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Sub Modul 1 -->
      <div id="view-materi-pengelompokan" class="hidden space-y-6">
        <div class="bg-gradient-to-r from-brand-700 to-navy-800 rounded-3xl p-6 text-white flex flex-wrap items-center justify-between gap-4">
          <div>
            <span class="px-3 py-1 bg-white/20 text-white text-[11px] font-bold rounded-full uppercase">Materi Pokok 1</span>
            <h2 class="text-xl sm:text-2xl font-black mt-2">PENGELOMPOKAN SOSIAL DI MASYARAKAT</h2>
          </div>
          <button onclick="switchMateriSub('daftar')" class="px-4 py-2 bg-white/10 hover:bg-white/20 border border-white/20 text-white rounded-xl text-xs font-bold transition flex items-center space-x-2">
            <i class="fa-solid fa-arrow-left"></i><span>Kembali ke Daftar Modul</span>
          </button>
        </div>
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-6">
          <div class="lg:col-span-4 bg-white rounded-3xl p-5 border border-slate-200 shadow-sm space-y-3">
            <h4 class="text-xs font-bold text-slate-800 uppercase tracking-wider pb-2 border-b">Daftar Pokok Bahasan</h4>
            <div class="space-y-1.5" id="pengelompokan-topics-menu"></div>
          </div>
          <div class="lg:col-span-8 bg-white rounded-3xl p-6 sm:p-8 border border-slate-200 shadow-sm space-y-6" id="pengelompokan-article-content"></div>
        </div>
      </div>

      <!-- Sub Modul 2 -->
      <div id="view-materi-permasalahan" class="hidden space-y-6">
        <div class="bg-gradient-to-r from-rose-700 to-slate-900 rounded-3xl p-6 text-white flex flex-wrap items-center justify-between gap-4">
          <div>
            <span class="px-3 py-1 bg-white/20 text-white text-[11px] font-bold rounded-full uppercase">Materi Pokok 2</span>
            <h2 class="text-xl sm:text-2xl font-black mt-2">PERMASALAHAN SOSIAL DALAM LINGKUP KELOMPOK SOSIAL</h2>
          </div>
          <button onclick="switchMateriSub('daftar')" class="px-4 py-2 bg-white/10 hover:bg-white/20 border border-white/20 text-white rounded-xl text-xs font-bold transition flex items-center space-x-2">
            <i class="fa-solid fa-arrow-left"></i><span>Kembali ke Daftar Modul</span>
          </button>
        </div>
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-6">
          <div class="lg:col-span-4 bg-white rounded-3xl p-5 border border-slate-200 shadow-sm space-y-3">
            <h4 class="text-xs font-bold text-slate-800 uppercase tracking-wider pb-2 border-b">Topik Permasalahan</h4>
            <div class="space-y-1.5" id="permasalahan-topics-menu"></div>
          </div>
          <div class="lg:col-span-8 bg-white rounded-3xl p-6 sm:p-8 border border-slate-200 shadow-sm space-y-6" id="permasalahan-article-content"></div>
        </div>
      </div>

      <!-- Sub Modul 3 -->
      <div id="view-materi-kesetaraan" class="hidden space-y-6">
        <div class="bg-gradient-to-r from-indigo-700 to-slate-900 rounded-3xl p-6 text-white flex flex-wrap items-center justify-between gap-4">
          <div>
            <span class="px-3 py-1 bg-white/20 text-white text-[11px] font-bold rounded-full uppercase">Materi Pokok 3</span>
            <h2 class="text-xl sm:text-2xl font-black mt-2">KESETARAAN DALAM PERBEDAAN SOSIAL DI MASYARAKAT</h2>
          </div>
          <button onclick="switchMateriSub('daftar')" class="px-4 py-2 bg-white/10 hover:bg-white/20 border border-white/20 text-white rounded-xl text-xs font-bold transition flex items-center space-x-2">
            <i class="fa-solid fa-arrow-left"></i><span>Kembali ke Daftar Modul</span>
          </button>
        </div>
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-6">
          <div class="lg:col-span-4 bg-white rounded-3xl p-5 border border-slate-200 shadow-sm space-y-3">
            <h4 class="text-xs font-bold text-slate-800 uppercase tracking-wider pb-2 border-b">Topik Kesetaraan</h4>
            <div class="space-y-1.5" id="kesetaraan-topics-menu"></div>
          </div>
          <div class="lg:col-span-8 bg-white rounded-3xl p-6 sm:p-8 border border-slate-200 shadow-sm space-y-6" id="kesetaraan-article-content"></div>
        </div>
      </div>
    </section>

    <!-- TAB 3: KUIS & GAME -->
    <section id="tab-quiz-content" class="tab-pane hidden space-y-6">
      <div class="flex items-center justify-between border-b border-slate-200 pb-4">
        <div>
          <h3 class="text-xl sm:text-2xl font-black text-slate-800">Arena Kuis Cepat & Mini Game Edukasi</h3>
          <p class="text-xs sm:text-sm text-slate-500 mt-1">Pilih salah satu mode permainan di bawah untuk menguji pemahaman konsep sosiologimu!</p>
        </div>
      </div>

      <!-- Katalog 3 Mode Kuis Berbentuk Kartu Kotak dengan Logo Visual Menarik -->
      <div id="quiz-hub-catalog" class="space-y-6">
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6 max-w-6xl mx-auto">
          
          <!-- Kotak Mode 1: Pilihan Ganda -->
          <div onclick="selectQuizMode('mcq')" class="group cursor-pointer bg-white rounded-3xl p-6 sm:p-7 border-2 border-slate-200 hover:border-emerald-500 shadow-sm hover:shadow-2xl hover:-translate-y-1.5 transition-all duration-300 flex flex-col justify-between relative overflow-hidden">
            <div class="absolute -right-8 -top-8 w-28 h-28 bg-emerald-50 rounded-full group-hover:scale-150 transition-transform duration-500 -z-0"></div>
            
            <div class="space-y-4 relative z-10">
              <div class="flex items-center justify-between">
                <span class="px-3 py-1 bg-emerald-100 text-emerald-800 rounded-full text-[10px] font-black uppercase tracking-wider">Mode 01 • Uji Teori</span>
                <span class="text-[11px] font-bold text-slate-400 flex items-center space-x-1"><i class="fa-regular fa-clock text-emerald-600"></i><span>30d / Soal</span></span>
              </div>

              <div class="w-20 h-20 mx-auto rounded-3xl bg-gradient-to-tr from-emerald-500 to-teal-400 p-0.5 shadow-lg shadow-emerald-500/30 group-hover:rotate-3 group-hover:scale-110 transition-transform duration-300 flex items-center justify-center">
                <div class="w-full h-full bg-emerald-50 rounded-[22px] flex items-center justify-center text-emerald-600 text-3xl font-black">
                  <i class="fa-solid fa-list-check"></i>
                </div>
              </div>

              <div class="text-center pt-2">
                <h4 class="text-lg font-black text-slate-800 group-hover:text-emerald-600 transition">Pilihan Ganda Cepat</h4>
                <span class="inline-block mt-1 text-[11px] font-extrabold text-emerald-700 bg-emerald-50 px-2.5 py-0.5 rounded-md">Materi: Pengelompokan Sosial</span>
                <p class="text-xs text-slate-500 mt-2.5 leading-relaxed">Tantangan 5 butir soal pilihan ganda acak dari 15 bank soal. Opsi diacak otomatis!</p>
              </div>
            </div>

            <div class="pt-5 mt-4 border-t border-slate-100 flex items-center justify-between relative z-10">
              <span class="text-xs font-black text-emerald-600 flex items-center space-x-1">
                <span>Mulai Main</span>
                <i class="fa-solid fa-circle-play text-sm"></i>
              </span>
              <div class="w-8 h-8 rounded-xl bg-emerald-50 group-hover:bg-emerald-600 text-emerald-600 group-hover:text-white flex items-center justify-center transition">
                <i class="fa-solid fa-arrow-right text-xs"></i>
              </div>
            </div>
          </div>

          <!-- Kotak Mode 2: Benar / Salah -->
          <div onclick="selectQuizMode('tf')" class="group cursor-pointer bg-white rounded-3xl p-6 sm:p-7 border-2 border-slate-200 hover:border-amber-500 shadow-sm hover:shadow-2xl hover:-translate-y-1.5 transition-all duration-300 flex flex-col justify-between relative overflow-hidden">
            <div class="absolute -right-8 -top-8 w-28 h-28 bg-amber-50 rounded-full group-hover:scale-150 transition-transform duration-500 -z-0"></div>

            <div class="space-y-4 relative z-10">
              <div class="flex items-center justify-between">
                <span class="px-3 py-1 bg-amber-100 text-amber-800 rounded-full text-[10px] font-black uppercase tracking-wider">Mode 02 • Nalar Kritis</span>
                <span class="text-[11px] font-bold text-slate-400 flex items-center space-x-1"><i class="fa-regular fa-clock text-amber-600"></i><span>30d / Soal</span></span>
              </div>

              <div class="w-20 h-20 mx-auto rounded-3xl bg-gradient-to-tr from-amber-500 to-yellow-400 p-0.5 shadow-lg shadow-amber-500/30 group-hover:-rotate-3 group-hover:scale-110 transition-transform duration-300 flex items-center justify-center">
                <div class="w-full h-full bg-amber-50 rounded-[22px] flex items-center justify-center text-amber-600 text-3xl font-black">
                  <i class="fa-solid fa-scale-balanced"></i>
                </div>
              </div>

              <div class="text-center pt-2">
                <h4 class="text-lg font-black text-slate-800 group-hover:text-amber-600 transition">Benar atau Salah?</h4>
                <span class="inline-block mt-1 text-[11px] font-extrabold text-amber-700 bg-amber-50 px-2.5 py-0.5 rounded-md">Materi: Pengelompokan Sosial</span>
                <p class="text-xs text-slate-500 mt-2.5 leading-relaxed">Uji ketajaman berpikirmu dengan membedah 5 butir pernyataan sosiologis kilat!</p>
              </div>
            </div>

            <div class="pt-5 mt-4 border-t border-slate-100 flex items-center justify-between relative z-10">
              <span class="text-xs font-black text-amber-600 flex items-center space-x-1">
                <span>Tantang Dirimu</span>
                <i class="fa-solid fa-bolt text-sm"></i>
              </span>
              <div class="w-8 h-8 rounded-xl bg-amber-50 group-hover:bg-amber-600 text-amber-600 group-hover:text-white flex items-center justify-center transition">
                <i class="fa-solid fa-arrow-right text-xs"></i>
              </div>
            </div>
          </div>

          <!-- Kotak Mode 3: Teka-Teki Silang -->
          <div onclick="selectQuizMode('tts')" class="group cursor-pointer bg-white rounded-3xl p-6 sm:p-7 border-2 border-slate-200 hover:border-rose-500 shadow-sm hover:shadow-2xl hover:-translate-y-1.5 transition-all duration-300 flex flex-col justify-between relative overflow-hidden">
            <div class="absolute -right-8 -top-8 w-28 h-28 bg-rose-50 rounded-full group-hover:scale-150 transition-transform duration-500 -z-0"></div>

            <div class="space-y-4 relative z-10">
              <div class="flex items-center justify-between">
                <span class="px-3 py-1 bg-rose-100 text-rose-800 rounded-full text-[10px] font-black uppercase tracking-wider">Mode 03 • Santai & Seru</span>
                <span class="text-[11px] font-bold text-slate-400 flex items-center space-x-1"><i class="fa-solid fa-wand-magic-sparkles text-rose-600"></i><span>5 Bantuan</span></span>
              </div>

              <div class="w-20 h-20 mx-auto rounded-3xl bg-gradient-to-tr from-rose-500 to-pink-400 p-0.5 shadow-lg shadow-rose-500/30 group-hover:rotate-6 group-hover:scale-110 transition-transform duration-300 flex items-center justify-center">
                <div class="w-full h-full bg-rose-50 rounded-[22px] flex items-center justify-center text-rose-600 text-3xl font-black">
                  <i class="fa-solid fa-cubes"></i>
                </div>
              </div>

              <div class="text-center pt-2">
                <h4 class="text-lg font-black text-slate-800 group-hover:text-rose-600 transition">Teka-Teki Silang</h4>
                <span class="inline-block mt-1 text-[11px] font-extrabold text-rose-700 bg-rose-50 px-2.5 py-0.5 rounded-md">Materi: Masalah Sosial Kelompok</span>
                <p class="text-xs text-slate-500 mt-2.5 leading-relaxed">Teka-teki silang 10 kata santai dan populer. Lengkap dengan 5 kali bantuan huruf emas!</p>
              </div>
            </div>

            <div class="pt-5 mt-4 border-t border-slate-100 flex items-center justify-between relative z-10">
              <span class="text-xs font-black text-rose-600 flex items-center space-x-1">
                <span>Bermain TTS</span>
                <i class="fa-solid fa-gamepad text-sm"></i>
              </span>
              <div class="w-8 h-8 rounded-xl bg-rose-50 group-hover:bg-rose-600 text-rose-600 group-hover:text-white flex items-center justify-center transition">
                <i class="fa-solid fa-arrow-right text-xs"></i>
              </div>
            </div>
          </div>

        </div>
      </div>

      <!-- Area Game MCQ -->
      <div id="mcq-game-area" class="hidden max-w-2xl mx-auto space-y-4">
        <div class="flex items-center justify-between pb-2">
          <button onclick="backToQuizHub()" class="px-3.5 py-1.5 bg-slate-100 hover:bg-slate-200 text-slate-700 rounded-xl text-xs font-bold transition flex items-center space-x-1.5">
            <i class="fa-solid fa-arrow-left"></i><span>Pilih Kuis Lain</span>
          </button>
          <span class="text-xs font-bold text-brand-600">Mode Pilihan Ganda (A-D)</span>
        </div>
        <div id="mcq-start-card" class="bg-white rounded-3xl p-6 sm:p-8 border-2 border-slate-200 shadow-md text-center space-y-5">
          <div class="w-16 h-16 mx-auto rounded-3xl bg-brand-50 border-2 border-brand-300 flex items-center justify-center text-brand-600 text-3xl font-black">
            <i class="fa-solid fa-list-check"></i>
          </div>
          <div class="space-y-2">
            <h4 class="text-xl font-black text-slate-800">Kuis Pilihan Ganda: Pengelompokan Sosial</h4>
            <p class="text-xs text-slate-500 max-w-md mx-auto">Jawab 5 soal acak dalam waktu 30 detik per nomor!</p>
          </div>
          <button onclick="startMCQGame()" class="w-full py-3.5 bg-brand-600 hover:bg-brand-700 text-white font-extrabold rounded-2xl text-sm shadow-md transition flex items-center justify-center space-x-2">
            <i class="fa-solid fa-play"></i><span>Mulai Kuis Pilihan Ganda</span>
          </button>
        </div>
        <div id="mcq-play-card" class="hidden bg-white rounded-3xl p-6 sm:p-8 border-2 border-slate-200 shadow-md space-y-6">
          <div class="flex items-center justify-between pb-3 border-b border-slate-100">
            <span class="px-2.5 py-1 bg-slate-100 text-slate-800 rounded-lg text-xs font-black" id="mcq-progress-label">1 / 5</span>
            <span class="text-xs font-black text-brand-700 bg-brand-50 px-3.5 py-1.5 rounded-full border border-brand-200" id="mcq-timer-display">30s</span>
          </div>
          <div class="w-full bg-slate-100 h-2 rounded-full overflow-hidden">
            <div id="mcq-timer-bar" class="h-full bg-brand-500 transition-all duration-1000 ease-linear w-full"></div>
          </div>
          <p class="text-sm sm:text-base font-bold text-slate-800" id="mcq-question-text"></p>
          <div class="space-y-2.5 pt-1" id="mcq-options-container"></div>
          <div id="mcq-feedback-box" class="hidden p-4 rounded-2xl border text-xs space-y-2">
            <div class="font-bold flex items-center space-x-1.5" id="mcq-feedback-title"></div>
            <p class="text-slate-600 leading-relaxed" id="mcq-feedback-expl"></p>
            <div class="pt-1 flex justify-end">
              <button onclick="nextMCQQuestion()" id="mcq-btn-next" class="px-4 py-2 bg-slate-800 text-white rounded-xl text-xs font-bold">Soal Berikutnya</button>
            </div>
          </div>
        </div>
        <div id="mcq-result-card" class="hidden bg-white rounded-3xl p-6 border-2 border-slate-200 shadow-md text-center space-y-5">
          <h4 class="text-2xl font-black text-slate-800">Skor Kuis Pilihan Ganda Anda</h4>
          <span class="text-4xl font-black text-brand-600" id="mcq-final-score">0</span>
          <div class="grid grid-cols-2 gap-3 max-w-xs mx-auto text-xs">
            <div class="p-3 bg-emerald-50 rounded-xl font-bold text-emerald-800">Benar: <span id="mcq-correct-count">0</span></div>
            <div class="p-3 bg-rose-50 rounded-xl font-bold text-rose-800">Salah: <span id="mcq-wrong-count">0</span></div>
          </div>
          <button onclick="startMCQGame()" class="px-5 py-2.5 bg-brand-600 text-white rounded-xl text-xs font-bold">Coba Lagi (Soal Baru)</button>
        </div>
      </div>

      <!-- Area Game True/False -->
      <div id="miniquiz-game-area" class="hidden max-w-2xl mx-auto space-y-4">
        <div class="flex items-center justify-between pb-2">
          <button onclick="backToQuizHub()" class="px-3.5 py-1.5 bg-slate-100 hover:bg-slate-200 text-slate-700 rounded-xl text-xs font-bold transition flex items-center space-x-1.5">
            <i class="fa-solid fa-arrow-left"></i><span>Pilih Kuis Lain</span>
          </button>
          <span class="text-xs font-bold text-amber-600">Mode Benar / Salah</span>
        </div>
        <div id="mq-start-card" class="bg-white rounded-3xl p-6 sm:p-8 border-2 border-slate-200 shadow-md text-center space-y-5">
          <div class="w-16 h-16 mx-auto rounded-3xl bg-amber-50 border-2 border-amber-300 flex items-center justify-center text-amber-600 text-3xl font-black">
            <i class="fa-solid fa-scale-balanced"></i>
          </div>
          <div class="space-y-2">
            <h4 class="text-xl font-black text-slate-800">Tantangan Benar / Salah Sosiologi</h4>
            <p class="text-xs text-slate-500 max-w-md mx-auto">Tentukan apakah setiap pernyataan yang muncul Benar atau Salah dalam 30 detik!</p>
          </div>
          <button onclick="startMiniQuizGame()" class="w-full py-3.5 bg-amber-500 hover:bg-amber-600 text-white font-extrabold rounded-2xl text-sm shadow-md transition flex items-center justify-center space-x-2">
            <i class="fa-solid fa-play"></i><span>Mulai Tantangan Sekarang</span>
          </button>
        </div>
        <div id="mq-play-card" class="hidden bg-white rounded-3xl p-6 sm:p-8 border-2 border-slate-200 shadow-md space-y-6">
          <div class="flex items-center justify-between pb-3 border-b border-slate-100">
            <span class="px-2.5 py-1 bg-slate-100 text-slate-800 rounded-lg text-xs font-black" id="mq-progress-label">1 / 5</span>
            <span class="text-xs font-black text-amber-700 bg-amber-50 px-3.5 py-1.5 rounded-full border border-amber-200" id="mq-timer-display">30s</span>
          </div>
          <div class="w-full bg-slate-100 h-2 rounded-full overflow-hidden">
            <div id="mq-timer-bar" class="h-full bg-amber-500 transition-all duration-1000 ease-linear w-full"></div>
          </div>
          <p class="text-sm sm:text-base font-bold text-slate-800" id="mq-question-text"></p>
          <div class="grid grid-cols-1 sm:grid-cols-2 gap-3.5 pt-1" id="mq-options-container"></div>
          <div id="mq-feedback-box" class="hidden p-4 rounded-2xl border text-xs space-y-2">
            <div class="font-bold flex items-center space-x-1.5" id="mq-feedback-title"></div>
            <p class="text-slate-600 leading-relaxed" id="mq-feedback-expl"></p>
            <div class="pt-1 flex justify-end">
              <button onclick="nextMiniQuizQuestion()" id="mq-btn-next" class="px-4 py-2 bg-slate-800 text-white rounded-xl text-xs font-bold">Soal Berikutnya</button>
            </div>
          </div>
        </div>
        <div id="mq-result-card" class="hidden bg-white rounded-3xl p-6 border-2 border-slate-200 shadow-md text-center space-y-5">
          <h4 class="text-2xl font-black text-slate-800">Skor Tantangan Benar/Salah Anda</h4>
          <span class="text-4xl font-black text-amber-600" id="mq-final-score">0</span>
          <div class="grid grid-cols-2 gap-3 max-w-xs mx-auto text-xs">
            <div class="p-3 bg-emerald-50 rounded-xl font-bold text-emerald-800">Tepat: <span id="mq-correct-count">0</span></div>
            <div class="p-3 bg-rose-50 rounded-xl font-bold text-rose-800">Keliru: <span id="mq-wrong-count">0</span></div>
          </div>
          <button onclick="startMiniQuizGame()" class="px-5 py-2.5 bg-amber-500 text-white rounded-xl text-xs font-bold">Coba Lagi (Soal Baru)</button>
        </div>
      </div>

      <!-- Area Game TTS -->
      <div id="tts-game-area" class="hidden max-w-5xl mx-auto space-y-6">
        <div class="flex items-center justify-between pb-2">
          <button onclick="backToQuizHub()" class="px-3.5 py-1.5 bg-slate-100 hover:bg-slate-200 text-slate-700 rounded-xl text-xs font-bold transition flex items-center space-x-1.5">
            <i class="fa-solid fa-arrow-left"></i><span>Pilih Kuis Lain</span>
          </button>
          <span class="px-3 py-1 bg-rose-50 border border-rose-200 text-rose-700 rounded-full text-xs font-black">
            TTS Santai: Masalah Sosial Kelompok (10 Kata Gampang)
          </span>
        </div>

        <div class="bg-white rounded-3xl p-5 sm:p-7 border-2 border-slate-200 shadow-sm space-y-6">
          <div class="flex flex-wrap items-center justify-between gap-3 border-b border-slate-100 pb-4">
            <div>
              <h4 class="text-base sm:text-lg font-black text-slate-800">Teka-Teki Silang: Masalah Sosial Santai</h4>
              <p class="text-xs text-slate-500 mt-0.5">Ketik huruf pada kotak putih. Ada 5 kali kuota bantuan huruf!</p>
            </div>
            <div class="flex items-center space-x-2">
              <button onclick="revealTTSHint()" id="btn-tts-hint" class="px-3 py-1.5 bg-amber-50 hover:bg-amber-100 text-amber-700 border border-amber-200 rounded-xl text-xs font-bold transition flex items-center space-x-1.5 shadow-sm">
                <i class="fa-solid fa-lightbulb text-amber-500"></i>
                <span>Bantuan Huruf</span>
                <span id="tts-hint-counter" class="px-1.5 py-0.5 bg-amber-200 text-amber-900 rounded-md text-[10px] font-black">5 / 5</span>
              </button>
              <button onclick="resetTTS()" class="px-3 py-1.5 bg-slate-100 hover:bg-slate-200 text-slate-700 rounded-xl text-xs font-bold">
                <i class="fa-solid fa-rotate-left"></i><span>Reset</span>
              </button>
            </div>
          </div>

          <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 items-start">
            <div class="lg:col-span-7 flex flex-col items-center">
              <div class="p-3 bg-slate-900 rounded-3xl shadow-lg border-4 border-slate-800 overflow-x-auto max-w-full">
                <div id="tts-grid" class="grid grid-cols-10 gap-1 select-none" style="grid-template-columns: repeat(10, minmax(28px, 36px));"></div>
              </div>
            </div>
            <div class="lg:col-span-5 space-y-4 text-xs">
              <div class="p-4 bg-rose-50/60 border border-rose-200 rounded-2xl space-y-2">
                <div class="text-rose-800 font-black uppercase text-[11px]"><i class="fa-solid fa-arrow-right mr-1"></i>Mendatar (Across)</div>
                <div class="space-y-2 max-h-52 overflow-y-auto pr-1 custom-scroll" id="tts-clues-across"></div>
              </div>
              <div class="p-4 bg-indigo-50/60 border border-indigo-200 rounded-2xl space-y-2">
                <div class="text-indigo-800 font-black uppercase text-[11px]"><i class="fa-solid fa-arrow-down mr-1"></i>Menurun (Down)</div>
                <div class="space-y-2 max-h-52 overflow-y-auto pr-1 custom-scroll" id="tts-clues-down"></div>
              </div>
            </div>
          </div>

          <div class="pt-4 border-t border-slate-100 flex flex-wrap items-center justify-between gap-3">
            <div id="tts-status-badge" class="text-xs font-semibold text-slate-500">Ketik kata yang Anda tahu, gunakan bantuan huruf jika ragu!</div>
            <button onclick="checkTTSAnswers()" class="px-6 py-3 bg-rose-600 hover:bg-rose-700 text-white font-extrabold rounded-2xl text-xs sm:text-sm shadow-md transition">
              <i class="fa-solid fa-circle-check mr-1.5"></i>Periksa & Kumpulkan Jawaban TTS
            </button>
          </div>
        </div>

        <div id="tts-result-card" class="hidden bg-white rounded-3xl p-6 sm:p-8 border-2 border-slate-200 shadow-md text-center space-y-5">
          <h4 class="text-2xl font-black text-slate-800">Skor Teka-Teki Silang Anda</h4>
          <span class="text-4xl font-black text-rose-600" id="tts-final-score">0</span>
          <div class="grid grid-cols-2 gap-3 max-w-xs mx-auto text-xs">
            <div class="p-3 bg-emerald-50 rounded-xl font-bold text-emerald-800">Kata Tepat: <span id="tts-correct-words">0 / 10</span></div>
            <div class="p-3 bg-rose-50 rounded-xl font-bold text-rose-800">Keliru/Kosong: <span id="tts-wrong-words">0 / 10</span></div>
          </div>
          <button onclick="resetTTS(); document.getElementById('tts-result-card').classList.add('hidden');" class="px-5 py-2.5 bg-rose-600 text-white rounded-xl text-xs font-bold">Coba Mainkan Lagi</button>
        </div>
      </div>
    </section>

    <!-- TAB 4: DATA SISWA -->
    <section id="tab-siswa-content" class="tab-pane hidden space-y-6">
      <div class="bg-white rounded-3xl p-6 border border-slate-200 shadow-sm space-y-4">
        <div class="flex flex-wrap items-center justify-between gap-4">
          <div>
            <h3 class="text-lg font-black text-slate-800">Direktori Data Siswa SMAN 12 Gowa</h3>
            <p class="text-xs text-slate-500">Data kepesertaan siswa kelas XII tahun ajaran aktif.</p>
          </div>
          <div class="flex items-center space-x-2">
            <button onclick="exportStudentsToCSV()" class="px-3.5 py-2 bg-slate-100 hover:bg-slate-200 text-slate-700 rounded-xl text-xs font-bold transition flex items-center space-x-1.5">
              <i class="fa-solid fa-file-csv"></i><span>Ekspor CSV</span>
            </button>
          </div>
        </div>

        <div class="grid grid-cols-1 sm:grid-cols-3 gap-3 pt-2">
          <div class="sm:col-span-2 relative">
            <span class="absolute inset-y-0 left-0 pl-3 flex items-center text-slate-400">
              <i class="fa-solid fa-magnifying-glass"></i>
            </span>
            <input type="text" id="search-student-input" oninput="renderStudentsTable()" placeholder="Cari nama siswa atau NIS..."
              class="w-full pl-9 pr-4 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-xs focus:ring-2 focus:ring-brand-500 outline-none">
          </div>
          <div>
            <select id="filter-kelas-select" onchange="renderStudentsTable()"
              class="w-full px-3 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-xs font-medium focus:ring-2 focus:ring-brand-500 outline-none">
              <option value="ALL">Semua Kelas</option>
              <option value="XII IPS 1">XII IPS 1</option>
              <option value="XII IPS 2">XII IPS 2</option>
              <option value="XII IPA 1">XII IPA 1</option>
              <option value="XII IPA 2">XII IPA 2</option>
              <option value="XII IPA 3">XII IPA 3</option>
            </select>
          </div>
        </div>

        <div class="overflow-x-auto rounded-2xl border border-slate-200">
          <table class="w-full text-left text-xs">
            <thead class="bg-slate-100 text-slate-700 uppercase font-black tracking-wider border-b border-slate-200">
              <tr>
                <th class="p-3.5">No</th>
                <th class="p-3.5">NIS</th>
                <th class="p-3.5">Nama Lengkap Siswa</th>
                <th class="p-3.5">Kelas</th>
                <th class="p-3.5">Status Partisipasi</th>
              </tr>
            </thead>
            <tbody id="student-table-body" class="divide-y divide-slate-100 text-slate-700"></tbody>
          </table>
        </div>
      </div>
    </section>

  </main>

  <!-- FOOTER -->
  <footer class="mt-auto border-t border-slate-200 bg-white py-6 text-center text-xs text-slate-500">
    <div class="max-w-7xl mx-auto px-4 space-y-1">
      <p class="font-bold text-slate-700">SOSIOPEDIA - Portal Pendidikan Sosiologi SMA Negeri 12 Gowa</p>
      <p>Created by: <span class="font-extrabold text-brand-700">MUH. FADHLI NUGRAHA M</span></p>
      <p class="text-[11px] text-slate-400">Diproteksi dan Terintegrasi untuk Pembelajaran Berbasis HOTS 2026</p>
    </div>
  </footer>

  <!-- MODAL ADMIN AUTH -->
  <div id="modal-admin-auth" class="fixed inset-0 z-50 bg-slate-900/60 backdrop-blur-sm hidden flex items-center justify-center p-4">
    <div class="bg-white rounded-3xl p-6 sm:p-8 max-w-sm w-full shadow-2xl border border-slate-200 space-y-5 text-center">
      <div class="w-14 h-14 mx-auto rounded-2xl bg-amber-50 border border-amber-200 flex items-center justify-center text-amber-600 text-xl font-black">
        <i class="fa-solid fa-shield-halved"></i>
      </div>
      <div>
        <h4 class="text-base font-black text-slate-800">Verifikasi PIN Guru / Admin</h4>
        <p class="text-xs text-slate-500 mt-1">Masukkan PIN 2202 untuk membuka kunci jawaban rubrik.</p>
      </div>
      <div>
        <input type="password" id="admin-pin-input" maxlength="20" placeholder="Ketik PIN..." autocomplete="off"
          onkeydown="if(event.key === 'Enter') verifyAdminPin();"
          class="w-full text-center tracking-widest text-lg font-black py-3 bg-slate-50 border border-slate-300 rounded-2xl outline-none focus:ring-2 focus:ring-brand-500">
        <p id="admin-pin-error" class="hidden text-rose-600 text-[11px] font-bold mt-2">PIN salah! Pastikan memasukkan PIN 2202.</p>
      </div>
      <div class="flex items-center space-x-2">
        <button type="button" onclick="closeAdminAuthModal()" class="flex-1 py-2.5 bg-slate-100 hover:bg-slate-200 text-slate-700 rounded-xl text-xs font-bold">Batal</button>
        <button type="button" onclick="verifyAdminPin()" class="flex-1 py-2.5 bg-brand-600 hover:bg-brand-700 text-white rounded-xl text-xs font-bold transition shadow-sm">Verifikasi</button>
      </div>
    </div>
  </div>

  <!-- MODAL PANEL GURU -->
  <div id="modal-admin-panel" class="fixed inset-0 z-50 bg-slate-900/60 backdrop-blur-sm hidden flex items-center justify-center p-4">
    <div class="bg-white rounded-3xl p-6 sm:p-8 max-w-lg w-full shadow-2xl border border-slate-200 space-y-6">
      <div class="flex items-center justify-between pb-3 border-b border-slate-100">
        <h4 class="text-base font-black text-slate-800 flex items-center space-x-2">
          <i class="fa-solid fa-sliders text-brand-600"></i><span>Pengaturan Panel Guru</span>
        </h4>
        <button onclick="closeAdminPanelModal()" class="text-slate-400 hover:text-slate-600"><i class="fa-solid fa-xmark text-lg"></i></button>
      </div>
      <div class="space-y-4 text-xs text-slate-600">
        <div>
          <label class="block font-bold text-slate-700 mb-1">URL Google Apps Script (Web App /exec):</label>
          <input type="url" id="admin-sheet-url" placeholder="https://script.google.com/macros/s/.../exec"
            class="w-full p-3 bg-slate-50 border border-slate-300 rounded-2xl text-xs font-mono focus:ring-2 focus:ring-brand-500 outline-none">
          <p class="text-[11px] text-slate-400 mt-1">Hasil ujian siswa akan otomatis terkirim tanpa diketahui siswa.</p>
        </div>
      </div>
      <div class="flex justify-end space-x-2 pt-2 border-t border-slate-100">
        <button onclick="saveAdminSettings()" class="px-5 py-2.5 bg-brand-600 hover:bg-brand-700 text-white rounded-xl text-xs font-bold shadow-sm">Simpan Pengaturan</button>
      </div>
    </div>
  </div>

  <!-- ================= JAVASCRIPT & DATABASE ================= -->
  <script>
    const ADMIN_PIN = "2202";
    const ASSESSMENT_ACCESS_CODE = "SMAN12";
    let teacherAuthenticated = false;
    let pendingAction = null;
    let pendingRubricButton = null;

    let currentStudent = { name: "", kelas: "" };
    let sessionQuestions = [];
    let currentQuestionIdx = 0;
    let studentAnswers = {};

    // DATA SISWA DATABASE SMAN 12 GOWA
    const STUDENTS_DATABASE = [
      { nis: "1001", name: "Andi Ahmad Fauzan", kelas: "XII IPS 1", status: "Aktif" },
      { nis: "1002", name: "Siti Nurhaliza", kelas: "XII IPS 1", status: "Aktif" },
      { nis: "1003", name: "Muh. Fadhli Nugraha", kelas: "XII IPS 1", status: "Aktif" },
      { nis: "1004", name: "Nurul Aisyah", kelas: "XII IPS 2", status: "Aktif" },
      { nis: "1005", name: "Ahmad Zulfikar", kelas: "XII IPA 1", status: "Aktif" },
      { nis: "1006", name: "Dewi Lestari", kelas: "XII IPA 2", status: "Aktif" },
      { nis: "1007", name: "Rezky Pratama", kelas: "XII IPA 3", status: "Aktif" }
    ];

    // BANK SOAL SIMULASI TKA 40 BUTIR
    const QUIZ_QUESTIONS = Array.from({ length: 40 }, (_, i) => ({
      id: i + 1,
      category: i < 15 ? "Pengelompokan Sosial" : (i < 28 ? "Permasalahan Sosial" : "Kesetaraan Sosial"),
      question: `Butir Soal Simulasi TKA Sosiologi Nomor ${i + 1}: Analisislah fenomena sosiologis berikut mengenai struktur kelompok dan masyarakat multikultural di Indonesia...`,
      options: [
        "Pilihan A: Keteraturan sosial terbentuk melalui konsensus nilai yang dijunjung bersama.",
        "Pilihan B: Terjadi segregasi akibat kuatnya batas primordialisme sempit.",
        "Pilihan C: Mobilitas sosial vertikal naik mempercepat integrasi kebudayaan.",
        "Pilihan D: Disorganisasi kelompok dipicu oleh ketimpangan struktural ekonomi.",
        "Pilihan E: Konflik horizontal muncul akibat dominasi kelompok mayoritas."
      ],
      correctIndex: 0,
      explanation: "Pembahasan TKA: Fenomena tersebut mencerminkan dinamika integrasi sosial di mana konsensus nilai menjadi fondasi stabilitas kelompok masyarakat."
    }));

    // DATA MATERI POKOK 1: PENGELOMPOKAN SOSIAL
    const PENGELOMPOKAN_MODULES = [
      {
        title: "1. Hakikat dan Dasar Pembentukan Kelompok Sosial",
        content: `
          <h4 class='text-base font-black text-slate-800 mb-2'>Hakikat Kelompok Sosial</h4>
          <p class='text-xs sm:text-sm text-slate-600 leading-relaxed mb-4'>
            Manusia adalah makhluk sosial (<i>zoon politicon</i> menurut Aristoteles) yang tidak dapat hidup sendiri tanpa bantuan sesama. Dorongan naluriah untuk hidup bersama (<i>gregariousness</i>) melahirkan interaksi dan membentuk kelompok sosial.
          </p>
          <h5 class='text-xs font-bold text-slate-800 uppercase mb-2'>Syarat Kelompok Sosial (Soerjono Soekanto):</h5>
          <ul class='list-disc list-inside text-xs sm:text-sm text-slate-600 space-y-1.5 mb-4'>
            <li>Adanya kesadaran sebagai bagian dari kelompok yang bersangkutan.</li>
            <li>Ada hubungan timbal balik (interaksi) antar anggota kelompok.</li>
            <li>Memiliki faktor pengikat yang sama (kesamaan nasib, hobi, ideologi, atau darah).</li>
            <li>Berstruktur, berkaidah, dan memiliki sistem pola perilaku tertentu.</li>
          </ul>
        `,
        cases: [
          {
            title: "Studi Kasus 1: Komunitas Peduli Lingkungan",
            problem: "Sekelompok pemuda di Gowa membentuk wadah peduli sungai setelah melihat tingginya pencemaran sampah plastik. Analisislah apakah komunitas ini memenuhi syarat kelompok sosial menurut Soerjono Soekanto!",
            rubric: "Siswa harus menguraikan terpenuhinya syarat: kesadaran bersama (peduli lingkungan), interaksi rutin, faktor pengikat yang sama (kepedulian ekologis), serta struktur organisasi internal."
          },
          {
            title: "Studi Kasus 2: Antrean di Loket Stasiun",
            problem: "Puluhan orang berdiri mengantre tiket kereta di stasiun secara tertib tanpa saling mengenal. Apakah kerumunan antrean ini dapat dikategorikan sebagai kelompok sosial? Jelaskan alasannya!",
            rubric: "Bukan kelompok sosial, melainkan kerumunan (crowd) atau kategori sosial sementara, karena tidak memiliki kesadaran kelompok yang permanen, struktur, maupun interaksi timbal balik yang intens."
          }
        ]
      },
      {
        title: "2. Faktor Pendorong Pembentukan Kelompok",
        content: `
          <h4 class='text-base font-black text-slate-800 mb-2'>Faktor Pendorong Utama</h4>
          <p class='text-xs sm:text-sm text-slate-600 leading-relaxed mb-3'>
            <b>1. Teori Kedekatan (Propinquity Theory):</b> Individu cenderung membentuk kelompok dengan orang-orang yang berada di sekitar geografis yang sama (tetangga, rekan sekantor).<br>
            <b>2. Kesamaan Minat & Tujuan:</b> Dorongan untuk mencapai tujuan bersama (organisasi belajar, klub olahraga).<br>
            <b>3. Kesamaan Asal-usul & Keturunan:</b> Ikatan genealogis (paguyuban marga, ikatan keluarga daerah).
          </p>
        `,
        cases: [
          {
            title: "Studi Kasus 1: Perantau Asal Sulawesi Selatan",
            problem: "Perantau asal Sulawesi Selatan di berbagai kota besar mendirikan kerukunan keluarga (KKSS). Faktor apakah yang paling dominan mendorong terbentuknya kelompok tersebut?",
            rubric: "Faktor kesamaan asal-usul, ikatan genealogis, dan kebutuhan solidaritas kultural di perantauan."
          },
          {
            title: "Studi Kasus 2: Kelompok Belajar Sebaya",
            problem: "Siswa kelas XII membentuk kelompok belajar persiapan UTBK berdasarkan kesamaan target universitas impian. Analisislah faktor pembentuknya!",
            rubric: "Faktor kesamaan tujuan, minat akademik, dan kebutuhan strategis dalam menghadapi ujian seleksi."
          }
        ]
      },
      {
        title: "3. Klasifikasi Kelompok: Paguyuban (Gemeinschaft) & Patembayan (Gesellschaft)",
        content: `
          <h4 class='text-base font-black text-slate-800 mb-2'>Teori Ferdinand Tönnies</h4>
          <p class='text-xs sm:text-sm text-slate-600 leading-relaxed mb-3'>
            <b>• Gemeinschaft (Paguyuban):</b> Bentuk kehidupan bersama yang intim, privat, dan eksklusif. Didasari ikatan batin murni (keluarga, rukun tetangga tradisional).<br>
            <b>• Gesellschaft (Patembayan):</b> Ikatan lahir yang bersifat pokok untuk jangka waktu pendek, berorientasi pamrih/ekonomis (PT, CV, serikat buruh kontrak).
          </p>
        `,
        cases: [
          {
            title: "Studi Kasus 1: Hubungan Kerja di Perusahaan Multinasional",
            problem: "Karyawan di sebuah korporasi besar berinteraksi secara formal berdasarkan kontrak kerja dan target profit. Termasuk jenis kelompok apa dan berikan argumennya!",
            rubric: "Patembayan (Gesellschaft), karena didasarkan pada hubungan rasional, kontraktual, dan orientasi ekonomi praktis."
          },
          {
            title: "Studi Kasus 2: Arisan Keluarga Besar",
            problem: "Kegiatan arisan bulanan keluarga besar di kampung halaman yang diwarnai kekeluargaan erat. Klasifikasikan bentuk kelompok ini menurut Tönnies!",
            rubric: "Gemeinschaft of blood atau mind (Paguyuban), karena didasari ikatan batin yang kuat dan kekeluargaan."
          }
        ]
      },
      {
        title: "4. In-Group dan Out-Group",
        content: `
          <h4 class='text-base font-black text-slate-800 mb-2'>Pandangan William Graham Sumner</h4>
          <p class='text-xs sm:text-sm text-slate-600 leading-relaxed mb-3'>
            <b>• In-Group:</b> Kelompok di mana individu merasa dirinya menjadi anggota (rasa 'kita' / <i>we-feeling</i> sangat kuat).<br>
            <b>• Out-Group:</b> Kelompok di luar dirinya yang sering kali diasosiasikan dengan perasaan 'mereka' atau bahkan prasangka/antagonisme.
          </p>
        `,
        cases: [
          {
            title: "Studi Kasus 1: Suporter Klub Sepak Bola",
            problem: "Suporter klub bola fanatik menganggap kelompoknya sebagai yang terbaik dan memandang suporter klub lain sebagai musuh. Bagaimana sosiologi menjelaskan gejala in-group dan out-group ini?",
            rubric: "Menjelaskan batas tegas antara loyalitas kelompok sendiri (in-group) dan potensi prasangka terhadap kelompok luar (out-group)."
          },
          {
            title: "Studi Kasus 2: Loyalitas Alumni Sekolah",
            problem: "Alumni SMA Negeri 12 Gowa memiliki ikatan solidaritas yang kuat saat bertemu di perguruan tinggi melawan alumni sekolah lain.",
            rubric: "Refleksi in-group feeling yang positif dalam membangun jejaring alumni."
          }
        ]
      },
      {
        title: "5. Primary Group dan Secondary Group",
        content: `
          <h4 class='text-base font-black text-slate-800 mb-2'>Klasifikasi Charles Horton Cooley</h4>
          <p class='text-xs sm:text-sm text-slate-600 leading-relaxed mb-3'>
            <b>• Primary Group (Kelompok Primer):</b> Hubungan tatap muka yang akrab, personal, dan menyeluruh (keluarga, sahabat karib).<br>
            <b>• Secondary Group (Kelompok Sekunder):</b> Hubungan formal, berorientasi tugas, dan tidak mendalam secara personal (organisasi profesi, birokrasi).
          </p>
        `,
        cases: [
          {
            title: "Studi Kasus 1: Hubungan Dokter dan Pasien di Rumah Sakit",
            problem: "Interaksi antara dokter spesialis dan pasien di ruang pemeriksaan rumah sakit. Termasuk kelompok primer atau sekunder? Jelaskan!",
            rubric: "Kelompok sekunder, karena bersifat formal, kontraktual, berorientasi penyembuhan medis semata."
          },
          {
            title: "Studi Kasus 2: Perkumpulan Sahabat Masa Kecil",
            problem: "Sekelompok teman masa kecil yang selalu saling membantu dalam suka dan duka tanpa pamrih.",
            rubric: "Kelompok primer, ditandai keintiman emosional dan hubungan personal yang mendalam."
          }
        ]
      },
      {
        title: "6. Membership Group dan Reference Group",
        content: `
          <h4 class='text-base font-black text-slate-800 mb-2'>Teori Robert K. Merton</h4>
          <p class='text-xs sm:text-sm text-slate-600 leading-relaxed mb-3'>
            <b>• Membership Group:</b> Kelompok di mana seseorang secara resmi tercatat dan menjadi anggota.<br>
            <b>• Reference Group:</b> Kelompok acuan yang digunakan seseorang sebagai standar untuk membentuk kepribadian, sikap, dan perilakunya (meskipun ia bukan anggota kelompok tersebut).
          </p>
        `,
        cases: [
          {
            title: "Studi Kasus 1: Gaya Hidup Atlet Profesional",
            problem: "Seorang remaja biasa meniru gaya latihan, disiplin, dan pola makan bintang sepak bola dunia idolanya. Analisislah konsep membership group dan reference group kasus ini!",
            rubric: "Remaja tersebut memiliki membership group di klub lokalnya, namun menjadikan atlet dunia sebagai reference group."
          },
          {
            title: "Studi Kasus 2: Anggota Parpol dan Tokoh Intelektual",
            problem: "Seorang politisi muda meniru cara berpidato seorang negarawan senior idealnya.",
            rubric: "Negarawan senior berfungsi sebagai reference group bagi pembentukan gaya politik kader muda tersebut."
          }
        ]
      },
      {
        title: "7. Dinamika Perkembangan Kelompok (Bruce Tuckman)",
        content: `
          <h4 class='text-base font-black text-slate-800 mb-2'>Teori 5 Tahap Pembentukan Kelompok</h4>
          <p class='text-xs sm:text-sm text-slate-600 leading-relaxed mb-3'>
            1. <b>Forming (Pembentukan):</b> Orientasi awal.<br>
            2. <b>Storming (Pemberontakan/Konflik):</b> Gesekan antar anggota.<br>
            3. <b>Norming (Penormaan):</b> Rekonsiliasi dan kesepakatan aturan.<br>
            4. <b>Performing (Berkinerja Tinggi):</b> Kolaborasi efektif.<br>
            5. <b>Adjourning (Penyelesaian/Pembubaran):</b> Tugas selesai.
          </p>
        `,
        cases: [
          {
            title: "Studi Kasus 1: Panitia Pensi Sekolah",
            problem: "Panitia pentas seni sempat bersitegang hebat mengenai alokasi anggaran, namun akhirnya berhasil menyepakati SOP kerja sama. Di tahap manakah panitia tersebut berada?",
            rubric: "Berada di transisi dari tahap Storming menuju Norming."
          },
          {
            title: "Studi Kasus 2: Tim Riset Karya Ilmiah",
            problem: "Tim peneliti bekerja secara sinergis, saling percaya, dan berhasil menyelesaikan laporan tepat waktu.",
            rubric: "Tahap Performing (kinerja optimal)."
          }
        ]
      }
    ];

    // DATA MATERI POKOK 2: PERMASALAHAN SOSIAL DALAM LINGKUP KELOMPOK SOSIAL
    const PERMASALAHAN_MODULES = [
      {
        title: "1. Pengertian Masalah Sosial",
        content: `
          <h4 class='text-base font-black text-slate-800 mb-2'>Konseptual Masalah Sosial</h4>
          <p class='text-xs sm:text-sm text-slate-600 leading-relaxed mb-3'>
            Menurut Soerjono Soekanto, masalah sosial adalah suatu ketidaksesuaian antara unsur-unsur kebudayaan atau masyarakat, yang membahayakan kehidupan kelompok sosial. Masalah sosial menyangkut nilai-nilai sosial yang diabaikan.
          </p>
          <ul class='list-disc list-inside text-xs sm:text-sm text-slate-600 space-y-1.5 mb-3'>
            <li><b>Elemen Objektif:</b> Kondisi nyata yang dapat diamati dan diukur dalam masyarakat.</li>
            <li><b>Elemen Subjektif:</b> Keyakinan kolektif bahwa kondisi tersebut tidak diinginkan dan harus segera diatasi.</li>
          </ul>
        `,
        cases: [
          {
            title: "Studi Kasus 1: Maraknya Judi Online di Kalangan Remaja",
            problem: "Peningkatan kasus kecanduan judi online di kalangan remaja desa maupun kota telah merusak produktivitas belajar. Analisislah fenomena ini dari sudut pandang elemen objektif dan subjektif masalah sosial!",
            rubric: "Elemen objektif: peningkatan jumlah pemain dan kerugian finansial nyata. Elemen subjektif: keresahan kolektif masyarakat dan orang tua yang menuntut pemberantasan."
          },
          {
            title: "Studi Kasus 2: Vandalisme Fasilitas Umum",
            problem: "Aksi perusakan halte bus oleh oknum tidak bertanggung jawab yang dianggap meresahkan warga kota.",
            rubric: "Memenuhi kriteria masalah sosial karena melanggar nilai ketertiban umum dan merugikan kepentingan publik."
          }
        ]
      },
      {
        title: "2. Penyebab Timbulnya Masalah Sosial",
        content: `
          <h4 class='text-base font-black text-slate-800 mb-2'>Empat Faktor Determinan Utama</h4>
          <p class='text-xs sm:text-sm text-slate-600 leading-relaxed mb-3'>
            <b>1. Faktor Ekonomis:</b> Pengangguran, kemiskinan, inflasi, dan krisis distribusi pendapatan.<br>
            <b>2. Faktor Biologis:</b> Wabah penyakit menular, malnutrisi/stunting, dan disabilitas fisik massal.<br>
            <b>3. Faktor Psikologis:</b> Tekanan jiwa, skizofrenia, stres sosial, dan penyimpangan perilaku akibat trauma.<br>
            <b>4. Faktor Kebudayaan:</b> <i>Cultural lag</i> (ketertinggalan budaya), disorganisasi keluarga, dan modernisasi tanpa filter.
          </p>
        `,
        cases: [
          {
            title: "Studi Kasus 1: Cultural Lag Era Digital",
            problem: "Kemajuan teknologi kecerdasan buatan (AI) disalahgunakan untuk kejahatan siber (deepfake scams) karena regulasi hukum terlambat mengantisipasinya. Konsep apa yang menjelaskan hal ini?",
            rubric: "Konsep Cultural Lag (Ketertinggalan Budaya), di mana perangkat materiil berkembang lebih cepat daripada kesiapan non-materiil (norma/etika hukum)."
          },
          {
            title: "Studi Kasus 2: Depresi Massal Akibat PHK Korporasi",
            problem: "Gelombang pemutusan hubungan kerja (PHK) massal memicu lonjakan kasus stres dan gangguan psikologis di perkotaan.",
            rubric: "Kombinasi faktor ekonomis (PHK) yang memicu faktor psikologis (depresi/stres sosial)."
          }
        ]
      },
      {
        title: "3a. Masalah Sosial di Indonesia: Kemiskinan",
        content: `
          <h4 class='text-base font-black text-slate-800 mb-2'>Dimensi & Lingkaran Setan Kemiskinan</h4>
          <p class='text-xs sm:text-sm text-slate-600 leading-relaxed mb-3'>
            <b>• Kemiskinan Absolut:</b> Pendapatan di bawah garis kemiskinan minimum untuk mencukupi kebutuhan dasar.<br>
            <b>• Kemiskinan Relatif:</b> Standar kemiskinan berdasarkan perbandingan tingkat kesejahteraan antar kelompok.<br>
            <b>• Kemiskinan Kultural:</b> Akibat mentalitas, adat, atau sikap hidup (malas, pasrah pada nasib).<br>
            <b>• Kemiskinan Struktural:</b> Akibat kebijakan ekonomi atau struktur kekuasaan yang timpang (Ragnar Nurkse: <i>Vicious Circle of Poverty</i>).
          </p>
        `,
        cases: [
          {
            title: "Studi Kasus 1: Petani Penggarap Tanpa Lahan",
            problem: "Petani di perdesaan tetap miskin turun-temurun meski bekerja keras, karena seluruh hasil panen habis untuk membayar sewa tanah kepada tuan tanah pemilik modal. Jenis kemiskinan apa ini?",
            rubric: "Kemiskinan Struktural, disebabkan oleh ketimpangan penguasaan alat produksi (tanah) dan sistem bagi hasil yang eksploitatif."
          },
          {
            title: "Studi Kasus 2: Budaya Cepat Puas dan Enggan Berinovasi",
            problem: "Sebagian masyarakat menolak modernisasi pertanian karena menganggap cara leluhur sudah cukup meskipun hasilnya minim.",
            rubric: "Kemiskinan Kultural, yang berakar dari resistensi terhadap perubahan nilai kemajuan."
          }
        ]
      },
      {
        title: "3b. Masalah Sosial di Indonesia: Perilaku Kekerasan",
        content: `
          <h4 class='text-base font-black text-slate-800 mb-2'>Segitiga Kekerasan Johan Galtung</h4>
          <p class='text-xs sm:text-sm text-slate-600 leading-relaxed mb-3'>
            <b>1. Kekerasan Langsung (Direct Violence):</b> Tindakan agresi fisik kasatmata (tawuran, perundungan).<br>
            <b>2. Kekerasan Struktural:</b> Penindasan yang dilembagakan melalui sistem sosial/ekonomi (eksploitasi buruh).<br>
            <b>3. Kekerasan Kultural:</b> Aspek kebudayaan (agama, ideologi, seni) yang melegitimasi kekerasan langsung atau struktural.
          </p>
        `,
        cases: [
          {
            title: "Studi Kasus 1: Perundungan Senioritas di Sekolah",
            problem: "Tradisi 'ospek' tersembunyi di mana senior melakukan kekerasan fisik dengan dalih 'membangun mental disiplin junior'. Bedah kasus ini menggunakan konsep Johan Galtung!",
            rubric: "Kekerasan langsung (pemukulan fisik), didukung kekerasan kultural (mitos bahwa senioritas harus dihormati lewat kekerasan)."
          },
          {
            title: "Studi Kasus 2: Upah Murah Buruh Pabrik",
            problem: "Sistem pengupahan di bawah standar minimum yang dipaksakan oleh regulasi perusahaan demi keuntungan korporasi.",
            rubric: "Kekerasan Struktural, kekerasan yang tertanam dalam sistem dan struktur birokrasi ekonomi."
          }
        ]
      },
      {
        title: "3c. Masalah Sosial di Indonesia: Ketenagakerjaan (Pengangguran)",
        content: `
          <h4 class='text-base font-black text-slate-800 mb-2'>Jenis & Akar Pengangguran</h4>
          <p class='text-xs sm:text-sm text-slate-600 leading-relaxed mb-3'>
            <b>• Pengangguran Friksional:</b> Peralihan pekerjaan antar pencari kerja.<br>
            <b>• Pengangguran Struktural:</b> Ketidakse
