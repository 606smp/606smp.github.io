<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>606-SMP | 1.16.5 Survival</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css">
  <style>
    body { font-family: 'Inter', system-ui, sans-serif; }
    .neon-text { text-shadow: 0 0 20px #22d3ee, 0 0 40px #22d3ee; }
    .card-hover:hover { transform: translateY(-10px); box-shadow: 0 0 30px rgba(34, 211, 238, 0.5); }
    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(30px); }
      to { opacity: 1; transform: translateY(0); }
    }
    .animate-in { animation: fadeInUp 0.8s ease forwards; }
  </style>
</head>
<body class="bg-zinc-950 text-white min-h-screen">

  <!-- Hero Section -->
  <section class="relative h-screen flex items-center justify-center overflow-hidden">
    <div class="absolute inset-0 bg-[radial-gradient(at_center,#22d3ee_0%,transparent_70%)] opacity-10"></div>
    
    <div class="text-center z-10 px-6">
      <h1 class="text-7xl md:text-8xl font-bold neon-text mb-4 tracking-tighter">606-SMP</h1>
      <p class="text-2xl md:text-3xl text-cyan-400 mb-8">Premium 1.16.5 Survival Experience</p>
      
      <div class="inline-flex items-center gap-3 bg-zinc-900 border border-cyan-500 rounded-2xl px-8 py-4 text-xl mb-10">
        <span class="text-emerald-400">🟢</span>
        <code class="font-mono">606smp.aternos.me</code>
      </div>

      <button onclick="copyIP()" 
              class="bg-cyan-500 hover:bg-cyan-400 text-black font-bold text-xl px-10 py-4 rounded-2xl transition-all duration-300 hover:scale-105">
        📋 Copy IP
      </button>
    </div>

    <div class="absolute bottom-10 text-cyan-500 animate-bounce">
      <i class="fas fa-chevron-down text-4xl"></i>
    </div>
  </section>

  <!-- Features -->
  <section class="py-20 px-6 bg-zinc-900">
    <div class="max-w-6xl mx-auto">
      <h2 class="text-5xl font-bold text-center mb-16 neon-text">Why Join 606-SMP?</h2>
      
      <div class="grid md:grid-cols-3 gap-8">
        <div class="bg-zinc-800 p-8 rounded-3xl card-hover transition-all duration-300 animate-in">
          <i class="fas fa-swords text-5xl text-cyan-400 mb-6"></i>
          <h3 class="text-2xl font-bold mb-3">True Survival</h3>
          <p class="text-zinc-400">No pay-to-win. Everything is earned through gameplay.</p>
        </div>
        <div class="bg-zinc-800 p-8 rounded-3xl card-hover transition-all duration-300 animate-in" style="animation-delay: 0.2s">
          <i class="fas fa-users text-5xl text-cyan-400 mb-6"></i>
          <h3 class="text-2xl font-bold mb-3">Great Community</h3>
          <p class="text-zinc-400">Friendly players & active staff.</p>
        </div>
        <div class="bg-zinc-800 p-8 rounded-3xl card-hover transition-all duration-300 animate-in" style="animation-delay: 0.4s">
          <i class="fas fa-shield-alt text-5xl text-cyan-400 mb-6"></i>
          <h3 class="text-2xl font-bold mb-3">Protected Builds</h3>
          <p class="text-zinc-400">Land claiming system to keep your base safe.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- IP + Version -->
  <section class="py-16 px-6 text-center bg-black">
    <div class="max-w-2xl mx-auto">
      <h2 class="text-4xl font-bold mb-6">Server Information</h2>
      <p class="text-2xl mb-4">IP: <span class="font-mono text-cyan-400">606smp.aternos.me</span></p>
      <p class="text-red-400 font-bold text-xl">✅ Only Minecraft 1.16.5 Works</p>
      <p class="text-zinc-500 mt-2">Newer versions will NOT connect</p>
    </div>
  </section>

  <!-- Premium Ranks -->
  <section class="py-20 px-6">
    <div class="max-w-5xl mx-auto text-center">
      <h2 class="text-5xl font-bold mb-4 neon-text">Premium Ranks</h2>
      <p class="text-xl text-zinc-400 mb-12">Support the server • Cosmetic rewards only</p>
      
      <div class="grid md:grid-cols-4 gap-6">
        <div class="bg-zinc-800 p-6 rounded-3xl">Iron</div>
        <div class="bg-amber-500 text-black p-6 rounded-3xl font-bold">Gold</div>
        <div class="bg-cyan-400 text-black p-6 rounded-3xl font-bold">Diamond</div>
        <div class="bg-emerald-500 text-black p-6 rounded-3xl font-bold">Emerald</div>
      </div>
    </div>
  </section>

  <footer class="bg-black py-12 text-center text-zinc-500">
    <p class="text-xl mb-2">Made with ❤️ for the 606-SMP Community</p>
    <p>© 2026 606-SMP • All Rights Reserved</p>
  </footer>

  <script>
    function copyIP() {
      navigator.clipboard.writeText("606smp.aternos.me");
      const btn = document.querySelector("button");
      const original = btn.innerHTML;
      btn.innerHTML = "✅ Copied!";
      setTimeout(() => btn.innerHTML = original, 2000);
    }

    // Tailwind script already included
  </script>
</body>
</html>
