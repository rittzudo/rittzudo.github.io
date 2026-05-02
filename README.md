# rittzudo.github.io
<!DOCTYPE html>

<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Plano de Estudos SAT 2026</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700;900&family=DM+Mono:wght@300;400;500&family=Lora:ital,wght@0,400;0,600;1,400&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #0d0d0d;
    --surface: #141414;
    --surface2: #1c1c1c;
    --border: #2a2a2a;
    --accent: #c8a96e;
    --accent2: #7ec8a9;
    --accent3: #c87e7e;
    --accent4: #7e9ec8;
    --text: #e8e2d9;
    --muted: #6b6560;
    --phase1: #c8a96e;
    --phase2: #7ec8a9;
    --phase3: #7e9ec8;
    --phase4: #c87e7e;
  }

- { margin: 0; padding: 0; box-sizing: border-box; }

body {
background: var(–bg);
color: var(–text);
font-family: ‘Lora’, Georgia, serif;
min-height: 100vh;
overflow-x: hidden;
}

/* HEADER */
header {
position: relative;
padding: 60px 40px 40px;
border-bottom: 1px solid var(–border);
overflow: hidden;
}

header::before {
content: ‘SAT’;
position: absolute;
right: -20px;
top: -30px;
font-family: ‘Playfair Display’, serif;
font-size: 260px;
font-weight: 900;
color: #ffffff06;
line-height: 1;
pointer-events: none;
user-select: none;
}

.header-tag {
font-family: ‘DM Mono’, monospace;
font-size: 11px;
letter-spacing: 3px;
color: var(–accent);
text-transform: uppercase;
margin-bottom: 12px;
}

h1 {
font-family: ‘Playfair Display’, serif;
font-size: clamp(32px, 6vw, 64px);
font-weight: 900;
line-height: 1.05;
letter-spacing: -1px;
color: var(–text);
}

h1 span { color: var(–accent); }

.header-meta {
margin-top: 20px;
display: flex;
gap: 32px;
flex-wrap: wrap;
}

.meta-pill {
background: var(–surface2);
border: 1px solid var(–border);
border-radius: 4px;
padding: 8px 16px;
font-family: ‘DM Mono’, monospace;
font-size: 12px;
color: var(–muted);
}

.meta-pill strong { color: var(–text); }

/* PHASE LEGEND */
.legend {
display: flex;
gap: 20px;
padding: 24px 40px;
border-bottom: 1px solid var(–border);
flex-wrap: wrap;
background: var(–surface);
}

.legend-item {
display: flex;
align-items: center;
gap: 8px;
font-family: ‘DM Mono’, monospace;
font-size: 11px;
color: var(–muted);
cursor: pointer;
transition: color .2s;
}

.legend-item:hover { color: var(–text); }

.legend-dot {
width: 10px; height: 10px;
border-radius: 50%;
flex-shrink: 0;
}

/* FILTERS */
.filters {
padding: 20px 40px;
display: flex;
gap: 10px;
flex-wrap: wrap;
align-items: center;
border-bottom: 1px solid var(–border);
}

.filter-label {
font-family: ‘DM Mono’, monospace;
font-size: 11px;
color: var(–muted);
letter-spacing: 2px;
text-transform: uppercase;
margin-right: 8px;
}

.filter-btn {
background: none;
border: 1px solid var(–border);
color: var(–muted);
font-family: ‘DM Mono’, monospace;
font-size: 11px;
padding: 6px 14px;
border-radius: 3px;
cursor: pointer;
transition: all .2s;
letter-spacing: 1px;
}

.filter-btn:hover, .filter-btn.active {
border-color: var(–accent);
color: var(–accent);
background: rgba(200,169,110,0.06);
}

/* PROGRESS */
.progress-bar-wrap {
padding: 16px 40px;
background: var(–surface);
border-bottom: 1px solid var(–border);
display: flex;
align-items: center;
gap: 16px;
}

.progress-label {
font-family: ‘DM Mono’, monospace;
font-size: 11px;
color: var(–muted);
white-space: nowrap;
}

.progress-track {
flex: 1;
height: 4px;
background: var(–border);
border-radius: 2px;
overflow: hidden;
}

.progress-fill {
height: 100%;
background: linear-gradient(90deg, var(–phase1), var(–phase2), var(–phase3), var(–phase4));
border-radius: 2px;
transition: width .5s ease;
}

.progress-pct {
font-family: ‘DM Mono’, monospace;
font-size: 12px;
color: var(–accent);
white-space: nowrap;
}

/* SESSIONS GRID */
.sessions-container {
padding: 32px 40px;
}

.phase-section {
margin-bottom: 48px;
}

.phase-header {
display: flex;
align-items: baseline;
gap: 16px;
margin-bottom: 20px;
padding-bottom: 12px;
border-bottom: 1px solid var(–border);
}

.phase-num {
font-family: ‘DM Mono’, monospace;
font-size: 11px;
letter-spacing: 2px;
color: var(–muted);
}

.phase-title {
font-family: ‘Playfair Display’, serif;
font-size: 22px;
font-weight: 700;
}

.phase-range {
font-family: ‘DM Mono’, monospace;
font-size: 11px;
color: var(–muted);
margin-left: auto;
}

.sessions-grid {
display: grid;
grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
gap: 12px;
}

/* SESSION CARD */
.session-card {
background: var(–surface);
border: 1px solid var(–border);
border-radius: 6px;
padding: 16px 18px;
cursor: pointer;
transition: all .2s;
position: relative;
overflow: hidden;
}

.session-card::before {
content: ‘’;
position: absolute;
left: 0; top: 0; bottom: 0;
width: 3px;
border-radius: 3px 0 0 3px;
}

.session-card.phase-1::before { background: var(–phase1); }
.session-card.phase-2::before { background: var(–phase2); }
.session-card.phase-3::before { background: var(–phase3); }
.session-card.phase-4::before { background: var(–phase4); }

.session-card:hover {
border-color: #3a3a3a;
transform: translateY(-1px);
background: var(–surface2);
}

.session-card.done {
opacity: 0.5;
}

.session-card.done .session-title {
text-decoration: line-through;
text-decoration-color: var(–muted);
}

.session-top {
display: flex;
justify-content: space-between;
align-items: flex-start;
margin-bottom: 10px;
}

.session-date {
font-family: ‘DM Mono’, monospace;
font-size: 11px;
color: var(–muted);
}

.session-type {
font-family: ‘DM Mono’, monospace;
font-size: 10px;
letter-spacing: 1px;
padding: 3px 8px;
border-radius: 2px;
text-transform: uppercase;
}

.type-math { background: rgba(126,158,200,0.15); color: var(–accent4); }
.type-reading { background: rgba(126,200,169,0.15); color: var(–accent2); }
.type-mixed { background: rgba(200,169,110,0.15); color: var(–accent); }
.type-simulado { background: rgba(200,126,126,0.15); color: var(–accent3); }

.session-num {
font-family: ‘DM Mono’, monospace;
font-size: 10px;
color: var(–muted);
}

.session-title {
font-family: ‘Lora’, serif;
font-size: 14px;
font-weight: 600;
color: var(–text);
margin-bottom: 6px;
line-height: 1.35;
}

.session-topics {
font-family: ‘DM Mono’, monospace;
font-size: 10px;
color: var(–muted);
line-height: 1.7;
}

.session-topics span {
display: inline-block;
margin-right: 6px;
}

.session-topics span::before { content: ’· ’; }

.check-btn {
position: absolute;
right: 12px;
bottom: 12px;
width: 22px; height: 22px;
border-radius: 50%;
border: 1px solid var(–border);
background: none;
cursor: pointer;
display: flex; align-items: center; justify-content: center;
transition: all .2s;
color: var(–muted);
font-size: 11px;
}

.check-btn:hover { border-color: var(–accent2); color: var(–accent2); }
.session-card.done .check-btn {
background: var(–accent2);
border-color: var(–accent2);
color: #0d0d0d;
}

/* TIPS PANEL */
.tips-section {
padding: 0 40px 40px;
}

.tips-title {
font-family: ‘Playfair Display’, serif;
font-size: 20px;
margin-bottom: 16px;
padding-bottom: 12px;
border-bottom: 1px solid var(–border);
}

.tips-grid {
display: grid;
grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
gap: 12px;
}

.tip-card {
background: var(–surface);
border: 1px solid var(–border);
border-radius: 6px;
padding: 16px;
}

.tip-icon {
font-size: 20px;
margin-bottom: 8px;
}

.tip-title {
font-family: ‘DM Mono’, monospace;
font-size: 11px;
letter-spacing: 1px;
color: var(–accent);
margin-bottom: 6px;
text-transform: uppercase;
}

.tip-text {
font-size: 13px;
color: var(–muted);
line-height: 1.6;
}

/* HIDDEN */
.session-card.hidden { display: none; }

@media (max-width: 600px) {
header, .sessions-container, .filters, .tips-section, .progress-bar-wrap, .legend { padding-left: 20px; padding-right: 20px; }
h1 { font-size: 28px; }
header::before { font-size: 140px; }
}
</style>

</head>
<body>

<header>
  <div class="header-tag">▸ Plano de Estudos Personalizado</div>
  <h1>Preparação para o <span>SAT</span></h1>
  <div class="header-meta">
    <div class="meta-pill">📅 Início: <strong>03 Mai 2026</strong></div>
    <div class="meta-pill">🏁 Meta: <strong>Setembro 2026</strong></div>
    <div class="meta-pill">📆 Dias: <strong>Domingo + Segunda</strong></div>
    <div class="meta-pill">📚 Total: <strong id="total-sessions">-- sessões</strong></div>
  </div>
</header>

<div class="legend">
  <div class="legend-item"><div class="legend-dot" style="background:var(--phase1)"></div> Fase 1 – Fundamentos</div>
  <div class="legend-item"><div class="legend-dot" style="background:var(--phase2)"></div> Fase 2 – Aprofundamento</div>
  <div class="legend-item"><div class="legend-dot" style="background:var(--phase3)"></div> Fase 3 – Prática Intensiva</div>
  <div class="legend-item"><div class="legend-dot" style="background:var(--phase4)"></div> Fase 4 – Simulados & Revisão</div>
</div>

<div class="filters">
  <span class="filter-label">Filtrar</span>
  <button class="filter-btn active" onclick="filterSessions('all')">Todas</button>
  <button class="filter-btn" onclick="filterSessions('math')">Matemática</button>
  <button class="filter-btn" onclick="filterSessions('reading')">Reading & Writing</button>
  <button class="filter-btn" onclick="filterSessions('mixed')">Misto</button>
  <button class="filter-btn" onclick="filterSessions('simulado')">Simulados</button>
  <button class="filter-btn" onclick="filterSessions('pending')" style="margin-left:auto">⏳ Pendentes</button>
</div>

<div class="progress-bar-wrap">
  <span class="progress-label">PROGRESSO GERAL</span>
  <div class="progress-track"><div class="progress-fill" id="progress-fill" style="width:0%"></div></div>
  <span class="progress-pct" id="progress-pct">0 / 0</span>
</div>

<div class="sessions-container" id="sessions-container"></div>

<div class="tips-section">
  <div class="tips-title">Dicas Essenciais para o SAT</div>
  <div class="tips-grid">
    <div class="tip-card">
      <div class="tip-icon">📖</div>
      <div class="tip-title">Material Oficial</div>
      <div class="tip-text">Use sempre o Khan Academy SAT (gratuito e oficial). Faça os testes diagnósticos para personalizar ainda mais seu plano.</div>
    </div>
    <div class="tip-card">
      <div class="tip-icon">🧠</div>
      <div class="tip-title">Revisão Espaçada</div>
      <div class="tip-text">Revise erros da sessão anterior antes de começar uma nova. O cérebro consolida memória com repetição espaçada.</div>
    </div>
    <div class="tip-card">
      <div class="tip-icon">⏱️</div>
      <div class="tip-title">Sessões Cronometradas</div>
      <div class="tip-text">Desde o início, pratique com tempo. O SAT Digital é 2h 14min. Treinar com pressão de tempo é fundamental.</div>
    </div>
    <div class="tip-card">
      <div class="tip-icon">📊</div>
      <div class="tip-title">Analise seus Erros</div>
      <div class="tip-text">Mantenha um caderno de erros. Categorize por tipo (conceito, distração, tempo). Isso revela padrões e direciona revisões.</div>
    </div>
    <div class="tip-card">
      <div class="tip-icon">🎯</div>
      <div class="tip-title">SAT Digital</div>
      <div class="tip-text">O SAT atual é totalmente digital (Bluebook App). Pratique na plataforma oficial para se familiarizar com a interface.</div>
    </div>
    <div class="tip-card">
      <div class="tip-icon">💪</div>
      <div class="tip-title">Consistência > Intensidade</div>
      <div class="tip-text">Duas sessões focadas por semana valem mais que uma maratona mensal. Mantenha a consistência e respeite o plano.</div>
    </div>
  </div>
</div>

<script>
const SESSIONS_KEY = 'sat_done_sessions_v2';

// ---- BUILD SCHEDULE ----
function getSessionDates(startDate, endDate) {
  const dates = [];
  const current = new Date(startDate);
  const end = new Date(endDate);

  // Alternating variable days: Sun, Mon, Sun, Mon...
  // But per user: Mondays fixed + variable day starting tomorrow (Sunday)
  // Strategy: sessions on Sundays and Mondays
  while (current <= end) {
    const dow = current.getDay(); // 0=Sun, 1=Mon
    if (dow === 0 || dow === 1) {
      dates.push(new Date(current));
    }
    current.setDate(current.getDate() + 1);
  }
  return dates;
}

const START = '2026-05-03';
const END   = '2026-09-28';
const dates = getSessionDates(START, END);

// ---- CURRICULUM ----
const curriculum = [
  // PHASE 1: May 3 – June 14 (Fundamentos)
  { title: 'Diagnóstico Inicial', type: 'simulado', topics: ['Mini-simulado oficial', 'Identificar pontos fracos', 'Definir metas de pontuação'] },
  { title: 'Álgebra Linear I', type: 'math', topics: ['Equações de 1º grau', 'Inequações', 'Sistemas lineares'] },
  { title: 'Reading: Ideia Principal', type: 'reading', topics: ['Main idea & purpose', 'Inferências diretas', 'Vocabulário em contexto'] },
  { title: 'Álgebra Linear II', type: 'math', topics: ['Funções lineares', 'Gráficos lineares', 'Interceptos e inclinação'] },
  { title: 'Writing: Gramática Essencial', type: 'reading', topics: ['Sujeito-verbo concordância', 'Pronomes', 'Pontuação básica'] },
  { title: 'Funções & Gráficos', type: 'math', topics: ['Domínio e imagem', 'Funções quadráticas', 'Parábolas'] },
  { title: 'Reading: Estrutura de Texto', type: 'reading', topics: ['Text structure', 'Transições', 'Propósito retórico'] },
  { title: 'Percentuais & Razões', type: 'math', topics: ['Porcentagem', 'Proporção', 'Razão e taxa de variação'] },
  { title: 'Writing: Coesão e Fluxo', type: 'reading', topics: ['Coerência de argumento', 'Ordem lógica', 'Conectivos'] },
  { title: 'Revisão Fase 1 + Simulado Parcial', type: 'simulado', topics: ['Revisão de erros acumulados', 'Mini-simulado módulo Math', 'Análise de desempenho'] },
  { title: 'Equações Quadráticas', type: 'math', topics: ['Fatoração', 'Fórmula quadrática', 'Discriminante'] },
  { title: 'Reading: Evidência & Dados', type: 'reading', topics: ['Command of evidence', 'Gráficos e tabelas', 'Interpretação de dados'] },

  // PHASE 2: June 15 – July 26 (Aprofundamento)
  { title: 'Sistemas Quadráticos', type: 'math', topics: ['Sistemas linear-quadrático', 'Número de soluções', 'Problemas contextuais'] },
  { title: 'Writing: Precisão Linguística', type: 'reading', topics: ['Word choice', 'Concisão', 'Tom e audiência'] },
  { title: 'Estatística & Probabilidade I', type: 'math', topics: ['Média, mediana, moda', 'Desvio padrão (conceito)', 'Probabilidade básica'] },
  { title: 'Reading: Textos Literários', type: 'reading', topics: ['Ficção e narrativa', 'Personagem e ponto de vista', 'Tom e atmosfera'] },
  { title: 'Exponenciais & Radicais', type: 'math', topics: ['Propriedades de expoentes', 'Funções exponenciais', 'Radicais e potências fracionárias'] },
  { title: 'Writing: Edição Avançada', type: 'reading', topics: ['Estrutura de sentença', 'Modificadores', 'Paralelismo'] },
  { title: 'Geometria I – Plana', type: 'math', topics: ['Área e perímetro', 'Triângulos', 'Círculos'] },
  { title: 'Reading: Textos de Ciências', type: 'reading', topics: ['Ciência e dados', 'Causa e efeito', 'Hipótese e conclusão'] },
  { title: 'Geometria II – Analítica', type: 'math', topics: ['Distância e ponto médio', 'Equação da reta', 'Equação do círculo'] },
  { title: 'Simulado Completo #1', type: 'simulado', topics: ['Simulado full (2h14)', 'Revisão detalhada', 'Ajuste de estratégia'] },
  { title: 'Trigonometria Básica', type: 'math', topics: ['Seno, cosseno, tangente', 'Triângulos especiais', 'SOH-CAH-TOA'] },
  { title: 'Reading: Textos de História & Humanidades', type: 'reading', topics: ['Textos históricos', 'Argumento e evidência', 'Perspectiva e contexto'] },
  { title: 'Estatística II & Amostras', type: 'math', topics: ['Tipos de estudo', 'Amostras e viés', 'Interpretação de gráficos'] },
  { title: 'Misto: Revisão Mid-Plan', type: 'mixed', topics: ['Revisão Math Fases 1-2', 'Revisão Reading Fases 1-2', 'Caderno de erros'] },

  // PHASE 3: July 27 – August 30 (Prática Intensiva)
  { title: 'Álgebra Avançada: Polinômios', type: 'math', topics: ['Divisão de polinômios', 'Teorema do resto', 'Zeros de funções'] },
  { title: 'Reading: Argumentação Complexa', type: 'reading', topics: ['Contraargumentos', 'Suposições implícitas', 'Enfraquecimento/fortalecimento'] },
  { title: 'Inequações Quadráticas & Racionais', type: 'math', topics: ['Inequações de 2º grau', 'Teste de intervalos', 'Problemas aplicados'] },
  { title: 'Writing: Simulação Intensiva', type: 'reading', topics: ['30 questões cronometradas', 'Revisão imediata', 'Padrões de erro'] },
  { title: 'Problemas em Contexto – Math', type: 'math', topics: ['Word problems', 'Modelagem matemática', 'Unidades de medida'] },
  { title: 'Simulado Completo #2', type: 'simulado', topics: ['Simulado full (2h14)', 'Revisão intensiva', 'Comparação com Simulado #1'] },
  { title: 'Funções Avançadas', type: 'math', topics: ['Composição de funções', 'Funções inversas', 'Transformações'] },
  { title: 'Reading: Vocabulário Avançado', type: 'reading', topics: ['High-frequency SAT words', 'Contexto dedutivo', 'Palavras-raiz latinas'] },
  { title: 'Geometria III – Sólidos', type: 'math', topics: ['Volume e área superficial', 'Cone, esfera, cilindro', 'Problemas contextuais'] },
  { title: 'Misto: Pontos Fracos', type: 'mixed', topics: ['Foco nos tópicos com mais erros', 'Exercícios direcionados', 'Khan Academy adaptativo'] },

  // PHASE 4: Aug 31 – Sep 27 (Simulados & Revisão)
  { title: 'Simulado Completo #3', type: 'simulado', topics: ['Simulado full (2h14)', 'Revisão detalhada', 'Score projetado'] },
  { title: 'Revisão: Math de Alta Frequência', type: 'math', topics: ['Tópicos mais cobrados', 'Truques e atalhos', 'Gestão de tempo Math'] },
  { title: 'Revisão: Reading de Alta Frequência', type: 'reading', topics: ['Tipos de questão mais comuns', 'Estratégia de eliminação', 'Gestão de tempo R&W'] },
  { title: 'Simulado Completo #4', type: 'simulado', topics: ['Simulado full (2h14)', 'Análise final de erros', 'Metas por seção'] },
  { title: 'Revisão Final – Math', type: 'math', topics: ['Flash cards de fórmulas', 'Últimas revisões de conceito', 'Relaxamento de estratégia'] },
  { title: 'Revisão Final – Reading & Writing', type: 'reading', topics: ['Técnicas de leitura rápida', 'Checklist de gramática', 'Confiança e calma'] },
  { title: 'Simulado Diagnóstico Final', type: 'simulado', topics: ['Simulado completo', 'Avaliação do progresso total', '🎯 Pronto para o SAT!'] },
];

const phases = [
  { id: 1, label: 'FASE 01', title: 'Fundamentos', range: 'Mai – Jun 14', sessions: [0, 11], cls: 'phase-1' },
  { id: 2, label: 'FASE 02', title: 'Aprofundamento', range: 'Jun 15 – Jul 26', sessions: [12, 25], cls: 'phase-2' },
  { id: 3, label: 'FASE 03', title: 'Prática Intensiva', range: 'Jul 27 – Ago 30', sessions: [26, 35], cls: 'phase-3' },
  { id: 4, label: 'FASE 04', title: 'Simulados & Revisão Final', range: 'Ago 31 – Set', sessions: [36, 99], cls: 'phase-4' },
];

const phaseForIndex = (i) => {
  if (i <= 11) return 1;
  if (i <= 25) return 2;
  if (i <= 35) return 3;
  return 4;
};

const typeLabel = { math: 'Matemática', reading: 'Reading & Writing', mixed: 'Misto', simulado: 'Simulado' };
const typeClass = { math: 'type-math', reading: 'type-reading', mixed: 'type-mixed', simulado: 'type-simulado' };

function formatDate(d) {
  const days = ['Dom','Seg','Ter','Qua','Qui','Sex','Sáb'];
  const months = ['Jan','Fev','Mar','Abr','Mai','Jun','Jul','Ago','Set','Out','Nov','Dez'];
  return `${days[d.getDay()]}, ${String(d.getDate()).padStart(2,'0')} ${months[d.getMonth()]}`;
}

// Load done state
let done = {};
try { done = JSON.parse(localStorage.getItem(SESSIONS_KEY) || '{}'); } catch(e) {}

function saveDone() {
  try { localStorage.setItem(SESSIONS_KEY, JSON.stringify(done)); } catch(e) {}
}

function toggleDone(idx) {
  done[idx] = !done[idx];
  saveDone();
  render();
  updateProgress();
}

// Map curriculum to dates
const sessionData = curriculum.map((s, i) => ({
  ...s,
  idx: i,
  date: dates[i] || null,
  phase: phaseForIndex(i),
}));

document.getElementById('total-sessions').textContent = sessionData.length + ' sessões';

let currentFilter = 'all';

function filterSessions(type) {
  currentFilter = type;
  document.querySelectorAll('.filter-btn').forEach(b => b.classList.remove('active'));
  event.target.classList.add('active');
  render();
}

function render() {
  const container = document.getElementById('sessions-container');
  container.innerHTML = '';

  phases.forEach(phase => {
    const phaseSessions = sessionData.filter(s => s.phase === phase.id);
    const filtered = phaseSessions.filter(s => {
      if (currentFilter === 'all') return true;
      if (currentFilter === 'pending') return !done[s.idx];
      return s.type === currentFilter;
    });
    if (filtered.length === 0) return;

    const section = document.createElement('div');
    section.className = 'phase-section';

    section.innerHTML = `
      <div class="phase-header">
        <span class="phase-num">${phase.label}</span>
        <span class="phase-title" style="color:var(--phase${phase.id})">${phase.title}</span>
        <span class="phase-range">${phase.range}</span>
      </div>
      <div class="sessions-grid"></div>
    `;

    const grid = section.querySelector('.sessions-grid');

    filtered.forEach(s => {
      const card = document.createElement('div');
      card.className = `session-card phase-${s.phase} ${done[s.idx] ? 'done' : ''}`;
      card.innerHTML = `
        <div class="session-top">
          <div>
            <div class="session-date">${s.date ? formatDate(s.date) : 'Data a definir'}</div>
            <div class="session-num">#${String(s.idx + 1).padStart(2,'0')}</div>
          </div>
          <div class="session-type ${typeClass[s.type]}">${typeLabel[s.type]}</div>
        </div>
        <div class="session-title">${s.title}</div>
        <div class="session-topics">
          ${s.topics.map(t => `<span>${t}</span>`).join('')}
        </div>
        <button class="check-btn" onclick="event.stopPropagation(); toggleDone(${s.idx})" title="${done[s.idx] ? 'Marcar como pendente' : 'Marcar como concluído'}">
          ${done[s.idx] ? '✓' : '○'}
        </button>
      `;
      grid.appendChild(card);
    });

    container.appendChild(section);
  });
}

function updateProgress() {
  const total = sessionData.length;
  const completed = sessionData.filter(s => done[s.idx]).length;
  const pct = total ? Math.round(completed / total * 100) : 0;
  document.getElementById('progress-fill').style.width = pct + '%';
  document.getElementById('progress-pct').textContent = `${completed} / ${total} concluídas`;
}

render();
updateProgress();
</script>

</body>
</html>
