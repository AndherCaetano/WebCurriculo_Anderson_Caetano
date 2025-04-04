<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Anderson Caetano - Desenvolvedor Full Stack</title>
    <style>
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #3498db;
            --accent-color: #e74c3c;
            --light-color: #ecf0f1;
            --dark-color: #2c3e50;
            --text-color: #333;
            --text-light: #7f8c8d;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            line-height: 1.6;
            color: var(--text-color);
            background-color: #f5f5f5;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            background-color: var(--primary-color);
            color: white;
            padding: 20px 0;
            text-align: center;
            border-bottom: 5px solid var(--secondary-color);
        }
        
        header h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }
        
        header p {
            font-size: 1.2rem;
            opacity: 0.9;
        }
        
        .contact-info {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 15px;
        }
        
        .contact-info a {
            color: white;
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 5px;
        }
        
        .contact-info a:hover {
            color: var(--secondary-color);
        }
        
        .main-content {
            display: grid;
            grid-template-columns: 1fr;
            gap: 30px;
            margin-top: 30px;
        }
        
        @media (min-width: 768px) {
            .main-content {
                grid-template-columns: 1fr 2fr;
            }
        }
        
        .sidebar {
            background-color: white;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        
        .content {
            background-color: white;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        
        h2 {
            color: var(--primary-color);
            margin-bottom: 15px;
            padding-bottom: 10px;
            border-bottom: 2px solid var(--secondary-color);
        }
        
        h3 {
            color: var(--dark-color);
            margin: 15px 0 10px;
        }
        
        .section {
            margin-bottom: 25px;
        }
        
        .job, .education {
            margin-bottom: 20px;
        }
        
        .job-header, .education-header {
            display: flex;
            justify-content: space-between;
            margin-bottom: 5px;
        }
        
        .job-title, .education-title {
            font-weight: bold;
            color: var(--primary-color);
        }
        
        .job-period, .education-period {
            color: var(--text-light);
            font-style: italic;
        }
        
        .job-company, .education-institution {
            font-weight: bold;
            color: var(--secondary-color);
        }
        
        ul {
            padding-left: 20px;
        }
        
        li {
            margin-bottom: 5px;
            text-align: justify;
        }
        
        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }
        
        .skill-tag {
            background-color: var(--light-color);
            padding: 5px 10px;
            border-radius: 20px;
            font-size: 0.9rem;
        }
        
        .filter-section {
            margin-bottom: 20px;
        }
        
        .filter-btn {
            background-color: var(--secondary-color);
            color: white;
            border: none;
            padding: 8px 15px;
            border-radius: 5px;
            cursor: pointer;
            display: flex;
            align-items: center;
            gap: 5px;
            margin-bottom: 10px;
            width: 100%;
            text-align: left;
        }
        
        .filter-btn:hover {
            background-color: var(--primary-color);
        }
        
        .filter-btn .arrow {
            transition: transform 0.3s;
            margin-left: auto;
        }
        
        .filter-btn.active .arrow {
            transform: rotate(180deg);
        }
        
        .filter-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease-out;
        }
        
        .filter-content.show {
            max-height: 1000px;
        }
        
        .presentation-letter {
            text-align: justify;
            line-height: 1.6;
        }
        
        .presentation-letter p {
            margin-bottom: 15px;
        }
        
        .presentation-letter ul {
            margin-bottom: 15px;
        }
        
        .presentation-letter li {
            margin-bottom: 8px;
        }
        
        .signature {
            font-style: italic;
            margin-top: 20px;
        }
        
        footer {
            text-align: center;
            padding: 20px;
            background-color: var(--primary-color);
            color: white;
            margin-top: 30px;
        }
        
        @media (max-width: 768px) {
            header h1 {
                font-size: 2rem;
            }
            
            .job-header, .education-header {
                flex-direction: column;
            }
            
            .job-period, .education-period {
                margin-top: 5px;
            }
        }
        
        @media (max-width: 480px) {
            header h1 {
                font-size: 1.8rem;
            }
            
            .contact-info {
                flex-direction: column;
                align-items: center;
                gap: 10px;
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
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" viewBox="0 0 16 16">
                        <path d="M.05 3.555A2 2 0 0 1 2 2h12a2 2 0 0 1 1.95 1.555L8 8.414.05 3.555ZM0 4.697v7.104l5.803-3.558L0 4.697ZM6.761 8.83l-6.57 4.027A2 2 0 0 0 2 14h12a2 2 0 0 0 1.808-1.144l-6.57-4.027L8 9.586l-1.239-.757Zm3.436-.586L16 11.801V4.697l-5.803 3.546Z"/>
                    </svg>
                    andersonsilcaetano@icloud.com
                </a>
                <a href="tel:+5521980081646">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" viewBox="0 0 16 16">
                        <path d="M3.654 1.328a.678.678 0 0 0-1.015-.063L1.605 2.3c-.483.484-.661 1.169-.45 1.77a17.568 17.568 0 0 0 4.168 6.608 17.569 17.569 0 0 0 6.608 4.168c.601.211 1.286.033 1.77-.45l1.034-1.034a.678.678 0 0 0-.063-1.015l-2.307-1.794a.678.678 0 0 0-.58-.122l-2.19.547a1.745 1.745 0 0 1-1.657-.459L5.482 8.062a1.745 1.745 0 0 1-.46-1.657l.548-2.19a.678.678 0 0 0-.122-.58L3.654 1.328zM1.884.511a1.745 1.745 0 0 1 2.612.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.678.678 0 0 0 .178.643l2.457 2.457a.678.678 0 0 0 .644.178l2.189-.547a1.745 1.745 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.634 18.634 0 0 1-7.01-4.42 18.634 18.634 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877L1.885.511z"/>
                    </svg>
                    +55 21 98008-1646
                </a>
                <a href="#" target="_blank">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" viewBox="0 0 16 16">
                        <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
                    </svg>
                    GitHub
                </a>
                <a href="#" target="_blank">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" viewBox="0 0 16 16">
                        <path d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854V1.146zm4.943 12.248V6.169H2.542v7.225h2.401zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248-.822 0-1.359.54-1.359 1.248 0 .694.521 1.248 1.327 1.248h.016zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016a5.54 5.54 0 0 1 .016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225h2.4z"/>
                    </svg>
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
                    <h2>Habilidades Técnicas</h2>
                    <div class="skills">
                        <span class="skill-tag">HTML5</span>
                        <span class="skill-tag">CSS3</span>
                        <span class="skill-tag">JavaScript</span>
                        <span class="skill-tag">PHP</span>
                        <span class="skill-tag">Laravel</span>
                        <span class="skill-tag">CMS Personalizado</span>
                        <span class="skill-tag">AWS</span>
                        <span class="skill-tag">Git/GitHub</span>
                        <span class="skill-tag">Zendesk</span>
                        <span class="skill-tag">Freshdesk</span>
                        <span class="skill-tag">Salesforce</span>
                        <span class="skill-tag">APIs</span>
                        <span class="skill-tag">Webhooks</span>
                        <span class="skill-tag">UX/UI Design</span>
                        <span class="skill-tag">SEO</span>
                        <span class="skill-tag">Redes</span>
                        <span class="skill-tag">VOIP</span>
                        <span class="skill-tag">Windows Server</span>
                        <span class="skill-tag">Linux</span>
                        <span class="skill-tag">MySQL</span>
                        <span class="skill-tag">Excel Avançado</span>
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
                <div class="section filter-section">
                    <button class="filter-btn" onclick="toggleFilter('presentation-letter')">
                        <span>Carta de Apresentação</span>
                        <span class="arrow">▼</span>
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
                        <span class="arrow">▼</span>
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
                        
                        <div class="job">
                            <div class="job-header">
                                <span class="job-title">Analista de Suporte e SAC</span>
                                <span class="job-period">Jun/2016 – Jan/2018 (Home Office)</span>
                            </div>
                            <div class="job-company">Seguradora Líder DPVAT (Home Agent)</div>
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
                        </div>
                        
                        <div class="job">
                            <div class="job-header">
                                <span class="job-title">Suporte Técnico Oi Fibra</span>
                                <span class="job-period">Jun/2013 – Jan/2016 (Presencial)</span>
                            </div>
                            <div class="job-company">Contax/Liq S/A</div>
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
                        </div>
                        
                        <div class="job">
                            <div class="job-header">
                                <span class="job-title">Analista de BackOffice</span>
                                <span class="job-period">Jun/2010 – Jan/2013 (Presencial)</span>
                            </div>
                            <div class="job-company">Contax/Liq S/A</div>
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
                        </div>
                        
                        <div class="job">
                            <div class="job-header">
                                <span class="job-title">Administrativo Geral</span>
                                <span class="job-period">Fev/1999 – Set/2009 (Presencial)</span>
                            </div>
                            <div class="job-company">GPA – Grupo Pão de Açúcar</div>
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
