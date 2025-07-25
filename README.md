
<html lang="pt-BR" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projeto de Segurança Estratégica | Netcom para Universidade Tiradentes</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <!-- Chosen Palette: Corporate Clean (Preto, Cinza, Laranja/Âmbar) -->
    <!-- Application Structure Plan: Uma SPA de rolagem única com navegação superior que se torna fixa. A estrutura foi redesenhada para um formato de "relatório digital interativo", mais moderno e profissional. As seções são temáticas e usam layouts de grade para misturar texto, dados e visuais, melhorando a legibilidade. A interatividade principal está concentrada nos detalhes técnicos (abas) e na calculadora de investimento, guiando o cliente de forma lógica. -->
    <!-- Visualization & Content Choices: Dados do Campus -> Cartões de estatística; Arquitetura -> Diagrama visual com HTML/CSS; Inteligências -> Cartões com abas interativas para separar "Técnica" de "Benefícios"; Cronograma -> Timeline visual; Investimento -> Calculadora JS + Gráfico Donut (Chart.js). Confirmado: SEM SVG, SEM Mermaid JS. -->
    <!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f3f4f6;
        }
        .nav-sticky {
            position: sticky;
            top: 0;
            z-index: 50;
            transition: all 0.3s ease-in-out;
            backdrop-filter: blur(10px);
        }
        .tab-button.active {
            border-color: #F59E0B; /* Ambar-500 */
            color: #F59E0B;
            background-color: #fffbeb;
        }
        .hero-bg {
            background-color: #111827;
            background-image: linear-gradient(to right, rgba(17, 24, 39, 0.95), rgba(17, 24, 39, 0.8)), url('https://placehold.co/1200x800/111827/333333?text=Campus+UNIT');
            background-size: cover;
            background-position: center;
        }
    </style>
</head>
<body class="text-gray-700">

    <!-- Container Principal -->
    <div class="max-w-5xl mx-auto bg-white shadow-2xl">

        <!-- Cabeçalho (Hero Section) -->
        <header class="hero-bg text-white">
            <div class="max-w-5xl mx-auto px-6 py-20 md:py-32 text-center">
                <h1 class="text-4xl md:text-5xl font-bold mb-2">Projeto de Segurança Estratégica</h1>
                <p class="text-xl md:text-2xl text-gray-300">Solução de Segurança e Gestão para a Universidade Tiradentes</p>
            </div>
        </header>

        <!-- Navegação -->
        <nav id="navbar" class="bg-white/80 py-3 shadow-md nav-sticky">
            <div class="max-w-5xl mx-auto px-6">
                <div class="flex justify-center space-x-4 md:space-x-8 text-sm md:text-base font-medium text-gray-600">
                    <a href="#visao-geral" class="hover:text-amber-500 transition-colors">Visão Geral</a>
                    <a href="#solucao" class="hover:text-amber-500 transition-colors">Solução Técnica</a>
                    <a href="#inteligencias" class="hover:text-amber-500 transition-colors">Inteligências</a>
                    <a href="#lgpd" class="hover:text-amber-500 transition-colors">LGPD</a>
                    <a href="#investimento" class="hover:text-amber-500 transition-colors">Investimento</a>
                    <a href="#parceria" class="hover:text-amber-500 transition-colors">Parceria</a>
                </div>
            </div>
        </nav>

        <!-- Conteúdo do Projeto -->
        <main class="p-6 md:p-12">

            <section id="visao-geral" class="mb-16">
                <h2 class="text-3xl font-bold text-gray-800 border-b-4 border-amber-400 pb-3 mb-6">1. Sumário Executivo e Visão Estratégica</h2>
                <p class="mb-6">Este documento detalha uma solução completa de <strong>Segurança como Serviço (HaaS)</strong>, projetada pela Netcom para o <strong>Campus Farolândia</strong> da <strong>Universidade Tiradentes</strong>. O objetivo é transformar o sistema de segurança em um ativo estratégico de inteligência e gestão. O modelo de locação (comodato) elimina o investimento inicial, convertendo-o em uma despesa operacional mensal previsível que inclui todos os equipamentos, software, instalação e os serviços de manutenção e suporte contínuo.</p>
                <div class="grid grid-cols-2 lg:grid-cols-4 gap-6 text-center">
                    <div class="bg-gray-50 p-4 rounded-lg border border-gray-200">
                        <p class="text-sm text-gray-500">Área do Terreno</p>
                        <p class="text-2xl font-bold text-amber-500">166.595 m²</p>
                    </div>
                    <div class="bg-gray-50 p-4 rounded-lg border border-gray-200">
                        <p class="text-sm text-gray-500">Área Construída</p>
                        <p class="text-2xl font-bold text-amber-500">78.268 m²</p>
                    </div>
                    <div class="bg-gray-50 p-4 rounded-lg border border-gray-200">
                        <p class="text-sm text-gray-500">Área Livre</p>
                        <p class="text-2xl font-bold text-amber-500">88.326 m²</p>
                    </div>
                    <div class="bg-gray-50 p-4 rounded-lg border border-gray-200">
                        <p class="text-sm text-gray-500">Gabarito de Altura</p>
                        <p class="text-2xl font-bold text-amber-500">23,11 m</p>
                    </div>
                </div>
            </section>

            <section id="solucao" class="mb-16">
                <h2 class="text-3xl font-bold text-gray-800 border-b-4 border-amber-400 pb-3 mb-6">2. Arquitetura Técnica da Solução</h2>
                <p class="mb-8">A solução é projetada sob uma arquitetura híbrida e centralizada para garantir máxima performance, segurança e escalabilidade, com componentes de alta disponibilidade.</p>
                <div class="bg-gray-50 p-8 rounded-lg border border-gray-200">
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-8 text-center items-start">
                        <div>
                            <div class="text-4xl mb-3">🏢</div>
                            <h3 class="text-xl font-semibold text-gray-800 mb-2">Borda (Campus UNIT)</h3>
                            <p class="text-sm text-gray-600">Câmeras LPR/Facial e NVRs para gravação contínua 24/7, garantindo a integridade dos dados mesmo sem conexão.</p>
                        </div>
                        <div>
                            <div class="text-4xl mb-3">🌐</div>
                            <h3 class="text-xl font-semibold text-gray-800 mb-2">Conectividade Gerenciada</h3>
                            <p class="text-sm text-gray-600">Link de Fibra Óptica Dedicado de 100 Mbps simétricos com SLA de 99.8%, garantindo a comunicação estável para os analíticos.</p>
                        </div>
                        <div>
                            <div class="text-4xl mb-3">⚙️</div>
                            <h3 class="text-xl font-semibold text-gray-800 mb-2">Plataforma Central Netcom</h3>
                            <p class="text-sm text-gray-600">Servidor Dedicado (Xeon, 64GB ECC RAM, GPU NVIDIA) com VMS Defense IA para processamento de IA e gestão unificada.</p>
                        </div>
                    </div>
                </div>
            </section>

            <section id="inteligencias" class="mb-16">
                <h2 class="text-3xl font-bold text-gray-800 border-b-4 border-amber-400 pb-3 mb-6">3. Catálogo de Inteligências de Vídeo (IA)</h2>
                <p class="mb-8">A plataforma Defense IA transforma câmeras padrão em sensores inteligentes. Abaixo, detalhamos as funcionalidades que podem ser ativadas para otimizar a segurança e a gestão do campus.</p>
                <div class="space-y-8">
                    <div class="bg-white p-6 rounded-lg shadow-sm border border-gray-200">
                        <h3 class="text-2xl font-semibold text-gray-800 mb-4">Leitura de Placas (LPR)</h3>
                        <div class="mb-4 border-b">
                            <button class="tab-button py-2 px-4 border-b-2 active" onclick="openTab(event, 'lpr-tech', this)">Detalhe Técnico</button>
                            <button class="tab-button py-2 px-4 border-b-2" onclick="openTab(event, 'lpr-benefit', this)">Benefício Estratégico</button>
                            <button class="tab-button py-2 px-4 border-b-2" onclick="openTab(event, 'lpr-usecase', this)">Caso de Uso no Campus</button>
                        </div>
                        <div id="lpr-tech" class="tab-content">
                            <p>A câmera LPR (VIP 7250) utiliza sensor de alta sensibilidade e obturador ajustável para capturar uma imagem nítida da placa. O Defense IA aplica algoritmos de OCR para extrair o texto e compará-lo com o banco de dados para automação e auditoria.</p>
                        </div>
                        <div id="lpr-benefit" class="tab-content hidden">
                            <p>Automação do fluxo de veículos, geração de relatórios de auditoria precisos (placa, data, hora, foto) e criação de alertas para veículos não autorizados, aumentando a segurança perimetral de forma proativa.</p>
                        </div>
                        <div id="lpr-usecase" class="tab-content hidden">
                            <p><strong>Acesso da Direção:</strong> Liberação automática da cancela para veículos cadastrados, sem necessidade de crachá ou controle. <strong>Estacionamento de Alunos:</strong> Registro de todas as placas que entram e saem para controle de pátio e futuras integrações.</p>
                        </div>
                    </div>
                    <div class="bg-white p-6 rounded-lg shadow-sm border border-gray-200">
                        <h3 class="text-2xl font-semibold text-gray-800 mb-4">Reconhecimento Facial</h3>
                         <div class="mb-4 border-b">
                            <button class="tab-button py-2 px-4 border-b-2 active" onclick="openTab(event, 'facial-tech', this)">Detalhe Técnico</button>
                            <button class="tab-button py-2 px-4 border-b-2" onclick="openTab(event, 'facial-benefit', this)">Benefício Estratégico</button>
                            <button class="tab-button py-2 px-4 border-b-2" onclick="openTab(event, 'facial-usecase', this)">Caso de Uso no Campus</button>
                        </div>
                        <div id="facial-tech" class="tab-content">
                            <p>A câmera (VIP 9450) detecta um rosto, analisa múltiplos pontos biométricos e os converte em um código numérico único (template). Este template é comparado pelo Defense IA com um banco de dados de faces cadastradas para identificação.</p>
                        </div>
                        <div id="facial-benefit" class="tab-content hidden">
                            <p>Acesso "hands-free" a áreas de alta segurança. A função de busca forense permite que a segurança encontre rapidamente todas as aparições de uma pessoa de interesse em todo o campus, otimizando o tempo de resposta a incidentes.</p>
                        </div>
                        <div id="facial-usecase" class="tab-content hidden">
                            <p><strong>Acessos aos Blocos:</strong> Liberação de catracas para alunos e funcionários. <strong>Áreas Restritas:</strong> Controle de acesso a laboratórios, CPD ou áreas administrativas sem a necessidade de cartões.</p>
                        </div>
                    </div>
                     <div class="bg-white p-6 rounded-lg shadow-sm border border-gray-200">
                        <h3 class="text-2xl font-semibold text-gray-800 mb-4">Inteligência Perimetral</h3>
                         <div class="mb-4 border-b">
                            <button class="tab-button py-2 px-4 border-b-2 active" onclick="openTab(event, 'perimeter-tech', this)">Detalhe Técnico</button>
                            <button class="tab-button py-2 px-4 border-b-2" onclick="openTab(event, 'perimeter-benefit', this)">Benefício Estratégico</button>
                            <button class="tab-button py-2 px-4 border-b-2" onclick="openTab(event, 'perimeter-usecase', this)">Caso de Uso no Campus</button>
                        </div>
                        <div id="perimeter-tech" class="tab-content">
                            <p>Permite a criação de cercas e linhas virtuais sobre a imagem da câmera. O sistema utiliza algoritmos de Deep Learning para distinguir entre humanos e veículos, ignorando movimentos irrelevantes (como animais ou vegetação) para gerar alertas precisos de intrusão.</p>
                        </div>
                        <div id="perimeter-benefit" class="tab-content hidden">
                            <p>Proteção proativa das fronteiras do campus e áreas restritas durante horários de baixo movimento, com uma drástica redução de falsos alarmes, otimizando o tempo da equipe de segurança.</p>
                        </div>
                        <div id="perimeter-usecase" class="tab-content hidden">
                            <p><strong>Segurança Noturna:</strong> Monitorar os limites do campus, gerando um alerta na central de segurança caso uma pessoa cruze o muro após o horário de fechamento. <strong>Áreas de Risco:</strong> Criar uma cerca virtual ao redor de um gerador ou subestação para alertar sobre aproximação não autorizada.</p>
                        </div>
                    </div>
                     <div class="bg-white p-6 rounded-lg shadow-sm border border-gray-200">
                        <h3 class="text-2xl font-semibold text-gray-800 mb-4">Busca Forense e Contagem de Pessoas</h3>
                         <div class="mb-4 border-b">
                            <button class="tab-button py-2 px-4 border-b-2 active" onclick="openTab(event, 'forensic-tech', this)">Detalhe Técnico</button>
                            <button class="tab-button py-2 px-4 border-b-2" onclick="openTab(event, 'forensic-benefit', this)">Benefício Estratégico</button>
                            <button class="tab-button py-2 px-4 border-b-2" onclick="openTab(event, 'forensic-usecase', this)">Caso de Uso no Campus</button>
                        </div>
                        <div id="forensic-tech" class="tab-content">
                            <p>O sistema extrai e cataloga metadados de objetos (pessoas e veículos), permitindo buscas por características como "pessoa de camisa vermelha" ou "carro de cor preta". A Contagem de Pessoas utiliza algoritmos que identificam e contam indivíduos que cruzam uma linha virtual.</p>
                        </div>
                        <div id="forensic-benefit" class="tab-content hidden">
                            <p>Reduz o tempo de investigação de horas para minutos. Fornece dados operacionais valiosos sobre o fluxo em bibliotecas, refeitórios e acessos, permitindo à gestão otimizar a alocação de recursos e serviços.</p>
                        </div>
                        <div id="forensic-usecase" class="tab-content hidden">
                            <p><strong>Investigação de Incidentes:</strong> Em caso de um furto, a segurança pode buscar por "pessoa com mochila azul" na área do ocorrido. <strong>Gestão de Espaços:</strong> A reitoria pode obter relatórios sobre os horários de maior fluxo na biblioteca para otimizar a alocação de funcionários.</p>
                        </div>
                    </div>
                </div>
            </section>
            
            <section id="lgpd" class="mb-16">
                <h2 class="text-3xl font-bold text-gray-800 border-b-4 border-amber-400 pb-3 mb-6">4. Conformidade com a Lei Geral de Proteção de Dados (LGPD)</h2>
                <p class="mb-4">A Netcom reconhece a criticidade do tratamento de dados pessoais, especialmente em um ambiente acadêmico. Nossa solução é projetada com o conceito de <span class="highlight">Privacy by Design</span>, oferecendo as ferramentas necessárias para que a UNIT cumpra integralmente as exigências da LGPD.</p>
                <div class="grid md:grid-cols-2 gap-8 mt-6">
                    <div class="bg-white p-6 rounded-lg shadow">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Ferramentas Técnicas para Conformidade</h3>
                        <ul class="list-disc list-inside space-y-2 text-gray-600">
                            <li><strong>Controle de Acesso Granular:</strong> Criação de perfis de usuário detalhados, garantindo que cada operador acesse apenas as câmeras e informações pertinentes à sua função (Princípio da Necessidade).</li>
                            <li><strong>Logs de Auditoria Completos:</strong> Todas as ações no sistema (login, visualização de câmera, exportação de vídeo) são registradas, garantindo total rastreabilidade e responsabilização.</li>
                            <li><strong>Política de Retenção de Dados:</strong> As gravações podem ser configuradas para serem automaticamente anonimizadas ou deletadas após um período pré-determinado, em conformidade com os princípios de finalidade e adequação.</li>
                        </ul>
                    </div>
                    <div class="bg-white p-6 rounded-lg shadow">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Responsabilidade Compartilhada</h3>
                        <p class="text-gray-600">A Netcom, como **Operadora de Dados**, fornece a tecnologia e a infraestrutura segura para o tratamento dos dados. A **Universidade Tiradentes**, como **Controladora de Dados**, é responsável por definir e aplicar as políticas de uso, privacidade, e garantir a base legal para o tratamento dos dados coletados, com o apoio de seu Encarregado de Proteção de Dados (DPO).</p>
                    </div>
                </div>
            </section>

            <section id="investimento" class="mb-16">
                 <h2 class="text-3xl font-bold text-gray-800 border-b-4 border-amber-400 pb-2 mb-6">5. Simulador de Investimento (Contrato 12 Meses)</h2>
                <div class="bg-white p-8 rounded-xl shadow-lg border border-gray-200">
                    <p class="mb-8 text-center text-gray-600">Configure os componentes do projeto para simular o valor mensal da solução como serviço. A proposta é totalmente modular para se adequar às suas prioridades.</p>
                    <div class="grid md:grid-cols-2 gap-8 items-center">
                        <div class="space-y-4">
                            <div class="bg-gray-100 p-4 rounded-lg border border-gray-200">
                                <label class="font-bold text-lg text-gray-800">Plataforma e Link Dedicado (Base)</label>
                                <p class="text-2xl font-bold text-right">R$ 6.780,00 / mês</p>
                            </div>
                            <div>
                                <label for="lpr_cameras" class="font-semibold">Câmeras LPR (R$ 675/un)</label>
                                <input type="number" id="lpr_cameras" value="12" min="0" class="w-full p-2 border border-gray-300 rounded mt-1">
                            </div>
                            <div>
                                <label for="facial_cameras" class="font-semibold">Câmeras Faciais (R$ 910/un)</label>
                                <input type="number" id="facial_cameras" value="4" min="0" class="w-full p-2 border border-gray-300 rounded mt-1">
                            </div>
                            <div>
                                <label for="speed_domes" class="font-semibold">Speed Domes (R$ 710/un)</label>
                                <input type="number" id="speed_domes" value="2" min="0" class="w-full p-2 border border-gray-300 rounded mt-1">
                            </div>
                            <div>
                                <label for="fixed_cameras" class="font-semibold">Câmeras Fixas (R$ 80/un)</label>
                                <input type="number" id="fixed_cameras" value="6" min="0" class="w-full p-2 border border-gray-300 rounded mt-1">
                            </div>
                            <div>
                                <label for="wifi_kit" class="font-semibold">Kit Wi-Fi Remoto (R$ 680/kit)</label>
                                <input type="number" id="wifi_kit" value="1" min="0" max="1" class="w-full p-2 border border-gray-300 rounded mt-1">
                            </div>
                            <div>
                                <label for="storage_kit" class="font-semibold">Kit de Gravação (R$ 580/kit)</label>
                                <input type="number" id="storage_kit" value="1" min="0" max="1" class="w-full p-2 border border-gray-300 rounded mt-1">
                            </div>
                        </div>
                        <div class="text-center">
                             <div class="chart-container relative h-80 w-full max-w-sm mx-auto">
                                <canvas id="costChart"></canvas>
                            </div>
                            <div class="mt-6 bg-gray-800 text-white p-6 rounded-lg">
                                <p class="text-lg">Total Mensal Estimado</p>
                                <p id="totalCost" class="text-4xl font-bold text-amber-400">R$ 21.680,00</p>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <section id="parceria" class="mb-16">
                <h2 class="text-3xl font-bold text-gray-800 border-b-4 border-amber-400 pb-3 mb-6">6. Nossa Parceria: Um Compromisso Contínuo</h2>
                <p class="mb-6 text-lg text-gray-600">O modelo de locação da Netcom é um compromisso com a performance contínua. A mensalidade não cobre apenas os equipamentos, mas um ecossistema completo de serviços para garantir sua tranquilidade.</p>
                <div class="grid md:grid-cols-2 gap-8 mt-6">
                    <div class="bg-white p-6 rounded-lg shadow">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Suporte e Manutenção</h3>
                        <ul class="list-disc list-inside space-y-2 text-gray-600">
                            <li><strong>Garantia Total:</strong> Substituição de qualquer equipamento que apresente defeito, sem custos.</li>
                            <li><strong>Manutenção Preventiva:</strong> Visitas técnicas trimestrais para otimização do sistema.</li>
                            <li><strong>Suporte Prioritário:</strong> Atendimento ágil para resolver qualquer eventualidade.</li>
                        </ul>
                    </div>
                    <div class="bg-white p-6 rounded-lg shadow">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Evolução e Termos</h3>
                        <ul class="list-disc list-inside space-y-2 text-gray-600">
                            <li><strong>Atualização Tecnológica:</strong> A cada 36 meses, apresentaremos um plano de modernização dos ativos.</li>
                            <li><strong>Renovação Flexível:</strong> Ao final do contrato, oferecemos opções de renovação, upgrade ou aquisição dos equipamentos.</li>
                            <li><strong>Prazo do Contrato:</strong> 12 meses, com renovação automática.</li>
                        </ul>
                    </div>
                </div>
            </section>
        </main>

        <!-- Rodapé -->
        <footer class="bg-gray-800 text-white text-center p-8">
            <p class="font-bold text-lg">Estamos convictos de que esta parceria tecnológica representa o futuro da segurança e gestão do campus. A Netcom está pronta para iniciar este projeto transformador.</p>
            <p class="mt-4 text-gray-400">Netcom</p>
        </footer>
    </div>

    <script>
        const costs = {
            plataforma: 6780,
            lpr: 675,
            facial: 910,
            speed: 710,
            fixed: 80,
            wifi: 680,
            storage: 580
        };

        const lprInput = document.getElementById('lpr_cameras');
        const facialInput = document.getElementById('facial_cameras');
        const speedInput = document.getElementById('speed_domes');
        const fixedInput = document.getElementById('fixed_cameras');
        const wifiInput = document.getElementById('wifi_kit');
        const storageInput = document.getElementById('storage_kit');
        const totalCostEl = document.getElementById('totalCost');
        
        const inputs = [lprInput, facialInput, speedInput, fixedInput, wifiInput, storageInput];

        const ctx = document.getElementById('costChart').getContext('2d');
        let costChart = new Chart(ctx, {
            type: 'doughnut',
            data: {
                labels: ['Plataforma', 'LPR', 'Facial', 'Speed Dome', 'Fixas', 'Wi-Fi', 'Gravação'],
                datasets: [{
                    label: 'Composição do Custo Mensal',
                    data: [],
                    backgroundColor: [
                        '#1a202c', // Cinza bem escuro
                        '#E69B00', // Laranja
                        '#4a5568', // Cinza escuro
                        '#f6e05e', // Amarelo
                        '#a0aec0', // Cinza médio
                        '#fbd38d', // Laranja claro
                        '#718096'  // Cinza
                    ],
                    borderColor: '#ffffff',
                    borderWidth: 2
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                plugins: {
                    legend: {
                        position: 'bottom',
                        labels: {
                            font: {
                                size: 12
                            }
                        }
                    }
                },
                cutout: '60%'
            }
        });

        function formatCurrency(value) {
            return value.toLocaleString('pt-BR', { style: 'currency', currency: 'BRL' });
        }

        function calculateTotal() {
            const lprValue = (parseInt(lprInput.value) || 0) * costs.lpr;
            const facialValue = (parseInt(facialInput.value) || 0) * costs.facial;
            const speedValue = (parseInt(speedInput.value) || 0) * costs.speed;
            const fixedValue = (parseInt(fixedInput.value) || 0) * costs.fixed;
            const wifiValue = (parseInt(wifiInput.value) || 0) * costs.wifi;
            const storageValue = (parseInt(storageInput.value) || 0) * costs.storage;

            const total = costs.plataforma + lprValue + facialValue + speedValue + fixedValue + wifiValue + storageValue;
            
            totalCostEl.textContent = formatCurrency(total);

            costChart.data.datasets[0].data = [
                costs.plataforma,
                lprValue,
                facialValue,
                speedValue,
                fixedValue,
                wifiValue,
                storageValue
            ];
            costChart.update();
        }

        inputs.forEach(input => {
            input.addEventListener('input', calculateTotal);
        });

        // Initial calculation
        calculateTotal();

        function openTab(event, tabID, element) {
            let i, tabcontent, tabbuttons;
            const parent = element.closest('.bg-white');
            tabcontent = parent.getElementsByClassName("tab-content");
            for (i = 0; i < tabcontent.length; i++) {
                tabcontent[i].classList.add("hidden");
            }
            tabbuttons = parent.getElementsByClassName("tab-button");
            for (i = 0; i < tabbuttons.length; i++) {
                tabbuttons[i].classList.remove("active");
            }
            parent.querySelector("#" + tabID).classList.remove("hidden");
            event.currentTarget.classList.add("active");
        }
    </script>
</body>
</html>

