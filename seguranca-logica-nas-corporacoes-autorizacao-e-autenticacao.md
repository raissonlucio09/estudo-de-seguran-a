# Segurança lógica nas corporações: métodos para autorização e autenticação

A segurança lógica usa controles "invisíveis" (senhas, permissões, registros) para que, mesmo com acesso físico ao equipamento, uma pessoa sem autorização não consiga usar os dados. Ela se liga à confidencialidade, integridade, autenticidade e rastreabilidade.

 Conceitos
- Acesso lógico: permissão a recursos de informação, controlada por mecanismos como listas de controle de acesso (ACL)
- Identificação: quem é o usuário (nome cadastrado em uma lista)
- Autenticação: prova de que o usuário é quem diz ser
- Autorização: o que o usuário autenticado pode fazer
- Auditoria: registrar e verificar o que foi feito com o acesso (arquivos de log)
- Gestão de Identidades e Acessos (IAM): administrar e controlar a identificação e os acessos dos colaboradores aos sistemas

 Exemplos e lugares aplicados
Login e senha em sistemas, cartões e tokens, biometria, revogar o acesso de ex-funcionários, criptografia de dados em notebooks.

 Minhas anotações da aula
- Autenticação pode usar algo que a pessoa sabe (senha), algo que ela tem (cartão, token) e algo que ela é (biometria). Senha e artefato podem ser adivinhados, perdidos ou emprestados, e a biometria dá mais segurança.
- Perguntas para definir os controles: quem acessa, o que pode fazer, quando, como monitorar e em que horário.
- Níveis da segurança lógica: dados (permissões, criptografia, auditoria), aplicativos e sistemas operacionais (antivírus, anti-keylogger, anti-spyware, backup, atualizações) e ferramentas de defesa (firewall, IDS, VPN, proxy).
- Senhas: senha compartilhada ou fraca (como usar o nome do usuário) é a causa da maior parte das invasões. Boas práticas: combinar letras maiúsculas e minúsculas, números e símbolos, usar frases mnemônicas e trocar letras por símbolos (S por $, E por 3, A por @, O por 0). A empresa deve ter uma política de senhas.
- IAM surgiu com o crescimento das empresas e do número de sistemas interligados. Resolve problemas de controle de acessos e senhas, revisão de acessos quando as pessoas mudam de área e contas privilegiadas de ex-funcionários.
- Vantagens do IAM: mais produtividade para usuários e para TI e suporte, e mais conformidade com as políticas de segurança.
