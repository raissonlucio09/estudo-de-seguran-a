# Métodos para garantir redundância nos ambientes corporativos

Tolerância a falhas (fault tolerance) é manter o serviço funcionando mesmo com a presença de uma falha. Ela aumenta a disponibilidade dos ativos de TI de que os processos de negócio dependem.

 Conceitos
- Falha (fault): problema, defeito ou erro. As falhas são inevitáveis, porque os componentes envelhecem, se desgastam e sofrem interferências
- Falhas comuns: queda de energia, falha de switch ou roteador, defeito de hardware do servidor, falha de software ou vírus, problemas no data center (desastres, incêndio, ações criminosas)
- Disponibilidade medida em "noves"
- Níveis: disponibilidade básica, alta disponibilidade e disponibilidade contínua
- Replicação de dados, virtualização e uso de SLA com terceiros

 Exemplos e lugares aplicados
Segunda fonte de energia no servidor, segundo link de internet, segunda placa de rede, sistemas de UTI e satélites (que não podem parar).

 Minhas anotações da aula
Indisponibilidade aproximada por nível de disponibilidade:

| Disponibilidade | Indisponibilidade por ano |
|---|---|
| 90% (um nove) | cerca de 36,5 dias |
| 99% (dois noves) | cerca de 3,65 dias (7,2 h por mês) |
| 99,9% (três noves) | cerca de 9 horas |
| 99,99% (quatro noves) | cerca de 50 minutos |

- Quanto mais noves, mais recursos de redundância são necessários e mais cara fica a solução.
- Básica (três noves): sistemas que podem parar um curto período sem grande impacto. Alta: sistemas críticos, com um segundo equipamento que assume sem intervenção humana. Contínua (quatro noves ou mais): sistemas cuja parada afeta muita gente.
- Equipamentos de apoio (nobreaks, geradores, ar-condicionado) também precisam de capacidade extra e reserva.
- Quando a empresa terceiriza, define as metas no SLA (Acordo de Nível de Serviço), com métricas como MTTF (tempo até a primeira falha), MTTR (tempo médio de reparo) e MTBF (tempo médio entre falhas).
- O processo deve ser contínuo, seguindo o ciclo PDCA: planejar (Plan), implementar (Do), monitorar (Check) e melhorar (Action).
