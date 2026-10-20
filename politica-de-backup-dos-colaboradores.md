# Política de backup dos colaboradores

Backup é uma cópia de segurança feita para recuperar dados quando necessário. A política de backup define as atividades para proteger os dados da empresa e permitir a continuidade dos negócios depois de um incidente.

## Conceitos
- A política de backup trata de: tecnologia, volume de dados, periodicidade, tempo de guarda, janela de backup, responsáveis, procedimentos, armazenamento e tipos de mídia, custos, replicação, testes de restauração e conscientização dos usuários
- Atributo do arquivo: a maioria dos programas marca um atributo para saber se o arquivo é novo ou foi alterado desde o último backup
- Janela de backup: tempo disponível para executar o backup em um volume de dados
- Cinco tipos de backup: diário, cópia, full (normal), incremental e diferencial

## Exemplos e lugares aplicados
Backup full no domingo e incremental de segunda a sábado, uso de agentes para copiar bancos de dados e correio eletrônico, mídias como fitas, HDs, NAS e SAN.

## Minhas anotações da aula

| Tipo | O que copia | Mexe no atributo? |
|---|---|---|
| Diário | arquivos criados ou alterados no dia | não |
| Cópia | tudo o que foi selecionado | não |
| Full (normal) | tudo o que foi selecionado | sim, desmarca |
| Incremental | só os marcados (novos ou alterados) | sim, desmarca |
| Diferencial | só os marcados (novos ou alterados) | não |

- Estratégia full + incrementais: backup diário rápido, mas para restaurar é preciso o full e todas as fitas incrementais; se uma fita falhar, aquele dia é perdido.
- Estratégia full + diferenciais: o backup cresce a cada dia, mas para restaurar basta o full e o último diferencial.
- O que copiar: depende do valor e da validade da informação, e do impacto da perda. Análise de risco e classificação da informação ajudam.
- Software: os recursos nativos do sistema operacional podem não bastar. Bancos de dados e e-mail precisam de agentes. Verificar se agenda automaticamente, copia arquivos abertos e guarda histórico.
- Observações: testar restaurações (restore) para saber se os dados voltam, guardar mídias em outro local, duplicar dispositivos e centralizar os dados em servidores de arquivos, não nas estações de trabalho.
