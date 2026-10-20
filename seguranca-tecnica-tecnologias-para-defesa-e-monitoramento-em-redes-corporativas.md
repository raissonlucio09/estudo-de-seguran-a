# Segurança técnica - tecnologias para defesa e monitoramento em redes corporativas

Como não existe segurança 100%, os componentes de segurança precisam interagir entre si para reduzir a chance de erros e incidentes. Este tópico trata de hash, assinatura e certificado digital, PKI, VLAN e segurança de redes sem fio.

## Conceitos
- Hash: função unidirecional que gera um resumo de tamanho fixo (MD5: 128 bits, SHA: 160 bits). Garante a integridade
- Assinatura digital: código que identifica o autor da mensagem em meio digital
- Autoridade Certificadora (CA, "cartório digital"): emite certificados digitais
- Certificado digital: chave pública assinada por uma CA, que atesta que a chave pertence a uma pessoa ou empresa (padrão X.509)
- CRL: lista de certificados revogados
- PKI (infraestrutura de chaves públicas): infraestrutura que habilita aplicações seguras
- VLAN: rede local virtual que isola grupos de computadores
- Redes sem fio: WEP, WPA (Personal e Enterprise), Rogue AP, VPN, filtro de MAC

## Exemplos e lugares aplicados
Conferir o hash de um arquivo baixado, navegador que valida o certificado de uma loja virtual, Wi-Fi corporativo com servidor RADIUS.

## Minhas anotações da aula
- Hash: fácil de calcular e difícil de inverter, como resumir um livro. Mudar um único caractere muda todo o resultado. Exemplo: MD5 de "Gabriella" = 88f418d385fe30d5a2bfd3e17c732b28 e de "Gabriela" = 3045c3c6443d58c4e72e76fbcbcb2df3.
- Usos do hash: o resumo é enviado junto com a mensagem, e o destinatário calcula de novo e compara; se for diferente, a mensagem foi alterada. Também serve para conferir arquivos baixados.
- Observação: hoje MD5 e SHA-1 não são mais considerados seguros, porque já foram encontradas colisões. Usa-se SHA-256 ou mais forte.
- Certificado digital: contém versão, número de série, algoritmo, emissor, validade, dados do usuário, chave pública e assinatura da CA. Quando vence, a CA o atualiza ou o coloca na CRL. Também pode ser revogado se o usuário sair do domínio, perder a chave privada ou houver suspeita de ataque.
- PKI: reúne autoridade certificadora, diretório, políticas, certificados, chaves, criptografia e assinatura digital. O navegador aceita o site se a CA estiver na sua lista de confiáveis; senão, avisa o usuário.
- VLAN: o tráfego de uma VLAN não pode ser "escutado" por outra. A comunicação entre elas só acontece por um roteador, onde se aplicam as regras de segurança.
- Redes sem fio: o sinal se propaga em todas as direções e pode ser captado fora da empresa (um Access Point alcança até cerca de 300 m). Ameaças: vazamento de informações, acesso não autorizado, interrupção do serviço e acesso indevido à internet.
- Rogue AP: Access Point instalado sem permissão dos administradores.
- WEP: protocolo original do IEEE 802.11, considerado fraco porque usa a mesma chave para todos e não autentica o usuário.
- WPA: usa chave dinâmica e criptografia única por usuário. WPA-Personal (WPA-PSK) é a versão doméstica, com chave compartilhada. WPA-Enterprise (WPA-RADIUS) usa um servidor RADIUS para autenticar. A principal vulnerabilidade é o uso de senhas curtas e fáceis. Hoje se usa WPA2 ou WPA3 (complemento, não está no material).
- Proteções extras: VPN na conexão sem fio e filtro de endereço MAC.
- Dicas para o Access Point: ativar a criptografia, alterar o SSID e desabilitar o broadcast dele, filtrar MAC, mudar parâmetros SNMP padrão, usar senhas, analisar o tráfego, atualizar o software, padronizar os dispositivos clientes, gerenciar de forma centralizada e desabilitar a administração pela rede sem fio.
