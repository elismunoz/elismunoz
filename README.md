<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Elis | Portfolio</title>
  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  <!-- FontAwesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap');
    body {
      font-family: 'Inter', sans-serif;
      background-color: #030712;
      color: #f3f4f6;
    }
    .bg-space {
      background-image: linear-gradient(to right, rgba(3, 7, 18, 0.85) 30%, rgba(3, 7, 18, 0.4) 100%), 
                        url('https://images.unsplash.com/photo-1506703719100-a0f3a48c0f86?q=80&w=2070&auto=format&fit=crop');
      background-size: cover;
      background-position: center;
    }
    .glass-card {
      background: rgba(15, 23, 42, 0.65);
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      border: 1px solid rgba(255, 255, 255, 0.1);
    }
    .glass-pill {
      background: rgba(255, 255, 255, 0.08);
      backdrop-filter: blur(10px);
      border: 1px solid rgba(255, 255, 255, 0.15);
    }
  </style>
</head>
<body class="min-h-screen bg-space flex flex-col justify-between overflow-x-hidden relative">

  <!-- Navbar -->
  <header class="w-full max-w-7xl mx-auto px-6 py-6 flex items-center justify-between z-20">
    <div class="flex items-center gap-2">
     <div class="w-8 h-8 rounded-full bg-cyan-500 flex items-center justify-center font-bold text-black text-lg">
        E
      </div>
      <span class="text-xl font-bold tracking-wider">Elis</span>
    </div>

    <nav class="hidden md:flex items-center gap-8 text-sm font-medium text-gray-300">
      <a href="#acerca" class="hover:text-cyan-400 transition-colors">Acerca de mí</a>
      <a href="#proyectos" class="hover:text-cyan-400 transition-colors">Proyectos</a>
      <a href="#blog" class="hover:text-cyan-400 transition-colors">Blog</a>
      <a href="#contacto" class="hover:text-cyan-400 transition-colors">Contacto</a>
    </nav>

    <a href="#contacto" class="glass-pill px-5 py-2 rounded-full text-sm font-semibold hover:bg-white hover:text-black transition-all">
      Contacto
    </a>
  </header>

  <!-- Hero Section -->
  <main class="w-full max-w-7xl mx-auto px-6 py-12 flex-1 flex flex-col lg:flex-row items-center justify-between gap-12 z-10">
    <!-- Columna Izquierda: Textos -->
    <div class="w-full lg:w-1/2 space-y-6">
      <div class="inline-flex items-center gap-2 glass-pill px-4 py-1.5 rounded-full text-xs font-semibold text-cyan-300">
        <span class="w-2 h-2 rounded-full bg-cyan-400 animate-pulse"></span>
        Disponible para nuevos proyectos
      </div>

      <h1 class="text-5xl sm:text-6xl font-extrabold tracking-tight text-white leading-tight">
        Hi, I'm <span class="text-transparent bg-clip-text bg-gradient-to-r from-cyan-400 to-blue-500">Elis.</span>
      </h1>

      class="text-xl font-medium text-cyan-200/90 italic">
        "Never give up, do your voice a big voice"
      </p>

      <p class="text-gray-300 text-lg leading-relaxed max-w-xl">
        Manejo múltiples plataformas como Excel, Word y nivel básico de Python. Pero, mi mayor herramienta siempre será mi voz.
      </p>

      <div class="pt-4 flex flex-wrap gap-4">
        <a href="#cv" class="bg-cyan-500 hover:bg-cyan-400 text-black font-bold px-8 py-3.5 rounded-full transition-all transform hover:scale-105 shadow-lg shadow-cyan-500/20">
          Ver CV <i class="fa-solid fa-arrow-down-long ml-2"></i>
        </a>
      </div>
    </div>

    <!-- Columna Derecha: Tarjeta de Perfil / Imagen estilo 11x -->
    <div class="w-full lg:w-5/12 flex justify-center">
      <div class="glass-card w-full max-w-md rounded-3xl p-4 shadow-2xl relative overflow-hidden group">
        <div class="relative h-96 w-full rounded-2xl overflow-hidden bg-gray-900">
          <img 
            src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?q=80&w=1000&auto=format&fit=crop" 
            alt="Elis Profile" 
            class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500"
          >
          
          <!-- Badge Superior estilo Autopilot -->
          <div class="absolute top-4 left-4 glass-pill px-3 py-1 rounded-full text-xs font-medium text-white flex items-center gap-1.5">
            <i class="fa-solid fa-microphone text-cyan-400"></i> Voice Activated
          </div>

          <!-- Banner Flotante Inferior -->
          <div class="absolute bottom-4 left-4 right-4 glass-card p-3 rounded-xl flex items-center gap-3 border border-white/10">
            <div class="w-10 h-10 rounded-lg bg-cyan-500/20 border border-cyan-400/30 flex items-center justify-center text-cyan-400">
              <i class="fa-solid fa-comment-dots text-lg"></i>
              </div>
            <div>
              <p class="text-xs font-semibold text-white">Elis Voice Assistant</p>
              <p class="text-[11px] text-gray-300">Comunicación efectiva & Gestión tecnológica</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>

  <!-- Banner Inferior de Tecnologías y Habilidades -->
  <footer class="w-full border-t border-white/10 glass-card py-6 mt-12 z-10">
    <div class="max-w-7xl mx-auto px-6">
      <p class="text-center text-xs font-semibold text-gray-400 uppercase tracking-widest mb-4">Herramientas & Habilidades clave</p>
      <div class="flex flex-wrap justify-center items-center gap-8 md:gap-16 text-gray-400 text-sm font-medium">
        <div class="flex items-center gap-2 hover:text-white transition-colors">
          <i class="fa-solid fa-file-excel text-green-500 text-xl"></i> Microsoft Excel
        </div>
        <div class="flex items-center gap-2 hover:text-white transition-colors">
          <i class="fa-solid fa-file-word text-blue-500 text-xl"></i> Microsoft Word
        </div>
        <div class="flex items-center gap-2 hover:text-white transition-colors">
          <i class="fa-brands fa-python text-yellow-400 text-xl"></i> Python (Básico)
        </div>
        <div class="flex items-center gap-2 hover:text-white transition-colors">
          <i class="fa-solid fa-palette text-pink-500 text-xl"></i> Canva
        </div>
        <div class="flex items-center gap-2 hover:text-white transition-colors">
          <i class="fa-solid fa-bullhorn text-cyan-400 text-xl"></i> Oratoria & Voz
        </div>
      </div>
    </div>
  </footer>

</body>
</html>
