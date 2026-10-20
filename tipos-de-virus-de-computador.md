 # Tipos de vírus de computador: Worm, Trojan, Hoax, Backdoor e outros

Vírus de computador é um programa autorreplicante que se anexa a outros programas para se espalhar. Vírus e programas parecidos geram grande carga de trabalho para o administrador de redes.

 Conceitos
- Vírus de boot: infecta a área de inicialização de discos e mídias e pode impedir o login
- Trojan (cavalo de troia): fica escondido dentro de um programa aparentemente inofensivo
- Worm: não precisa de programa hospedeiro, é autossuficiente e se espalha pela rede
- Hoax: boato que leva o próprio usuário a causar o dano (não é vírus de fato)
- Vírus de macro: usa macros do Word e do Excel
- Backdoor: "porta dos fundos" que permite acesso remoto não autorizado (não é detalhado no material da aula)
- Malwares: spyware, adware, hijacker, keylogger e screenlogger
- Antivírus: compara os arquivos com uma biblioteca de assinaturas de vírus

 Exemplos e lugares aplicados
Vírus famosos: Melissa, I Love You, Nimda e Code Red.

 Minhas anotações da aula
- Efeitos: lentidão, alteração e exclusão de arquivos, mensagens indesejadas, captura de teclas, abertura de portas para acesso externo, reprodução ilimitada e indisponibilidade de computadores.
- Como entravam: antes, por disquetes; depois, por redes, e-mail, internet, downloads de executáveis (.exe, .bat, .com) e macros do Office. Falhas de política, como usuários no grupo de administrador da máquina, facilitam a infecção.
- Vírus famosos:
  - Melissa: se espalhava por e-mail e mandava cópias para os 50 primeiros contatos.
  - I Love You: worm que fazia cópias de si mesmo e alterava o registro do sistema.
  - Nimda (admin ao contrário): atacava servidores para deixar o tráfego da web lento.
  - Code Red e Code Red II: worms de 2001 que exploravam falha de estouro de buffer no Windows 2000 e NT.
- Assinatura: sequência de caracteres que cada vírus deixa e que o antivírus reconhece. O antivírus pode bloquear, colocar em quarentena, apagar ou isolar o arquivo.
- Malwares: spyware monitora o uso do computador; adware mostra anúncios e monitora a navegação; hijacker altera o comportamento do navegador; keylogger guarda o que é digitado e envia ao atacante; screenlogger captura a tela e a posição do mouse nos cliques.
- Solução corporativa: um servidor de antivírus baixa as assinaturas novas e distribui para as estações, e um agente em cada estação consulta o servidor de tempos em tempos. O administrador deve conferir se a atualização funcionou (falhas de comunicação, bugs, agente com problema ou usuário que desabilita o antivírus).
