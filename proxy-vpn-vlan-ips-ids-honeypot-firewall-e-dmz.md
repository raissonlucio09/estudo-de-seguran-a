# PROXY, VPN, VLAN, IPS, IDS, HONEYPOT, FIREWALL E DMZ

São tecnologias de segurança lógica que reduzem acessos indevidos e o uso da rede por pessoas sem autorização, protegendo a troca de dados entre os computadores.

 Conceitos
- Firewall: fica entre a rede interna e a externa, isolando e controlando o acesso (hardware ou software)
- IDS (Sistema de Detecção de Intrusão): identifica atividades suspeitas. HIDS (no servidor) e NIDS (no segmento da rede)
- IPS (Sistema de Prevenção de Intrusão): além de detectar, bloqueia o ataque (não detalhado no material)
- VPN (Virtual Private Network): túnel criptografado pela internet
- Proxy: "procurador" que acessa a internet em nome dos usuários internos
- Honeypot: sistema-isca para atrair e estudar atacantes
- DMZ (zona desmilitarizada): segmento acessível de fora, sem dados críticos
- VLAN: rede virtual isolada dentro da rede física (veja o tópico de Segurança técnica)

Exemplos e lugares aplicados
Firewall na fronteira da empresa, VPN para o funcionário remoto e para ligar filiais, proxy que bloqueia sites e registra os acessos, servidor web na DMZ e banco de dados na zona interna.

 Minhas anotações da aula
- Firewall: comparado a um muro com portas. Cada porta nova facilita o acesso, mas também precisa de controle. Controla por serviço, sentido, usuário e comportamento, e registra o tráfego.
- IDS: o HIDS gera poucos falsos positivos e vê o comportamento das aplicações da máquina. O NIDS gera mais falsos positivos e fica perto de roteadores e firewalls analisando pacotes, mas não vê ataques feitos direto na máquina. Nenhum IDS protege 100%, mas diminui o risco.
- VPN: reduz custos de links dedicados e conecta filiais, parceiros e funcionários em casa. O túnel voluntário é criado pelo software do usuário. O túnel compulsório é criado pelos equipamentos da rede, sem software no cliente.
- Proxy: guarda respostas em cache, centraliza e controla o uso da internet (sites permitidos, horários, grupos), registra os acessos e protege as máquinas internas do contato direto com a internet.
- Honeypot: como não tem serviço real, qualquer interação com ele indica sondagem ou acesso não autorizado. De produção: distrai atacantes e alerta o IDS. De pesquisa: estuda o comportamento e as ferramentas dos atacantes.
- DMZ: hospeda equipamentos que recebem conexões externas. A zona interna guarda bancos de dados, senhas, cadastros e sistemas críticos e só deve ser acessada por usuários autorizados.
