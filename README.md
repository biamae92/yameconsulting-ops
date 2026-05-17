<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>YAME Consulting Dashboard</title>

  <script src="https://cdn.tailwindcss.com"></script>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">

  <style>
    * { font-family: 'Inter', sans-serif; }

    body {
      background:
        radial-gradient(circle at top left, rgba(16,185,129,.18), transparent 30%),
        radial-gradient(circle at bottom right, rgba(250,204,21,.14), transparent 30%),
        linear-gradient(to bottom right, #020617, #0f172a, #052e16);
      overflow-x: hidden;
      color: white;
    }

    .glass {
      background: rgba(255,255,255,0.05);
      backdrop-filter: blur(14px);
      border: 1px solid rgba(255,255,255,0.08);
    }

    .perspective { perspective: 1400px; }

    .card3d {
      transform-style: preserve-3d;
      transform: rotateY(14deg) rotateX(7deg);
      transition: all .8s ease;
    }

    .card3d:hover {
      transform: rotateY(0deg) rotateX(0deg) scale(1.03);
    }

    .gradient-text {
      background: linear-gradient(to right, #6ee7b7, #fde68a);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .metric-bar {
      height: 10px;
      border-radius: 999px;
      overflow: hidden;
      background: rgba(255,255,255,.08);
    }

    .metric-fill {
      height: 100%;
      background: linear-gradient(to right, #10b981, #fde047);
    }
  </style>
</head>

<body class="min-h-screen">

  <section class="px-6 py-10 md:px-14">
    <div class="max-w-7xl mx-auto glass rounded-[34px] p-8 md:p-14">

      <div class="flex flex-col lg:flex-row items-center justify-between gap-14">

        <div class="max-w-2xl space-y-7">

          <div class="inline-flex items-center gap-3 px-5 py-2 rounded-full bg-emerald-500/10 border border-emerald-400/20 text-emerald-300 text-sm">
            AFTER-HOURS DAILY OPERATIONS SOP
          </div>

          <div class="space-y-4">
            <h1 class="text-5xl md:text-7xl font-black leading-none tracking-tight">
              YAME
              <span class="block gradient-text">CONSULTING</span>
            </h1>

            <p class="text-slate-300 text-lg leading-relaxed">
              Immersive operational oversight dashboard for time entries,
              ticket activity, ShareFile verification, billing integrity,
              and accountability monitoring.
            </p>
          </div>

          <div class="flex flex-wrap gap-4">
            <button class="px-7 py-4 rounded-2xl bg-gradient-to-r from-emerald-400 to-emerald-600 font-bold shadow-2xl hover:scale-105 transition-all duration-300">
              Launch Dashboard
            </button>

            <button class="px-7 py-4 rounded-2xl border border-white/10 bg-white/5 hover:bg-white/10 transition-all duration-300">
              View SOP
            </button>
          </div>
        </div>

        <div class="perspective">
          <div class="card3d glass rounded-[34px] p-8 shadow-2xl">
            <img src="logo.png" alt="YAME Logo" class="w-[320px] max-w-full drop-shadow-2xl" />
          </div>
        </div>

      </div>
    </div>
  </section>

  <section class="px-6 py-6 md:px-14">
    <div class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-3 gap-7">

      <div class="glass rounded-[30px] p-8 hover:-translate-y-2 transition-all duration-500">
        <h2 class="text-2xl font-black mb-5">⏱️ Time Entries</h2>
        <ul class="space-y-3 text-slate-300">
          <li>✓ Missing entries</li>
          <li>✓ Incorrect descriptions</li>
          <li>✓ Incomplete descriptions</li>
          <li>✓ QBO login mismatch</li>
          <li>✓ Overlogged hours</li>
        </ul>
      </div>

      <div class="glass rounded-[30px] p-8 hover:-translate-y-2 transition-all duration-500">
        <h2 class="text-2xl font-black mb-5">🎫 Ticket Health</h2>
        <ul class="space-y-3 text-slate-300">
          <li>✓ Stale tickets >24h</li>
          <li>✓ Update mismatches</li>
          <li>✓ Comments outside logged time</li>
          <li>✓ Client service risks</li>
          <li>✓ Daily validation review</li>
        </ul>
      </div>

      <div class="glass rounded-[30px] p-8 hover:-translate-y-2 transition-all duration-500">
        <h2 class="text-2xl font-black mb-5">📂 ShareFile Verification</h2>
        <ul class="space-y-3 text-slate-300">
          <li>✓ Upload completion</li>
          <li>✓ Correct folder placement</li>
          <li>✓ No partial files</li>
          <li>✓ Naming conventions</li>
          <li>✓ Documentation completeness</li>
        </ul>
      </div>

    </div>
  </section>

  <section class="px-6 py-10 md:px-14">
    <div class="max-w-7xl mx-auto glass rounded-[34px] overflow-hidden">

      <div class="flex flex-col md:flex-row items-center justify-between gap-4 px-8 py-7 border-b border-white/10">
        <div>
          <h2 class="text-4xl font-black">Daily Ops Dashboard</h2>
          <p class="text-slate-400 mt-2">
            Real-time operational health scoring and accountability tracking.
          </p>
        </div>

        <div class="px-6 py-4 rounded-3xl bg-gradient-to-r from-emerald-500/10 to-yellow-400/10 border border-white/10">
          <div class="text-slate-400 text-sm">Target Score</div>
          <div class="text-4xl font-black text-emerald-300">12/15</div>
        </div>
      </div>

      <div class="overflow-x-auto">
        <table class="w-full text-left">
          <thead class="bg-white/5 text-slate-300">
            <tr>
              <th class="p-6">Area</th>
              <th class="p-6">Score</th>
              <th class="p-6">Status</th>
              <th class="p-6">Progress</th>
              <th class="p-6">Notes</th>
            </tr>
          </thead>

          <tbody>
            <tr class="border-t border-white/10 hover:bg-white/5 transition">
              <td class="p-6 font-semibold">Time Entries</td>
              <td class="p-6 text-2xl font-black text-emerald-300">5/5</td>
              <td class="p-6"><span class="px-4 py-2 rounded-full text-sm font-semibold bg-emerald-500/20 text-emerald-300">GREEN</span></td>
              <td class="p-6">
                <div class="metric-bar w-40"><div class="metric-fill" style="width:100%"></div></div>
              </td>
              <td class="p-6 text-slate-300">All entries verified and matched.</td>
            </tr>

            <tr class="border-t border-white/10 hover:bg-white/5 transition">
              <td class="p-6 font-semibold">Tickets</td>
              <td class="p-6 text-2xl font-black text-yellow-300">4/5</td>
              <td class="p-6"><span class="px-4 py-2 rounded-full text-sm font-semibold bg-yellow-500/20 text-yellow-300">WARNING</span></td>
              <td class="p-6">
                <div class="metric-bar w-40"><div class="metric-fill" style="width:80%"></div></div>
              </td>
              <td class="p-6 text-slate-300">Minor stale ticket risk detected.</td>
            </tr>

            <tr class="border-t border-white/10 hover:bg-white/5 transition">
              <td class="p-6 font-semibold">ShareFile</td>
              <td class="p-6 text-2xl font-black text-emerald-300">5/5</td>
              <td class="p-6"><span class="px-4 py-2 rounded-full text-sm font-semibold bg-emerald-500/20 text-emerald-300">GREEN</span></td>
              <td class="p-6">
                <div class="metric-bar w-40"><div class="metric-fill" style="width:100%"></div></div>
              </td>
              <td class="p-6 text-slate-300">Uploads complete and organized.</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </section>

  <footer class="px-6 py-10 md:px-14 text-center text-slate-400 border-t border-white/10 mt-10">
    © 2026 YAME Consulting — After-Hours Operations Monitoring System
  </footer>

</body>
</html>
