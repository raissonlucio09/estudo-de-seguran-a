# Tipos de RAIDs e tipos de clusters

RAID (Redundant Array of Independent Disks) é um conjunto de discos independentes que trabalham juntos como uma única unidade lógica, para aumentar o desempenho e a tolerância a falhas. Clusters usam vários servidores para aumentar a disponibilidade.

Conceitos
- Termos: array (conjunto de discos), hot spare (disco reserva pronto para uso), rebuild (reconstrução do disco que falhou) e HDC (conectar e desconectar HDs a quente)
- RAID por hardware (placa controladora, melhor desempenho, mais caro) ou por software (feito pelo sistema operacional, mais barato e mais lento)
- Cluster: conjunto de servidores (nós) que parecem um só para o usuário
- Failover: o sistema assume sozinho, sem intervenção humana, quando um servidor falha

 Exemplos e lugares aplicados
Servidores que usam RAID 1 para o sistema operacional e RAID 5 para os dados, clusters de banco de dados e de servidores web.

 Minhas anotações da aula

| Nível | Como funciona | Mínimo de discos | Ponto principal |
|---|---|---|---|
| RAID 0 (striping) | divide os dados entre os discos | 2 | alto desempenho, mas sem proteção: se um disco falha, perde tudo |
| RAID 1 (mirroring) | espelha os dados | 2 | redundância, mas desperdiça 50% do espaço |
| RAID 0+1 e 1+0 | combina striping e espelhamento | 4 | bom desempenho e redundância; no 1+0 suporta a perda de até metade dos discos, se não for os dois do mesmo espelho |
| RAID 5 | dados e paridade distribuídos entre os discos | 3 | recupera dados de um disco que falhou; leitura mais rápida que o RAID 1 |
| RAID 1 + 5 | RAID 1 para o sistema e RAID 5 para os dados | 5 | muito usado em servidores |

- Depois de configurar o RAID, é preciso testar simulando a falha de um disco. Antes de trocar um disco com defeito, fazer backup, e o equipamento deve ter alertas sonoros, luminosos ou de sistema.
- Cluster ativo/passivo: o segundo servidor só entra quando o principal falha. Ativo/ativo: os dois dividem as requisições. Os nós têm pelo menos duas placas de rede, uma rede privada entre eles e um software de gerenciamento.
- Tipos de cluster: de alta disponibilidade (HA), de balanceamento de carga (load balancing) e a combinação dos dois.
