<!-- ... existing code ... -->
<!DOCTYPE html>
<html lang="ja" class="h-full bg-slate-900 text-slate-100">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
  <title>日本株 BS・財務データ分析ダッシュボード</title>
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <!-- Lucide Icons -->
  <script src="https://unpkg.com/lucide@latest"></script>
  <!-- Chart.js -->
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <style>
    /* Mobile Touch Optimizations & Custom Scrollbars */
    * { -webkit-tap-highlight-color: transparent; }
    .no-scrollbar::-webkit-scrollbar { display: none; }
    .no-scrollbar { -ms-overflow-style: none; scrollbar-width: none; }
    .custom-scroll::-webkit-scrollbar { width: 4px; height: 4px; }
    .custom-scroll::-webkit-scrollbar-thumb { background: #475569; border-radius: 4px; }
    .custom-scroll::-webkit-scrollbar-track { background: transparent; }
    .safe-bottom-padding { padding-bottom: calc(4.5rem + env(safe-area-inset-bottom, 0px)); }
  </style>
</head>
<body class="h-full flex flex-col font-sans bg-slate-900 text-slate-100 antialiased selection:bg-cyan-500 selection:text-white safe-bottom-padding">

  <!-- TOP STICKY HEADER & TICKER SELECTOR -->
  <header class="sticky top-0 z-30 bg-slate-800/95 backdrop-blur border-b border-slate-700 shadow-lg">
    <div class="max-w-7xl mx-auto px-3 py-2 flex items-center justify-between gap-2">
      <!-- Logo & Title -->
      <div class="flex items-center gap-2 shrink-0">
        <div class="p-1.5 bg-gradient-to-tr from-cyan-500 to-blue-600 rounded-lg text-white shadow-md">
          <i data-lucide="bar-chart-3" class="w-5 h-5"></i>
        </div>
        <div class="hidden sm:block">
          <h1 class="text-sm font-bold text-slate-100 leading-none">日本株 BS・財務分析</h1>
          <p class="text-[10px] text-slate-400">J-Stock Visualizer Mobile</p>
        </div>
      </div>

      <!-- Quick Ticker Selector Horizontal Scroll Bar -->
      <div id="quickTickerList" class="flex items-center gap-1.5 overflow-x-auto no-scrollbar py-1 px-1">
        <!-- Rendered dynamically -->
      </div>

      <!-- Quick Action Buttons -->
      <div class="flex items-center gap-1 shrink-0">
        <button id="addTickerQuickBtn" onclick="openModal('addTickerModal')" class="p-2 bg-cyan-600/20 text-cyan-400 hover:bg-cyan-600/30 active:scale-95 rounded-lg border border-cyan-500/30 flex items-center justify-center text-xs font-medium transition">
          <i data-lucide="plus" class="w-4 h-4"></i>
        </button>
      </div>
    </div>
  </header>

  <!-- MAIN CONTAINER -->
  <main class="flex-1 max-w-7xl w-full mx-auto px-3 py-3">

    <!-- VIEW 1: 銘柄詳細 (DETAIL) -->
    <section id="viewDetail" class="tab-content space-y-4">
      
      <!-- Company Overview Header Card -->
      <div id="companyHeaderCard" class="bg-slate-800 border border-slate-700/80 rounded-xl p-4 shadow-md">
        <!-- JS Dynamic Content -->
      </div>

      <!-- Key KPI Grid (Mobile Cards) -->
      <div id="kpiGrid" class="grid grid-cols-2 md:grid-cols-4 gap-2.5">
        <!-- JS Dynamic Content -->
      </div>

      <!-- Balance Sheet Visualizer (Horizontal Scrollable/Swipeable Stacked Charts & Year Cards) -->
      <div class="bg-slate-800 border border-slate-700/80 rounded-xl p-3 sm:p-4 shadow-md space-y-3">
        <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-2">
          <div class="flex items-center gap-2">
            <i data-lucide="layers" class="w-5 h-5 text-cyan-400"></i>
            <h2 class="text-base font-bold text-slate-100">BS (貸借対照表) 推移 & 構成比</h2>
          </div>
          <div class="flex items-center gap-2 text-xs">
            <span class="text-slate-400">表示単位:</span>
            <button onclick="toggleAmountUnit('hundred_million')" id="unitBtn1" class="px-2.5 py-1 rounded bg-cyan-600 text-white font-medium">億円</button>
            <button onclick="toggleAmountUnit('million')" id="unitBtn2" class="px-2.5 py-1 rounded bg-slate-700 text-slate-300">百万円</button>
          </div>
        </div>

        <!-- BS Visualizer Chart Box -->
        <div class="relative w-full overflow-x-auto custom-scroll pb-2">
          <div class="min-w-[600px] sm:min-w-full h-64 sm:h-80">
            <canvas id="bsChart"></canvas>
          </div>
        </div>
      </div>

      <!-- Detailed Financial Metrics & Collapsible B/S Accordion -->
      <div class="bg-slate-800 border border-slate-700/80 rounded-xl p-3 sm:p-4 shadow-md space-y-3">
        <div class="flex items-center justify-between">
          <h3 class="text-sm font-bold text-slate-200 flex items-center gap-1.5">
            <i data-lucide="list-filter" class="w-4 h-4 text-cyan-400"></i>
            財務詳細 breakdown (年別アコーディオン)
          </h3>
          <span class="text-[11px] text-slate-400">タップで詳細開閉</span>
        </div>

        <!-- Collapsible Year Accordions -->
        <div id="bsDetailAccordion" class="space-y-2">
          <!-- Dynamic Content -->
        </div>
      </div>
    </section>

    <!-- VIEW 2: 複数比較 (COMPARE) -->
    <section id="viewCompare" class="tab-content hidden space-y-4">
      <div class="bg-slate-800 border border-slate-700/80 rounded-xl p-3 sm:p-4 shadow-md space-y-3">
        <h2 class="text-base font-bold text-slate-100 flex items-center gap-2">
          <i data-lucide="columns" class="w-5 h-5 text-cyan-400"></i>
          複数銘柄の比較 (Side-by-Side Comparison)
        </h2>
        
        <!-- Multi Select Checkboxes -->
        <div id="compareTickerSelector" class="flex flex-wrap gap-2 py-1">
          <!-- Dynamic Content -->
        </div>

        <div class="relative w-full overflow-x-auto custom-scroll pt-2">
          <div class="min-w-[550px] sm:min-w-full h-72">
            <canvas id="compareChart"></canvas>
          </div>
        </div>
      </div>

      <!-- Comparison Data Table -->
      <div class="bg-slate-800 border border-slate-700/80 rounded-xl p-3 sm:p-4 shadow-md overflow-x-auto custom-scroll">
        <table id="compareTable" class="w-full text-left text-xs text-slate-300">
          <!-- Dynamic Table Content -->
        </table>
      </div>
    </section>

    <!-- VIEW 3: 財務比率 (RATIOS) -->
    <section id="viewRatios" class="tab-content hidden space-y-4">
      <div class="bg-slate-800 border border-slate-700/80 rounded-xl p-3 sm:p-4 shadow-md space-y-3">
        <h2 class="text-base font-bold text-slate-100 flex items-center gap-2">
          <i data-lucide="pie-chart" class="w-5 h-5 text-cyan-400"></i>
          安全性・収益性・効率性指標
        </h2>
        
        <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
          <div class="bg-slate-900/60 p-3 rounded-lg border border-slate-700/50">
            <h3 class="text-xs font-semibold text-slate-300 mb-2">自己資本比率 (%) & ROE (%) 推移</h3>
            <div class="h-56">
              <canvas id="ratioChart1"></canvas>
            </div>
          </div>

          <div class="bg-slate-900/60 p-3 rounded-lg border border-slate-700/50">
            <h3 class="text-xs font-semibold text-slate-300 mb-2">流動比率 (%) & 固定比率 (%)</h3>
            <div class="h-56">
              <canvas id="ratioChart2"></canvas>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- VIEW 4: 銘柄追加/管理 (MANAGE) -->
    <section id="viewManage" class="tab-content hidden space-y-4">
      <div class="bg-slate-800 border border-slate-700/80 rounded-xl p-4 shadow-md space-y-4">
        <div class="flex items-center justify-between">
          <h2 class="text-base font-bold text-slate-100 flex items-center gap-2">
            <i data-lucide="database" class="w-5 h-5 text-cyan-400"></i>
            銘柄データ管理 & カスタム追加
          </h2>
          <button onclick="openModal('addTickerModal')" class="px-3 py-1.5 bg-cyan-600 hover:bg-cyan-500 text-white rounded-lg text-xs font-medium flex items-center gap-1 shadow">
            <i data-lucide="plus" class="w-4 h-4"></i> 新規銘柄追加
          </button>
        </div>

        <!-- Ticker List Table / Card View -->
        <div id="managedTickersList" class="space-y-2">
          <!-- Dynamic Ticker Cards -->
        </div>
      </div>
    </section>

    <!-- VIEW 5: データ出力 / 設定 (EXPORT / API) -->
    <section id="viewExport" class="tab-content hidden space-y-4">
      <div class="bg-slate-800 border border-slate-700/80 rounded-xl p-4 shadow-md space-y-4">
        <h2 class="text-base font-bold text-slate-100 flex items-center gap-2">
          <i data-lucide="download" class="w-5 h-5 text-cyan-400"></i>
          CSVエクスポート & EDINET API連携シミュレータ
        </h2>

        <!-- CSV Export Button -->
        <div class="p-3 bg-slate-900/60 rounded-lg border border-slate-700/50 flex flex-col sm:flex-row items-start sm:items-center justify-between gap-3">
          <div>
            <h3 class="text-sm font-semibold text-slate-200">現在選択中の財務データをCSV保存</h3>
            <p class="text-xs text-slate-400">直近10年分の財務数値データをCSVフォーマットで出力します。</p>
          </div>
          <button onclick="exportCurrentTickerCSV()" class="w-full sm:w-auto px-4 py-2 bg-emerald-600 hover:bg-emerald-500 text-white text-xs font-semibold rounded-lg flex items-center justify-center gap-1.5 shadow">
            <i data-lucide="file-spread-sheet" class="w-4 h-4"></i> CSVダウンロード
          </button>
        </div>

        <!-- EDINET API Simulation -->
        <div class="p-3 bg-slate-900/60 rounded-lg border border-slate-700/50 space-y-3">
          <h3 class="text-sm font-semibold text-slate-200 flex items-center gap-1.5">
            <i data-lucide="globe" class="w-4 h-4 text-cyan-400"></i> EDINET API 簡易データ取得シミュレータ
          </h3>
          <p class="text-xs text-slate-400">
            EDINET書類コード（例: S100XXXX）または証券コードを入力し、自動財務計算シミュレーションを行います。
          </p>
          <div class="flex gap-2">
            <input id="edinetInput" type="text" placeholder="例: 7203 や S100RXYZ" class="flex-1 bg-slate-800 border border-slate-700 rounded-lg px-3 py-2 text-xs text-slate-100 focus:outline-none focus:border-cyan-500">
            <button onclick="simulateEdinetFetch()" class="px-4 py-2 bg-cyan-600 hover:bg-cyan-500 text-white text-xs font-semibold rounded-lg shrink-0">
              取得試行
            </button>
          </div>
          <div id="edinetStatus" class="hidden p-2.5 rounded bg-slate-800 border border-slate-700 text-xs text-slate-300 font-mono">
            <!-- Simulated logs -->
          </div>
        </div>
      </div>
    </section>

  </main>

  <!-- MOBILE BOTTOM NAVIGATION BAR (FIXED FOR THUMB NAVIGATION) -->
  <nav class="fixed bottom-0 left-0 right-0 z-40 bg-slate-800/95 backdrop-blur border-t border-slate-700 px-1 py-1 sm:hidden">
    <div class="grid grid-cols-5 gap-1 text-center">
      <button onclick="switchTab('Detail')" id="navDetail" class="nav-btn flex flex-col items-center justify-center py-1.5 rounded-lg text-cyan-400 transition">
        <i data-lucide="bar-chart-2" class="w-5 h-5"></i>
        <span class="text-[10px] font-medium mt-0.5">詳細</span>
      </button>
      <button onclick="switchTab('Compare')" id="navCompare" class="nav-btn flex flex-col items-center justify-center py-1.5 rounded-lg text-slate-400 hover:text-slate-200 transition">
        <i data-lucide="columns" class="w-5 h-5"></i>
        <span class="text-[10px] font-medium mt-0.5">比較</span>
      </button>
      <button onclick="switchTab('Ratios')" id="navRatios" class="nav-btn flex flex-col items-center justify-center py-1.5 rounded-lg text-slate-400 hover:text-slate-200 transition">
        <i data-lucide="pie-chart" class="w-5 h-5"></i>
        <span class="text-[10px] font-medium mt-0.5">比率</span>
      </button>
      <button onclick="switchTab('Manage')" id="navManage" class="nav-btn flex flex-col items-center justify-center py-1.5 rounded-lg text-slate-400 hover:text-slate-200 transition">
        <i data-lucide="sliders" class="w-5 h-5"></i>
        <span class="text-[10px] font-medium mt-0.5">管理</span>
      </button>
      <button onclick="switchTab('Export')" id="navExport" class="nav-btn flex flex-col items-center justify-center py-1.5 rounded-lg text-slate-400 hover:text-slate-200 transition">
        <i data-lucide="download" class="w-5 h-5"></i>
        <span class="text-[10px] font-medium mt-0.5">出力</span>
      </button>
    </div>
  </nav>

  <!-- DESKTOP TOP TAB NAV OVERLAY (VISIBLE ON TABLET/DESKTOP) -->
  <div class="hidden sm:block fixed top-2 right-14 z-40">
    <div class="flex items-center bg-slate-800 border border-slate-700 rounded-lg p-1 text-xs shadow-md">
      <button onclick="switchTab('Detail')" class="desktop-tab-btn px-3 py-1 rounded-md text-cyan-400 font-medium">詳細</button>
      <button onclick="switchTab('Compare')" class="desktop-tab-btn px-3 py-1 rounded-md text-slate-300 font-medium hover:text-slate-100">複数比較</button>
      <button onclick="switchTab('Ratios')" class="desktop-tab-btn px-3 py-1 rounded-md text-slate-300 font-medium hover:text-slate-100">財務比率</button>
      <button onclick="switchTab('Manage')" class="desktop-tab-btn px-3 py-1 rounded-md text-slate-300 font-medium hover:text-slate-100">銘柄管理</button>
      <button onclick="switchTab('Export')" class="desktop-tab-btn px-3 py-1 rounded-md text-slate-300 font-medium hover:text-slate-100">データ出力</button>
    </div>
  </div>

  <!-- ADD TICKER MODAL -->
  <div id="addTickerModal" class="fixed inset-0 z-50 hidden bg-slate-950/80 backdrop-blur-sm flex items-center justify-center p-4">
    <div class="bg-slate-800 border border-slate-700 rounded-xl max-w-md w-full p-4 space-y-4 shadow-2xl animate-in fade-in zoom-in duration-150">
      <div class="flex items-center justify-between border-b border-slate-700 pb-2">
        <h3 class="text-sm font-bold text-slate-100 flex items-center gap-1.5">
          <i data-lucide="plus-circle" class="w-4 h-4 text-cyan-400"></i> 新規銘柄データ追加
        </h3>
        <button onclick="closeModal('addTickerModal')" class="text-slate-400 hover:text-white p-1">
          <i data-lucide="x" class="w-5 h-5"></i>
        </button>
      </div>

      <form id="addTickerForm" onsubmit="handleCustomTickerSubmit(event)" class="space-y-3 text-xs">
        <div>
          <label class="block text-slate-300 font-medium mb-1">証券コード & 会社名</label>
          <div class="grid grid-cols-3 gap-2">
            <input type="text" id="newCode" placeholder="コード (例: 9984)" required class="bg-slate-900 border border-slate-700 rounded p-2 text-slate-100">
            <input type="text" id="newName" placeholder="社名 (例: SBG)" required class="col-span-2 bg-slate-900 border border-slate-700 rounded p-2 text-slate-100">
          </div>
        </div>

        <div>
          <label class="block text-slate-300 font-medium mb-1">業種分類</label>
          <input type="text" id="newSector" placeholder="例: 情報・通信業" required class="w-full bg-slate-900 border border-slate-700 rounded p-2 text-slate-100">
        </div>

        <div class="border-t border-slate-700/60 pt-2 space-y-2">
          <p class="text-[11px] text-cyan-400 font-medium">直近1年分の試算データ入力 (単位: 億円)</p>
          <div class="grid grid-cols-2 gap-2">
            <div>
              <span class="text-slate-400 text-[10px]">流動資産</span>
              <input type="number" id="newCurrentAssets" placeholder="1000" required class="w-full bg-slate-900 border border-slate-700 rounded p-1.5 text-slate-100">
            </div>
            <div>
              <span class="text-slate-400 text-[10px]">固定資産</span>
              <input type="number" id="newFixedAssets" placeholder="1500" required class="w-full bg-slate-900 border border-slate-700 rounded p-1.5 text-slate-100">
            </div>
            <div>
              <span class="text-slate-400 text-[10px]">流動負債</span>
              <input type="number" id="newCurrentLiab" placeholder="600" required class="w-full bg-slate-900 border border-slate-700 rounded p-1.5 text-slate-100">
            </div>
            <div>
              <span class="text-slate-400 text-[10px]">固定負債</span>
              <input type="number" id="newFixedLiab" placeholder="800" required class="w-full bg-slate-900 border border-slate-700 rounded p-1.5 text-slate-100">
            </div>
            <div class="col-span-2">
              <span class="text-slate-400 text-[10px]">純資産 (自己資本)</span>
              <input type="number" id="newEquity" placeholder="1100" required class="w-full bg-slate-900 border border-slate-700 rounded p-1.5 text-slate-100">
            </div>
          </div>
        </div>

        <div class="pt-2 flex justify-end gap-2">
          <button type="button" onclick="closeModal('addTickerModal')" class="px-3 py-1.5 bg-slate-700 text-slate-300 rounded font-medium">キャンセル</button>
          <button type="submit" class="px-4 py-1.5 bg-cyan-600 hover:bg-cyan-500 text-white rounded font-semibold">保存・反映</button>
        </div>
      </form>
    </div>
  </div>

  <!-- SCRIPT LOGIC -->
  <script>
    /* ==========================================================================
       1. FINANCIAL DATASTORE (10-YEAR HISTORICAL DATA FOR MAJOR J-STOCKS)
       ========================================================================== */
    const DEFAULT_STOCKS = [
      {
        code: "7203",
        name: "トヨタ自動車",
        sector: "輸送用機器",
        years: [2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023, 2024],
        currentAssets: [168000, 172000, 181000, 191000, 198000, 201000, 215000, 235000, 258000, 281000], // 億円
        fixedAssets:   [202000, 205000, 218000, 222000, 228000, 225000, 248000, 271000, 294000, 319000],
        currentLiab:   [135000, 138000, 142000, 148000, 152000, 158000, 169000, 185000, 201000, 218000],
        fixedLiab:     [121000, 124000, 131000, 135000, 141000, 139000, 151000, 168000, 182000, 195000],
        equity:        [114000, 115000, 126000, 130000, 133000, 129000, 143000, 153000, 169000, 187000],
        netIncome:     [21733,  23126,  18311,  24939,  18828,  20761,  22452,  28501,  24513,  49449]
      },
      {
        code: "6758",
        name: "ソニーグループ",
        sector: "電気機器",
        years: [2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023, 2024],
        currentAssets: [61000, 63000, 68000, 75000, 81000, 89000, 98000, 110000, 121000, 132000],
        fixedAssets:   [97000, 103000, 108000, 115000, 128000, 141000, 158000, 172000, 189000, 205000],
        currentLiab:   [49000, 52000, 55000, 60000, 64000, 71000, 79000, 88000, 96000, 105000],
        fixedLiab:     [85000, 88000, 92000, 96000, 103000, 110000, 121000, 132000, 143000, 152000],
        equity:        [24000, 26000, 29000, 34000, 42000, 49000, 56000, 62000, 71000, 80000],
        netIncome:     [-1259, 1478,   732,   4907,   9162,   5821,   11717,  8822,   9371,   9706]
      },
      {
        code: "9983",
        name: "ファーストリテイリング",
        sector: "小売業",
        years: [2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023, 2024],
        currentAssets: [7100, 7400, 8900, 10800, 12400, 13800, 15900, 18500, 21000, 23800],
        fixedAssets:   [4500, 4900, 5200, 5700, 6200, 6800, 7200, 8100, 9200, 10400],
        currentLiab:   [3800, 4100, 4800, 5500, 6100, 6900, 7500, 8800, 9900, 11200],
        fixedLiab:     [1800, 2000, 2200, 2600, 2800, 3100, 3400, 3900, 4300, 4800],
        equity:        [6000, 6200, 7100, 8400, 9700, 10600, 12200, 13900, 16000, 18200],
        netIncome:     [1100,  480,   1192,  1548,  1625,  903,   1698,  2733,  2962,  3719]
      }
    ];

    /* App State */
    let stockData = [...DEFAULT_STOCKS];
    let selectedTickerCode = "7203";
    let activeTab = "Detail";
    let amountUnit = "hundred_million"; // 'hundred_million' (億円) or 'million' (百万円)
    let bsChartInstance = null;
    let compareChartInstance = null;
    let ratioChart1Instance = null;
    let ratioChart2Instance = null;

    /* Initialize App on Load */
    window.addEventListener('DOMContentLoaded', () => {
      lucide.createIcons();
      renderQuickTickerBar();
      renderCurrentView();
    });

    /* Switch Tabs */
    function switchTab(tabName) {
      activeTab = tabName;
      document.querySelectorAll('.tab-content').forEach(el => el.classList.add('hidden'));
      document.getElementById(`view${tabName}`).classList.remove('hidden');

      // Update Navigation Visuals
      document.querySelectorAll('.nav-btn').forEach(btn => {
        btn.classList.remove('text-cyan-400');
        btn.classList.add('text-slate-400');
      });
      const activeNavBtn = document.getElementById(`nav${tabName}`);
      if (activeNavBtn) {
        activeNavBtn.classList.remove('text-slate-400');
        activeNavBtn.classList.add('text-cyan-400');
      }

      // Re-render components for tab
      renderCurrentView();
    }

    /* Set Active Ticker */
    function selectTicker(code) {
      selectedTickerCode = code;
      renderQuickTickerBar();
      renderCurrentView();
    }

    /* Unit Switcher */
    function toggleAmountUnit(unit) {
      amountUnit = unit;
      document.getElementById('unitBtn1').className = unit === 'hundred_million' ? "px-2.5 py-1 rounded bg-cyan-600 text-white font-medium" : "px-2.5 py-1 rounded bg-slate-700 text-slate-300";
      document.getElementById('unitBtn2').className = unit === 'million' ? "px-2.5 py-1 rounded bg-cyan-600 text-white font-medium" : "px-2.5 py-1 rounded bg-slate-700 text-slate-300";
      renderCurrentView();
    }

    /* RENDER CONTROLLER */
    function renderCurrentView() {
      const stock = stockData.find(s => s.code === selectedTickerCode) || stockData[0];
      
      if (activeTab === "Detail") {
        renderHeaderCard(stock);
        renderKPIGrid(stock);
        renderBSChart(stock);
        renderBSAccordion(stock);
      } else if (activeTab === "Compare") {
        renderCompareSection();
      } else if (activeTab === "Ratios") {
        renderRatioCharts(stock);
      } else if (activeTab === "Manage") {
        renderManageSection();
      }
    }

    /* 1. Quick Ticker Bar Render */
    function renderQuickTickerBar() {
      const container = document.getElementById('quickTickerList');
      container.innerHTML = stockData.map(s => {
        const isSelected = s.code === selectedTickerCode;
        return `
          <button onclick="selectTicker('${s.code}')" class="px-2.5 py-1 rounded-full text-xs font-semibold whitespace-nowrap transition ${
            isSelected 
              ? 'bg-cyan-500 text-slate-950 shadow-md shadow-cyan-500/20' 
              : 'bg-slate-700/80 text-slate-300 hover:bg-slate-700'
          }">
            ${s.code} ${s.name.substring(0, 4)}
          </button>
        `;
      }).join('');
    }

    /* 2. Company Header Card */
    function renderHeaderCard(stock) {
      const latestIdx = stock.years.length - 1;
      const totalAssets = stock.currentAssets[latestIdx] + stock.fixedAssets[latestIdx];
      const equityRatio = ((stock.equity[latestIdx] / totalAssets) * 100).toFixed(1);

      document.getElementById('companyHeaderCard').innerHTML = `
        <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-2">
          <div>
            <div class="flex items-center gap-2">
              <span class="px-2 py-0.5 rounded text-[11px] font-bold bg-cyan-500/20 text-cyan-400 border border-cyan-500/30">${stock.code}</span>
              <h2 class="text-base sm:text-lg font-bold text-slate-100">${stock.name}</h2>
              <span class="text-xs text-slate-400">(${stock.sector})</span>
            </div>
            <p class="text-xs text-slate-400 mt-1">最新決算期: ${stock.years[latestIdx]}年3月期 | 総資産: ${formatValue(totalAssets)}</p>
          </div>
          <div class="flex items-center gap-3 bg-slate-900/60 p-2 rounded-lg border border-slate-700/50 self-start sm:self-auto">
            <div class="text-right">
              <span class="block text-[10px] text-slate-400">自己資本比率</span>
              <span class="text-sm font-extrabold text-cyan-400">${equityRatio}%</span>
            </div>
            <div class="h-6 w-px bg-slate-700"></div>
            <div class="text-right">
              <span class="block text-[10px] text-slate-400">当期純利益</span>
              <span class="text-sm font-extrabold text-emerald-400">${formatValue(stock.netIncome[latestIdx])}</span>
            </div>
          </div>
        </div>
      `;
    }

    /* 3. KPI Grid Cards */
    function renderKPIGrid(stock) {
      const idx = stock.years.length - 1;
      const prevIdx = idx - 1;

      const totalAssets = stock.currentAssets[idx] + stock.fixedAssets[idx];
      const prevAssets = stock.currentAssets[prevIdx] + stock.fixedAssets[prevIdx];
      const assetsGrowth = (((totalAssets - prevAssets) / prevAssets) * 100).toFixed(1);

      const netIncomeGrowth = (((stock.netIncome[idx] - stock.netIncome[prevIdx]) / Math.abs(stock.netIncome[prevIdx])) * 100).toFixed(1);
      const currentRatio = ((stock.currentAssets[idx] / stock.currentLiab[idx]) * 100).toFixed(1);
      const fixedRatio = ((stock.fixedAssets[idx] / stock.equity[idx]) * 100).toFixed(1);

      document.getElementById('kpiGrid').innerHTML = `
        <div class="bg-slate-800 border border-slate-700/80 p-3 rounded-xl shadow-sm">
          <span class="text-[10px] text-slate-400 block mb-1">総資産 (YoY)</span>
          <span class="text-sm sm:text-base font-bold text-slate-100">${formatValue(totalAssets)}</span>
          <span class="text-[10px] ml-1.5 ${assetsGrowth >= 0 ? 'text-emerald-400' : 'text-rose-400'}">
            ${assetsGrowth >= 0 ? '↑' : '↓'}${Math.abs(assetsGrowth)}%
          </span>
        </div>

        <div class="bg-slate-800 border border-slate-700/80 p-3 rounded-xl shadow-sm">
          <span class="text-[10px] text-slate-400 block mb-1">当期純利益 (YoY)</span>
          <span class="text-sm sm:text-base font-bold text-slate-100">${formatValue(stock.netIncome[idx])}</span>
          <span class="text-[10px] ml-1.5 ${netIncomeGrowth >= 0 ? 'text-emerald-400' : 'text-rose-400'}">
            ${netIncomeGrowth >= 0 ? '↑' : '↓'}${Math.abs(netIncomeGrowth)}%
          </span>
        </div>

        <div class="bg-slate-800 border border-slate-700/80 p-3 rounded-xl shadow-sm">
          <span class="text-[10px] text-slate-400 block mb-1">流動比率 (安全性)</span>
          <span class="text-sm sm:text-base font-bold text-cyan-400">${currentRatio}%</span>
          <span class="text-[10px] text-slate-400 block">目安: 100%以上</span>
        </div>

        <div class="bg-slate-800 border border-slate-700/80 p-3 rounded-xl shadow-sm">
          <span class="text-[10px] text-slate-400 block mb-1">固定比率 (長期安全性)</span>
          <span class="text-sm sm:text-base font-bold text-indigo-400">${fixedRatio}%</span>
          <span class="text-[10px] text-slate-400 block">目安: 100%以下</span>
        </div>
      `;
    }

    /* 4. Chart.js Stacked BS Visualizer */
    function renderBSChart(stock) {
      const ctx = document.getElementById('bsChart').getContext('2d');
      if (bsChartInstance) bsChartInstance.destroy();

      const mult = amountUnit === 'million' ? 100 : 1;

      bsChartInstance = new Chart(ctx, {
        type: 'bar',
        data: {
          labels: stock.years.map(y => `${y}期`),
          datasets: [
            {
              label: '流動資産',
              data: stock.currentAssets.map(v => v * mult),
              backgroundColor: '#06b6d4',
              stack: 'Stack 0',
            },
            {
              label: '固定資産',
              data: stock.fixedAssets.map(v => v * mult),
              backgroundColor: '#3b82f6',
              stack: 'Stack 0',
            },
            {
              label: '流動負債',
              data: stock.currentLiab.map(v => v * mult),
              backgroundColor: '#f43f5e',
              stack: 'Stack 1',
            },
            {
              label: '固定負債',
              data: stock.fixedLiab.map(v => v * mult),
              backgroundColor: '#fb7185',
              stack: 'Stack 1',
            },
            {
              label: '純資産 (自己資本)',
              data: stock.equity.map(v => v * mult),
              backgroundColor: '#10b981',
              stack: 'Stack 1',
            }
          ]
        },
        options: {
          responsive: true,
          maintainAspectRatio: false,
          plugins: {
            legend: {
              position: 'top',
              labels: { color: '#94a3b8', font: { size: 10 }, boxWidth: 12 }
            },
            tooltip: {
              callbacks: {
                label: (context) => `${context.dataset.label}: ${context.raw.toLocaleString()} ${amountUnit === 'million' ? '百万円' : '億円'}`
              }
            }
          },
          scales: {
            x: {
              ticks: { color: '#94a3b8', font: { size: 10 } },
              grid: { color: '#334155' }
            },
            y: {
              ticks: { color: '#94a3b8', font: { size: 10 } },
              grid: { color: '#334155' }
            }
          }
        }
      });
    }

    /* 5. Collapsible Year Accordion for Detailed BS Breakdown */
    function renderBSAccordion(stock) {
      const container = document.getElementById('bsDetailAccordion');
      container.innerHTML = stock.years.slice().reverse().map((year, revIdx) => {
        const idx = stock.years.length - 1 - revIdx;
        const curA = stock.currentAssets[idx];
        const fixA = stock.fixedAssets[idx];
        const curL = stock.currentLiab[idx];
        const fixL = stock.fixedLiab[idx];
        const eq = stock.equity[idx];
        const total = curA + fixA;

        return `
          <div class="border border-slate-700/60 rounded-lg overflow-hidden bg-slate-900/40">
            <button onclick="toggleAccordion('acc-${year}')" class="w-full px-3 py-2.5 flex items-center justify-between text-left hover:bg-slate-800/50 transition">
              <div class="flex items-center gap-2">
                <span class="font-bold text-xs text-cyan-400">${year}年3月期</span>
                <span class="text-[11px] text-slate-400">総資産: ${formatValue(total)}</span>
              </div>
              <i data-lucide="chevron-down" class="w-4 h-4 text-slate-400"></i>
            </button>
            <div id="acc-${year}" class="hidden p-3 border-t border-slate-700/50 bg-slate-900/80 text-xs space-y-2">
              <div class="grid grid-cols-2 gap-3">
                <div class="space-y-1">
                  <span class="block font-semibold text-cyan-400 text-[11px] border-b border-cyan-500/20 pb-0.5">資産の部</span>
                  <div class="flex justify-between text-slate-300"><span>流動資産:</span> <span>${formatValue(curA)}</span></div>
                  <div class="flex justify-between text-slate-300"><span>固定資産:</span> <span>${formatValue(fixA)}</span></div>
                  <div class="flex justify-between font-bold text-slate-100 border-t border-slate-700 pt-1"><span>資産合計:</span> <span>${formatValue(total)}</span></div>
                </div>
                <div class="space-y-1">
                  <span class="block font-semibold text-rose-400 text-[11px] border-b border-rose-500/20 pb-0.5">負債・純資産の部</span>
                  <div class="flex justify-between text-slate-300"><span>流動負債:</span> <span>${formatValue(curL)}</span></div>
                  <div class="flex justify-between text-slate-300"><span>固定負債:</span> <span>${formatValue(fixL)}</span></div>
                  <div class="flex justify-between text-emerald-400"><span>純資産:</span> <span>${formatValue(eq)}</span></div>
                  <div class="flex justify-between font-bold text-slate-100 border-t border-slate-700 pt-1"><span>負債純資産計:</span> <span>${formatValue(curL + fixL + eq)}</span></div>
                </div>
              </div>
            </div>
          </div>
        `;
      }).join('');
      lucide.createIcons();
    }

    function toggleAccordion(id) {
      const el = document.getElementById(id);
      if (el) el.classList.toggle('hidden');
    }

    /* 6. Multi-Stock Comparison Section */
    function renderCompareSection() {
      const selectorContainer = document.getElementById('compareTickerSelector');
      selectorContainer.innerHTML = stockData.map(s => `
        <label class="flex items-center gap-1.5 bg-slate-900/80 px-2.5 py-1 rounded border border-slate-700 cursor-pointer text-xs">
          <input type="checkbox" value="${s.code}" checked onchange="updateCompareChart()" class="accent-cyan-500 rounded">
          <span class="text-slate-200">${s.code} ${s.name}</span>
        </label>
      `).join('');

      updateCompareChart();
    }

    function updateCompareChart() {
      const checkedCodes = Array.from(document.querySelectorAll('#compareTickerSelector input:checked')).map(cb => cb.value);
      const selectedStocks = stockData.filter(s => checkedCodes.includes(s.code));

      const ctx = document.getElementById('compareChart').getContext('2d');
      if (compareChartInstance) compareChartInstance.destroy();

      const colors = ['#06b6d4', '#10b981', '#f59e0b', '#ec4899', '#8b5cf6'];

      compareChartInstance = new Chart(ctx, {
        type: 'line',
        data: {
          labels: DEFAULT_STOCKS[0].years.map(y => `${y}期`),
          datasets: selectedStocks.map((s, idx) => ({
            label: `${s.name} 自己資本比率(%)`,
            data: s.years.map((y, i) => {
              const total = s.currentAssets[i] + s.fixedAssets[i];
              return ((s.equity[i] / total) * 100).toFixed(1);
            }),
            borderColor: colors[idx % colors.length],
            backgroundColor: colors[idx % colors.length],
            tension: 0.2
          }))
        },
        options: {
          responsive: true,
          maintainAspectRatio: false,
          plugins: {
            legend: { labels: { color: '#94a3b8', font: { size: 10 } } }
          },
          scales: {
            x: { ticks: { color: '#94a3b8', font: { size: 10 } }, grid: { color: '#334155' } },
            y: { ticks: { color: '#94a3b8', font: { size: 10 } }, grid: { color: '#334155' } }
          }
        }
      });

      // Comparison Table Render
      const table = document.getElementById('compareTable');
      table.innerHTML = `
        <thead>
          <tr class="border-b border-slate-700 text-slate-400">
            <th class="py-2 px-2">銘柄</th>
            <th class="py-2 px-2">自己資本比率</th>
            <th class="py-2 px-2">流動比率</th>
            <th class="py-2 px-2">総資産</th>
          </tr>
        </thead>
        <tbody>
          ${selectedStocks.map(s => {
            const idx = s.years.length - 1;
            const total = s.currentAssets[idx] + s.fixedAssets[idx];
            const eqRatio = ((s.equity[idx] / total) * 100).toFixed(1);
            const curRatio = ((s.currentAssets[idx] / s.currentLiab[idx]) * 100).toFixed(1);
            return `
              <tr class="border-b border-slate-700/50 hover:bg-slate-700/30">
                <td class="py-2 px-2 font-bold text-slate-100">${s.name} (${s.code})</td>
                <td class="py-2 px-2 text-cyan-400 font-semibold">${eqRatio}%</td>
                <td class="py-2 px-2 text-slate-200">${curRatio}%</td>
                <td class="py-2 px-2 text-slate-300">${formatValue(total)}</td>
              </tr>
            `;
          }).join('')}
        </tbody>
      `;
    }

    /* 7. Ratio Charts Section */
    function renderRatioCharts(stock) {
      const ctx1 = document.getElementById('ratioChart1').getContext('2d');
      if (ratioChart1Instance) ratioChart1Instance.destroy();

      ratioChart1Instance = new Chart(ctx1, {
        type: 'line',
        data: {
          labels: stock.years.map(y => `${y}期`),
          datasets: [
            {
              label: '自己資本比率 (%)',
              data: stock.years.map((y, i) => ((stock.equity[i] / (stock.currentAssets[i] + stock.fixedAssets[i])) * 100).toFixed(1)),
              borderColor: '#06b6d4',
              backgroundColor: '#06b6d4',
            },
            {
              label: 'ROE (自己資本利益率 %)',
              data: stock.years.map((y, i) => ((stock.netIncome[i] / stock.equity[i]) * 100).toFixed(1)),
              borderColor: '#10b981',
              backgroundColor: '#10b981',
            }
          ]
        },
        options: {
          responsive: true,
          maintainAspectRatio: false,
          plugins: { legend: { labels: { color: '#94a3b8', font: { size: 10 } } } },
          scales: {
            x: { ticks: { color: '#94a3b8', font: { size: 10 } }, grid: { color: '#334155' } },
            y: { ticks: { color: '#94a3b8', font: { size: 10 } }, grid: { color: '#334155' } }
          }
        }
      });

      const ctx2 = document.getElementById('ratioChart2').getContext('2d');
      if (ratioChart2Instance) ratioChart2Instance.destroy();

      ratioChart2Instance = new Chart(ctx2, {
        type: 'bar',
        data: {
          labels: stock.years.map(y => `${y}期`),
          datasets: [
            {
              label: '流動比率 (%)',
              data: stock.years.map((y, i) => ((stock.currentAssets[i] / stock.currentLiab[i]) * 100).toFixed(1)),
              backgroundColor: '#3b82f6',
            },
            {
              label: '固定比率 (%)',
              data: stock.years.map((y, i) => ((stock.fixedAssets[i] / stock.equity[i]) * 100).toFixed(1)),
              backgroundColor: '#f43f5e',
            }
          ]
        },
        options: {
          responsive: true,
          maintainAspectRatio: false,
          plugins: { legend: { labels: { color: '#94a3b8', font: { size: 10 } } } },
          scales: {
            x: { ticks: { color: '#94a3b8', font: { size: 10 } }, grid: { color: '#334155' } },
            y: { ticks: { color: '#94a3b8', font: { size: 10 } }, grid: { color: '#334155' } }
          }
        }
      });
    }

    /* 8. Manage Stock Section */
    function renderManageSection() {
      const container = document.getElementById('managedTickersList');
      container.innerHTML = stockData.map(s => `
        <div class="p-3 bg-slate-900/60 rounded-lg border border-slate-700 flex items-center justify-between gap-2">
          <div>
            <div class="flex items-center gap-2">
              <span class="font-bold text-xs text-cyan-400">${s.code}</span>
              <span class="text-xs font-semibold text-slate-100">${s.name}</span>
            </div>
            <p class="text-[10px] text-slate-400 mt-0.5">${s.sector} | 登録データ期間: ${s.years[0]} - ${s.years[s.years.length-1]}</p>
          </div>
          <button onclick="selectTicker('${s.code}'); switchTab('Detail');" class="px-3 py-1 bg-slate-800 hover:bg-slate-700 border border-slate-600 rounded text-xs text-slate-200 shrink-0">
            表示
          </button>
        </div>
      `).join('');
    }

    /* Custom Ticker Form Handler */
    function handleCustomTickerSubmit(e) {
      e.preventDefault();
      const code = document.getElementById('newCode').value.trim();
      const name = document.getElementById('newName').value.trim();
      const sector = document.getElementById('newSector').value.trim();
      
      const curA = parseFloat(document.getElementById('newCurrentAssets').value);
      const fixA = parseFloat(document.getElementById('newFixedAssets').value);
      const curL = parseFloat(document.getElementById('newCurrentLiab').value);
      const fixL = parseFloat(document.getElementById('newFixedLiab').value);
      const eq = parseFloat(document.getElementById('newEquity').value);

      const newStock = {
        code,
        name,
        sector,
        years: [2024],
        currentAssets: [curA],
        fixedAssets: [fixA],
        currentLiab: [curL],
        fixedLiab: [fixL],
        equity: [eq],
        netIncome: [Math.round(eq * 0.08)]
      };

      stockData.push(newStock);
      selectedTickerCode = code;
      closeModal('addTickerModal');
      renderQuickTickerBar();
      switchTab('Detail');
    }

    /* 9. CSV Export */
    function exportCurrentTickerCSV() {
      const stock = stockData.find(s => s.code === selectedTickerCode) || stockData[0];
      let csvContent = "data:text/csv;charset=utf-8,年度,流動資産(億円),固定資産(億円),流動負債(億円),固定負債(億円),純資産(億円),当期純利益(億円)\n";

      stock.years.forEach((y, i) => {
        csvContent += `${y},${stock.currentAssets[i]},${stock.fixedAssets[i]},${stock.currentLiab[i]},${stock.fixedLiab[i]},${stock.equity[i]},${stock.netIncome[i]}\n`;
      });

      const encodedUri = encodeURI(csvContent);
      const link = document.createElement("a");
      link.setAttribute("href", encodedUri);
      link.setAttribute("download", `${stock.code}_${stock.name}_Financials.csv`);
      document.body.appendChild(link);
      link.click();
      document.body.removeChild(link);
    }

    /* 10. EDINET API Simulator */
    function simulateEdinetFetch() {
      const val = document.getElementById('edinetInput').value.trim();
      const statusBox = document.getElementById('edinetStatus');
      statusBox.classList.remove('hidden');

      if (!val) {
        statusBox.innerHTML = '<span class="text-rose-400">コードを入力してください。</span>';
        return;
      }

      statusBox.innerHTML = '<span class="text-cyan-400">EDINET APIエンドポイントへリクエスト送信中...</span>';

      setTimeout(() => {
        statusBox.innerHTML = `
          <div class="space-y-1 text-slate-300">
            <p class="text-emerald-400 font-bold">[成功] 書類データを検出しました (DocID: S100${Math.floor(Math.random()*90000+10000)})</p>
            <p>対象コード: ${val} | 提出日時: 2024-06-25</p>
            <p class="text-slate-400 text-[10px]">XBRL要素解析完了: 流動資産, 固定資産, 自己資本科目マッピング完了。</p>
          </div>
        `;
      }, 800);
    }

    /* Modal Controls */
    function openModal(id) { document.getElementById(id).classList.remove('hidden'); }
    function closeModal(id) { document.getElementById(id).classList.add('hidden'); }

    /* Helper: Format Money Values */
    function formatValue(valInHundredMillion) {
      if (amountUnit === 'million') {
        return (valInHundredMillion * 100).toLocaleString() + '百万円';
      }
      return valInHundredMillion.toLocaleString() + '億円';
    }
  </script>
</body>
</html>
