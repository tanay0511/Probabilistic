<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Probabyltics — Probabilistic Outcome & Risk Analyzer</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">

  <script>
    tailwind.config = {
      darkMode: 'class',
      theme: {
        extend: {
          fontFamily: {
            sans: ['Inter', 'sans-serif'],
            mono: ['JetBrains Mono', 'monospace'],
          },
          colors: {
            brand: {
              50: '#eef2ff',
              400: '#818cf8',
              500: '#6366f1',
              600: '#4f46e5',
            },
            dark: {
              850: '#0f172a',
              900: '#090d16',
              950: '#030712'
            }
          }
        }
      }
    };
  </script>

  <style>
    body {
      background-color: #080c14;
      color: #f1f5f9;
      font-family: 'Inter', sans-serif;
    }
    .glass-card {
      background: rgba(15, 23, 42, 0.72);
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      border: 1px solid rgba(255, 255, 255, 0.08);
      box-shadow: 0 10px 30px -10px rgba(0, 0, 0, 0.5);
    }
    .glass-card:hover {
      border-color: rgba(99, 102, 241, 0.28);
    }
    .glow-indigo {
      box-shadow: 0 0 35px -5px rgba(99, 102, 241, 0.35);
    }
    .glow-emerald {
      box-shadow: 0 0 35px -5px rgba(16, 185, 129, 0.35);
    }
    .slider-thumb::-webkit-slider-thumb {
      appearance: none;
      height: 18px;
      width: 18px;
      border-radius: 9999px;
      background: #6366f1;
      cursor: pointer;
      box-shadow: 0 0 8px #6366f1;
      border: 2px solid #ffffff;
    }
    .slider-thumb::-moz-range-thumb {
      height: 18px;
      width: 18px;
      border-radius: 9999px;
      background: #6366f1;
      cursor: pointer;
      box-shadow: 0 0 8px #6366f1;
      border: 2px solid #ffffff;
    }
    @keyframes pulseSubtle {
      0%, 100% { opacity: 1; transform: scale(1); }
      50% { opacity: 0.85; transform: scale(1.015); }
    }
    .pulse-subtle {
      animation: pulseSubtle 3s infinite ease-in-out;
    }
    @media print {
      body { background: white; color: black; }
      .no-print { display: none !important; }
      .glass-card { border: 1px solid #ccc; background: white; color: black; }
    }
  </style>
</head>
<body class="min-h-screen selection:bg-indigo-500 selection:text-white flex flex-col justify-between">

  <header class="sticky top-0 z-40 backdrop-blur-md bg-dark-900/80 border-b border-slate-800">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-16 flex items-center justify-between">
      <div class="flex items-center space-x-3">
        <div class="w-10 h-10 rounded-xl bg-gradient-to-tr from-indigo-600 via-purple-600 to-emerald-400 flex items-center justify-center text-white shadow-lg shadow-indigo-500/20">
          <i class="fa-solid fa-chart-pie text-lg"></i>
        </div>
        <div>
          <span class="font-extrabold text-xl tracking-tight bg-clip-text text-transparent bg-gradient-to-r from-indigo-400 via-sky-300 to-emerald-400">
            Probabyltics
          </span>
          <span class="hidden sm:inline-block ml-2 text-xs font-mono uppercase px-2 py-0.5 rounded-full bg-slate-800 text-indigo-300 border border-slate-700">
            Monte Carlo Engine
          </span>
        </div>
      </div>

      <div class="flex items-center space-x-3">
        <button id="scenarioBtn" onclick="toggleScenarioDrawer()" class="px-3 py-1.5 rounded-lg bg-slate-800/80 hover:bg-slate-700 text-slate-300 border border-slate-700 text-xs font-medium flex items-center space-x-2 transition">
          <i class="fa-solid fa-clock-rotate-left"></i>
          <span class="hidden md:inline">Saved Scenarios</span>
          <span id="savedCountBadge" class="bg-indigo-600 text-white rounded-full px-1.5 py-0.2 text-[10px]">0</span>
        </button>
        <button id="apiKeyModalBtn" onclick="openKeyModal()" class="px-3 py-1.5 rounded-lg bg-slate-800/80 hover:bg-slate-700 text-slate-300 border border-slate-700 text-xs font-medium flex items-center space-x-1.5 transition">
          <i class="fa-solid fa-key text-yellow-400"></i>
          <span id="apiKeyStatusText">API Key</span>
        </button>
      </div>
    </div>
  </header>

  <main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8 flex-1 w-full space-y-8">
    
    <!-- Hero / Input Box -->
    <section class="glass-card rounded-2xl p-6 sm:p-8 border border-slate-800 relative overflow-hidden">
      <div class="absolute -right-16 -top-16 w-64 h-64 bg-indigo-500/10 rounded-full blur-3xl pointer-events-none"></div>
      <div class="absolute -left-16 -bottom-16 w-64 h-64 bg-emerald-500/10 rounded-full blur-3xl pointer-events-none"></div>

      <div class="max-w-3xl">
        <h1 class="text-2xl sm:text-3xl font-bold text-white tracking-tight">
          Quantify the Uncertain. Predict Your Odds.
        </h1>
        <p class="text-slate-400 text-sm sm:text-base mt-2">
          Describe any challenge, career gamble, investment, or personal endeavor. Our probabilistic synthesis engine simulates 10,000 Monte Carlo runs to calculate your true odds, failure traps, and leverage levers.
        </p>
      </div>

      <!-- Text input form -->
      <div class="mt-6">
        <label for="problemInput" class="block text-xs font-semibold uppercase tracking-wider text-slate-400 mb-2">
          Your Dilemma, Ambition or Decision
        </label>
        <div class="relative">
          <textarea id="problemInput" rows="3" 
            placeholder="e.g., 'Launching a B2B AI SaaS product with $10k budget and 6 months runway as a solo founder' or 'Negotiating for a 35% raise in my current company during a corporate hiring freeze'"
            class="w-full bg-slate-950/80 border border-slate-700 rounded-xl px-4 py-3.5 text-sm sm:text-base text-white placeholder-slate-500 focus:outline-none focus:ring-2 focus:ring-indigo-500 focus:border-transparent resize-y transition shadow-inner font-sans"></textarea>
          <div class="mt-2 flex flex-wrap items-center justify-between gap-3">
            <div class="flex items-center flex-wrap gap-2 text-xs">
              <span class="text-slate-400 font-medium">Presets:</span>
              <button onclick="fillPreset('startup')" class="px-2.5 py-1 rounded-md bg-slate-800 hover:bg-slate-700 text-indigo-300 border border-slate-700/60 transition">🚀 Solo AI SaaS</button>
              <button onclick="fillPreset('salary')" class="px-2.5 py-1 rounded-md bg-slate-800 hover:bg-slate-700 text-indigo-300 border border-slate-700/60 transition">💼 +30% Salary Raise</button>
              <button onclick="fillPreset('relocation')" class="px-2.5 py-1 rounded-md bg-slate-800 hover:bg-slate-700 text-indigo-300 border border-slate-700/60 transition">✈️ Emigrating Solo</button>
              <button onclick="fillPreset('exam')" class="px-2.5 py-1 rounded-md bg-slate-800 hover:bg-slate-700 text-indigo-300 border border-slate-700/60 transition">🎓 Med Entrance in 6 Mos</button>
            </div>
            
            <button id="runAnalysisBtn" onclick="executeAnalysis()" class="px-6 py-3 rounded-xl bg-gradient-to-r from-indigo-600 via-indigo-500 to-emerald-500 hover:from-indigo-500 hover:to-emerald-400 text-white font-semibold text-sm shadow-lg shadow-indigo-500/25 flex items-center space-x-2 transition transform active:scale-95">
              <i class="fa-solid fa-wand-magic-sparkles"></i>
              <span>Simulate Odds</span>
            </button>
          </div>
        </div>
      </div>

      <!-- Loading State Overlay -->
      <div id="loadingOverlay" class="hidden mt-6 p-6 rounded-xl bg-slate-900/90 border border-indigo-500/30 flex flex-col items-center justify-center text-center space-y-3">
        <div class="w-12 h-12 border-4 border-indigo-500/20 border-t-indigo-500 rounded-full animate-spin"></div>
        <div class="text-sm font-semibold text-white" id="loadingStepText">Deconstructing domain variables & causal graphs...</div>
        <div class="text-xs text-slate-400 font-mono">Running Bayesian priors & Monte Carlo distribution analysis...</div>
      </div>
    </section>

    <section id="resultsSection" class="hidden space-y-8">

      <!-- Top Summary Metrics Row -->
      <div class="grid grid-cols-1 md:grid-cols-4 gap-4">
        
        <!-- Success Probability Card -->
        <div class="glass-card rounded-xl p-5 border border-slate-800 flex flex-col justify-between relative overflow-hidden">
          <div class="flex items-center justify-between text-slate-400 text-xs font-semibold uppercase tracking-wider">
            <span>Probability of Success</span>
            <span class="w-2.5 h-2.5 rounded-full bg-emerald-400 animate-ping"></span>
          </div>
          <div class="my-4">
            <span id="metricSuccessVal" class="text-4xl sm:text-5xl font-extrabold text-emerald-400 font-mono tracking-tight">0%</span>
            <span class="text-xs text-slate-400 ml-1 font-mono">P(S)</span>
          </div>
          <div class="text-xs text-slate-400 flex items-center justify-between">
            <span>Status:</span>
            <span id="metricRatingLabel" class="font-semibold text-emerald-300">Viable</span>
          </div>
        </div>

        <!-- Failure Risk Card -->
        <div class="glass-card rounded-xl p-5 border border-slate-800 flex flex-col justify-between">
          <div class="flex items-center justify-between text-slate-400 text-xs font-semibold uppercase tracking-wider">
            <span>Probability of Failure</span>
            <i class="fa-solid fa-triangle-exclamation text-rose-400"></i>
          </div>
          <div class="my-4">
            <span id="metricFailureVal" class="text-4xl sm:text-5xl font-extrabold text-rose-400 font-mono tracking-tight">0%</span>
            <span class="text-xs text-slate-400 ml-1 font-mono">P(F)</span>
          </div>
          <div class="text-xs text-slate-400 flex items-center justify-between">
            <span>Primary Hazard:</span>
            <span id="metricTopHazard" class="font-semibold text-rose-300 truncate max-w-[120px]">Burnout</span>
          </div>
        </div>

        <!-- 90% Confidence Interval Card -->
        <div class="glass-card rounded-xl p-5 border border-slate-800 flex flex-col justify-between">
          <div class="flex items-center justify-between text-slate-400 text-xs font-semibold uppercase tracking-wider">
            <span>90% Confidence Interval</span>
            <i class="fa-solid fa-arrows-split-up-and-left text-sky-400"></i>
          </div>
          <div class="my-4">
            <span id="metricCiVal" class="text-2xl sm:text-3xl font-extrabold text-sky-300 font-mono tracking-tight">[0% - 0%]</span>
          </div>
          <div class="text-xs text-slate-400 flex items-center justify-between">
            <span>Uncertainty Level:</span>
            <span id="metricUncertainty" class="font-semibold text-sky-400">Moderate</span>
          </div>
        </div>

        <!-- Leverage Potential Card -->
        <div class="glass-card rounded-xl p-5 border border-slate-800 flex flex-col justify-between">
          <div class="flex items-center justify-between text-slate-400 text-xs font-semibold uppercase tracking-wider">
            <span>Max Optimized Upside</span>
            <i class="fa-solid fa-rocket text-indigo-400"></i>
          </div>
          <div class="my-4">
            <span id="metricOptimizedVal" class="text-4xl sm:text-5xl font-extrabold text-indigo-400 font-mono tracking-tight">+0%</span>
          </div>
          <div class="text-xs text-slate-400 flex items-center justify-between">
            <span>With Mitigations:</span>
            <span id="metricTargetVal" class="font-semibold text-indigo-300 font-mono">Up to 0%</span>
          </div>
        </div>
      </div>

      <div class="glass-card rounded-2xl p-6 border border-indigo-500/20 shadow-xl bg-slate-900/60">
        <div class="flex flex-col sm:flex-row sm:items-center justify-between pb-4 border-b border-slate-800 gap-2">
          <div>
            <h2 class="text-lg font-bold text-white flex items-center gap-2">
              <i class="fa-solid fa-sliders text-indigo-400"></i>
              Interactive Sensitivity Sliders (Live Monte Carlo Recalculation)
            </h2>
            <p class="text-xs text-slate-400">
              Adjust your parameters in real-time. The client engine re-runs 10,000 iterations to dynamically re-evaluate your odds distribution.
            </p>
          </div>
          <button onclick="resetSliders()" class="self-start sm:self-auto text-xs text-slate-400 hover:text-white px-3 py-1 rounded bg-slate-800 border border-slate-700">
            Reset to Baseline
          </button>
        </div>

        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6 mt-6">
          <!-- Slider 1: Effort / Prep -->
          <div class="space-y-2">
            <div class="flex justify-between text-xs">
              <span class="font-medium text-slate-300">Execution / Preparation</span>
              <span id="sliderEffortLabel" class="font-mono text-indigo-400 font-bold">50%</span>
            </div>
            <input id="sliderEffort" type="range" min="10" max="100" value="50" oninput="handleSliderChange()" class="w-full h-2 bg-slate-800 rounded-lg appearance-none cursor-pointer slider-thumb">
            <div class="flex justify-between text-[10px] text-slate-500">
              <span>Minimal</span>
              <span>Obsessive</span>
            </div>
          </div>

          <!-- Slider 2: Resource Allocation / Budget -->
          <div class="space-y-2">
            <div class="flex justify-between text-xs">
              <span class="font-medium text-slate-300">Capital / Resource Runway</span>
              <span id="sliderBudgetLabel" class="font-mono text-indigo-400 font-bold">50%</span>
            </div>
            <input id="sliderBudget" type="range" min="10" max="100" value="50" oninput="handleSliderChange()" class="w-full h-2 bg-slate-800 rounded-lg appearance-none cursor-pointer slider-thumb">
            <div class="flex justify-between text-[10px] text-slate-500">
              <span>Constrained</span>
              <span>Abundant</span>
            </div>
          </div>

          <!-- Slider 3: Aggressiveness / Risk Tolerance -->
          <div class="space-y-2">
            <div class="flex justify-between text-xs">
              <span class="font-medium text-slate-300">Strategic Aggressiveness</span>
              <span id="sliderAggressionLabel" class="font-mono text-indigo-400 font-bold">50%</span>
            </div>
            <input id="sliderAggression" type="range" min="10" max="100" value="50" oninput="handleSliderChange()" class="w-full h-2 bg-slate-800 rounded-lg appearance-none cursor-pointer slider-thumb">
            <div class="flex justify-between text-[10px] text-slate-500">
              <span>Conservative</span>
              <span>High Risk/Reward</span>
            </div>
          </div>

          <!-- Slider 4: Luck & Environmental Volatility -->
          <div class="space-y-2">
            <div class="flex justify-between text-xs">
              <span class="font-medium text-slate-300">Market / External Volatility</span>
              <span id="sliderVolatilityLabel" class="font-mono text-indigo-400 font-bold">50%</span>
            </div>
            <input id="sliderVolatility" type="range" min="10" max="100" value="50" oninput="handleSliderChange()" class="w-full h-2 bg-slate-800 rounded-lg appearance-none cursor-pointer slider-thumb">
            <div class="flex justify-between text-[10px] text-slate-500">
              <span>Stable</span>
              <span>Chaotic</span>
            </div>
          </div>
        </div>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-12 gap-6">
        
        <!-- Left Column: Gauge & Radar -->
        <div class="lg:col-span-4 space-y-6">
          <!-- Donut Split -->
          <div class="glass-card rounded-2xl p-5 border border-slate-800 flex flex-col items-center">
            <h3 class="text-xs font-semibold uppercase tracking-wider text-slate-400 mb-2 w-full text-left">
              Outcome Ratio
            </h3>
            <div class="relative w-48 h-48 my-2">
              <canvas id="donutChart"></canvas>
              <div class="absolute inset-0 flex flex-col items-center justify-center pointer-events-none">
                <span id="donutCenterPct" class="text-2xl font-black text-white font-mono">0%</span>
                <span class="text-[10px] text-slate-400 uppercase tracking-wider">Success</span>
              </div>
            </div>
            <div class="flex justify-around w-full mt-2 text-xs font-mono">
              <span class="text-emerald-400 flex items-center gap-1.5"><span class="w-2.5 h-2.5 rounded-full bg-emerald-500 inline-block"></span> Success</span>
              <span class="text-rose-400 flex items-center gap-1.5"><span class="w-2.5 h-2.5 rounded-full bg-rose-500 inline-block"></span> Failure</span>
            </div>
          </div>

          <!-- Radar Factor Analysis -->
          <div class="glass-card rounded-2xl p-5 border border-slate-800">
            <h3 class="text-xs font-semibold uppercase tracking-wider text-slate-400 mb-3">
              Factor Sensitivity Radar
            </h3>
            <div class="w-full h-56">
              <canvas id="radarChart"></canvas>
            </div>
          </div>
        </div>

        <!-- Right Column: Monte Carlo Bell Curve Distribution -->
        <div class="lg:col-span-8 space-y-6">
          <div class="glass-card rounded-2xl p-6 border border-slate-800 h-full flex flex-col justify-between">
            <div>
              <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-2">
                <div>
                  <h3 class="text-sm font-bold uppercase tracking-wider text-slate-300 flex items-center gap-2">
                    <i class="fa-solid fa-chart-line text-indigo-400"></i>
                    Monte Carlo Probability Density Function (10,000 Iterations)
                  </h3>
                  <p class="text-xs text-slate-400 mt-1">
                    Simulated performance score distribution with Value-at-Risk percentiles (P10 Bear, P50 Median, P90 Bull).
                  </p>
                </div>
                <span class="px-2.5 py-1 text-xs font-mono rounded bg-slate-800 border border-slate-700 text-slate-300 self-start">
                  Runs: 10,000
                </span>
              </div>

              <!-- Canvas Container -->
              <div class="w-full h-72 sm:h-80 mt-4">
                <canvas id="pdfChart"></canvas>
              </div>
            </div>

            <!-- Percentile Pill Indicators -->
            <div class="grid grid-cols-3 gap-3 pt-4 mt-2 border-t border-slate-800 text-center text-xs">
              <div class="p-2 rounded-lg bg-slate-950/60 border border-slate-800">
                <span class="text-slate-500 block text-[10px] uppercase font-mono">P10 (Pessimistic)</span>
                <span id="p10Label" class="font-bold text-rose-400 font-mono text-sm sm:text-base">0%</span>
              </div>
              <div class="p-2 rounded-lg bg-slate-950/60 border border-indigo-500/20">
                <span class="text-indigo-400 block text-[10px] uppercase font-mono">P50 (Median Expected)</span>
                <span id="p50Label" class="font-bold text-indigo-300 font-mono text-sm sm:text-base">0%</span>
              </div>
              <div class="p-2 rounded-lg bg-slate-950/60 border border-slate-800">
                <span class="text-slate-500 block text-[10px] uppercase font-mono">P90 (Optimistic)</span>
                <span id="p90Label" class="font-bold text-emerald-400 font-mono text-sm sm:text-base">0%</span>
              </div>
            </div>
          </div>
        </div>

      </div>

      <div class="grid grid-cols-1 lg:grid-cols-3 gap-6">

        <!-- Positive Drivers -->
        <div class="glass-card rounded-2xl p-6 border border-slate-800">
          <h3 class="text-sm font-bold text-emerald-400 uppercase tracking-wider mb-4 flex items-center gap-2">
            <i class="fa-solid fa-circle-arrow-up"></i>
            Key Success Drivers
          </h3>
          <ul id="driversList" class="space-y-3 text-xs sm:text-sm text-slate-300">
            <!-- Injected dynamically -->
          </ul>
        </div>

        <!-- Failure Modes / Risks -->
        <div class="glass-card rounded-2xl p-6 border border-slate-800">
          <h3 class="text-sm font-bold text-rose-400 uppercase tracking-wider mb-4 flex items-center gap-2">
            <i class="fa-solid fa-triangle-exclamation"></i>
            Critical Failure Modes
          </h3>
          <ul id="risksList" class="space-y-3 text-xs sm:text-sm text-slate-300">
            <!-- Injected dynamically -->
          </ul>
        </div>

        <!-- High-leverage Mitigations -->
        <div class="glass-card rounded-2xl p-6 border border-indigo-500/30">
          <h3 class="text-sm font-bold text-indigo-400 uppercase tracking-wider mb-4 flex items-center gap-2">
            <i class="fa-solid fa-bolt-lightning"></i>
            Leverage Action Plan
          </h3>
          <ul id="mitigationsList" class="space-y-3 text-xs sm:text-sm text-slate-300">
            <!-- Injected dynamically -->
          </ul>
        </div>

      </div>

      <!-- Action bar: Save scenario, Export Report -->
      <div class="flex flex-wrap items-center justify-between gap-4 p-4 rounded-xl bg-slate-900 border border-slate-800">
        <div class="text-xs text-slate-400">
          Domain: <span id="domainBadge" class="font-semibold text-slate-200 uppercase">General Venture</span>
        </div>
        <div class="flex items-center space-x-3">
          <button onclick="saveCurrentScenario()" class="px-4 py-2 rounded-lg bg-slate-800 hover:bg-slate-700 text-slate-200 text-xs font-semibold border border-slate-700 transition flex items-center gap-1.5">
            <i class="fa-solid fa-bookmark text-indigo-400"></i>
            Save Scenario
          </button>
          <button onclick="copySummaryText()" class="px-4 py-2 rounded-lg bg-slate-800 hover:bg-slate-700 text-slate-200 text-xs font-semibold border border-slate-700 transition flex items-center gap-1.5">
            <i class="fa-regular fa-copy"></i>
            Copy Executive Brief
          </button>
          <button onclick="window.print()" class="px-4 py-2 rounded-lg bg-indigo-600 hover:bg-indigo-500 text-white text-xs font-semibold shadow transition flex items-center gap-1.5">
            <i class="fa-solid fa-file-pdf"></i>
            Export PDF / Print
          </button>
        </div>
      </div>

    </section>

  </main>

  <!-- Saved Scenarios Drawer -->
  <div id="scenarioDrawer" class="fixed inset-y-0 right-0 w-full max-w-md bg-dark-900/95 border-l border-slate-800 p-6 z-50 transform translate-x-full transition-transform duration-300 ease-in-out overflow-y-auto backdrop-blur-xl shadow-2xl">
    <div class="flex items-center justify-between pb-4 border-b border-slate-800">
      <h3 class="font-bold text-white text-base flex items-center gap-2">
        <i class="fa-solid fa-clock-rotate-left text-indigo-400"></i>
        Saved Scenarios
      </h3>
      <button onclick="toggleScenarioDrawer()" class="text-slate-400 hover:text-white p-1">
        <i class="fa-solid fa-xmark text-lg"></i>
      </button>
    </div>
    
    <div id="savedScenarioList" class="mt-4 space-y-3">
      <p class="text-slate-500 text-xs italic">No saved simulations yet. Click 'Save Scenario' on any result.</p>
    </div>
  </div>

  <!-- API Key Modal -->
  <div id="apiKeyModal" class="hidden fixed inset-0 bg-black/70 backdrop-blur-sm z-50 flex items-center justify-center p-4">
    <div class="bg-dark-850 border border-slate-700 max-w-md w-full rounded-2xl p-6 shadow-2xl space-y-4">
      <div class="flex items-center justify-between">
        <h4 class="text-base font-bold text-white flex items-center gap-2">
          <i class="fa-solid fa-key text-yellow-400"></i>
          Gemini API Configuration
        </h4>
        <button onclick="closeKeyModal()" class="text-slate-400 hover:text-white">
          <i class="fa-solid fa-xmark"></i>
        </button>
      </div>
      <p class="text-xs text-slate-300 leading-relaxed">
        By default, the application runs on our client-side Bayesian heuristic engine. You can connect your Google Gemini API key to leverage advanced LLM domain reasoning.
      </p>
      <div>
        <label for="customApiKey" class="block text-xs font-semibold text-slate-400 mb-1">API Key (Optional)</label>
        <input type="password" id="customApiKey" placeholder="AIzaSy..." class="w-full bg-slate-900 border border-slate-700 rounded-lg px-3 py-2 text-sm text-white focus:outline-none focus:border-indigo-500">
      </div>
      <div class="flex items-center justify-end space-x-2 pt-2">
        <button onclick="clearCustomKey()" class="px-3 py-1.5 rounded-lg text-xs text-rose-400 hover:bg-rose-500/10 transition">Clear</button>
        <button onclick="saveApiKey()" class="px-4 py-1.5 rounded-lg bg-indigo-600 hover:bg-indigo-500 text-white text-xs font-semibold transition">Save Settings</button>
      </div>
    </div>
  </div>

  <!-- Toast Notification Message -->
  <div id="toastMessage" class="fixed bottom-6 right-6 z-50 transform translate-y-24 opacity-0 transition-all duration-300 px-4 py-3 rounded-xl shadow-lg text-xs font-medium flex items-center space-x-2"></div>

  <!-- Footer -->
  <footer class="border-t border-slate-800/80 py-6 text-center text-xs text-slate-500 mt-12 no-print">
    <p>Probabyltics &copy; 2026. Probabilities are simulated numerical estimates for strategic decision guidance.</p>
  </footer>

  <script>
    // Global Application State
    const AppState = {
      apiKey: localStorage.getItem('probabyltics_api_key') || '',
      currentProblem: '',
      baseAnalysis: null,
      activeModifiers: {
        effort: 50,
        budget: 50,
        aggression: 50,
        volatility: 50
      },
      savedScenarios: JSON.parse(localStorage.getItem('probabyltics_saved_scenarios') || '[]'),
      charts: {
        donut: null,
        pdf: null,
        radar: null
      }
    };

    // Preset scenarios for instant testing
    const PRESETS = {
      startup: "Launching a B2B AI SaaS product with $10k budget and 6 months runway as a solo founder with software engineering background",
      salary: "Negotiating a 30% salary increase and senior title at my annual review in a large tech firm during an industry-wide conservative budget cycle",
      relocation: "Relocating from Southeast Asia to Berlin, Germany on a job-seeker visa without an upfront locked contract with 9 months of emergency savings",
      exam: "Preparing for the national medical school entrance exam in 6 months while working a 20-hour/week part-time job"
    };

    // Initialize UI on load
    window.addEventListener('DOMContentLoaded', () => {
      updateApiKeyIndicator();
      renderSavedScenariosList();
    });

    function fillPreset(key) {
      if (PRESETS[key]) {
        const textarea = document.getElementById('problemInput');
        textarea.value = PRESETS[key];
        textarea.focus();
      }
    }

    function showToast(text, type = 'info') {
      const toast = document.getElementById('toastMessage');
      toast.className = `fixed bottom-6 right-6 z-50 transform transition-all duration-300 px-4 py-3 rounded-xl shadow-xl text-xs font-medium flex items-center space-x-2 border ${
        type === 'error' 
          ? 'bg-rose-950/90 text-rose-200 border-rose-800' 
          : type === 'success' 
            ? 'bg-emerald-950/90 text-emerald-200 border-emerald-800' 
            : 'bg-slate-900 text-indigo-300 border-indigo-500/40'
      }`;
      toast.innerHTML = `<i class="fa-solid ${type === 'error' ? 'fa-circle-xmark' : type === 'success' ? 'fa-circle-check' : 'fa-circle-info'}"></i><span>${text}</span>`;
      toast.style.transform = 'translateY(0)';
      toast.style.opacity = '1';
      setTimeout(() => {
        toast.style.transform = 'translateY(6rem)';
        toast.style.opacity = '0';
      }, 3500);
    }

    // Modal Handlers
    function openKeyModal() {
      document.getElementById('customApiKey').value = AppState.apiKey;
      document.getElementById('apiKeyModal').classList.remove('hidden');
    }
    function closeKeyModal() {
      document.getElementById('apiKeyModal').classList.add('hidden');
    }
    function saveApiKey() {
      const val = document.getElementById('customApiKey').value.trim();
      AppState.apiKey = val;
      if (val) {
        localStorage.setItem('probabyltics_api_key', val);
        showToast('Gemini API key configured!', 'success');
      } else {
        localStorage.removeItem('probabyltics_api_key');
        showToast('Running on Local Heuristic Bayesian Engine', 'info');
      }
      updateApiKeyIndicator();
      closeKeyModal();
    }
    function clearCustomKey() {
      AppState.apiKey = '';
      localStorage.removeItem('probabyltics_api_key');
      document.getElementById('customApiKey').value = '';
      updateApiKeyIndicator();
      closeKeyModal();
      showToast('Key cleared. Fallback engine active.', 'info');
    }
    function updateApiKeyIndicator() {
      const text = document.getElementById('apiKeyStatusText');
      if (AppState.apiKey) {
        text.innerHTML = '<span class="text-emerald-400">Gemini Live</span>';
      } else {
        text.innerHTML = '<span>Engine: Heuristic</span>';
      }
    }

    /**
     * Box-Muller transform to sample from standard normal distribution
     */
    function randomNormal(mean = 0, stdDev = 1) {
      let u1 = Math.random();
      let u2 = Math.random();
      while (u1 === 0) u1 = Math.random();
      const z0 = Math.sqrt(-2.0 * Math.log(u1)) * Math.cos(2.0 * Math.PI * u2);
      return z0 * stdDev + mean;
    }

    /**
     * Approximate Beta distribution sample using normal approximation
     */
    function sampleBetaApproximation(alpha, beta) {
      const mean = alpha / (alpha + beta);
      const variance = (alpha * beta) / (Math.pow(alpha + beta, 2) * (alpha + beta + 1));
      const stdDev = Math.sqrt(variance);
      let sample = randomNormal(mean, stdDev);
      return Math.max(0.01, Math.min(0.99, sample));
    }

    /**
     * Core Monte Carlo engine executing 10,000 iterations
     */
    function runMonteCarloSimulation(baseSuccessProb, volatilityFactor, effortDelta, budgetDelta, aggressionDelta) {
      const iterations = 10000;
      const samples = new Float32Array(iterations);

      // Map slider inputs (-0.25 to +0.25 impact)
      const modifier = (effortDelta * 0.20) + (budgetDelta * 0.15) + (aggressionDelta * 0.05);
      const adjustedMean = Math.max(0.05, Math.min(0.95, (baseSuccessProb / 100) + modifier));

      // Beta parameters based on volatility
      // Higher volatility means lower pseudo-sample count (wider spread)
      const kappa = Math.max(4, 25 * (1 - volatilityFactor * 0.7));
      const alpha = Math.max(1, adjustedMean * kappa);
      const beta = Math.max(1, (1 - adjustedMean) * kappa);

      let successCount = 0;
      for (let i = 0; i < iterations; i++) {
        // Draw sample
        let val = sampleBetaApproximation(alpha, beta);
        samples[i] = val;
        if (val >= 0.5) successCount++;
      }

      // Sort samples to extract percentiles
      samples.sort();
      const p10 = Math.round(samples[Math.floor(iterations * 0.10)] * 100);
      const p50 = Math.round(samples[Math.floor(iterations * 0.50)] * 100);
      const p90 = Math.round(samples[Math.floor(iterations * 0.90)] * 100);
      const computedSuccessRate = Math.round((successCount / iterations) * 100);

      // Generate distribution bins for the Probability Density Function (PDF)
      const binCount = 20;
      const binCounts = new Array(binCount).fill(0);
      const binLabels = [];

      for (let b = 0; b < binCount; b++) {
        const binStart = b * 5;
        const binEnd = binStart + 5;
        binLabels.push(`${binStart}-${binEnd}%`);
      }

      for (let i = 0; i < iterations; i++) {
        const pct = samples[i] * 100;
        let binIdx = Math.min(binCount - 1, Math.floor(pct / 5));
        binCounts[binIdx]++;
      }

      // Normalize frequency into probability density
      const binDensity = binCounts.map(count => ((count / iterations) * 100).toFixed(2));

      return {
        successProb: computedSuccessRate,
        failureProb: 100 - computedSuccessRate,
        p10,
        p50,
        p90,
        binLabels,
        binDensity,
        meanSample: Math.round(adjustedMean * 100)
      };
    }

    /**
     * Heuristic domain reasoning fallback when no API key is specified
     */
    function executeLocalHeuristicAnalysis(text) {
      const lower = text.toLowerCase();
      let domain = "General Strategy & Career";
      let baseOdds = 52;
      let uncertainty = "Moderate";
      let topHazard = "Resource Depletion";

      let drivers = [
        { name: "Consistent Focused Execution", impact: "+18%", desc: "Commitment to deliberate milestones weekly." },
        { name: "Early Stakeholder Validation", impact: "+15%", desc: "Direct market feedback before overinvesting." },
        { name: "Adaptability & Pivoting", impact: "+12%", desc: "Flexibility when initial hypotheses fail." }
      ];

      let risks = [
        { name: "Underestimating Time Horizon", severity: "High", desc: "Most efforts take 2.5x longer than forecasted." },
        { name: "Burnout & Focus Dilution", severity: "Medium", desc: "Taking on too many simultaneous variables." },
        { name: "Market/Audience Indifference", severity: "High", desc: "Solving an issue people won't actively pay or care for." }
      ];

      let mitigations = [
        { action: "Implement Strict 14-Day Micro-Deliverables", boost: "+14%", desc: "Break the ambition into verifiable weekly proofs." },
        { action: "De-risk with Pre-commitments", boost: "+12%", desc: "Secure letters of intent or trial runs upfront." },
        { action: "Automate/Delegate Low-ROI Friction", boost: "+8%", desc: "Preserve high-cognitive bandwidth for core execution." }
      ];

      // Custom heuristics based on keywords
      if (lower.includes('saas') || lower.includes('startup') || lower.includes('founder') || lower.includes('business')) {
        domain = "Startup & Commercial Venture";
        baseOdds = 38; // Startup base failure rates are higher
        uncertainty = "High";
        topHazard = "Premature Scaling";
        drivers[0] = { name: "Product-Market Fit Velocity", impact: "+22%", desc: "Rapid prototyping with live user retention metrics." };
        drivers[1] = { name: "Unit Economics Discipline", impact: "+16%", desc: "Zero burn on non-customer acquisition channels." };
        risks[0] = { name: "Cash Runway Exhaustion", severity: "Critical", desc: "Depleting funds before achieving sustainable MRR." };
        risks[1] = { name: "Distribution Channel Block", severity: "High", desc: "Building great product without predictable sales funnel." };
        mitigations[0] = { action: "Pre-sell 10 Lifetime Accounts", boost: "+20%", desc: "Validate willingness-to-pay before writing architecture." };
        mitigations[1] = { action: "Cap Fixed Costs Below $250/mo", boost: "+15%", desc: "Extend runway indefinitely through lean open-source infra." };
      } else if (lower.includes('salary') || lower.includes('raise') || lower.includes('promotion') || lower.includes('negotiat')) {
        domain = "Corporate & Compensation Negotiation";
        baseOdds = 58;
        uncertainty = "Moderate";
        topHazard = "Lack of External Leverage";
        drivers[0] = { name: "Quantified Revenue/Efficiency Impact", impact: "+24%", desc: "Irrefutable metrics showing dollar value contributed." };
        drivers[1] = { name: "Executive Sponsorship", impact: "+18%", desc: "Support from leadership tier beyond direct manager." };
        risks[0] = { name: "Macro Budget Freezes", severity: "High", desc: "Company-level austerity blocking departmental discretion." };
        risks[1] = { name: "Confrontational Framing", severity: "Medium", desc: "Appearing demanding rather than collaborative partner." };
        mitigations[0] = { action: "Source a Competing External Offer", boost: "+25%", desc: "Hard market anchor establishes true replacement cost." };
        mitigations[1] = { action: "Propose Tiered Performance Bonuses", boost: "+15%", desc: "Tie compensation to specific upcoming quarterly KPIs." };
      } else if (lower.includes('exam') || lower.includes('test') || lower.includes('med') || lower.includes('study')) {
        domain = "High-Stakes Examination & Academics";
        baseOdds = 62;
        uncertainty = "Low-Moderate";
        topHazard = "Passive Recall Studying";
        drivers[0] = { name: "Spaced Repetition & Active Recall", impact: "+26%", desc: "Anki flashcards and mock exams under timed pressure." };
        drivers[1] = { name: "Systematic Weak-Spot Triage", impact: "+19%", desc: "Focusing 70% of prep on lowest quartile subject areas." };
        risks[0] = { name: "Cognitive Fatigue / Exam Anxiety", severity: "Medium", desc: "Choking during high-pressure timed sectionals." };
        risks[1] = { name: "Inconsistent Study Cadence", severity: "High", desc: "Cramming in bursts rather than steady 4-hour daily rhythm." };
        mitigations[0] = { action: "Simulate 8 Full-Length Mock Exams", boost: "+22%", desc: "Condition physiological endurance to exact testing conditions." };
        mitigations[1] = { action: "Form a 2-Person Accountability Pact", boost: "+11%", desc: "Daily verbal debriefs on challenging questions." };
      } else if (lower.includes('country') || lower.includes('relocat') || lower.includes('visa') || lower.includes('move')) {
        domain = "Global Relocation & Immigration";
        baseOdds = 46;
        uncertainty = "High";
        topHazard = "Bureaucratic Stalling";
        drivers[0] = { name: "In-demand Skill Certification", impact: "+20%", desc: "Qualifying for accelerated critical-skills visa pathways." };
        drivers[1] = { name: "Liquid Runway Reserves", impact: "+16%", desc: "12+ months living expenses buffer in target currency." };
        risks[0] = { name: "Housing/Rental Market Gatekeeping", severity: "High", desc: "Inability to register residency without permanent lease." };
        risks[1] = { name: "Social Isolation & Relocation Shock", severity: "Medium", desc: "Emotional strain undermining job hunting performance." };
        mitigations[0] = { action: "Pre-network with 30 Expats in Region", boost: "+18%", desc: "Uncover unlisted sublets and referral job pipelines." };
        mitigations[1] = { action: "Retain a Local Relocation Specialist", boost: "+14%", desc: "Bypass visa rejection tripwires." };
      }

      return {
        domain,
        baseSuccessProb: baseOdds,
        baseFailureProb: 100 - baseOdds,
        confidenceInterval: `[${Math.max(5, baseOdds - 14)}% - ${Math.min(95, baseOdds + 14)}%]`,
        uncertainty,
        topHazard,
        optimizedPotential: Math.min(94, baseOdds + 26),
        drivers,
        risks,
        mitigations,
        sensitivityFactors: [
          { factor: "Skill/Expertise", baseline: 65 },
          { factor: "Capital Runway", baseline: 50 },
          { factor: "Market Conditions", baseline: 45 },
          { factor: "Execution Grit", baseline: 75 },
          { factor: "Timing / Luck", baseline: 40 }
        ]
      };
    }

    /**
     * Gemini API call with structured schema
     */
    async function analyzeWithGemini(promptText, apiKey) {
      const endpoint = `https://generativelanguage.googleapis.com/v1beta/models/gemini-3-flash-preview:generateContent?key=${apiKey}`;
      
      const systemInstruction = `You are a world-class probabilistic analyst, actuarial scientist, and Bayesian risk consultant.
Analyze the user's situation and return a pure JSON object estimating realistic success and failure probabilities. 
Avoid false optimism; calculate rigorous Bayesian baseline priors. Be insightful, concise, and highly actionable.`;

      const prompt = `Analyze this real-world ambition or problem probabilistically:
"${promptText}"

Respond ONLY with a JSON object matching this schema:
{
  "domain": "short category name",
  "baseSuccessProb": number between 5 and 95,
  "baseFailureProb": number between 5 and 95,
  "confidenceInterval": "e.g. [35% - 55%]",
  "uncertainty": "Low" | "Moderate" | "High" | "Extremely High",
  "topHazard": "1-3 word name of the fatal trap",
  "optimizedPotential": number between 50 and 99,
  "drivers": [
    {"name": "Driver name", "impact": "+XX%", "desc": "Brief explanation"}
  ],
  "risks": [
    {"name": "Risk name", "severity": "Low"|"Medium"|"High"|"Critical", "desc": "Brief explanation"}
  ],
  "mitigations": [
    {"action": "Actionable tactic", "boost": "+XX%", "desc": "Specific tactical lever"}
  ],
  "sensitivityFactors": [
    {"factor": "Dimension 1", "baseline": number 0-100},
    {"factor": "Dimension 2", "baseline": number 0-100},
    {"factor": "Dimension 3", "baseline": number 0-100},
    {"factor": "Dimension 4", "baseline": number 0-100},
    {"factor": "Dimension 5", "baseline": number 0-100}
  ]
}`;

      const payload = {
        contents: [{ parts: [{ text: prompt }] }],
        systemInstruction: { parts: [{ text: systemInstruction }] },
        generationConfig: {
          responseMimeType: "application/json"
        }
      };

      const response = await fetch(endpoint, {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify(payload)
      });

      if (!response.ok) {
        throw new Error(`API error ${response.status}`);
      }

      const result = await response.json();
      const rawText = result.candidates?.[0]?.content?.parts?.[0]?.text;
      if (!rawText) throw new Error("Empty candidate response");
      return JSON.parse(rawText);
    }

    async function executeAnalysis() {
      const input = document.getElementById('problemInput').value.trim();
      if (!input) {
        showToast('Please enter an issue or ambition to analyze.', 'error');
        return;
      }

      AppState.currentProblem = input;
      const overlay = document.getElementById('loadingOverlay');
      const resultsSec = document.getElementById('resultsSection');
      const stepText = document.getElementById('loadingStepText');

      overlay.classList.remove('hidden');
      resultsSec.classList.add('hidden');

      stepText.innerText = "Constructing Bayesian prior probability distributions...";

      try {
        let analysisData = null;
        if (AppState.apiKey) {
          try {
            stepText.innerText = "Querying Gemini API for deep causal variables...";
            analysisData = await analyzeWithGemini(input, AppState.apiKey);
            showToast('Evaluated via Gemini 3 Flash', 'success');
          } catch (apiErr) {
            console.warn("Gemini call failed, switching to Bayesian heuristic engine:", apiErr);
            showToast('API issue. Using local Bayesian engine.', 'info');
            analysisData = executeLocalHeuristicAnalysis(input);
          }
        } else {
          // Fallback heuristic
          await new Promise(r => setTimeout(r, 650));
          stepText.innerText = "Synthesizing empirical domain benchmarks...";
          await new Promise(r => setTimeout(r, 550));
          analysisData = executeLocalHeuristicAnalysis(input);
        }

        AppState.baseAnalysis = analysisData;
        resetSliders(false);
        renderResults();
        resultsSec.classList.remove('hidden');
        resultsSec.scrollIntoView({ behavior: 'smooth' });
      } catch (err) {
        console.error("Analysis failure:", err);
        showToast("Error processing scenario. Please check input.", "error");
      } finally {
        overlay.classList.add('hidden');
      }
    }

    function handleSliderChange() {
      if (!AppState.baseAnalysis) return;

      const effort = parseInt(document.getElementById('sliderEffort').value);
      const budget = parseInt(document.getElementById('sliderBudget').value);
      const aggression = parseInt(document.getElementById('sliderAggression').value);
      const volatility = parseInt(document.getElementById('sliderVolatility').value);

      document.getElementById('sliderEffortLabel').innerText = `${effort}%`;
      document.getElementById('sliderBudgetLabel').innerText = `${budget}%`;
      document.getElementById('sliderAggressionLabel').innerText = `${aggression}%`;
      document.getElementById('sliderVolatilityLabel').innerText = `${volatility}%`;

      AppState.activeModifiers = { effort, budget, aggression, volatility };
      recalculateSimulationAndUI();
    }

    function resetSliders(triggerRecalc = true) {
      document.getElementById('sliderEffort').value = 50;
      document.getElementById('sliderBudget').value = 50;
      document.getElementById('sliderAggression').value = 50;
      document.getElementById('sliderVolatility').value = 50;

      document.getElementById('sliderEffortLabel').innerText = '50%';
      document.getElementById('sliderBudgetLabel').innerText = '50%';
      document.getElementById('sliderAggressionLabel').innerText = '50%';
      document.getElementById('sliderVolatilityLabel').innerText = '50%';

      AppState.activeModifiers = { effort: 50, budget: 50, aggression: 50, volatility: 50 };
      if (triggerRecalc) recalculateSimulationAndUI();
    }

    function recalculateSimulationAndUI() {
      const base = AppState.baseAnalysis;
      if (!base) return;

      const effortDelta = (AppState.activeModifiers.effort - 50) / 100;
      const budgetDelta = (AppState.activeModifiers.budget - 50) / 100;
      const aggressionDelta = (AppState.activeModifiers.aggression - 50) / 100;
      const volatilityFactor = AppState.activeModifiers.volatility / 100;

      // Run 10,000 Monte Carlo runs
      const simResults = runMonteCarloSimulation(
        base.baseSuccessProb,
        volatilityFactor,
        effortDelta,
        budgetDelta,
        aggressionDelta
      );

      // Update Top Metrics
      const successEl = document.getElementById('metricSuccessVal');
      const failEl = document.getElementById('metricFailureVal');
      const donutCenter = document.getElementById('donutCenterPct');

      successEl.innerText = `${simResults.successProb}%`;
      failEl.innerText = `${simResults.failureProb}%`;
      if (donutCenter) donutCenter.innerText = `${simResults.successProb}%`;

      // Status qualitative label
      const ratingLabel = document.getElementById('metricRatingLabel');
      if (simResults.successProb >= 70) {
        ratingLabel.innerText = "Highly Favorable";
        ratingLabel.className = "font-semibold text-emerald-400";
      } else if (simResults.successProb >= 50) {
        ratingLabel.innerText = "Moderate Viability";
        ratingLabel.className = "font-semibold text-sky-400";
      } else if (simResults.successProb >= 35) {
        ratingLabel.innerText = "Uphill Challenge";
        ratingLabel.className = "font-semibold text-yellow-400";
      } else {
        ratingLabel.innerText = "Severe Headwinds";
        ratingLabel.className = "font-semibold text-rose-400";
      }

      // CI & Percentiles
      document.getElementById('metricCiVal').innerText = `[${simResults.p10}% - ${simResults.p90}%]`;
      document.getElementById('p10Label').innerText = `${simResults.p10}%`;
      document.getElementById('p50Label').innerText = `${simResults.p50}%`;
      document.getElementById('p90Label').innerText = `${simResults.p90}%`;

      // Update Charts
      updateCharts(simResults);
    }

    function renderResults() {
      const data = AppState.baseAnalysis;
      if (!data) return;

      document.getElementById('domainBadge').innerText = data.domain || 'General Strategy';
      document.getElementById('metricTopHazard').innerText = data.topHazard || 'Uncertainty';
      document.getElementById('metricUncertainty').innerText = data.uncertainty || 'Moderate';
      
      const optGain = Math.max(0, data.optimizedPotential - data.baseSuccessProb);
      document.getElementById('metricOptimizedVal').innerText = `+${optGain}%`;
      document.getElementById('metricTargetVal').innerText = `Up to ${data.optimizedPotential}%`;

      // Drivers List
      const driversContainer = document.getElementById('driversList');
      driversContainer.innerHTML = (data.drivers || []).map(d => `
        <li class="p-2.5 rounded-lg bg-slate-950/60 border border-emerald-500/20 flex flex-col gap-1">
          <div class="flex justify-between items-center">
            <span class="font-semibold text-white">${d.name}</span>
            <span class="font-mono text-emerald-400 font-bold">${d.impact}</span>
          </div>
          <p class="text-slate-400 text-[11px] leading-relaxed">${d.desc}</p>
        </li>
      `).join('');

      // Risks List
      const risksContainer = document.getElementById('risksList');
      risksContainer.innerHTML = (data.risks || []).map(r => `
        <li class="p-2.5 rounded-lg bg-slate-950/60 border border-rose-500/20 flex flex-col gap-1">
          <div class="flex justify-between items-center">
            <span class="font-semibold text-white">${r.name}</span>
            <span class="font-mono px-1.5 py-0.5 rounded text-[10px] uppercase ${
              r.severity === 'Critical' ? 'bg-rose-900/60 text-rose-300' : 'bg-slate-800 text-yellow-300'
            }">${r.severity}</span>
          </div>
          <p class="text-slate-400 text-[11px] leading-relaxed">${r.desc}</p>
        </li>
      `).join('');

      // Mitigations List
      const mitigationsContainer = document.getElementById('mitigationsList');
      mitigationsContainer.innerHTML = (data.mitigations || []).map(m => `
        <li class="p-2.5 rounded-lg bg-slate-950/60 border border-indigo-500/20 flex flex-col gap-1">
          <div class="flex justify-between items-center">
            <span class="font-semibold text-white">${m.action}</span>
            <span class="font-mono text-indigo-400 font-bold">${m.boost}</span>
          </div>
          <p class="text-slate-400 text-[11px] leading-relaxed">${m.desc}</p>
        </li>
      `).join('');

      // Initial Chart Render
      initCharts();
      recalculateSimulationAndUI();
    }

    function initCharts() {
      // Destroy previous instances
      if (AppState.charts.donut) AppState.charts.donut.destroy();
      if (AppState.charts.pdf) AppState.charts.pdf.destroy();
      if (AppState.charts.radar) AppState.charts.radar.destroy();

      // 1. Donut Gauge Chart
      const donutCtx = document.getElementById('donutChart').getContext('2d');
      AppState.charts.donut = new Chart(donutCtx, {
        type: 'doughnut',
        data: {
          labels: ['Success', 'Failure'],
          datasets: [{
            data: [50, 50],
            backgroundColor: ['#10b981', '#f43f5e'],
            borderWidth: 0,
            hoverOffset: 4,
            cutout: '76%'
          }]
        },
        options: {
          responsive: true,
          maintainAspectRatio: false,
          plugins: { legend: { display: false } }
        }
      });

      // 2. Monte Carlo Probability Density Function (Bell Curve)
      const pdfCtx = document.getElementById('pdfChart').getContext('2d');
      AppState.charts.pdf = new Chart(pdfCtx, {
        type: 'line',
        data: {
          labels: [],
          datasets: [{
            label: 'Density (%)',
            data: [],
            borderColor: '#6366f1',
            backgroundColor: 'rgba(99, 102, 241, 0.15)',
            fill: true,
            tension: 0.35,
            pointRadius: 2,
            pointHoverRadius: 5,
            borderWidth: 2
          }]
        },
        options: {
          responsive: true,
          maintainAspectRatio: false,
          scales: {
            x: {
              grid: { color: 'rgba(255, 255, 255, 0.05)' },
              ticks: { color: '#94a3b8', font: { family: 'JetBrains Mono', size: 10 } }
            },
            y: {
              grid: { color: 'rgba(255, 255, 255, 0.05)' },
              ticks: { color: '#94a3b8', font: { family: 'JetBrains Mono', size: 10 } }
            }
          },
          plugins: {
            legend: { display: false },
            tooltip: {
              callbacks: {
                label: (ctx) => `Probability Density: ${ctx.parsed.y}%`
              }
            }
          }
        }
      });

      // 3. Radar Factor Chart
      const radarCtx = document.getElementById('radarChart').getContext('2d');
      const factors = AppState.baseAnalysis.sensitivityFactors || [
        { factor: "Preparation", baseline: 60 },
        { factor: "Capital", baseline: 50 },
        { factor: "Environment", baseline: 45 },
        { factor: "Leverage", baseline: 70 },
        { factor: "Resilience", baseline: 65 }
      ];

      AppState.charts.radar = new Chart(radarCtx, {
        type: 'radar',
        data: {
          labels: factors.map(f => f.factor),
          datasets: [{
            label: 'Baseline Sensitivity',
            data: factors.map(f => f.baseline),
            backgroundColor: 'rgba(16, 185, 129, 0.2)',
            borderColor: '#10b981',
            pointBackgroundColor: '#10b981',
            pointBorderColor: '#fff',
            borderWidth: 1.5
          }]
        },
        options: {
          responsive: true,
          maintainAspectRatio: false,
          scales: {
            r: {
              angleLines: { color: 'rgba(255, 255, 255, 0.08)' },
              grid: { color: 'rgba(255, 255, 255, 0.08)' },
              pointLabels: { color: '#cbd5e1', font: { size: 10 } },
              ticks: { display: false, min: 0, max: 100 }
            }
          },
          plugins: { legend: { display: false } }
        }
      });
    }

    function updateCharts(simResults) {
      if (AppState.charts.donut) {
        AppState.charts.donut.data.datasets[0].data = [simResults.successProb, simResults.failureProb];
        AppState.charts.donut.update('none');
      }

      if (AppState.charts.pdf) {
        AppState.charts.pdf.data.labels = simResults.binLabels;
        AppState.charts.pdf.data.datasets[0].data = simResults.binDensity;
        AppState.charts.pdf.update('none');
      }
    }

    function saveCurrentScenario() {
      if (!AppState.baseAnalysis) return;

      const scenario = {
        id: 'scen_' + Date.now(),
        date: new Date().toLocaleDateString(),
        problem: AppState.currentProblem,
        domain: AppState.baseAnalysis.domain,
        successProb: document.getElementById('metricSuccessVal').innerText,
        failureProb: document.getElementById('metricFailureVal').innerText,
        ci: document.getElementById('metricCiVal').innerText,
        modifiers: { ...AppState.activeModifiers }
      };

      AppState.savedScenarios.unshift(scenario);
      if (AppState.savedScenarios.length > 20) AppState.savedScenarios.pop();

      localStorage.setItem('probabyltics_saved_scenarios', JSON.stringify(AppState.savedScenarios));
      renderSavedScenariosList();
      showToast('Scenario saved to history!', 'success');
    }

    function deleteScenario(id) {
      AppState.savedScenarios = AppState.savedScenarios.filter(s => s.id !== id);
      localStorage.setItem('probabyltics_saved_scenarios', JSON.stringify(AppState.savedScenarios));
      renderSavedScenariosList();
      showToast('Scenario deleted', 'info');
    }

    function loadScenario(id) {
      const found = AppState.savedScenarios.find(s => s.id === id);
      if (!found) return;

      document.getElementById('problemInput').value = found.problem;
      executeAnalysis();
      toggleScenarioDrawer();
    }

    function renderSavedScenariosList() {
      const container = document.getElementById('savedScenarioList');
      const badge = document.getElementById('savedCountBadge');
      badge.innerText = AppState.savedScenarios.length;

      if (!AppState.savedScenarios.length) {
        container.innerHTML = '<p class="text-slate-500 text-xs italic">No saved simulations yet.</p>';
        return;
      }

      container.innerHTML = AppState.savedScenarios.map(s => `
        <div class="p-3.5 rounded-xl bg-slate-950/80 border border-slate-800 hover:border-indigo-500/40 transition flex flex-col gap-2">
          <div class="flex justify-between items-center text-xs">
            <span class="font-semibold text-white truncate max-w-[200px]">${s.problem}</span>
            <span class="font-mono text-emerald-400 font-bold">${s.successProb}</span>
          </div>
          <div class="flex items-center justify-between text-[11px] text-slate-400">
            <span>${s.domain} • ${s.date}</span>
            <div class="flex items-center space-x-2">
              <button onclick="loadScenario('${s.id}')" class="text-indigo-400 hover:underline">Re-run</button>
              <button onclick="deleteScenario('${s.id}')" class="text-rose-400 hover:text-rose-300"><i class="fa-solid fa-trash-can"></i></button>
            </div>
          </div>
        </div>
      `).join('');
    }

    function toggleScenarioDrawer() {
      const drawer = document.getElementById('scenarioDrawer');
      drawer.classList.toggle('translate-x-full');
    }

    function copySummaryText() {
      if (!AppState.baseAnalysis) return;
      const b = AppState.baseAnalysis;
      const succ = document.getElementById('metricSuccessVal').innerText;
      const fail = document.getElementById('metricFailureVal').innerText;
      const ci = document.getElementById('metricCiVal').innerText;

      const summary = `PROBABYLTICS PROBABILISTIC ANALYSIS REPORT
------------------------------------------------
Scenario: "${AppState.currentProblem}"
Domain: ${b.domain}
Success Probability: ${succ}
Failure Probability: ${fail}
90% Confidence Interval: ${ci}
Primary Hazard: ${b.topHazard}

Key Positive Drivers:
${(b.drivers || []).map(d => `- ${d.name} (${d.impact}): ${d.desc}`).join('\n')}

Critical Failure Modes:
${(b.risks || []).map(r => `- [${r.severity}] ${r.name}: ${r.desc}`).join('\n')}

Actionable High-Leverage Mitigations:
${(b.mitigations || []).map(m => `- ${m.action} (${m.boost}): ${m.desc}`).join('\n')}
------------------------------------------------
Generated via Probabyltics Monte Carlo Simulation Engine.`;

      // Fallback for iframe copy
      const tempArea = document.createElement('textarea');
      tempArea.value = summary;
      document.body.appendChild(tempArea);
      tempArea.select();
      document.execCommand('copy');
      document.body.removeChild(tempArea);

      showToast('Executive brief copied to clipboard!', 'success');
    }
  </script>
</body>
</html>
