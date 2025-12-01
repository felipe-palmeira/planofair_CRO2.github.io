# planofair_CRO2.github.io
Plano Fair
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Instituto Fair: Plano CRO 90 Dias (Landing Page)</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;900&display=swap');
        
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8fafc; /* Slate 50 */
            color: #334155; /* Slate 700 */
        }

        .chart-container {
            position: relative;
            width: 100%;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
            height: 300px;
            max-height: 400px;
        }

        @media (min-width: 768px) {
            .chart-container {
                height: 350px;
            }
        }

        .card-shadow {
            box-shadow: 0 4px 12px -1px rgba(0, 0, 0, 0.08);
        }

        .funnel-step {
            display: flex;
            align-items: center;
            padding: 12px;
            border-radius: 8px;
            margin-bottom: 12px;
            transition: all 0.2s;
        }
        .funnel-step:hover {
            transform: translateY(-2px);
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
        }

        .main-section {
            padding-top: 40px;
            padding-bottom: 40px;
            border-bottom: 1px solid #e2e8f0; /* Slate 200 */
        }
    </style>
    <!-- Chosen Palette: Clinical Focus - Slate (Neutrals), Sky Blue (Trust/CRO), Emerald (Growth/Gains), Rose (Pains/Caution) -->
    <!-- Application Structure Plan: The structure is a single, long-scrolling landing page. Content flow: 1. Header/Navigation Anchors 2. Dashboard (Vision & KPIs) 3. Roadmap (90-Day Tactical Plan) 4. Sales Playbook (Process & Objections) 5. Content Studio (Editorial Calendar & Scripts). This unified structure ensures continuous narrative flow from strategy to execution, prioritizing ease of consumption. -->
    <!-- Visualization & Content Choices: - Dashboard: Bar Chart for Funnel Conversion (Leads->Sales) and Doughnut Chart for Traffic Channel Allocation. Goal: Inform on targets and strategy focus. - Playbook: Funnel Stages (HTML/CSS Flowchart) and Interactive Accordion for Objections (addressing key Pains) including Gemini AI generator. Goal: Organize and Educate sales team. - Content Studio: Tabular/List view for 90-day plan linked to a Script Detail Pane (re-architected for side-by-side view in the scroll). Includes Gemini AI script expansion and Lead Magnet generator. - CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->
</head>
<body class="bg-slate-50 min-h-screen flex flex-col">

    <!-- Header & Navigation (Anchors for quick jump) -->
    <header class="bg-white border-b border-slate-200 sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center">
                    <span class="text-2xl font-bold text-slate-800 tracking-tight">Fair CRO <span class="text-sky-500 text-sm font-medium align-middle ml-2">90 Dias</span></span>
                </div>
                <nav class="hidden md:flex space-x-8">
                    <a href="#dashboard" class="px-3 py-2 text-sm font-medium text-slate-500 hover:text-sky-500 transition-colors">Dashboard</a>
                    <a href="#roadmap" class="px-3 py-2 text-sm font-medium text-slate-500 hover:text-sky-500 transition-colors">Roadmap</a>
                    <a href="#playbook" class="px-3 py-2 text-sm font-medium text-slate-500 hover:text-sky-500 transition-colors">Playbook</a>
                    <a href="#content" class="px-3 py-2 text-sm font-medium text-slate-500 hover:text-sky-500 transition-colors">Conteúdo</a>
                </nav>
            </div>
        </div>
        <!-- Mobile Nav: Simple anchors -->
        <div class="md:hidden bg-white border-b border-slate-200 flex justify-around py-3 text-xs">
            <a href="#dashboard" class="text-slate-600 font-semibold">Metas</a>
            <a href="#roadmap" class="text-slate-500">Roadmap</a>
            <a href="#playbook" class="text-slate-500">Vendas</a>
            <a href="#content" class="text-slate-500">Conteúdo</a>
        </div>
    </header>

    <!-- Main Content Area (Unified Scroll) -->
    <main class="flex-grow max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 w-full">

        <!-- SECTION 1: DASHBOARD & METRICS -->
        <section id="dashboard" class="main-section">
            <div class="bg-white p-6 rounded-xl card-shadow border border-slate-100">
                <h2 class="text-3xl font-bold text-slate-800 mb-2 border-b pb-2 border-sky-100">🎯 Painel de Alinhamento: Visão CRO</h2>
                <p class="text-slate-600 mb-6 max-w-4xl">
                    Esta seção alinha Marketing, Vendas e Receita. Nosso foco é a sustentabilidade, priorizando a qualidade do MQL (Marketing Qualified Lead) gerado via Orgânico e Pago. O alvo é 1000 Leads totais, convertendo em 78 Clientes de Transplante Capilar. (Ticket Médio Estimado: R$ 25.000,00).
                </p>

                <!-- KPI Cards & Revenue Projection -->
                <div class="grid grid-cols-2 md:grid-cols-5 gap-4 mb-8">
                    <!-- Card 1: LEADS (Blue) -->
                    <div class="bg-blue-100 p-4 rounded-lg border border-blue-200">
                        <div class="text-blue-700 text-xs font-semibold tracking-wider">LEADS</div>
                        <div class="text-2xl md:text-3xl font-bold text-slate-800 mt-1">1000</div>
                    </div>
                    <!-- Card 2: MQLs (Blue) -->
                    <div class="bg-blue-100 p-4 rounded-lg border border-blue-200">
                        <div class="text-blue-700 text-xs font-semibold uppercase tracking-wider">MQLs</div>
                        <div class="text-2xl md:text-3xl font-bold text-slate-800 mt-1">650</div>
                    </div>
                    <!-- Card 3: SQLs (Red) -->
                    <div class="bg-red-100 p-4 rounded-lg border border-red-200">
                        <div class="text-red-700 text-xs font-semibold uppercase tracking-wider">SQLs</div>
                        <div class="text-2xl md:text-3xl font-bold text-slate-800 mt-1">260</div>
                    </div>
                    <!-- Card 4: VENDAS (Red - Volume) -->
                    <div class="bg-red-100 p-4 rounded-lg border border-red-200">
                        <div class="text-red-700 text-xs font-semibold uppercase tracking-wider">VENDAS</div>
                        <div class="text-2xl md:text-3xl font-bold text-slate-800 mt-1">78</div>
                    </div>
                    <!-- Card 5: RECEITA (Green - Value) -->
                    <div class="bg-emerald-100 p-4 rounded-lg border border-emerald-200 col-span-2 md:col-span-1">
                        <div class="text-emerald-700 text-xs font-semibold uppercase tracking-wider">RECEITA</div>
                        <div class="text-xs font-medium text-emerald-600">TM R$ 25K</div>
                        <div class="text-2xl md:text-3xl font-bold text-slate-800 mt-1">R$ 1.95M</div>
                    </div>
                </div>

                <!-- Charts Area -->
                <div class="grid grid-cols-1 lg:grid-cols-2 gap-8">
                    <!-- Funnel Chart -->
                    <div class="bg-white p-4 rounded-lg border border-slate-100 shadow-sm">
                        <h3 class="text-lg font-semibold text-slate-700 mb-4">Funil de Conversão (KPIs de Equipe)</h3>
                        <div class="chart-container">
                            <canvas id="funnelChart"></canvas>
                        </div>
                        <p class="text-xs text-slate-400 mt-2 text-center">Taxas de Conversão Alvo: 65% (L→MQL), 40% (MQL→SQL), 30% (SQL→Venda)</p>
                    </div>

                    <!-- Channel Allocation Chart -->
                    <div class="bg-white p-4 rounded-lg border border-slate-100 shadow-sm">
                        <h3 class="text-lg font-semibold text-slate-700 mb-4">Alocação de Esforço (Aquisição)</h3>
                        <div class="chart-container">
                            <canvas id="sourceChart"></canvas>
                        </div>
                        <p class="text-xs text-slate-400 mt-2 text-center">Orgânico e Social Selling são prioridade no esforço e tempo de SDR/Closer.</p>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- SECTION 2: TACTICAL ROADMAP -->
        <section id="roadmap" class="main-section">
            <div class="bg-white p-6 rounded-xl card-shadow border border-slate-100">
                <h2 class="text-3xl font-bold text-slate-800 mb-2 border-b pb-2 border-sky-100">🗺️ Roadmap Tático de Aquisição (90 Dias)</h2>
                <p class="text-slate-600 mb-6">
                    A execução está dividida em três fases de 30 dias. A fase 1 foca na atração (TOFU), a fase 2 na nutrição (MOFU) e a fase 3 na conversão direta (BOFU) e escala, alinhando Tráfego Pago e Social Selling.
                </p>

                <!-- Phase Selectors -->
                <div class="flex space-x-2 mb-6 border-b border-slate-200">
                    <button onclick="updateRoadmap(1)" id="phase-1-btn" class="phase-btn active-phase px-4 py-2 text-sm font-semibold border-b-2 border-sky-500 text-sky-600">Dia 1-30: Fundação & Atração (TOFU)</button>
                    <button onclick="updateRoadmap(2)" id="phase-2-btn" class="phase-btn px-4 py-2 text-sm font-medium border-b-2 border-transparent text-slate-500 hover:text-sky-500">Dia 31-60: Nutrição & Autoridade (MOFU)</button>
                    <button onclick="updateRoadmap(3)" id="phase-3-btn" class="phase-btn px-4 py-2 text-sm font-medium border-b-2 border-transparent text-slate-500 hover:text-sky-500">Dia 61-90: Conversão & Escala (BOFU)</button>
                </div>

                <!-- Dynamic Content Container -->
                <div id="roadmap-content" class="grid grid-cols-1 md:grid-cols-3 gap-6">
                    <!-- Cards will be injected by JS -->
                </div>
            </div>
        </section>

        <!-- SECTION 3: SALES PLAYBOOK -->
        <section id="playbook" class="main-section">
            <div class="bg-white p-6 rounded-xl card-shadow border border-slate-100">
                <h2 class="text-3xl font-bold text-slate-800 mb-2 border-b pb-2 border-sky-100">📞 Playbook de Vendas & CRO (4 Vendedores)</h2>
                <p class="text-slate-600 mb-6">
                    O guia essencial para a equipe comercial, focando em alinhar o processo de vendas com o funil de marketing e dominar o contorno das objeções emocionais do público.
                </p>

                <div class="grid grid-cols-1 lg:grid-cols-3 gap-8">
                    
                    <!-- Left Column: Pipeline Flow & Metrics -->
                    <div class="lg:col-span-1 space-y-6">
                        <h3 class="text-xl font-bold text-slate-700 border-l-4 border-sky-500 pl-3">Fluxo do Pipeline e Metas</h3>
                        <div class="funnel-step bg-sky-50 border-l-4 border-sky-400">
                            <div><span class="text-sm font-semibold text-sky-700">1. Prospecção (Lead)</span> <span class="text-xs text-slate-500 ml-2">(1000 Volume)</span></div>
                            <div class="ml-auto text-xs font-bold text-slate-700">65% Target</div>
                        </div>
                        <div class="funnel-step bg-emerald-50 border-l-4 border-emerald-400">
                            <div><span class="text-sm font-semibold text-emerald-700">2. Qualificação (MQL)</span> <span class="text-xs text-slate-500 ml-2">(650 Volume)</span></div>
                            <div class="ml-auto text-xs font-bold text-slate-700">40% Target</div>
                        </div>
                        <div class="funnel-step bg-purple-50 border-l-4 border-purple-400">
                            <div><span class="text-sm font-semibold text-purple-700">3. Agendamento (SQL)</span> <span class="text-xs text-slate-500 ml-2">(260 Volume)</span></div>
                            <div class="ml-auto text-xs font-bold text-slate-700">30% Target</div>
                        </div>
                        <div class="funnel-step bg-yellow-50 border-l-4 border-yellow-400">
                            <div><span class="text-sm font-semibold text-yellow-700">4. Consulta / Proposta</span> <span class="text-xs text-slate-500 ml-2">(78 Volume)</span></div>
                            <div class="ml-auto text-xs font-bold text-slate-700">100% Target</div>
                        </div>
                        <div class="funnel-step bg-teal-50 border-l-4 border-teal-400">
                            <span class="text-sm font-semibold text-teal-700">5. Fechamento (Cliente)</span>
                            <div class="ml-auto text-xs font-bold text-slate-700">78 Clientes</div>
                        </div>
                        <p class="text-xs text-slate-400 pt-2">Regra de Ouro: Tempo de resposta para novos Leads - Máx. 1 Hora.</p>
                    </div>

                    <!-- Right Column: Interactive Objections & Generator -->
                    <div class="lg:col-span-2">
                        <h3 class="text-xl font-bold text-slate-700 border-l-4 border-rose-500 pl-3 mb-4">Contorno de Objeções Chave (Pains)</h3>
                        <div class="space-y-3" id="objection-list">
                            <!-- Existing Objections -->
                            <div class="border border-slate-200 rounded-lg overflow-hidden">
                                <button onclick="toggleObjection('obj-price')" class="w-full flex justify-between items-center p-4 bg-slate-50 hover:bg-slate-100 transition-colors text-left">
                                    <span class="font-medium text-slate-700">💰 "Está muito caro / Questão Financeira."</span>
                                    <span class="text-slate-400 text-xl" id="icon-obj-price">+</span>
                                </button>
                                <div id="obj-price" class="hidden p-4 bg-white border-t border-slate-200">
                                    <div class="text-xs font-bold text-rose-500 uppercase mb-2">Dor: Medo de Endividamento / Custo Incerteza</div>
                                    <p class="text-sm text-slate-600 italic mb-2">"Entendo. É um investimento na sua confiança e imagem profissional. Nosso foco é valor definitivo. Dr. Fábio tem +2.000 casos. Você prefere arriscar um retoque barato daqui a 1 ano ou garantir o resultado natural e único agora?"</p>
                                    <p class="text-sm text-slate-800 font-medium">Melhor Prática: Focar no Gasto Emocional Contínuo (Bonés) e Oferecer Plano de Parcelamento Acessível.</p>
                                </div>
                            </div>

                            <div class="border border-slate-200 rounded-lg overflow-hidden">
                                <button onclick="toggleObjection('obj-fake')" class="w-full flex justify-between items-center p-4 bg-slate-50 hover:bg-slate-100 transition-colors text-left">
                                    <span class="font-medium text-slate-700">🤡 "Tenho medo de ficar artificial / 'Cabelo de boneca'."</span>
                                    <span class="text-slate-400 text-xl" id="icon-obj-fake">+</span>
                                </button>
                                <div id="obj-fake" class="hidden p-4 bg-white border-t border-slate-200">
                                    <div class="text-xs font-bold text-rose-500 uppercase mb-2">Dor: Medo de Julgamento Social / Aparência Não Alinhada</div>
                                    <p class="text-sm text-slate-600 italic mb-2">"Isso mostra que você se preocupa com a naturalidade, assim como o Dr. Fábio! Ele é especialista em desenhar a 'Hairline' respeitando o formato único do seu rosto. Quer que eu te envie 3 exemplos de linhas frontais que NUNCA diriam que foi transplante?"</p>
                                    <p class="text-sm text-slate-800 font-medium">Melhor Prática: Prova Social Visual Imediata + Reforçar a Autoridade e a Precisão da técnica FUE.</p>
                                </div>
                            </div>

                            <div class="border border-slate-200 rounded-lg overflow-hidden">
                                <button onclick="toggleObjection('obj-time')" class="w-full flex justify-between items-center p-4 bg-slate-50 hover:bg-slate-100 transition-colors text-left">
                                    <span class="font-medium text-slate-700">🤔 "Vou pensar / Preciso de tempo."</span>
                                    <span class="text-slate-400 text-xl" id="icon-obj-time">+</span>
                                </button>
                                <div id="obj-time" class="hidden p-4 bg-white border-t border-slate-200">
                                    <div class="text-xs font-bold text-rose-500 uppercase mb-2">Dor: Ansiedade com a Decisão / Medo de Comprometimento</div>
                                    <p class="text-sm text-slate-600 italic mb-2">"É natural querer planejar. Mas, se o cabelo é importante para você, por que adiar? A única coisa que cresce com o tempo é a calvície. Temos apenas 5 vagas no próximo mês. Posso garantir a sua consulta para que você não perca o ano?"</p>
                                    <p class="text-sm text-slate-800 font-medium">Melhor Prática: Criar Escassez baseada em Agenda Real (Autoridade) + Focar no Custo da Inação (A Calvície Avança).</p>
                                </div>
                            </div>
                            <!-- End Existing Objections -->
                        </div>
                        
                        
                    </div>
                </div>
            </div>
        </section>

        <!-- SECTION 4: CONTENT STUDIO -->
        <section id="content" class="main-section">
            <h2 class="text-3xl font-bold text-slate-800 mb-6 border-b pb-2 border-sky-100 max-w-7xl mx-auto">🎬 Content Studio: Roteiros e Calendário</h2>
            <p class="text-slate-600 mb-8 max-w-4xl">
                O Content Studio operacionaliza a estratégia de Marketing, garantindo a produção diária de conteúdo (5 Reels/sem, 2 Carrosséis/sem, 5 Stories/dia) alinhada ao funil TOFU, MOFU e BOFU.
            </p>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 h-auto">
                
                <!-- Left: Calendar Navigation -->
                <div class="lg:col-span-5 bg-white p-6 rounded-xl card-shadow border border-slate-100 flex flex-col">
                    <h3 class="text-xl font-bold text-slate-800 mb-2">Calendário Editorial</h3>
                    <p class="text-sm text-slate-500 mb-4">Selecione um dia para ver o roteiro completo. (90 dias / 13 semanas)</p>
                    
                    <!-- WEEK SELECTOR (13 BUTTONS) -->
                    <div class="mb-4 border-b pb-2 border-slate-100 overflow-x-auto">
                        <div id="week-selector-container" class="flex flex-nowrap space-x-1" style="min-width: 600px;">
                            <!-- Buttons for Week 1 to 13 will be injected by JS -->
                        </div>
                    </div>

                    <div id="calendar-list" class="space-y-2 flex-grow pr-2">
                        <!-- Javascript populates list here -->
                    </div>
                </div>

                <!-- Right: Script Detail View - Moves to its own row on small screens, or remains right on large -->
                <div class="lg:col-span-7 bg-white p-6 rounded-xl card-shadow border border-slate-100 flex flex-col mt-6 lg:mt-0">
                    <div id="script-empty-state" class="flex flex-col items-center justify-center h-full text-slate-400">
                        <span class="text-4xl mb-2">📝</span>
                        <p>Selecione um conteúdo do calendário para ver a estrutura completa do roteiro (Reel de 60s).</p>
                    </div>

                    <div id="script-detail" class="hidden flex-col h-full">
                        <div class="flex justify-between items-start mb-4 pb-4 border-b border-slate-100">
                            <div>
                                <span id="script-funnel" class="px-2 py-1 rounded text-xs font-bold bg-slate-200 text-slate-700 uppercase tracking-wide">TOFU</span>
                                <span id="script-format" class="ml-2 px-2 py-1 rounded text-xs font-bold bg-indigo-100 text-indigo-700 uppercase tracking-wide">REEL</span>
                                <h3 id="script-title" class="text-xl font-bold text-slate-800 mt-2">Título do Conteúdo</h3>
                            </div>
                            <div class="text-right">
                                <div class="text-xs text-slate-400 uppercase">Foco | Tipo</div>
                                <div id="script-type" class="text-sm font-medium text-slate-700">Doação | Levantada de Mão</div>
                            </div>
                        </div>

                        <div class="flex-grow pr-4 space-y-6">
                            
                            <!-- Hook & Headline -->
                            <div class="bg-rose-50 p-4 rounded-lg border-l-4 border-rose-400">
                                <h4 class="text-xs font-bold text-rose-700 uppercase mb-1">🎣 Ganchos Sugeridos (0-3s)</h4>
                                <ul id="script-hooks" class="text-slate-800 font-medium list-disc ml-4"></ul>
                                <h4 class="text-xs font-bold text-slate-400 uppercase mt-3 mb-1">✍️ Headline</h4>
                                <p id="script-headline" class="text-slate-800 font-medium"></p>
                            </div>

                            <!-- Development & Climax -->
                            <div id="detailed-script-content">
                                <h4 class="text-xs font-bold text-slate-400 uppercase mb-2">📹 Estrutura do Roteiro (60s)</h4>
                                <div class="space-y-3">
                                    <p class="text-sm text-slate-800"><span class="font-bold text-sky-600">3-15s (Dor/Problema):</span> <span id="script-desenvolvimento">Conteúdo do roteiro...</span></p>
                                    <p class="text-sm text-slate-800"><span class="font-bold text-emerald-600">30-45s (Solução/Autoridade):</span> <span id="script-solucao">Conteúdo da solução...</span></p>
                                    <p class="text-sm text-slate-800 bg-yellow-50 p-2 rounded-md"><span class="font-bold text-yellow-700">45-55s (Climax UAU):</span> <span id="script-climax">Conteúdo do Climax...</span></p>
                                </div>
                            </div>

                            <!-- GEMINI FEATURE: SCRIPT EXPANSION -->
                            <div class="pt-4 border-t border-sky-100">
                                <button onclick="expandContentScript()" id="expand-script-btn" class="w-full bg-indigo-500 text-white font-semibold py-2 rounded-lg hover:bg-indigo-600 transition-colors flex items-center justify-center">
                                    <span id="expand-btn-text">✨ Expandir Roteiro Detalhado (IA)</span>
                                    <span id="expand-loader" class="hidden ml-2 h-4 w-4 border-2 border-white border-t-transparent rounded-full animate-spin"></span>
                                </button>
                                <div id="expand-response-area" class="mt-2 text-xs text-slate-500">Clique para gerar um roteiro de 60s pronto para gravação com narração e cenas detalhadas.</div>
                            </div>

                            <!-- CTA -->
                            <div class="bg-teal-50 p-4 rounded-lg border border-teal-100">
                                <h4 class="text-xs font-bold text-teal-700 uppercase mb-1">🚀 Chamada para Ação (3 Opções)</h4>
                                <ul id="script-ctas" class="text-slate-800 font-semibold list-disc ml-4"></ul>
                                <div class="text-xs text-teal-600 mt-2 italic">Automação DM: Palavra-Chave: <span class="font-bold text-sm" id="script-keyword">PALAVRA-CHAVE</span></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-white border-t border-slate-200 py-6 mt-auto">
        <div class="max-w-7xl mx-auto px-4 text-center text-slate-400 text-sm">
            <p>Instituto Fair - Estratégia de Crescimento Integrada (CRO). 2025</p>
        </div>
    </footer>


    <!-- JAVASCRIPT LOGIC -->
    <script>
        // --- DATA STORAGE ---
        const API_KEY = ""; 
        const API_URL = "https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash-preview-09-2025:generateContent?key=" + API_KEY;

        let currentScript = null; 

        // COLOR PALETTE FOR WEEK BUTTONS (13 DISTINCT COLORS) - MONOCHROMATIC BLUE
        const WEEK_COLORS = [
            { bg: 'bg-blue-600', active: 'bg-blue-700' }, 
            { bg: 'bg-sky-600', active: 'bg-sky-700' }, 
            { bg: 'bg-blue-500', active: 'bg-blue-600' }, 
            { bg: 'bg-sky-500', active: 'bg-sky-600' }, 
            { bg: 'bg-blue-400', active: 'bg-blue-500' }, 
            { bg: 'bg-sky-400', active: 'bg-sky-500' }, 
            { bg: 'bg-blue-500', active: 'bg-blue-600' }, 
            { bg: 'bg-sky-500', active: 'bg-sky-600' }, 
            { bg: 'bg-blue-600', active: 'bg-blue-700' }, 
            { bg: 'bg-sky-600', active: 'bg-sky-700' }, 
            { bg: 'bg-blue-700', active: 'bg-blue-800' }, 
            { bg: 'bg-sky-700', active: 'bg-sky-800' }, 
            { bg: 'bg-blue-800', active: 'bg-blue-900' }, 
        ];


        // Funnel & Revenue Data (Recalculado para 78 Vendas)
        const metrics = {
            leads: 1000,
            mql: 650,
            sql: 260, // 40% of 650
            deals: 78, // 30% of 260
            revenue: 1950000 // 78 * 25000
        };

        // Roadmap Data
        const roadmapData = {
            1: [
                { title: "Função: TOFU & Atração", icon: "🌱", desc: "Criação de 3 iscas digitais (e-Books, Planilha Custo). 100% dos Reels/Carrosséis TOFU na Semana 1. Foco em distribuição PAGA (tráfego) dos conteúdos de atração." },
                { title: "Função: Qualificação SDR", icon: "📞", desc: "Treinamento intensivo da equipe de 4 SDRs/Closers nos scripts de Social Selling. Regra de 1 hora no primeiro contato." },
                { title: "Função: SEO Local", icon: "📍", desc: "Otimização de 5 páginas para SEO Local (Minas Gerais). Criação de 5 Blog Posts TOFU (Mitos, Curiosidades)." }
            ],
            2: [
                { title: "Função: MOFU & Nutrição", icon: "💡", desc: "Lançamento de 2 Webinars educativos/Estudos de Caso (exclusivos para Leads). Conteúdos focados em Depoimentos e Autoridade do Dr. Fábio (MOFU)." },
                { title: "Função: Automação DM", icon: "🤖", desc: "Implementação de Automação de DM (palavras-chave) para qualificação e envio de materiais (e.g., Checklist)." },
                { title: "Função: Otimização Conversão", icon: "🛠️", desc: "Teste A/B de 5 Headlines de Reels. Otimização das Landing Pages das Iscas Digitais para maior MQL." }
            ],
            3: [
                { title: "Função: BOFU & Fechamento", icon: "💰", desc: "Criação de oferta de escassez (Vagas limitadas) e de urgência (Bônus). 80% dos conteúdos BOFU (CTA para agendamento)." },
                { title: "Função: Pipeline Management", icon: "📊", desc: "Revisão semanal do Pipeline de Vendas com Closers. Foco em Objeções de Preço e Tempo (Gatilho de Perda)." },
                { title: "Função: Indicação Estratégica", icon: "🤝", desc: "Ativação de programa de indicação de clientes satisfeitos (Ganhos: Autoestima, Orgulho)." }
            ]
        };

        // Content Calendar Data (Extending up to Week 13)
        const contentScripts = [
            // SEMANA 1 (TOFU Pesado & Prospecção) - EXISTING DATA
            { week: 1, day: "Seg 1", format: "REEL", funnel: "TOFU", type: "Doação", theme: "O Custo Silencioso da Calvície", 
                hooks: ["O espelho mente, a foto não.", "Pare de usar boné. Você não precisa.", "O que a calvície diz sobre você."], 
                headline: "O Custo Silencioso da Calvície que Ninguém Vê", 
                desenvolvimento: "3-15s: Apresentação da Dor (Vergonha, Insegurança, Medo de parecer mais velho). 15-30s: Explicação da Raiz do Problema (Genética e o avanço).", 
                solucao: "30-45s: Solução Rápida (Não é produto, é diagnóstico preciso do Dr. Fábio).",
                climax: "45-55s: Seu cabelo novo, desenhado para o seu rosto. Você não precisa se esconder mais.",
                ctas: [
                    "CTA 1: Digite 'GUIA' e receba o PDF.", 
                    "CTA 2: Link na Bio: Guia para Começar.", 
                    "CTA 3: Compartilhe com quem usa boné todo dia."
                ], keyword: "GUIA" 
            },
            { week: 1, day: "Ter 1", format: "STORIES", funnel: "TOFU", type: "Engajamento", hooks: [], headline: "Quiz: Aparência", desenvolvimento: "Caixa de perguntas: Qual sua maior dor capilar? Enquete: Calvície te faz parecer mais velho? (Sim/Não).", solucao: "", climax: "", ctas: ["Interaja nas caixinhas"], keyword: "N/A" },
            { week: 1, day: "Qua 1", format: "CARROSSEL", funnel: "TOFU", type: "Doação", theme: "5 Mitos do Transplante", 
                hooks: ["O que não te contaram sobre FUE.", "Calvície tem cura? (Sim/Não)."], 
                headline: "5 Mitos e 5 Fatos que Vão Mudar sua Visão sobre Transplante", 
                desenvolvimento: "Slide 1: Artificialidade. Slide 2: Dor. Slide 3: Custo. Slide 4: Fio de Boneca. Slide 5: Cresce de novo?", 
                solucao: "Slide 6: Fato: Com a Fair, o resultado é natural.",
                climax: "(Final Slide) A ciência real por trás dos resultados de excelência.",
                ctas: [
                    "CTA 1: Digite 'MITOS' e receba o Guia Completo.", 
                    "CTA 2: Salve para consultar depois.", 
                    "CTA 3: Link na Bio para o Guia."
                ], keyword: "MITOS" 
            },
            { week: 1, day: "Qui 1", format: "REEL", funnel: "MOFU", type: "Levantada de Mão", theme: "Linha Frontal Natural é Arte", 
                hooks: ["O detalhe que te entrega.", "O segredo para parecer 10 anos mais jovem.", "Linha frontal 'cabelo de boneca' NUNCA."], 
                headline: "A Arte e Ciência da Linha Frontal Perfeita (Não é Milagre)", 
                desenvolvimento: "3-15s: Mostra o resultado 'UAU' (Natural, denso, sem aparência de cirurgia). 15-30s: O que é preciso para chegar nesse nível de naturalidade.", 
                solucao: "30-45s: Explicação técnica (ângulo, densidade, FUE avançado) - Foco no Dr. Fábio, autoridade com +2000 casos.",
                climax: "45-55s: Seu cabelo novo, desenhado para o seu rosto. Resultado que te devolve a identidade.",
                ctas: [
                    "CTA 1: Digite 'AGENDA' e fale com especialista.", 
                    "CTA 2: Agende sua Consulta de Avaliação.", 
                    "CTA 3: Link na Bio: Fale Conosco."
                ], keyword: "AGENDA" 
            },
            { week: 1, day: "Sex 1", format: "REEL", funnel: "TOFU", type: "Doação", theme: "Checklist Pré-Transplante", 
                hooks: ["3 coisas para fazer antes do Transplante.", "Você está pronto? Não cometa este erro.", "Evite o arrependimento: O Guia de Preparação."], 
                headline: "Checklist de Preparação Rápida para o Seu Transplante Capilar", 
                desenvolvimento: "3-15s: Apresentação da Dor (medo de complicação/incerteza). 15-40s: 5 Passos cruciais de preparação (Hidratação, Exames, Corte).", 
                solucao: "40-55s: O checklist completo com 15 itens essenciais para você se sentir 100% seguro.",
                climax: "Garanta que seu procedimento seja um sucesso total com este guia.",
                ctas: [
                    "CTA 1: Digite 'CHECKLIST' e receba o PDF.", 
                    "CTA 2: Baixe o PDF de Preparação Agora.", 
                    "CTA 3: Salve para antes da sua cirurgia."
                ], keyword: "CHECKLIST" 
            },
            { week: 1, day: "Sáb 1", format: "CARROSSEL", funnel: "MOFU", type: "Levantada de Mão", theme: "A Profundidade do FUE", 
                hooks: ["O que é FUE, de verdade.", "A técnica que garante zero cicatriz.", "Não é milagre, é FUE."], 
                headline: "Técnica FUE: O Passo a Passo que Garante Resultados Naturais (Zero Cicatriz)", 
                desenvolvimento: "Slide 1: Diferença FUE vs. FUT. Slide 2: Extração unitária. Slide 3: Implantação com precisão. Slide 4: O papel da equipe (4 vendedores, 2 enfermeiras).", 
                solucao: "Slide 5: Foco na área doadora: 0 cicatriz aparente.",
                climax: "(Final Slide) O padrão ouro de transplante que devolve a liberdade do cabelo curto.",
                ctas: [
                    "CTA 1: Digite 'FUE' e receba a ficha técnica.", 
                    "CTA 2: Fale com nosso especialista FUE.", 
                    "CTA 3: Link direto para contato."
                ], keyword: "FUE" 
            },
            { week: 1, day: "Dom 1", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Medo de Agulha (Zero Dor)", 
                hooks: ["Medo de agulha? A única dor que você terá é a da espera.", "ZERO DOR: O Protocolo de Conforto.", "O que acontece antes de tudo."], 
                headline: "Protocolo ZERO DOR: Não Perca Mais Tempo por Medo", 
                desenvolvimento: "3-15s: Desmistificando a dor (anestesia local, sedação leve). 15-30s: Foco no conforto do paciente e no ambiente acolhedor da clínica.", 
                solucao: "30-45s: Apresentação da equipe de anestesia (autoridade/segurança).",
                climax: "45-55s: Seu maior medo não é a dor, é o arrependimento de não ter começado antes. Dê o primeiro passo.",
                ctas: [
                    "CTA 1: Digite 'CONFORTO' e agende.", 
                    "CTA 2: Fale com a equipe e tire o medo.", 
                    "CTA 3: Garanta sua consulta."
                ], keyword: "CONFORTO" 
            },

            // SEMANA 2 (MOFU e BOFU) - EXISTING DATA
            { week: 2, day: "Seg 2", format: "REEL", funnel: "MOFU", type: "Levantada de Mão", theme: "Por que 2000 Casos Importam?", 
                hooks: ["A verdade que nenhuma clínica barata te conta.", "Por que o número 2000 faz toda a diferença.", "O que a experiência do seu médico revela."], 
                headline: "2000 Casos: O Nível de Experiência que Garante Seu Resultado", 
                desenvolvimento: "3-15s: Problema (Clínicas novas/baratas = risco). 15-30s: Autoridade (Dr. Fábio: +2000 procedimentos). Diferencial em 5 clínicas em MG.", 
                solucao: "30-45s: O que 2000 procedimentos ensinam: mapear o doador, desenhar linhas frontais únicas e gerenciar expectativas.",
                climax: "45-55s: Segurança não tem preço. Invista na experiência que te devolve a confiança.",
                ctas: [
                    "CTA 1: Digite 'EXPERIÊNCIA' e agende.", 
                    "CTA 2: Agende com quem realmente entende.", 
                    "CTA 3: Confira nossos cases."
                ], keyword: "EXPERIENCIA" 
            },
            { week: 2, day: "Ter 2", format: "STORIES", funnel: "MOFU", type: "Engajamento", theme: "Bastidores e Segurança", hooks: [], headline: "Por dentro da Sala Cirúrgica", desenvolvimento: "Quiz: Qual o nível de esterilização? (Altíssimo). Vídeos curtos do Dr. Fábio explicando o processo de segurança.", solucao: "", climax: "", ctas: ["Reaja com 🔥 se sentiu seguro"], keyword: "N/A" },
            { week: 2, day: "Qua 2", format: "CARROSSEL", funnel: "MOFU", type: "Doação", theme: "As 4 Fases do Cabelo Novo", 
                hooks: ["Não é mágica, é ciência.", "O que te espera após a cirurgia.", "4 fases para o cabelo novo."], 
                headline: "As 4 Fases do Crescimento Pós-Transplante (A Ciência do Cabelo Novo)", 
                desenvolvimento: "Slide 1: Dia 1-15: Recuperação e Pós-Op. Slide 2: Shedding (Queda, A Calmaria). Slide 3: O Pulo do Gato (4-8 meses: O Crescimento). Slide 4: O Resultado Final.", 
                solucao: "Slide 5: O que você pode esperar em cada fase.",
                climax: "(Final Slide) Saiba exatamente quando o resultado final vai chegar (12-18 meses).",
                ctas: [
                    "CTA 1: Digite 'FASES' para baixar o Guia.", 
                    "CTA 2: Guia Completo no Link da Bio.", 
                    "CTA 3: Compartilhe este guia com quem está indeciso."
                ], keyword: "FASES" 
            },
            { week: 2, day: "Qui 2", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Custo da Inação (Boné)", 
                hooks: ["O custo de continuar usando boné.", "Não deixe sua calvície avançar.", "Quanto tempo você já perdeu?"], 
                headline: "O Maior Custo Não é o Transplante, é a Inação", 
                desenvolvimento: "3-15s: Foco na dor emocional (perda de oportunidades, autoestima despencando, vergonha). 15-30s: Explica o processo de avanço da calvície (piora da área doadora).", 
                solucao: "30-45s: Hoje é o melhor dia para começar. Dr. Fábio pode te ajudar a parar o processo.",
                climax: "45-55s: Devolva a si mesmo o prazer de se olhar no espelho. Não há tempo a perder.",
                ctas: [
                    "CTA 1: Digite 'AGORA' e agende sua Consulta.", 
                    "CTA 2: Não perca mais tempo, agende já.", 
                    "CTA 3: Fale com nossa equipe."
                ], keyword: "AGORA" 
            },
            { week: 2, day: "Sex 2", format: "REEL", funnel: "MOFU", type: "Doação", theme: "Solucionando o Shedding", 
                hooks: ["A fase que todos se desesperam.", "Vai cair de novo? Entenda.", "O que é Shedding (e por que é bom)."], 
                headline: "Shedding: Por que a Queda é Sinal de que Seu Cabelo Vai Crescer Forte!", 
                desenvolvimento: "3-15s: Apresenta o pânico do paciente com a queda inicial. 15-30s: Explica a ciência por trás do shedding (troca de folículo, ciclo capilar).", 
                solucao: "30-45s: É um sinal de que a cirurgia deu certo. Oferece guia de cuidados para esta fase.",
                climax: "45-55s: Calma! É normal, e a Fair te guia. Sua ansiedade termina com informação.",
                ctas: [
                    "CTA 1: Digite 'SHEDDING' e receba o Guia.", 
                    "CTA 2: Guia de Sobrevivência ao Shedding.", 
                    "CTA 3: Fale com a equipe sobre esta fase."
                ], keyword: "SHEDDING" 
            },
            { week: 2, day: "Sáb 2", format: "CARROSSEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Comparativo de Clínicas", 
                hooks: ["Clínica barata vs. Instituto Fair.", "O que observar antes de fechar.", "A tabela que te salva do arrependimento."], 
                headline: "Tabela Comparativa: Risco vs. Recompensa (Dr. Fábio Freitas)", 
                desenvolvimento: "Slide 1: Preço baixo = Risco, Falta de Experiência. Slide 2: Fair = +2000 Casos, Equipe Completa, 5 Clínicas. Slide 3: Anestesia/Dor. Slide 4: Naturalidade (Hairline).", 
                solucao: "Slide 5: O foco da Fair é o resultado que te dá orgulho.",
                climax: "(Final Slide) Escolha com a Razão, Feche com a Confiança.",
                ctas: [
                    "CTA 1: Digite 'COMPARE' e agende sua consulta.", 
                    "CTA 2: Fale com especialista.", 
                    "CTA 3: Garantia de Resultado: Fale com o time."
                ], keyword: "COMPARE" 
            },
            { week: 2, day: "Dom 2", format: "REEL", funnel: "TOFU", type: "Doação", theme: "Tipos de Calvície", 
                hooks: ["Qual seu tipo de calvície?", "Entenda o que está acontecendo.", "Você não está sozinho."], 
                headline: "Tipos Comuns de Calvície: Identifique o Seu e o Tratamento Certo", 
                desenvolvimento: "3-15s: Apresenta os 3-4 tipos de calvície (Androgenética, Alopecia Areata). 15-30s: Explica o que o Dr. Fábio avalia no diagnóstico (Área Doadora, Tipo de Queda).", 
                solucao: "30-45s: A solução é personalizada. Não existe 'uma' técnica para todos. Descubra o seu plano.",
                climax: "45-55s: O diagnóstico é o primeiro passo para a sua transformação. Comece pela informação.",
                ctas: [
                    "CTA 1: Digite 'DIAG' e receba a Tabela.", 
                    "CTA 2: Guia de Tipos de Calvície no Link.", 
                    "CTA 3: Marque quem precisa desse guia."
                ], keyword: "DIAG" 
            },

            // SEMANA 3 (MOFU - Foco em Autoridade e Processo)
            { week: 3, day: "Seg 3", format: "REEL", funnel: "MOFU", type: "Levantada de Mão", theme: "Consulta de Avaliação: O Que Ninguém Te Conta", hooks: ["O que acontece antes de tudo...", "O segredo de uma avaliação precisa.", "Sua chance de ter um plano único."], headline: "Sua Avaliação com o Dr. Fábio: Pare de Chutar o Diagnóstico", desenvolvimento: "Foco no processo de avaliação: mapeamento 3D, análise doadora.", solucao: "Você sai com um plano personalizado e preço fechado, sem surpresas.", climax: "A única forma de ter um resultado natural é começar com a avaliação certa.", ctas: [
                "CTA 1: Digite 'AVALIAÇÃO' e agende a sua.", 
                "CTA 2: Fale com a equipe.", 
                "CTA 3: Link na Bio: Agende Agora."
            ], keyword: "AVALIACAO" },
            { week: 3, day: "Ter 3", format: "STORIES", funnel: "MOFU", type: "Engajamento", theme: "Por Que FUE é Melhor?", hooks: [], headline: "FUT vs FUE: Vote na Enquete", desenvolvimento: "Enquete sobre preferência de técnica. Dr. Fábio responde os prós e contras.", solucao: "", climax: "", ctas: ["Vote e descubra a diferença"], keyword: "N/A" },
            { week: 3, day: "Qua 3", format: "CARROSSEL", funnel: "MOFU", type: "Doação", theme: "Dúvidas Pós-Operatórias", hooks: ["Guia para as primeiras 48h.", "Como lavar o cabelo (o jeito certo)."], headline: "Dúvidas de Pós-Operatório Resolvidas (Primeiros 7 Dias)", desenvolvimento: "Passo a passo da lavagem, cuidados com o sol e restrições de atividade física.", solucao: "Seu Guia completo para uma recuperação tranquila.", climax: "Recupere-se em tempo recorde seguindo o método Fair.", ctas: [
                "CTA 1: Digite 'PÓSOP' para receber o guia.", 
                "CTA 2: Link na Bio: PDF Grátis.", 
                "CTA 3: Compartilhe com quem vai operar em breve."
            ], keyword: "POSOP" },
            { week: 3, day: "Qui 3", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Medo da Cicatriz na Nuca", hooks: ["A cicatriz que te impede de usar cabelo curto.", "FUE: O fim da cicatriz aparente.", "O que o Dr. Fábio faz diferente."], headline: "Como Garantimos ZERO Cicatriz Aparente com o FUE", desenvolvimento: "Mostra zoom in na área doadora com FUE vs. FUT (antigo). Foco na extração e fechamento da Fair.", solucao: "Resultado natural e a liberdade de usar o cabelo como quiser.", climax: "A cicatriz é opcional. Escolha o método certo.", ctas: [
                "CTA 1: Digite 'FUE' e agende.", 
                "CTA 2: Fale com especialista.", 
                "CTA 3: Garantia de Cicatriz Mínima."
            ], keyword: "FUE" },
            { week: 3, day: "Sex 3", format: "REEL", funnel: "MOFU", type: "Levantada de Mão", theme: "O que é MQL para Transplante?", hooks: ["Quem está pronto para avançar?", "Você é um MQL? Teste rápido."], headline: "O Ponto de Virada: O Que te Torna um Candidato IDEAL (MQL)", desenvolvimento: "Explica que MQL é quem já tem dor, já pesquisou e precisa de credibilidade. Não é mais sobre o 'quê', mas sobre o 'quem'.", solucao: "Se você se identifica, está pronto para falar com o Dr. Fábio.", climax: "Perca o medo, não o cabelo. Estamos prontos para te receber.", ctas: [
                "CTA 1: Digite 'AVANÇAR' para falar com o time.", 
                "CTA 2: Link na Bio: MQL Ready.", 
                "CTA 3: Clique se você é um MQL."
            ], keyword: "AVANCAR" },
            { week: 3, day: "Sáb 3", format: "CARROSSEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Opções de Parcelamento", hooks: ["Seu sonho é mais acessível do que pensa.", "Como fazer caber no seu orçamento."], headline: "Plano Financeiro: Como Parcelar Seu Transplante (Opções Fair)", desenvolvimento: "Apresenta as opções de pagamento (cartão, boleto, financiamento) de forma clara e simples.", solucao: "O investimento na autoestima é possível hoje.", climax: "Planeje-se financeiramente e comece a contagem regressiva.", ctas: [
                "CTA 1: Digite 'CUSTO' e peça uma simulação.", 
                "CTA 2: Simule o Parcelamento Aqui.", 
                "CTA 3: Fale sobre opções de financiamento."
            ], keyword: "CUSTO" },
            { week: 3, day: "Dom 3", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Prova Social de Rejuvenescimento", hooks: ["O segredo para parecer 10 anos mais jovem.", "Autoestima não tem preço.", "De volta ao espelho."], headline: "O Efeito Rejuvenescedor do Transplante Capilar (Depoimento)", desenvolvimento: "Foco no ganho emocional: cliente fala sobre se sentir mais jovem, confiante em reuniões. Cenas de antes/depois focadas no rosto. Governo.", solucao: "Recuperar o cabelo é recuperar o tempo.", climax: "Sua melhor versão está a apenas uma decisão de distância.", ctas: [
                "CTA 1: Digite 'MUDAR' e agende.", 
                "CTA 2: Fale com a equipe.", 
                "CTA 3: Link direto para agendamento."
            ], keyword: "MUDAR" },

            // SEMANA 4 (MOFU/BOFU - Foco em Superar Objeções e Casos Reais)
            { week: 4, day: "Seg 4", format: "REEL", funnel: "MOFU", type: "Doação", theme: "O Papel da Área Doadora", hooks: ["De onde vem o cabelo novo?", "A regra de ouro da área doadora.", "Por que o seu transplante é limitado."], headline: "A Área Doadora é o Segredo (e a Limitação) do Seu Transplante", desenvolvimento: "Explica a importância da área doadora e por que é fundamental ter um bom diagnóstico.", solucao: "Guia sobre como maximizar a área doadora existente.", climax: "A avaliação correta preserva seus folículos.", ctas: [
                "CTA 1: Digite 'DOADOR' e receba o guia.", 
                "CTA 2: Baixe o PDF Fair.", 
                "CTA 3: Entenda a importância do doador."
            ], keyword: "DOADOR" },
            { week: 4, day: "Ter 4", format: "STORIES", funnel: "MOFU", type: "Engajamento", theme: "Dúvidas sobre o Dr. Fábio", hooks: [], headline: "Caixinha de Perguntas: Dr. Fábio", desenvolvimento: "Caixa de perguntas com foco em experiência, tempo de carreira e número de clínicas.", solucao: "", climax: "", ctas: ["Mande sua pergunta"], keyword: "N/A" },
            { week: 4, day: "Qua 4", format: "CARROSSEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Comparativo: Valor da Fair vs. Clínicas Baratas", hooks: ["Preço x Custo-Benefício.", "A diferença entre um bom e um mau resultado."], headline: "O Que o Preço da Fair Inclui (e o que você perde no barato)", desenvolvimento: "Compara itens: Experiência do Médico, Equipe Própria, Pós-Operatório Acompanhado, Protocolo Zero Dor.", solucao: "O barato sai caro. O investimento na Fair é garantia de satisfação.", climax: "Priorize a segurança e a naturalidade.", ctas: [
                "CTA 1: Digite 'VALOR' para entender o investimento.", 
                "CTA 2: Fale com nosso time.", 
                "CTA 3: Peça a Tabela de Comparação."
            ], keyword: "VALOR" },
            { week: 4, day: "Qui 4", format: "REEL", funnel: "MOFU", type: "Doação", theme: "Queda de Cabelo Inicial", hooks: ["O grande erro ao tratar a calvície.", "Remédios que não funcionam mais.", "A verdade sobre loções."], headline: "Remédios e Loções: Quando é Hora de Parar e Agir de Verdade", desenvolvimento: "Revisa os tratamentos não-cirúrgicos e o momento em que se tornam ineficazes.", solucao: "O transplante é a solução definitiva quando o folículo morre.", climax: "Não perca mais dinheiro com promessas. Invista na ciência.", ctas: [
                "CTA 1: Digite 'PARE' e receba o guia de quando parar.", 
                "CTA 2: Link na Bio: Guia de Transição.", 
                "CTA 3: Marque um amigo que ainda usa Minoxidil."
            ], keyword: "PARE" },
            { week: 4, day: "Sex 4", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Depoimento de Homem (Calvície Avançada)", hooks: ["De volta à juventude.", "O resultado que chocou os amigos.", "Transformação total."], headline: "A Transformação Total na Calvície Avançada (Case Real)", desenvolvimento: "Depoimento focado no GANHO: retomada da vida social e profissional. Cenas de antes/depois focadas no rosto. Demonstra a densidade do resultado final.", solucao: "O Instituto Fair tem solução mesmo para casos avançados.", climax: "O limite da calvície é o início da Fair.", ctas: [
                "CTA 1: Digite 'CASE' para ver o vídeo completo.", 
                "CTA 2: Agende sua avaliação avançada.", 
                "CTA 3: Peça um Antes/Depois pelo Direct."
            ], keyword: "CASE" },
            { week: 4, day: "Sáb 4", format: "CARROSSEL", funnel: "MOFU", type: "Levantada de Mão", theme: "O que o FUE Avançado da Fair Faz", hooks: ["FUE: O que mudou nos últimos 5 anos.", "O segredo da densidade Fair.", "Não é o mesmo FUE que você conhece."], headline: "O FUE Avançado do Dr. Fábio: Tecnologia e Precisão (5 Vantagens)", desenvolvimento: "Detalha as vantagens do FUE feito na Fair: menos tempo, mais folículos viáveis, melhor angulação.", solucao: "A precisão da Fair garante que cada folículo conte.", climax: "Maximizando o potencial do seu doador.", ctas: [
                "CTA 1: Digite 'VANTAGEM' e agende sua consulta.", 
                "CTA 2: Fale com especialista.", 
                "CTA 3: Entenda a diferença do nosso FUE."
            ], keyword: "VANTAGEM" },
            { week: 4, day: "Dom 4", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Escassez: Últimas Vagas do Mês", hooks: ["Atenção: A agenda está fechando!", "Não adie mais o seu sonho.", "Vagas limitadas."], headline: "ÚLTIMAS VAGAS DE AVALIAÇÃO COM DR. FÁBIO ESTE MÊS", desenvolvimento: "Mensagem de urgência: A agenda de cirurgia é limitada para garantir a qualidade. Cria escassez real.", solucao: "Garanta a sua vaga antes que feche para o próximo trimestre.", climax: "A decisão é sua, a oportunidade é agora.", ctas: [
                "CTA 1: Digite 'VAGA' e reserve seu horário.", 
                "CTA 2: Agende a ÚLTIMA vaga.", 
                "CTA 3: Link direto para checkout."
            ], keyword: "VAGA" },

            // SEMANA 5 (MOFU/BOFU - Foco em Medo de Artificialidade e Rotina)
            { week: 5, day: "Seg 5", format: "REEL", funnel: "MOFU", type: "Doação", theme: "O período de Shedding (Queda) - Normalizando o Medo", hooks: ["A fase que todos se desesperam.", "Vai cair de novo? Entenda.", "Por que a queda é o sinal de que deu certo."], headline: "Shedding: Por que é um BOM Sinal (e como sobreviver ao 3º mês)", desenvolvimento: "Explicação didática sobre o Shedding: é a troca do fio, não a perda do folículo.", solucao: "O guia da Fair para gerenciar a ansiedade.", climax: "Paciência e informação são a chave.", ctas: [
                "CTA 1: Digite 'SHEDDING' e receba o PDF.", 
                "CTA 2: Guia de Sobrevivência ao Shedding.", 
                "CTA 3: Fale com a equipe sobre esta fase."
            ], keyword: "SHEDDING" },
            { week: 5, day: "Ter 5", format: "STORIES", funnel: "MOFU", type: "Engajamento", theme: "Rotina Pós-Operatória", hooks: [], headline: "Rotina de 1º dia", desenvolvimento: "Perguntas e respostas sobre dormir, comer, dirigir, trabalhar após a cirurgia.", solucao: "", climax: "", ctas: ["Responda na caixinha"], keyword: "N/A" },
            { week: 5, day: "Qua 5", format: "CARROSSEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Garantia de Naturalidade", hooks: ["A garantia mais importante.", "Resultado artificial? NUNCA mais.", "O que é Hairline Perfeita."], headline: "Hairline Perfeita: O Padrão Ouro de Naturalidade do Dr. Fábio", desenvolvimento: "Mostra 4 exemplos de linhas frontais criadas pela Fair, focando na angulação e densidade.", solucao: "A garantia de que ninguém vai notar a cirurgia, apenas o cabelo.", climax: "Sua aparência final é nossa prioridade.", ctas: [
                "CTA 1: Digite 'GARANTIA' e fale com especialista.", 
                "CTA 2: Agende sua Consulta Foco em Hairline.", 
                "CTA 3: Peça para ver mais fotos de antes/depois."
            ], keyword: "GARANTIA" },
            { week: 5, day: "Qui 5", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Custo-Benefício: O Retoque Caro", hooks: ["O perigo do transplante barato.", "O custo de um retoque.", "Não faça duas vezes!"], headline: "O Custo de um Transplante Mal Feito: Por Que o Retoque é Tão Caro", desenvolvimento: "Explica que um transplante mal feito não só desperdiça dinheiro, mas também folículos doadores limitados.", solucao: "O investimento na Fair é único e definitivo.", climax: "Pague o preço justo pela tranquilidade e pelo resultado certo.", ctas: [
                "CTA 1: Digite 'PREVENÇÃO' e agende a primeira vez certa.", 
                "CTA 2: Fale com o time Fair.", 
                "CTA 3: Calcule o risco de um transplante barato."
            ], keyword: "PREVENCAO" },
            { week: 5, day: "Sex 5", format: "REEL", funnel: "MOFU", type: "Doação", theme: "Idade Certa para o Transplante", hooks: ["Existe idade certa?", "O que o médico realmente avalia.", "Não espere demais."], headline: "Qual a Idade Certa para o Transplante Capilar (E quando não é hora)", desenvolvimento: "Desmistifica a idade: foca na estabilidade da calvície e na qualidade da área doadora. Explica que a calvície avançando pode reduzir as opções.", solucao: "A avaliação do Dr. Fábio define o melhor timing para o seu caso.", climax: "Planeamento é crucial.", ctas: [
                "CTA 1: Digite 'IDADE' e receba o Guia de Timing.", 
                "CTA 2: Link na Bio: Guia de Planejamento.", 
                "CTA 3: Fale com um consultor sobre o seu caso."
            ], keyword: "IDADE" },
            { week: 5, day: "Sáb 5", format: "CARROSSEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Depoimento Focado em Profissionalismo", hooks: ["Profissionalismo que te dá segurança.", "A experiência que conta.", "O que o cliente sentiu na clínica."], headline: "Depoimento Cliente: 'Senti Segurança Desde o Primeiro Contato' (Case Profissionalismo)", desenvolvimento: "Cliente foca na equipe, na organização, na clareza da informação e no suporte pós-operatório.", solucao: "A Fair vende segurança, não apenas cabelo.", climax: "Transplante com padrão de excelência.", ctas: [
                "CTA 1: Digite 'SEGURANÇA' e agende.", 
                "CTA 2: Fale com especialista.", 
                "CTA 3: Peça para conhecer a clínica."
            ], keyword: "SEGURANCA" },
            { week: 5, day: "Dom 5", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Oferta Exclusiva Bônus", hooks: ["Bônus Exclusivo para quem fechar agora!", "Condição especial por tempo limitado.", "Sua chance de ter o transplante com bônus."], headline: "OFERTA EXCLUSIVA: Bônus de [Citar Bônus, ex: 6 Meses de Terapia Capilar] Para Avaliações Agendadas Esta Semana", desenvolvimento: "Cria urgência artificial (oferta de bônus, não desconto). Foca no valor agregado (ganho).", solucao: "Uma oportunidade imperdível de maximizar seu investimento.", climax: "Aja agora para não perder o bônus.", ctas: [
                "CTA 1: Digite 'OFERTA' e garanta o bônus.", 
                "CTA 2: Fale com o time.", 
                "CTA 3: Link direto para garantir a oferta."
            ], keyword: "OFERTA" },
            
            // --- Semanas 6 a 13: Continuação Estratégica (80% BOFU, 20% MOFU) ---
            
            // SEMANA 6 (BOFU - Foco em Fechamento e Resultados)
            { week: 6, day: "Seg 6", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Transformação Feminina (Hairline)", hooks: ["Cabelo é liberdade.", "Resultados para mulheres.", "Seu cabelo novo é possível."], headline: "Transplante Capilar Feminino: Resultados Naturais e Confiança Total", desenvolvimento: "Foco nos pormenores do transplante em mulheres e na linha frontal delicada.", solucao: "Dr. Fábio é especialista também em casos femininos.", climax: "Recupere sua autoestima.", ctas: [
                "CTA 1: Digite 'MULHER' e agende.", 
                "CTA 2: Fale com especialista.", 
                "CTA 3: Veja os cases femininos."
            ], keyword: "MULHER" },
            { week: 6, day: "Qua 6", format: "CARROSSEL", funnel: "BOFU", type: "Levantada de Mão", theme: "FAQ sobre Pagamento e Financeiro", hooks: ["Tudo sobre parcelamento.", "Dúvidas financeiras resolvidas."], headline: "FAQ Financeiro: Parcelamento, Formas de Pagamento e Condições", desenvolvimento: "Respostas diretas às 5 principais dúvidas sobre custo e pagamento.", solucao: "Planeje sem stress.", climax: "A parte mais fácil é a financeira.", ctas: [
                "CTA 1: Digite 'FAQ' para simular.", 
                "CTA 2: Fale com a equipe.", 
                "CTA 3: Peça a tabela de parcelamento."
            ], keyword: "FAQ" },
            { week: 6, day: "Sex 6", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Depoimento Focado em Família/Amigos", hooks: ["O elogio que mudou tudo.", "A surpresa da família.", "Finalmente, sem boné."], headline: "O Impacto Social: 'Meus Amigos Não Acreditavam que Era Natural'", desenvolvimento: "Depoimento focado nos elogios externos e na reação dos outros ao resultado natural.", solucao: "O resultado que fala por si.", climax: "A prova social definitiva.", ctas: [
                "CTA 1: Digite 'RESULTADO' e agende.", 
                "CTA 2: Fale com o Dr. Fábio.", 
                "CTA 3: Compartilhe o vídeo."
            ], keyword: "RESULTADO" },
            { week: 6, day: "Dom 6", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Micro-Agendamento Rápido", hooks: ["Agende em 30 segundos!", "Seu próximo passo é simples."], headline: "Decidiu? Agende Sua Pré-Consulta em 30 Segundos", desenvolvimento: "Foco na facilidade e velocidade do agendamento digital.", solucao: "Zero complicação, apenas ação.", climax: "Agir agora, colher depois.", ctas: [
                "CTA 1: Digite 'GO' e agende.", 
                "CTA 2: Link de Agendamento Rápido.", 
                "CTA 3: Clique para começar."
            ], keyword: "GO" },
            
            // SEMANA 7 (BOFU/MOFU - Foco em Durabilidade e Ciência)
            { week: 7, day: "Seg 7", format: "REEL", funnel: "MOFU", type: "Doação", theme: "Cabelo Transplantado é Definitivo?", hooks: ["Vai cair de novo?", "A durabilidade do transplante.", "Mito ou verdade?"], headline: "Transplante Capilar é Definitivo? A Ciência Por Trás da Resposta", desenvolvimento: "Explica que o cabelo transplantado é da área não afetada (nuca), sendo resistente à calvície genética.", solucao: "É um investimento permanente.", climax: "Durabilidade garantida.", ctas: [
                "CTA 1: Digite 'DEFINITIVO' e receba o Guia.", 
                "CTA 2: Guia de durabilidade.", 
                "CTA 3: Salve para ler depois."
            ], keyword: "DEFINITIVO" },
            { week: 7, day: "Qua 7", format: "CARROSSEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Como Escolher a Clínica Certa (Checklist)", hooks: ["3 perguntas para fazer à clínica.", "Não caia em golpes.", "Seu checklist de segurança."], headline: "CHECKLIST: 7 Pontos Cruciais Antes de Escolher Sua Clínica (Evite o Retoque)", desenvolvimento: "Lista os critérios de credibilidade: Experiência, Equipe, Tecnologia, Garantia, FUE Avançado.", solucao: "A Fair atende a todos os critérios.", climax: "Sua segurança em primeiro lugar.", ctas: [
                "CTA 1: Digite 'ESCOLHA' e agende com a clínica segura.", 
                "CTA 2: Checklist para agendamento.", 
                "CTA 3: Fale com a equipe sobre o checklist."
            ], keyword: "ESCOLHA" },
            { week: 7, day: "Sex 7", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Recuperação Rápida para Profissionais", hooks: ["Volte ao trabalho em [X] dias.", "Foco na recuperação rápida.", "Tempo é dinheiro."], headline: "Recuperação Rápida: Volte à Sua Rotina Sem Estresse", desenvolvimento: "Foca no tempo mínimo de afastamento do trabalho/rotina social (3-7 dias).", solucao: "Planejamento que respeita sua agenda.", climax: "Recuperação com o mínimo de interrupção.", ctas: [
                "CTA 1: Digite 'ROTINA' e agende o transplante planejado.", 
                "CTA 2: Fale sobre a recuperação.", 
                "CTA 3: Agende sua cirurgia."
            ], keyword: "ROTINA" },
            { week: 7, day: "Dom 7", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Oferta de Urgência (Vagas de Última Hora)", hooks: ["Restam X vagas na agenda do Dr. Fábio.", "Decisão imediata, resultado garantido.", "Últimas chances."], headline: "AGORA OU SÓ MÊS QUE VEM: Vagas de Última Hora com Dr. Fábio", desenvolvimento: "Urgência máxima e escassez.", solucao: "Não adie mais o seu sonho. Aja hoje.", climax: "Aproveite a oportunidade.", ctas: [
                "CTA 1: Digite 'ULTIMA' e garanta o horário.", 
                "CTA 2: Reserve sua vaga.", 
                "CTA 3: Agende a última vaga."
            ], keyword: "ULTIMA" },

            // SEMANA 8 (BOFU - Foco em Prova Social e Contorno de Medos)
            { week: 8, day: "Seg 8", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Depoimento de Autoestima", hooks: ["De volta à praia, sem boné.", "Autoestima renovada.", "Sorrindo para as fotos."], headline: "Depoimento: 'Voltei a Sorrir e a Tirar Fotos Sem Medo'", desenvolvimento: "Foco no ganho emocional puro (Autoestima, confiança em eventos sociais).", solucao: "O transplante é a ferramenta para a sua melhor vida.", climax: "Viva a vida que você merece.", ctas: [
                "CTA 1: Digite 'VIDA' e agende a transformação.", 
                "CTA 2: Fale com especialista.", 
                "CTA 3: Comece sua transformação."
            ], keyword: "VIDA" },
            { week: 8, day: "Qua 8", format: "CARROSSEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Desmistificando o Custo (Parcelas Reais)", hooks: ["Quanto custa por dia/mês?", "O valor da parcela é [X]."], headline: "Desmistificando o Custo: Quanto Custa a Liberdade de Não Usar Boné (Exemplo de Parcelamento)", desenvolvimento: "Apresenta exemplos de parcelamento de forma palpável (ex: R$ XX por dia, o preço de um café).", solucao: "Torne o investimento real e acessível.", climax: "Seu cabelo novo é mais barato do que você pensa.", ctas: [
                "CTA 1: Digite 'PARCELA' para simular.", 
                "CTA 2: Simule com a equipe.", 
                "CTA 3: Link direto para simulação."
            ], keyword: "PARCELA" },
            { week: 8, day: "Sex 8", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Medo de Não Ser Bom Candidato", hooks: ["Quem pode fazer?", "Você é elegível?", "Não desista antes da hora."], headline: "Será que Sou um BOM Candidato? Critérios de Elegibilidade do Dr. Fábio", desenvolvimento: "Aborda os critérios (idade, área doadora, tipo de calvície) para filtrar e educar o lead.", solucao: "Só a avaliação do Dr. Fábio pode dar o veredito final.", climax: "Tire a dúvida com o especialista.", ctas: [
                "CTA 1: Digite 'ELEGIVEL' e agende a avaliação.", 
                "CTA 2: Fale com o time Fair.", 
                "CTA 3: Descubra se você é candidato."
            ], keyword: "ELEGIVEL" },
            { week: 8, day: "Dom 8", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Oferta Agendamento Bônus", hooks: ["Ganhe uma Vantagem extra!", "O bônus para quem decide rápido."], headline: "AGENDE AGORA e Ganhe [Bônus] na Sua Cirurgia", desenvolvimento: "Reafirma a oferta de bônus ou um benefício extra para quem agenda imediatamente.", solucao: "Maximize o valor do seu investimento.", climax: "A oportunidade é sua.", ctas: [
                "CTA 1: Digite 'BÔNUS' e agende.", 
                "CTA 2: Garanta o seu benefício.", 
                "CTA 3: Clique para agendar."
            ], keyword: "BONUS" },
            
            // SEMANAS 9 a 13 - Foco em Prova Social, Oferta e Escassez (Ciclo de Fechamento)
            // SEMANA 9
            { week: 9, day: "Seg 9", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Depoimento de Confiança Profissional", hooks: ["O impacto na carreira.", "Confiante em reuniões.", "Sua imagem profissional."], headline: "Depoimento: O Transplante que Impulsionou Minha Carreira", desenvolvimento: "Foco no ganho funcional/profissional.", solucao: "O investimento que se paga na carreira.", climax: "Sua imagem, seu poder.", ctas: [
                "CTA 1: Digite 'PROFISSIONAL' e agende.", 
                "CTA 2: Fale com especialista.", 
                "CTA 3: Veja o case profissional."
            ], keyword: "PROFISSIONAL" },
            { week: 9, day: "Qua 9", format: "CARROSSEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Comparativo: Garantia Fair vs. Mercado", hooks: ["O que é garantia de resultado?", "A diferença Fair.", "Cuidado com garantias falsas."], headline: "Garantia de Resultado: O que o Instituto Fair Oferece de Verdade", desenvolvimento: "Foco na credibilidade da clínica e no acompanhamento pós-operatório estendido.", solucao: "Tranquilidade total no seu investimento.", climax: "Sua segurança, nossa promessa.", ctas: [
                "CTA 1: Digite 'GARANTIA' e agende.", 
                "CTA 2: Fale com o time Fair.", 
                "CTA 3: Peça o termo de garantia."
            ], keyword: "GARANTIA" },
            { week: 9, day: "Sex 9", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "O Custo de Esperar Mais 6 Meses", hooks: ["Não espere mais!", "O que a espera custa.", "O tempo não para."], headline: "A Espera Custa Folículos: O Prejuízo de Adiar Seu Transplante", desenvolvimento: "Urgência baseada na biologia: a calvície avança e a área doadora pode piorar.", solucao: "Aja agora para preservar o que resta.", climax: "O melhor dia para começar foi ontem, o segundo melhor é hoje.", ctas: [
                "CTA 1: Digite 'PREJUÍZO' e agende.", 
                "CTA 2: Fale com o especialista.", 
                "CTA 3: Não perca mais tempo."
            ], keyword: "PREJUIZO" },
            { week: 9, day: "Dom 9", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Última Chamada da Semana", hooks: ["Fechando a agenda.", "Resumo dos benefícios.", "Decisão ou Arrependimento?"], headline: "RESUMO: Por Que Você Deve Agendar Sua Avaliação HOJE", desenvolvimento: "Recapitulação dos 3 maiores ganhos e 3 maiores medos resolvidos pela Fair.", solucao: "O caminho mais seguro e natural.", climax: "Sua chance desta semana.", ctas: [
                "CTA 1: Digite 'FECHAR' e agende.", 
                "CTA 2: Link de agendamento.", 
                "CTA 3: Faça sua escolha final."
            ], keyword: "FECHAR" },

            // SEMANA 10
            { week: 10, day: "Seg 10", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Depoimento: Medo Resolvido", hooks: ["Superando o medo.", "Eu tinha medo de [X], mas fiz!", "A história da minha decisão."], headline: "Depoimento: 'Meu Medo Era o Artificial, Meu Ganho Foi a Naturalidade'", desenvolvimento: "Cliente que tinha a objeção 'medo artificial' relata a satisfação com a hairline natural.", solucao: "Prova de que o medo é infundado na Fair.", climax: "Confie em quem tem experiência.", ctas: [
                "CTA 1: Digite 'SUPERAR' e agende.", 
                "CTA 2: Fale com especialista.", 
                "CTA 3: Veja a transformação."
            ], keyword: "SUPERAR" },
            { week: 10, day: "Qua 10", format: "CARROSSEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Desmistificando o Pós-Op (Fotos)", hooks: ["Fotos reais do pós-op.", "O que acontece dia a dia.", "Não é tão feio quanto parece."], headline: "Pós-Operatório Dia a Dia: Fotos Reais e Recuperação Rápida", desenvolvimento: "Mostra fotos da recuperação (1º dia, 3º dia, 7º dia) para normalizar a aparência.", solucao: "Clareza total para eliminar a ansiedade.", climax: "Recuperação previsível e tranquila.", ctas: [
                "CTA 1: Digite 'FOTOS' e agende.", 
                "CTA 2: Fale com o time Fair.", 
                "CTA 3: Peça a galeria de recuperação."
            ], keyword: "FOTOS" },
            { week: 10, day: "Sex 10", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Comparativo de Preços (Implícito)", hooks: ["Seu investimento vs. seu sonho.", "A diferença entre preço e valor.", "Transplante por R$XX/dia."], headline: "Seu Investimento Mensal na Autoestima é Menor que sua Ansiedade (Custo/Dia)", desenvolvimento: "Volta ao argumento de custo/dia, comparando com gastos diários.", solucao: "Tornar o custo irrelevante perto do ganho emocional.", climax: "A prioridade é você.", ctas: [
                "CTA 1: Digite 'CUSTODIA' e simule.", 
                "CTA 2: Agende sua consulta.", 
                "CTA 3: Compare o custo/dia."
            ], keyword: "CUSTODIA" },
            { week: 10, day: "Dom 10", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Encerramento Agenda", hooks: ["Fechamos o mês com [X] novos clientes!", "A agenda foi um sucesso.", "Sua chance acabou (mas abra a DM!)."], headline: "Agenda de [Mês Atual] FECHADA: Mas Temos uma Última Vaga de Avaliação", desenvolvimento: "Usa a prova social (agenda lotada) para criar escassez extrema.", solucao: "Oferece uma última 'brecha' (vaga de avaliação de última hora) para quem agir em 1h.", climax: "Aja RÁPIDO.", ctas: [
                "CTA 1: Digite 'BRECHA' para a vaga imediata.", 
                "CTA 2: Link de espera.", 
                "CTA 3: Peça a última vaga."
            ], keyword: "BRECHA" },

            // SEMANA 11
            { week: 11, day: "Seg 11", format: "REEL", funnel: "MOFU", type: "Doação", theme: "Transplante em Entradas Iniciais", hooks: ["Não espere a calvície avançar!", "O melhor momento de agir.", "Calvície leve tem solução?"], headline: "Transplante para ENTRADAS: Por Que o Início é o Melhor Momento para Agir", desenvolvimento: "Foco em pessoas com calvície inicial e entradas. É mais fácil e o resultado é mais completo.", solucao: "A Fair pode mapear e prevenir o avanço.", climax: "A prevenção é a melhor cura.", ctas: [
                "CTA 1: Digite 'ENTRADAS' e receba o Guia.", 
                "CTA 2: Guia para calvície inicial.", 
                "CTA 3: Fale com um consultor."
            ], keyword: "ENTRADAS" },
            { week: 11, day: "Qua 11", format: "CARROSSEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Kit de Segurança da Fair", hooks: ["O que a Fair te entrega.", "Seu kit de conforto e segurança.", "Segurança em 5 itens."], headline: "O Kit Pós-Operatório e de Segurança que Você Recebe na Fair", desenvolvimento: "Mostra os itens de valor agregado (medicação, manual, shampoo especial, contato 24h).", solucao: "Você nunca estará sozinho no pós-op.", climax: "Cuidado e acompanhamento total.", ctas: [
                "CTA 1: Digite 'KIT' e agende.", 
                "CTA 2: Fale com especialista.", 
                "CTA 3: Peça a lista do Kit."
            ], keyword: "KIT" },
            { week: 11, day: "Sex 11", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Depoimento de Resultados a Longo Prazo", hooks: ["5 anos depois, e o cabelo?", "Resultado que dura.", "Meu transplante é permanente."], headline: "Resultados 5 Anos Depois: A Prova de que o Transplante é Definitivo (Case Longo Prazo)", desenvolvimento: "Depoimento de cliente com resultado estável após anos.", solucao: "Investimento que resiste ao tempo.", climax: "Tranquilidade e durabilidade.", ctas: [
                "CTA 1: Digite 'LONGO' e agende.", 
                "CTA 2: Fale com o time Fair.", 
                "CTA 3: Veja o case de 5 anos."
            ], keyword: "LONGO" },
            { week: 11, day: "Dom 11", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Oferta de Blackout (Último Mês)", hooks: ["Último mês do trimestre!", "Atenção: Meta Fechada!", "Bônus para o final do ciclo."], headline: "Fechando o Trimestre: Última Chance de Aproveitar Nossas Condições Especiais", desenvolvimento: "Urgência de fechamento de trimestre/ciclo de 90 dias.", solucao: "Condição especial válida apenas até [Data].", climax: "Aja antes que o trimestre acabe.", ctas: [
                "CTA 1: Digite 'TRIMESTRE' e garanta a condição.", 
                "CTA 2: Reserve sua vaga.", 
                "CTA 3: Fale sobre a condição especial."
            ], keyword: "TRIMESTRE" },

            // SEMANA 12
            { week: 12, day: "Seg 12", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Contorno: Medo de Complicações", hooks: ["O que pode dar errado?", "Minimizando os riscos.", "Procedimento 100% seguro."], headline: "Contorno de Objeção: O Risco de Complicações no Transplante Capilar", desenvolvimento: "Aborda os riscos de forma transparente, focando na segurança do ambiente cirúrgico e equipe médica da Fair.", solucao: "A segurança da Fair elimina a maioria dos riscos.", climax: "Transplante é cirurgia: faça com quem é especialista.", ctas: [
                "CTA 1: Digite 'RISCO' e agende com segurança.", 
                "CTA 2: Fale com especialista.", 
                "CTA 3: Peça o protocolo de segurança."
            ], keyword: "RISCO" },
            { week: 12, day: "Qua 12", format: "CARROSSEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Depoimentos em Série (3 em 1)", hooks: ["3 histórias, 1 resultado.", "O que 3 clientes amaram na Fair.", "Três visões da transformação."], headline: "Carrossel de Prova Social: 3 Coisas que Nossos Clientes Mais Amam na Fair", desenvolvimento: "Compila depoimentos curtos (1. Naturalidade. 2. Zero Dor. 3. Profissionalismo da Equipe).", solucao: "O melhor da Fair em um só lugar.", climax: "A escolha certa é consenso.", ctas: [
                "CTA 1: Digite 'CONSENSO' e agende.", 
                "CTA 2: Link na Bio.", 
                "CTA 3: Veja as 3 histórias."
            ], keyword: "CONSENSO" },
            { week: 12, day: "Sex 12", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Depoimento de Zero Arrependimento", hooks: ["O único arrependimento.", "Meu arrependimento: não ter feito antes!", "A decisão que valeu a pena."], headline: "O ÚNICO Arrependimento que Você Vai Ter: Não Ter Feito o Transplante Antes!", desenvolvimento: "Cliente fala sobre a hesitação e como se arrepende apenas de ter esperado tanto tempo.", solucao: "Elimine o arrependimento: comece hoje.", climax: "Não perca mais tempo.", ctas: [
                "CTA 1: Digite 'ARREPENDIMENTO' e agende.", 
                "CTA 2: Fale com o time Fair.", 
                "CTA 3: Comece sua jornada."
            ], keyword: "ARREPENDIMENTO" },
            { week: 12, day: "Dom 12", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Chave de Vagas do Próximo Mês", hooks: ["Abrindo a agenda de [Mês Novo]!", "Garanta sua vaga em primeira mão.", "Planejamento avançado."], headline: "ABRINDO A AGENDA EXCLUSIVA DE [MÊS SEGUINTE]: Garanta sua Avaliação", desenvolvimento: "Foca no futuro: abre vagas limitadas para o próximo ciclo, incentivando o agendamento avançado.", solucao: "Planeamento que garante sua cirurgia.", climax: "Seu 2025 com cabelo novo começa agora.", ctas: [
                "CTA 1: Digite 'ABRIR' e reserve sua vaga.", 
                "CTA 2: Agende agora.", 
                "CTA 3: Garanta seu lugar."
            ], keyword: "ABRIR" },

            // SEMANA 13
            { week: 13, day: "Seg 13", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Resumo Final de 90 Dias (Fechamento)", hooks: ["O que a Fair fez neste trimestre.", "Balanço de resultados.", "Fechando o ciclo de 90 dias."], headline: "Os 90 Dias de Transformação: Por Que Escolher a Fair Agora", desenvolvimento: "Revisa a autoridade do Dr. Fábio e o volume de clientes satisfeitos no último trimestre (Prova Social em massa).", solucao: "O momento é este: o sistema está funcionando.", climax: "Aproveite o fluxo de sucesso.", ctas: [
                "CTA 1: Digite 'FECHAMENTO' e agende a última vaga da campanha.", 
                "CTA 2: Fale com especialista.", 
                "CTA 3: Última chamada."
            ], keyword: "FECHAMENTO" },
            { week: 13, day: "Qua 13", format: "CARROSSEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Plano Financeiro: Fechando com Bônus", hooks: ["Plano Final de Fechamento.", "Últimas horas da condição X.", "O bônus termina hoje."], headline: "PLANO FINAL DE FINANCIAMENTO: Condições Encerrando em [Data]", desenvolvimento: "Ataque final na objeção de preço com urgência máxima.", solucao: "Não perca a chance de pagar com as melhores condições.", climax: "Seja rápido ou perca o bônus.", ctas: [
                "CTA 1: Digite 'ULTIMACHANCE' e garanta o financiamento.", 
                "CTA 2: Fale com o time.", 
                "CTA 3: Peça as condições finais."
            ], keyword: "ULTIMACHANCE" },
            { week: 13, day: "Sex 13", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Depoimento de Sucesso Final (Emocional)", hooks: ["A transformação mais emocionante do trimestre.", "O sorriso de quem se ama.", "Obrigado, Fair."], headline: "Depoimento Mais Emocional: O Reencontro com a Autoestima Plena", desenvolvimento: "O depoimento mais forte, focado no ganho emocional profundo (choro de alegria, gratidão).", solucao: "O propósito da Fair é transformar vidas.", climax: "O final feliz é possível.", ctas: [
                "CTA 1: Digite 'FIM' e comece o seu final feliz.", 
                "CTA 2: Agende sua transformação.", 
                "CTA 3: Fale com quem transforma vidas."
            ], keyword: "FIM" },
            { week: 13, day: "Dom 13", format: "REEL", funnel: "BOFU", type: "Levantada de Mão", theme: "Anúncio de Nova Campanha (Teaser)", hooks: ["Prepare-se para o novo ciclo!", "O que vem por aí.", "Nova meta de transformação."], headline: "TEASER: Prepare-se para a Nova Onda de Transformação da Fair em [Próximo Trimestre]", desenvolvimento: "Mantém o público engajado e encerra o ciclo de 90 dias com uma nota alta e de continuidade.", solucao: "A Fair nunca para de evoluir.", climax: "Junte-se à próxima geração de transformados.", ctas: [
                "CTA 1: Digite 'PROXIMO' para entrar na lista VIP.", 
                "CTA 2: Fale com a equipe.", 
                "CTA 3: Reserve seu lugar no futuro."
            ], keyword: "PROXIMO" },

        ];
        // --- CHART INITIALIZATION ---

        function initCharts() {
            // Funnel Chart
            const ctxFunnel = document.getElementById('funnelChart').getContext('2d');
            new Chart(ctxFunnel, {
                type: 'bar',
                data: {
                    labels: ['Leads (1000)', 'MQLs (650)', 'SQLs (260)', 'Vendas (78)'],
                    datasets: [{
                        label: 'Volume de Pessoas',
                        data: [metrics.leads, metrics.mql, metrics.sql, metrics.deals],
                        backgroundColor: ['#38bdf8', '#10b981', '#a78bfa', '#0d9488'],
                        borderRadius: 4,
                        barPercentage: 0.6
                    }]
                },
                options: {
                    indexAxis: 'y',
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: {
                        legend: { display: false },
                        tooltip: {
                            callbacks: { label: function(context) { return context.raw + ' Pessoas'; } }
                        }
                    },
                    scales: {
                        x: { display: false },
                        y: { grid: { display: false }, ticks: { font: { family: 'Inter', weight: '600' } } }
                    }
                }
            });

            // Source Chart
            const ctxSource = document.getElementById('sourceChart').getContext('2d');
            new Chart(ctxSource, {
                type: 'doughnut',
                data: {
                    labels: ['Tráfego Orgânico (SEO/Reels)', 'Tráfego Pago (Distribuição)', 'Social Selling / Indicação'],
                    datasets: [{
                        data: [50, 30, 20], 
                        backgroundColor: ['#0ea5e9', '#f97316', '#14b8a6'],
                        borderWidth: 0
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    cutout: '75%',
                    plugins: {
                        legend: { position: 'bottom', labels: { usePointStyle: true, padding: 20 } }
                    }
                }
            });
        }

        // --- GEMINI API HELPERS ---
        async function fetchGeminiResponse(systemPrompt, userQuery) {
            const payload = {
                contents: [{ parts: [{ text: userQuery }] }],
                systemInstruction: { parts: [{ text: systemPrompt }] },
            };

            for (let i = 0; i < 3; i++) {
                try {
                    const response = await fetch(API_URL, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify(payload)
                    });

                    if (response.ok) {
                        const result = await response.json();
                        const text = result.candidates?.[0]?.content?.parts?.[0]?.text;
                        if (text) return text;
                    }
                } catch (error) {
                    console.error("API Call failed, retrying...", error);
                }
                await new Promise(resolve => setTimeout(resolve, Math.pow(2, i) * 1000));
            }
            return "Erro ao gerar resposta da IA. Tente novamente mais tarde.";
        }


        // --- GEMINI FEATURE 2: SCRIPT EXPANSION ---
        async function expandContentScript() {
            if (!currentScript || currentScript.format !== 'REEL') {
                document.getElementById('expand-response-area').innerText = 'Esta função só é válida para Roteiros de REEL.';
                return;
            }

            const btn = document.getElementById('expand-script-btn');
            const loader = document.getElementById('expand-loader');
            const responseArea = document.getElementById('expand-response-area');
            const theme = currentScript.theme;
            const headline = currentScript.headline;
            
            btn.disabled = true;
            document.getElementById('expand-btn-text').innerText = 'A desenvolver...';
            loader.classList.remove('hidden');
            responseArea.innerHTML = `<p class="text-sm text-slate-600">A IA está a criar o roteiro detalhado (60s)...</p>`;

            const systemPrompt = `Você é um Copywriter Sênior e Estrategista de Conteúdo de Vídeo, focado em alta retenção (Reels). Expanda o roteiro de um REEL de 60 segundos com base no Tema e Headline fornecidos. A estrutura deve focar na persuasão emocional do público de Transplante Capilar (Dores: Vergonha, Medo Artificial; Ganhos: Autoestima, Juventude). O output deve retornar ESTREITAMENTE APENAS O TEXTO DENTRO DAS TAGS DE ROTEIRO, SEM INTRODUÇÃO, TITULO, CABEÇALHOS, TABELAS, OU FORMATACAO EXTRA. Use a seguinte formatação:
[GANCHO]: Conteúdo detalhado da cena e narração (3-15s).
[DESENVOLVIMENTO]: Conteúdo detalhado da cena e narração (15-30s).
[SOLUÇÃO]: Conteúdo detalhado da cena e narração (30-45s).
[CLIMAX]: Conteúdo detalhado da cena e narração (45-55s).
[CTA]: Conteúdo detalhado da cena e narração (55-60s).
`;
            const userQuery = `Gere um roteiro detalhado para o tema: "${theme}". Headline: "${headline}"`;
            
            const rawResponse = await fetchGeminiResponse(systemPrompt, userQuery);

            btn.disabled = false;
            document.getElementById('expand-btn-text').innerText = '✨ Expandir Roteiro Detalhado (IA)';
            loader.classList.add('hidden');

            try {
                // Adjusting regex to be more robust against newlines and spaces
                const ganchoMatch = rawResponse.match(/\[GANCHO\]:\s*([\s\S]*?)(?=\n?\[DESENVOLVIMENTO\])/);
                const desenvolvimentoMatch = rawResponse.match(/\[DESENVOLVIMENTO\]:\s*([\s\S]*?)(?=\n?\[SOLUÇÃO\])/);
                const solucaoMatch = rawResponse.match(/\[SOLUÇÃO\]:\s*([\s\S]*?)(?=\n?\[CLIMAX\])/);
                const climaxMatch = rawResponse.match(/\[CLIMAX\]:\s*([\s\S]*?)(?=\n?\[CTA\])/);
                const ctaMatch = rawResponse.match(/\[CTA\]:\s*([\s\S]*)/);

                if (ganchoMatch && desenvolvimentoMatch && solucaoMatch && climaxMatch) {
                    
                    document.getElementById('script-desenvolvimento').innerText = desenvolvimentoMatch[1].trim();
                    document.getElementById('script-solucao').innerText = solucaoMatch[1].trim();
                    document.getElementById('script-climax').innerText = climaxMatch[1].trim();
                    
                    // Update the hook list and CTA based on the generated text if applicable
                    document.getElementById('script-hooks').innerHTML = `<li>${ganchoMatch[1].trim()}</li>`;
                    if(ctaMatch) {
                        document.getElementById('script-ctas').innerHTML = `<li>${ctaMatch[1].trim()}</li>`;
                    }
                    
                    responseArea.innerHTML = `<span class="text-emerald-700 font-semibold">✅ Roteiro expandido e atualizado! (Verifique as secções acima).</span>`;
                } else {
                    responseArea.innerHTML = `<span class="text-rose-600">Erro de análise: A estrutura da IA não foi clara ou houve falha na extração.</span>`;
                    console.error("AI output parsing failed:", rawResponse);
                }

            } catch (e) {
                responseArea.innerHTML = `<span class="text-rose-600">Ocorreu um erro inesperado: ${e.message}</span>`;
                console.error("Processing error:", e, rawResponse);
            }
        }


        // --- UTILITY LOGIC ---

        function updateRoadmap(phase) {
            document.querySelectorAll('.phase-btn').forEach(btn => {
                btn.classList.remove('border-sky-500', 'text-sky-600', 'active-phase');
                btn.classList.add('border-transparent', 'text-slate-500');
            });
            const activeBtn = document.getElementById(`phase-${phase}-btn`);
            activeBtn.classList.remove('border-transparent', 'text-slate-500');
            activeBtn.classList.add('border-sky-500', 'text-sky-600', 'active-phase');

            const container = document.getElementById('roadmap-content');
            container.innerHTML = '';
            
            roadmapData[phase].forEach(item => {
                const card = document.createElement('div');
                card.className = "bg-slate-50 p-5 rounded-lg border border-slate-200 hover:border-sky-300 transition-colors";
                card.innerHTML = `
                    <div class="text-3xl mb-3">${item.icon}</div>
                    <h3 class="font-bold text-slate-800 mb-2">${item.title}</h3>
                    <p class="text-sm text-slate-600">${item.desc}</p>
                `;
                container.appendChild(card);
            });
        }

        function toggleObjection(id) {
            const el = document.getElementById(id);
            const icon = document.getElementById(`icon-${id}`);
            const isHidden = el.classList.contains('hidden');
            
            // Hide all and reset icons
            document.querySelectorAll('#objection-list > div, .new-objection').forEach(div => {
                const contentDiv = div.querySelector('div[id]');
                const iconSpan = div.querySelector('[id^="icon-"]');
                if (contentDiv && contentDiv.id !== id) contentDiv.classList.add('hidden');
                if (iconSpan && iconSpan.id !== icon.id) iconSpan.innerText = '+';
            });
            
            if (isHidden) {
                el.classList.remove('hidden');
                icon.innerText = '-';
            } else {
                el.classList.add('hidden');
                icon.innerText = '+';
            }
        }

        // NEW FUNCTION: Setup all 13 week buttons with custom colors
        function setupWeekSelectors() {
            const container = document.getElementById('week-selector-container');
            container.innerHTML = '';
            for (let i = 1; i <= 13; i++) {
                const colorIndex = (i - 1) % WEEK_COLORS.length;
                const colors = WEEK_COLORS[colorIndex];

                const btn = document.createElement('button');
                btn.type = 'button';
                btn.onclick = () => renderCalendar(i);
                btn.id = `btn-week-${i}`;
                
                // Base styling uses bg-color and text-white
                // Active state will use the darker shade (active class)
                btn.className = `py-1 px-2 text-[10px] md:text-xs font-bold rounded flex-shrink-0 transition-colors text-white ${colors.bg} hover:${colors.active} week-btn`;
                btn.innerText = `Sem ${i}`;
                
                // Store colors on the element for easy access in renderCalendar
                btn.setAttribute('data-bg', colors.bg);
                btn.setAttribute('data-active', colors.active);

                container.appendChild(btn);
            }
        }


        function renderCalendar(week) {
            // 1. Update Buttons State (Reset all, then set active)
            document.querySelectorAll('.week-btn').forEach(btn => {
                const bgClass = btn.getAttribute('data-bg');
                const activeClass = btn.getAttribute('data-active');
                
                // Reset all buttons to default color
                btn.classList.remove(activeClass);
                btn.classList.add(bgClass);
            });

            const activeBtn = document.getElementById(`btn-week-${week}`);
            if (activeBtn) {
                const bgClass = activeBtn.getAttribute('data-bg');
                const activeClass = activeBtn.getAttribute('data-active');
                
                // Set active button to the darker active color
                activeBtn.classList.remove(bgClass);
                activeBtn.classList.add(activeClass);
            }

            const list = document.getElementById('calendar-list');
            list.innerHTML = '';
            
            // 2. Render Content based on data availability
            
            // Filter scripts for the selected week
            const weekData = contentScripts.filter(s => s.week === week);

            if (weekData.length > 0) {
                // --- Content Rendering Logic ---
                weekData.forEach((script) => {
                    const item = document.createElement('div');
                    
                    let tagColor = "bg-slate-200 text-slate-600";
                    let typeColor = "bg-slate-100 text-slate-600";
                    
                    if(script.funnel === 'TOFU') tagColor = "bg-emerald-100 text-emerald-700";
                    if(script.funnel === 'MOFU') tagColor = "bg-sky-100 text-sky-700";
                    if(script.funnel === 'BOFU') tagColor = "bg-rose-100 text-rose-700";

                    if(script.type === 'Doação') typeColor = "bg-green-100 text-green-700";
                    if(script.type === 'Levantada de Mão') typeColor = "bg-amber-100 text-amber-700";
                    
                    item.className = "p-3 rounded-lg border border-slate-100 bg-slate-50 hover:bg-white hover:shadow-md cursor-pointer transition-all group";
                    item.onclick = () => showScriptDetail(script);
                    
                    item.innerHTML = `
                        <div class="flex justify-between items-start">
                            <span class="text-xs font-bold text-slate-400 group-hover:text-slate-600">${script.day}</span>
                            <div class="space-x-1">
                                <span class="text-[10px] font-bold px-1.5 py-0.5 rounded ${tagColor}">${script.funnel}</span>
                                <span class="text-[10px] font-bold px-1.5 py-0.5 rounded ${typeColor}">${script.type}</span>
                            </div>
                        </div>
                        <div class="text-sm font-semibold text-slate-700 mt-1 truncate">${script.headline}</div>
                        <div class="text-xs text-slate-400 mt-0.5 flex items-center">
                            <span class="mr-1">${getIcon(script.format)}</span> ${script.format} | Palavra: ${script.keyword}
                        </div>
                    `;
                    list.appendChild(item);
                });
                // --- End Content Rendering Logic ---
                document.getElementById('script-empty-state').classList.remove('hidden');
                document.getElementById('script-detail').classList.add('hidden');
                document.getElementById('script-empty-state').innerHTML = `<span class="text-4xl mb-2">📝</span><p>Selecione um conteúdo do calendário.</p>`;

            } else {
                // This branch should ideally not be hit with the new extended data, but acts as a fallback
                list.innerHTML = `
                    <div class="p-8 text-center bg-yellow-50 rounded-lg border border-yellow-200">
                        <span class="text-3xl text-yellow-700 block mb-2">🗓️</span>
                        <h4 class="font-bold text-slate-800">Planeamento Semanal (Semana ${week})</h4>
                        <p class="text-sm text-slate-600 mt-2">O detalhamento editorial completo (roteiros e copy) para esta semana deve ser preenchido pela equipe de Marketing na execução do Roadmap. O foco do Funil (MOFU/BOFU) já está definido no plano tático.</p>
                    </div>
                `;
                document.getElementById('script-detail').classList.add('hidden');
                document.getElementById('script-empty-state').classList.remove('hidden');
                document.getElementById('script-empty-state').innerHTML = `<span class="text-3xl mb-2 text-slate-400">Conteúdo da Semana ${week}</span>`;
            }
            
        }

        function getIcon(format) {
            if(format === 'REEL') return '🎬';
            if(format === 'STORIES') return '⭕';
            if(format === 'CARROSSEL') return '🖼️';
            if(format === 'STORIES') return '📸';
            return '📄';
        }

        function showScriptDetail(script) {
            currentScript = script; 

            document.getElementById('script-empty-state').classList.add('hidden');
            document.getElementById('script-detail').classList.remove('hidden');
            document.getElementById('script-detail').classList.add('flex');
            
            // Reset AI area
            document.getElementById('expand-response-area').innerHTML = `<p class="text-xs text-slate-500">Clique para gerar um roteiro de 60s pronto para gravação com narração e cenas detalhadas.</p>`;
            document.getElementById('expand-script-btn').disabled = false;
            document.getElementById('expand-btn-text').innerText = '✨ Expandir Roteiro Detalhado (IA)';


            document.getElementById('script-title').innerText = script.theme;
            document.getElementById('script-funnel').innerText = script.funnel;
            document.getElementById('script-format').innerText = script.format;
            document.getElementById('script-type').innerText = script.type;
            
            // Ganchos
            const hooksList = document.getElementById('script-hooks');
            hooksList.innerHTML = '';
            if (script.hooks && script.hooks.length > 0) {
                script.hooks.forEach(hook => {
                    const li = document.createElement('li');
                    li.innerText = hook;
                    hooksList.appendChild(li);
                });
            }

            // CTA
            const ctaList = document.getElementById('script-ctas');
            ctaList.innerHTML = '';
            if (script.ctas && script.ctas.length > 0) {
                script.ctas.forEach((cta, index) => {
                    const li = document.createElement('li');
                    // Ensures that CTA 1: is rendered correctly using the list index
                    li.innerText = `CTA ${index + 1}: ${cta.split(': ')[1] || cta}`; 
                    ctaList.appendChild(li);
                });
            }


            document.getElementById('script-headline').innerText = script.headline;
            document.getElementById('script-desenvolvimento').innerText = script.desenvolvimento;
            document.getElementById('script-solucao').innerText = script.solucao;
            document.getElementById('script-climax').innerText = script.climax;
            document.getElementById('script-keyword').innerText = script.keyword;
        }

        // --- INITIALIZATION ---

        window.onload = function() {
            initCharts();
            updateRoadmap(1);
            setupWeekSelectors(); // Setup all 13 buttons
            renderCalendar(1); // Render Week 1 by default
        };

    </script>
</body>
</html>
