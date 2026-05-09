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
    .neon-glow { text-shadow: 0 0 25px #22d3ee, 0 0 50px #22d3ee; }
    .card { transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1); }
    .card:hover { transform: translateY(-12px) scale(1.03); box-shadow: 0 0 40px rgba(34, 211, 238, 0.6); }
    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(40px); }
      to { opacity: 1; transform: translateY(0); }
    }
    .animate-in { animation: fadeInUp 0.9s ease forwards; }
  </style>
</head>
<body class="bg-zinc-950 text-white overflow-x-hidden">

  <!-- Top Title Bar -->
  <div class="fixed top-0 left-0 right-0 bg-black/80 backdrop-blur-md border-b border-cyan-900 z-50">
    <div class="max-w-6xl mx-auto px-6 py-5 flex justify-between items-center">
      <h1 class="text-3xl font-bold tracking-tight neon-glow">606-SMP</h1>
      <div class="text-cyan-400 font-mono text-sm">1.16.5 SURVIVAL</div>
    </div>
  </div>

  <!-- Hero Section -->
  <section class="min-h-screen flex items-center justify-center relative pt-20">
    <div class="absolute inset-0 bg-[radial-gradient(circle_at_center,#22d3ee_0%,transparent_60%)] opacity-10"></div>
    
    <div class="text-center px-6 max-w-4xl mx-auto">
      <h2 class="text-6xl md:text-7xl font-bold mb-6 neon-glow">Welcome to 606-SMP</h2>
      <p class="text-2xl text-zinc-400 mb-10">A premium fair-play survival experience on Minecraft 1.16.5</p>
      
      <div class="inline-flex items-center gap-4 bg-zinc-900 border border-cyan-500/50 rounded-3xl px-10 py-5 text-2xl mb-10">
        <span class="text-emerald-400">🟢 Online</span>
        <code class="font-mono bg-black px-6 py-2 rounded-2xl">606smp.aternos.me</code>
      </div>

      <button onclick="copyIP()" 
              class="bg-cyan-500 hover:bg-cyan-400 text-black font-bold text-xl px-12 py-5 rounded-2xl transition-all duration-300 hover:scale-105 active:scale-95">
        📋 Copy Server IP
      </button>
    </div>

    <div class="absolute bottom-10 w-full text-center">
      <i class="fas fa-chevron-down text-4xl text-cyan-500 animate-bounce"></i>
    </div>
  </section>

  <!-- Features -->
  <section class="py-24 px-6 bg-zinc-900">
    <div class="max-w-6xl mx-auto">
      <h2 class="text-5xl font-bold text-center mb-16 neon-glow">Why Players Love 606-SMP</h2>
      
      <div class="grid md:grid-cols-3 gap-8">
        <div class="bg-zinc-800/70 p-8 rounded-3xl card animate-in">
          <i class="fas fa-swords text-5xl text-cyan-400 mb-6"></i>
          <h3 class="text-2xl font-bold mb-3">Pure Survival</h3>
          <p class="text-zinc-400">No pay-to-win. Everything earned fairly.</p>
        </div>
        <div class="bg-zinc-800/70 p-8 rounded-3xl card animate-in" style="animation-delay: 150ms">
          <i class="fas fa-users text-5xl text-cyan-400 mb-6"></i>
          <h3 class="text-2xl font-bold mb-3">Amazing Community</h3>
          <p class="text-zinc-400">Friendly players and active moderation.</p>
        </div>
        <div class="bg-zinc-800/70 p-8 rounded-3xl card animate-in" style="animation-delay: 300ms">
          <i class="fas fa-shield-alt text-5xl text-cyan-400 mb-6"></i>
          <h3 class="text-2xl font-bold mb-3">Protected Builds</h3>
          <p class="text-zinc-400">Land claiming to keep your hard work safe.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Server Info -->
  <section class="py-20 px-6 text-center bg-black">
    <h2 class="text-4xl font-bold mb-8">Server Details</h2>
    <p class="text-3xl mb-3">IP: <span class="font-mono text-cyan-400">606smp.aternos.me</span></p>
    <p class="text-red-400 text-xl font-semibold">Only Minecraft 1.16.5 is supported</p>
  </section>

  <!-- Premium Ranks -->
  <section class="py-20 px-6 bg-zinc-900">
    <div class="max-w-5xl mx-auto text-center">
      <h2 class="text-5xl font-bold mb-6 neon-glow">Premium Ranks</h2>
      <p class="text-zinc-400 mb-12 text-lg">Support the server • Get cosmetic rewards</p>
      
      <div class="flex flex-wrap justify-center gap-6">
        <div class="bg-zinc-800 px-10 py-6 rounded-3xl text-xl font-semibold">Iron</div>
        <div class="bg-amber-500 text-black px-10 py-6 rounded-3xl text-xl font-bold">Gold</div>
        <div class="bg-cyan-400 text-black px-10 py-6 rounded-3xl text-xl font-bold">Diamond</div>
        <div class="bg-emerald-500 text-black px-10 py-6 rounded-3xl text-xl font-bold">Emerald</div>
      </div>
    </div>
  </section>

  <footer class="bg-black py-12 text-center text-zinc-500 border-t border-zinc-800">
    <p class="text-lg">Made with ❤️ for the 606-SMP Community</p>
    <p class="mt-2">© 2026 606-SMP • All Rights Reserved</p>
  </footer>

  <script>
    function copyIP() {
      navigator.clipboard.writeText("606smp.aternos.me");
      const btn = document.querySelector("button");
      const originalText = btn.innerHTML;
      btn.innerHTML = "✅ IP Copied!";
      setTimeout(() => { btn.innerHTML = originalText; }, 2500);
    }
  </script>
</body>
</html>
