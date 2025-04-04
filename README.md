<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Anderson Caetano - Desenvolvedor Full Stack</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #2563eb;       /* Modern blue */
            --primary-dark: #1e40af;
            --secondary: #10b981;     /* Teal */
            --accent: #f59e0b;        /* Amber */
            --dark: #1f2937;
            --light: #f3f4f6;
            --gray: #6b7280;
            --light-gray: #e5e7eb;
            --white: #ffffff;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', sans-serif;
        }
        
        body {
            line-height: 1.6;
            color: var(--dark);
            background-color: #f9fafb;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary), var(--primary-dark));
            color: var(--white);
            padding: 30px 0;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            position: relative;
            overflow: hidden;
        }
        
        header::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: var(--accent);
        }
        
        header h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            font-weight: 700;
        }
        
        header p {
            font-size: 1.2rem;
            opacity: 0.9;
            font-weight: 300;
        }
        
        .contact-info {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 20px;
        }
        
        .contact-info a {
            color: var(--white);
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 8px;
            padding: 8px 15px;
            background-color: rgba(255,255,255,0.1);
            border-radius: 50px;
            transition: all 0.3s ease;
        }
        
        .contact-info a:hover {
            background-color: rgba(255,255,255,0.2);
            transform: translateY(-2px);
        }
        
        .main-content {
            display: grid;
            grid-template-columns: 1fr;
            gap: 30px;
            margin-top: 40px;
        }
        
        @media (min-width: 992px) {
            .main-content {
                grid-template-columns: 1fr 2fr;
            }
        }
        
        .sidebar {
            background-color: var(--white);
            border-radius: 10px;
            padding: 25px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }
        
        .content {
            background-color: var(--white);
            border-radius: 10px;
            padding: 25px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }
        
        h2 {
            color: var(--primary);
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 2px solid var(--light-gray);
            font-size: 1.5rem;
            font-weight: 600;
            position: relative;
        }
        
        h2::after {
            content: "";
            position: absolute;
            bottom: -2px;
            left: 0;
            width: 50px;
            height: 2px;
            background-color: var(--accent);
        }
        
        h3 {
            color: var(--dark);
            margin: 20px 0 10px;
            font-size: 1.2rem;
            font-weight: 600;
        }
        
        h4 {
            color: var(--primary);
            margin: 15px 0 8px;
            font-size: 1.1rem;
            font-weight: 500;
        }
        
        .section {
            margin-bottom: 30px;
        }
        
        .job, .education {
            margin-bottom: 25px;
        }
        
        .job-header, .education-header {
            display: flex;
            justify-content: space-between;
            margin-bottom: 8px;
            flex-wrap: wrap;
        }
        
        .job-title, .education-title {
            font-weight: 600;
            color: var(--primary);
            font-size: 1.1rem;
        }
        
        .job-period, .education-period {
            color: var(--gray);
            font-style: italic;
            font-size: 0.9rem;
        }
        
        .job-company, .education-institution {
            font-weight: 600;
            color: var(--secondary);
            margin-bottom: 10px;
            display: block;
        }
        
        ul {
            padding-left: 20px;
        }
        
        li {
            margin-bottom: 8px;
            text-align: justify;
            position: relative;
            padding-left: 15px;
        }
        
        li::before {
            content: "•";
            color: var(--accent);
            font-weight: bold;
            position: absolute;
            left: 0;
        }
        
        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }
        
        .skill-tag {
            background-color: var(--light);
            padding: 6px 12px;
            border-radius: 20px;
            font-size: 0.85rem;
            color: var(--dark);
            border: 1px solid var(--light-gray);
        }
        
        .skill-tag:hover {
            background-color: var(--primary);
            color: white;
            transform: translateY(-2px);
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        
        .filter-section {
            margin-bottom: 25px;
        }
        
        .filter-btn {
            background-color: var(--light);
            color: var(--dark);
            border: none;
            padding: 12px 20px;
            border-radius: 8px;
            cursor: pointer;
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 15px;
            width: 100%;
            text-align: left;
            transition: all 0.3s ease;
            font-weight: 500;
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
        }
        
        .filter-btn:hover {
            background-color: var(--primary);
            color: var(--white);
        }
        
        .filter-btn.active {
            background-color: var(--primary);
            color: var(--white);
        }
        
        .filter-btn .arrow {
            transition: transform 0.3s;
            margin-left: auto;
            font-size: 0.9rem;
        }
        
        .filter-btn.active .arrow {
            transform: rotate(180deg);
        }
        
        .filter-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.4s ease-out;
        }
        
        .filter-content.show {
            max-height: 10000px;
        }
        
        .presentation-letter {
            text-align: justify;
            line-height: 1.7;
        }
        
        .presentation-letter p {
            margin-bottom: 15px;
        }
        
        .presentation-letter ul {
            margin-bottom: 20px;
        }
        
        .presentation-letter li {
            margin-bottom: 10px;
        }
        
        .signature {
            font-style: italic;
            margin-top: 25px;
            color: var(--gray);
        }
        
        .results {
            background-color: #f0fdf4;
            padding: 18px;
            border-radius: 8px;
            margin: 20px 0;
            border-left: 4px solid var(--secondary);
        }
        
        .results h4 {
            margin-top: 0;
            color: var(--secondary);
            display: flex;
            align-items: center;
            gap: 8px;
        }
        
        .results h4 i {
            color: var(--secondary);
        }
        
        .professional-summary {
            background-color: #eff6ff;
            padding: 20px;
            border-radius: 8px;
            margin-bottom: 25px;
            border-left: 4px solid var(--primary);
        }
        
        .professional-summary p {
            text-align: justify;
            line-height: 1.7;
        }
        
        .technical-skills {
            background-color: #f8fafc;
            padding: 20px;
            border-radius: 8px;
            margin-bottom: 25px;
            border-left: 4px solid var(--accent);
        }
        
        .skills-category {
            margin-bottom: 15px;
        }
        
        .skills-category h4 {
            color: var(--dark);
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 8px;
        }
        
        .skills-category h4 i {
            color: var(--accent);
        }
        
        footer {
            text-align: center;
            padding: 25px;
            background-color: var(--dark);
            color: var(--white);
            margin-top: 40px;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            header h1 {
                font-size: 2rem;
            }
            
            .job-header, .education-header {
                flex-direction: column;
                gap: 5px;
            }
            
            .job-period, .education-period {
                margin-top: 0;
            }
            
            .contact-info a {
                padding: 6px 12px;
                font-size: 0.9rem;
            }
        }
        
        @media (max-width: 480px) {
            header h1 {
                font-size: 1.8rem;
            }
            
            header p {
                font-size: 1rem;
            }
            
            .contact-info {
                flex-direction: column;
                align-items: center;
                gap: 10px;
            }
            
            .filter-btn {
                padding: 10px 15px;
                font-size: 0.9rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Anderson Caetano</h1>
            <p>Desenvolvedor Full Stack | Front-end Specialist</p>
            <div class="contact-info">
                <a href="mailto:andersonsilcaetano@icloud.com">
                    <i class="fas fa-envelope"></i>
                    andersonsilcaetano@icloud.com
                </a>
                <a href="tel:+5521980081646">
                    <i class="fas fa-phone"></i>
                    +55 21 98008-1646
                </a>
                <a href="#" target="_blank">
                    <i class="fab fa-github"></i>
                    GitHub
                </a>
                <a href="#" target="_blank">
                    <i class="fab fa-linkedin"></i>
                    LinkedIn
                </a>
            </div>
        </div>
    </header>
    
    <div class="container">
        <div class="main-content">
            <div class="sidebar">
                <div class="section">
                    <h2>Objetivo</h2>
                    <p>Analista de Suporte Técnico N1/N2, com 15+ anos de experiência comprovada em atendimento ao cliente, gestão de tickets, aplicando minhas experiências em sistemas multicanal (Unnichat, SendFlow, Live), CRM (Zendesk, Freshdesk) e ERP, buscando também contribuir no desenvolvimento web front end e back end.</p>
                </div>
                
                <div class="section">
                    <h2>Formação</h2>
                    <div class="education">
                        <div class="education-header">
                            <span class="education-title">Análise e Desenvolvimento de Sistemas</span>
                            <span class="education-period">2024</span>
                        </div>
                        <div class="education-institution">Unopar Universidade Anhanguera</div>
                        <p>Tecnólogo voltado a aplicações de desenvolvimento de negócios em aplicações Web no Mercado de Trabalho</p>
                    </div>
                </div>
                
                <div class="section">
                    <h2>Certificações</h2>
                    <ul>
                        <li>AWS Academy Cloud Developing - Amazon Web Services (2022)</li>
                        <li>AWS Academy Cloud Foundations - Amazon Web Services (2022)</li>
                        <li>UX/UI Designer - Coursera/Anhanguera (2023/24)</li>
                        <li>Redes de Computadores - Anhanguera (2023/24)</li>
                        <li>Segurança e Auditoria de Sistemas - Anhanguera (2023/24)</li>
                    </ul>
                </div>
            </div>
            
            <div class="content">
                <div class="section">
                    <div class="professional-summary">
                        <h2>Resumo Profissional</h2>
                        <p>Profissional com experiência em Suporte Técnico (N1/N2) e infraestrutura de redes, atuando em empresas como Contax (Oi Telecom) e Home Agent (Seguradora Líder DPVAT). Especializado em atendimento ao cliente multicanal (Unnichat, SendFlow, Live) e gestão de tickets em sistemas como Zendesk, Freshdesk e ERPs proprietários. Domínio em suporte remoto, automação de processos (Webhooks, APIs do Google e WhatsApp Oficial Meta) e integração de dados e IA. Experiência prática em soluções de TI, incluindo redes (Fibra), AWS Cloud, Windows e ferramentas de comunicação (VOIP - Neon Now, CloudTalk, ManyChat). Desenvolvimento Full Stack (HTML, CSS, JavaScript, back-end) aplicado a troubleshooting (problemas) e otimização de sistemas. Certificações(02) em AWS, Redes e Segurança da Informação.</p>
                    </div>
                </div>
                
                <div class="section">
                    <div class="technical-skills">
                        <h2>Habilidades Técnicas</h2>
                        <div class="skills-category">
                            <h4><i class="fas fa-network-wired"></i> Infraestrutura & Redes</h4>
                            <ul>
                                <li>Configuração de redes (DNS, DHCP)</li>
                                <li>Cabeamento RJ45, crimpagem, roteadores</li>
                            </ul>
                        </div>
                        
                        <div class="skills-category">
                            <h4><i class="fas fa-code"></i> Desenvolvimento & Automação</h4>
                            <ul>
                                <li>HTML, CSS, JavaScript</li>
                                <li>Suporte a APIs (Google, WhatsApp Meta)</li>
                                <li>SQL básico para análise de dados</li>
                                <li>Webhooks para automação de sistemas</li>
                            </ul>
                        </div>
                        
                        <div class="skills-category">
                            <h4><i class="fas fa-headset"></i> Suporte Técnico</h4>
                            <ul>
                                <li>Atendimento multicanal (chat, telefone, CRM)</li>
                                <li>Suporte remoto (AnyDesk, TeamViewer)</li>
                                <li>Resolução de problemas N1/N2/N3</li>
                            </ul>
                        </div>
                        
                        <div class="skills-category">
                            <h4><i class="fas fa-tools"></i> Ferramentas & Sistemas</h4>
                            <ul>
                                <li>CRMs: Zendesk, Freshdesk, sistemas proprietários (Oi Telecom, DPVAT)</li>
                                <li>Gestão de tickets, VOIP (CloudTalk, Neon Now), Manychat</li>
                                <li>ERP/CRM: Integração de dados, automação via scripts</li>
                            </ul>
                        </div>
                    </div>
                </div>
                
                <div class="section filter-section">
                    <button class="filter-btn" onclick="toggleFilter('presentation-letter')">
                        <span>Carta de Apresentação</span>
                        <span class="arrow"><i class="fas fa-chevron-down"></i></span>
                    </button>
                    <div class="filter-content" id="presentation-letter">
                        <div class="presentation-letter">
                            <p>Prezados(as) Recrutadores(as),</p>
                            <p>Com grande interesse, envio minha candidatura à vaga. Sou formado em Análise e Desenvolvimento de Sistemas (Unopar/2024) e atuo como Desenvolvedor Full Stack na Enceladus Market, onde lidero projetos end-to-end com foco em HTML5, CSS3, JavaScript e PHP (Laravel), além de integrações com APIs (Google, WhatsApp Business):</p>
                            <ul>
                                <li><strong>Experiência Front-end:</strong> Desenvolvimento de interfaces responsivas, aplicações dinâmicas (como e-commerces e sistemas de agendamento) e otimização de UX/UI com Canvas e técnicas de SEO.</li>
                                <li><strong>Domínio em CMS Personalizado:</strong> Criação e customização de sistemas de gerenciamento de conteúdo sob medida, utilizando tecnologias modernas para atender necessidades específicas de cada projeto.</li>
                                <li><strong>Habilidades Complementares:</strong> Conhecimento em back-end (PHP, Laravel) e DevOps (gerenciamento de hospedagem, SSL, CDN), permitindo uma visão holística do ciclo de desenvolvimento.</li>
                                <li><strong>Background em Suporte Técnico:</strong> 15+ anos resolvendo problemas complexos em TI (redes, CRM, ERP), o que agrega valor na identificação e correção de bugs com foco na experiência do usuário.</li>
                                <li><strong>Certificações AWS:</strong> Cloud Foundations e Cloud Developing, além de cursos em UX/UI Design e Segurança da Informação.</li>
                            </ul>
                            <p><strong>Por que me candidato?</strong></p>
                            <p>Minha trajetória combinando suporte técnico avançado e desenvolvimento web me permite criar soluções alinhadas às necessidades do usuário final, com código limpo e performance otimizada. Tenho facilidade para trabalhar em equipe (Git/GitHub) e adaptar-me a metodologias ágeis, sempre buscando entregar projetos que unam funcionalidade e design intuitivo.</p>
                            <p>Agradeço pela consideração e coloco-me à disposição para contribuir com minha expertise técnica e visão centrada no cliente. Estou disponível para entrevistas no horário que for conveniente.</p>
                            <p class="signature">Atenciosamente,<br>Anderson Caetano<br>Desenvolvedor Full Stack | Front-end Specialist</p>
                        </div>
                    </div>
                </div>
                
                <div class="section filter-section">
                    <button class="filter-btn" onclick="toggleFilter('professional-experience')">
                        <span>Experiência Profissional</span>
                        <span class="arrow"><i class="fas fa-chevron-down"></i></span>
                    </button>
                    <div class="filter-content show" id="professional-experience">
                        <div class="job">
                            <div class="job-header">
                                <span class="job-title">Desenvolvedor Web Full Stack</span>
                                <span class="job-period">Jan/2024 – Atualmente</span>
                            </div>
                            <div class="job-company">Enceladus Market</div>
                            <ul>
                                <li><strong>Desenvolvimento Full Stack:</strong> Liderança no ciclo completo de desenvolvimento, desde concepção até implementação, abrangendo front-end, back-end e banco de dados.</li>
                                <li><strong>Soluções Personalizadas:</strong> Blogs pessoais com CMS sob medida, e-commerces integrados a gateways de pagamento, aplicações web com funcionalidades dinâmicas (agendamento, autenticação).</li>
                                <li><strong>Integração de APIs:</strong> Google, WhatsApp Business e Webhooks para automação, gestão de domínios.</li>
                                <li><strong>Tecnologias:</strong> Front-end: HTML5, CSS3, JavaScript; Back-end: PHP (Laravel).</li>
                                <li><strong>Infraestrutura e DevOps:</strong> Configuração e manutenção de ambientes de hospedagem em Windows e UNIX (Linux, MacOS), otimização de desempenho, segurança (SSL, firewalls) e escalabilidade (load balancing, CDN).</li>
                                <li><strong>UX/UI Design:</strong> Aplicação de conceitos de UX/UI Design para melhorar usabilidade e engajamento, criação de elementos gráficos dinâmicos com Canvas (animações, gráficos interativos).</li>
                                <li><strong>Versionamento:</strong> Git (GitHub) no registro de versões do projeto entre equipe e segurança.</li>
                            </ul>
                        </div>
                        
                        <div class="job filter-section">
                            <button class="filter-btn" onclick="toggleFilter('seguradora-lider')">
                                <div class="job-header">
                                    <span class="job-title">Analista de Suporte e SAC</span>
                                    <span class="job-period">Jun/2016 – Jan/2018 (Home Office)</span>
                                </div>
                                <div class="job-company">Seguradora Líder DPVAT (Home Agent)</div>
                                <span class="arrow"><i class="fas fa-chevron-down"></i></span>
                            </button>
                            <div class="filter-content show" id="seguradora-lider">
                                <ul>
                                    <li><strong>Atendimento ao Cliente Multicanal:</strong>
                                        <ul>
                                            <li>Suporte via chat (ManyChat) e telefone VOIP (Neon Now, CloudTalk), incluindo suporte a PCDs.</li>
                                            <li>Orientação sobre trâmites do DPVAT: entrada de processos, documentação necessária (ex: laudos médicos, BOs), status de pagamentos e baixa do seguro.</li>
                                            <li>Resolução de dúvidas complexas sobre sinistros, prazos e conformidade legal.</li>
                                            <li>Scripts padronizados para agilizar respostas (FAQ interno) e garantir uniformidade nas informações.</li>
                                        </ul>
                                    </li>
                                    <li><strong>Ferramentas:</strong>
                                        <ul>
                                            <li>Plataformas de atendimento equivalentes a Unnichat/SendFlow (multicanal).</li>
                                            <li>Sistemas VOIP (Neon Now, CloudTalk) e ManyChat para automação de interações via chat.</li>
                                            <li>CRM/ERP proprietário para gestão de sinistros, validação de documentos, atualização em massa de status.</li>
                                            <li>Integração de dados entre sistemas via APIs ou planilhas (Excel/Google Sheets).</li>
                                        </ul>
                                    </li>
                                    <li><strong>Gestão de Dados e Processos:</strong>
                                        <ul>
                                            <li>Geração de relatórios estatísticos (volume de demandas, tempo médio de resolução).</li>
                                            <li>Identificação de padrões recorrentes para otimizar fluxos (documentos mais solicitados).</li>
                                            <li>Análise de inconsistências em processos (documentos incompletos, divergências cadastrais).</li>
                                        </ul>
                                    </li>
                                </ul>
                                <div class="results">
                                    <h4><i class="fas fa-chart-line"></i> Resultados e Métricas</h4>
                                    <ul>
                                        <li>Redução de 30% no tempo de processamento de sinistros após automação de etapas</li>
                                        <li>Aumento de 25% na satisfação do cliente (pesquisas pós-atendimento)</li>
                                        <li>Diminuição de inconsistências em processos devido à padronização de documentação</li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                        
                        <div class="job filter-section">
                            <button class="filter-btn" onclick="toggleFilter('contax-oi')">
                                <div class="job-header">
                                    <span class="job-title">Suporte Técnico Oi Fibra</span>
                                    <span class="job-period">Jun/2013 – Jan/2016 (Presencial)</span>
                                </div>
                                <div class="job-company">Contax/Liq S/A</div>
                                <span class="arrow"><i class="fas fa-chevron-down"></i></span>
                            </button>
                            <div class="filter-content show" id="contax-oi">
                                <ul>
                                    <li><strong>Atendimento Multicanal ao Cliente:</strong>
                                        <ul>
                                            <li>Prestação de suporte técnico N1 e N2 para clientes Oi Fibra (Banda Larga).</li>
                                            <li>Diagnóstico remoto de falhas em redes ADSL/VDSL (testes de linha, sincronização de router).</li>
                                            <li>Acesso remoto (via TeamViewer/AnyDesk) para configuração de dispositivos dos clientes.</li>
                                            <li>Escalonamento para N3 em casos complexos (problemas na infraestrutura Oi).</li>
                                            <li>Configuração de conexão, instalação, detecção e configuração em roteadores (TP-Link, Huawei), configuração TCP/IP, DNS, DHCP, análise de logs.</li>
                                            <li>Uso de scripts padronizados para orientação sobre falhas comuns (lentidão, instabilidade, bloqueio de MAC).</li>
                                        </ul>
                                    </li>
                                    <li><strong>Ferramentas de Atendimento:</strong>
                                        <ul>
                                            <li>Sistemas Unnichat, SendFlow (atendimento simultâneo em múltiplos canais).</li>
                                            <li>Plataformas de Live Chat e Unni IA para agilizar respostas automatizadas.</li>
                                            <li>Integração entre CRM e ferramentas de cobrança via APIs.</li>
                                            <li>Sistemas Windows, Linux e MacOS (básico), SAP (módulo de suporte) e Twilio Flex (chamadas VoIP).</li>
                                            <li>Configuração de Webhooks para notificações de falhas e alertas críticos.</li>
                                        </ul>
                                    </li>
                                    <li><strong>Gestão de Tickets e CRM:</strong>
                                        <ul>
                                            <li>Zendesk e Freshdesk para registro, triagem e acompanhamento de chamados.</li>
                                            <li>Salesforce/ERP proprietário para consulta de dados cadastrais, contratos e histórico do cliente.</li>
                                            <li>Recebimento, criação e encerramento de tickets conforme SLA (transbordos nos níveis N1 a N3).</li>
                                        </ul>
                                    </li>
                                </ul>
                                <div class="results">
                                    <h4><i class="fas fa-chart-line"></i> Resultados</h4>
                                    <ul>
                                        <li>Alta taxa de resolução no primeiro contato (N1/N2)</li>
                                        <li>Redução de 20% no tempo de atendimento após automação de processos</li>
                                        <li>Métricas de feedback positivo em pesquisas de satisfação (CSAT acima de 85%)</li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                        
                        <div class="job filter-section">
                            <button class="filter-btn" onclick="toggleFilter('contax-backoffice')">
                                <div class="job-header">
                                    <span class="job-title">Analista de BackOffice</span>
                                    <span class="job-period">Jun/2010 – Jan/2013 (Presencial)</span>
                                </div>
                                <div class="job-company">Contax/Liq S/A</div>
                                <span class="arrow"><i class="fas fa-chevron-down"></i></span>
                            </button>
                            <div class="filter-content show" id="contax-backoffice">
                                <ul>
                                    <li><strong>Principais Atividades:</strong>
                                        <ul>
                                            <li>Resolução técnica de casos complexos (telefonia fixa/móvel, banda larga Oi, TV por assinatura).</li>
                                            <li>Tratamento de demandas judiciais e regulatórias (PROCON, Juizado, Anatel - ODCs/PADOs/DOCs).</li>
                                            <li>Gestão integral de tickets críticos (abertura, acompanhamento e solução) com SLA rígido.</li>
                                            <li>Análise e correção sistêmica de falhas (faturamento, cadastro, provisionamento).</li>
                                        </ul>
                                    </li>
                                    <li><strong>Tratamento de Casos Complexos:</strong>
                                        <ul>
                                            <li>Solução de demandas não resolvidas pelo atendimento inicial (N1/N2), incluindo:
                                                <ul>
                                                    <li>Faturamento incorreto (ajuste de valores, reembolsos, cobranças indevidas).</li>
                                                    <li>Problemas cadastrais (migração de planos, portabilidade, bloqueios indevidos).</li>
                                                    <li>Falhas técnicas em serviços de telefonia fixa/móvel e banda larga (Oi Fibra).</li>
                                                    <li>Análise de inconsistências em sistemas de faturamento e cadastro (valores divergentes, planos não aplicados).</li>
                                                </ul>
                                            </li>
                                            <li>Colaboração com equipes de TI e desenvolvimento para correção de bugs (scripts em SQL, ajustes em códigos-fonte).</li>
                                        </ul>
                                    </li>
                                    <li><strong>Ferramentas e Técnicas Utilizadas:</strong>
                                        <ul>
                                            <li>Sistemas Corporativos: SAP CRM proprietário, Oi Telecom, GS3 (sistema de gestão de serviços técnicos da Oi).</li>
                                            <li>Redes e Telecom: Knowledge Base Oi, análise de logs (DSLAM, RAS), protocolos TCP/IP, ipconfig.</li>
                                            <li>Gestão de Tickets: Zendesk, Clarify, CRM Salesforce.</li>
                                            <li>Ferramentas Regulatórias: Anatel Consumidor, PROCON Digital.</li>
                                        </ul>
                                    </li>
                                    <li><strong>Competências Técnicas:</strong>
                                        <ul>
                                            <li>Domínio completo do ecossistema Oi (fixo/móvel/banda larga).</li>
                                            <li>Habilidade em debugging de sistemas de faturamento e provisionamento.</li>
                                            <li>Desenvolvimento de manuais técnicos e fluxogramas de processos.</li>
                                        </ul>
                                    </li>
                                </ul>
                                <div class="results">
                                    <h4><i class="fas fa-chart-line"></i> Resultados</h4>
                                    <ul>
                                        <li>92% de resolução na primeira análise (N3)</li>
                                        <li>Redução de 40% no backlog de casos judiciais</li>
                                        <li>100% de compliance em prazos Anatel (72h para ODCs)</li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                        
                        <div class="job filter-section">
                            <button class="filter-btn" onclick="toggleFilter('gpa')">
                                <div class="job-header">
                                    <span class="job-title">Administrativo Geral</span>
                                    <span class="job-period">Fev/1999 – Set/2009 (Presencial)</span>
                                </div>
                                <div class="job-company">GPA – Grupo Pão de Açúcar</div>
                                <span class="arrow"><i class="fas fa-chevron-down"></i></span>
                            </button>
                            <div class="filter-content show" id="gpa">
                                <ul>
                                    <li><strong>Principais Atividades:</strong>
                                        <ul>
                                            <li><strong>Gestão Multidisciplinar:</strong> Atuação em RH, Administração, Almoxarifado, Compras e TI.</li>
                                            <li><strong>Rotinas Administrativas:</strong>
                                                <ul>
                                                    <li>Controle de documentos e planilhas (Excel avançado).</li>
                                                    <li>Gestão de folha de pagamento e registros de ponto.</li>
                                                    <li>Integração de dados entre filiais e matriz.</li>
                                                </ul>
                                            </li>
                                            <li><strong>Suporte Técnico:</strong>
                                                <ul>
                                                    <li>Manutenção de desktops, PDVs e infraestrutura de rede.</li>
                                                    <li>Instalação de softwares e backups de sistemas.</li>
                                                    <li>Configuração de servidores locais.</li>
                                                </ul>
                                            </li>
                                        </ul>
                                    </li>
                                    <li><strong>Ferramentas e Sistemas:</strong>
                                        <ul>
                                            <li>Pacote Office (Excel, Word, Outlook, PowerPoint).</li>
                                            <li>Sistemas ERP corporativos (gestão de estoque e compras).</li>
                                            <li>Ferramentas de RH (controle de ponto digital).</li>
                                            <li>Software de backup e manutenção remota.</li>
                                        </ul>
                                    </li>
                                    <li><strong>Competências Desenvolvidas:</strong>
                                        <ul>
                                            <li>Visão estratégica para otimização de processos.</li>
                                            <li>Capacidade de resolver problemas técnicos e operacionais.</li>
                                            <li>Adaptabilidade entre áreas distintas (de RH a TI).</li>
                                        </ul>
                                    </li>
                                </ul>
                                <div class="results">
                                    <h4><i class="fas fa-chart-line"></i> Resultados</h4>
                                    <ul>
                                        <li>Padronização de 90% dos processos administrativos da filial</li>
                                        <li>Redução de 30% no tempo de processamento de folha de pagamento</li>
                                        <li>Implementação de sistema de backup que evitou perda crítica de dados</li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    
    <footer>
        <div class="container">
            <p>Anderson Caetano - Desenvolvedor Full Stack | Front-end Specialist</p>
            <p>© 2024 - Todos os direitos reservados</p>
        </div>
    </footer>
    
    <script>
        function toggleFilter(id) {
            const content = document.getElementById(id);
            const button = document.querySelector(`button[onclick="toggleFilter('${id}')]`);
            
            content.classList.toggle('show');
            button.classList.toggle('active');
        }
        
        // Initialize all filter contents as shown except presentation letter
        document.addEventListener('DOMContentLoaded', function() {
            const filterContents = document.querySelectorAll('.filter-content');
            filterContents.forEach(content => {
                if (content.id !== 'presentation-letter') {
                    content.classList.add('show');
                }
            });
        });
    </script>
</body>
</html>
