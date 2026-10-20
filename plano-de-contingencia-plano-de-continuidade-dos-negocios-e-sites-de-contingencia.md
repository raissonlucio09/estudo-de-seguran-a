# Plano de contingência, plano de continuidade dos negócios e sites de contingência - Cold site, Warm site e Hot site

Como não existe segurança 100%, a empresa precisa de planos para continuar operando, mesmo que parcialmente, quando um incidente acontece. Isso vai além de alta disponibilidade e backup.

Conceitos
- PCN (Plano de Continuidade dos Negócios), também chamado de BCP: foco nos negócios e nas pessoas durante e depois da interrupção
- BIA (Análise de Impacto nos Negócios): identifica a relevância dos processos e o tempo máximo que a empresa sobrevive sem eles, incluindo impactos financeiros, jurídicos e de imagem
- RTO (Recovery Time Objective): tempo máximo aceitável para o processo voltar a funcionar. RPO (Recovery Point Objective): até que ponto no tempo os dados devem ser restaurados, ligado à frequência do backup
- Sistemas críticos: aqueles cuja indisponibilidade causa perdas irreversíveis financeiras ou jurídicas

 Exemplos e lugares aplicados
Empresas que, no 11 de setembro de 2001, tinham o site de contingência na torre ao lado da principal e ficaram sem condição de operar.

 Minhas anotações da aula
- Subplanos do PCN:
  - PAC (Programa de Administração de Crise): organiza equipes e um centro de comando.
  - PRD ou DRP (Plano de Recuperação de Desastres): focado em TI, restaura o ambiente às condições anteriores ao incidente.
  - PCO (Plano de Continuidade Operacional): reduz o tempo de indisponibilidade dos ativos.
  - Plano de contingência de TI: um para cada aplicação crítica.
  - PCC (Plano de Comunicações de Crise): só declarações aprovadas são divulgadas.
- O PCN também preserva a integridade física dos funcionários. Antes dele devem ser feitas a análise de risco e a BIA.
- Sites alternativos (próprios, contratados, mistos ou por acordo de reciprocidade):

| Tipo | Características |
|---|---|
| Cold site | só a infraestrutura básica (energia, telecomunicações, climatização), sem equipamentos de TI; mais barato, mas difícil de testar e lento para entrar em operação |
| Warm site | parcialmente equipado com os equipamentos mais críticos; recursos precisam ser reconfigurados e os backups restaurados |
| Hot site | cópia idêntica do site principal, com dados replicados; custo alto, mas entra em operação quase na hora |

- Outros: mobile site (variação do hot site em um veículo) e acordo de reciprocidade entre empresas parecidas (o risco é as duas serem afetadas ao mesmo tempo).
