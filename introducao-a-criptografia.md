# Introdução à criptografia

Criptografia é a técnica de transmitir informações de forma codificada para que, se forem interceptadas, não possam ser lidas por quem não tem autorização. Contribui principalmente para a confidencialidade e a integridade.

## Conceitos
- Criptografar (encriptar): transformar o texto simples em texto cifrado, com um algoritmo e uma chave. Descriptografar: o processo inverso
- Chave: informação necessária para cifrar e decifrar
- Criptoanálise: ciência que tenta quebrar sistemas criptográficos sem conhecer a chave
- A segurança depende da força do algoritmo e da chave
- Técnicas básicas: cifra de transposição (muda a ordem das letras) e cifra de substituição (troca as letras por outras)
- Criptografia simétrica: uma mesma chave cifra e decifra
- Criptografia assimétrica: par de chaves, pública e privada

## Exemplos e lugares aplicados
Máquina Enigma na Segunda Guerra Mundial, Cifra de César, proteção de dados em notebooks e de comunicações na internet.

## Minhas anotações da aula
- Transposição: UNINOVE vira INVEOUN (as letras são preservadas, mudam de posição). Substituição: trocando cada letra pela seguinte, UNINOVE vira VOJOPWF.
- Cifra de César: substituição por deslocamento, em que a chave é o número de posições. Com chave 3, AMOR vira DPRU.
- Simétrica:
  - Vantagens: fácil de usar e rápida.
  - Desvantagens: a chave precisa ser compartilhada e pode ser interceptada, e é preciso uma chave para cada pessoa. A solução é enviar a chave por outro canal.
  - Exemplos: DES (56 bits), 3DES (112 ou 168 bits), IDEA (128 bits), RC2 e RC4. Hoje o padrão mais usado é o AES (complemento, não está no material).
- Assimétrica:
  - A chave pública cifra e pode ser divulgada; a chave privada decifra e fica em segredo. Das duas chaves, uma não revela a outra.
  - Exemplo: Gabriela cifra a mensagem com a chave pública do Édison, e só o Édison, com a chave privada, consegue abrir. Mesmo quem cifrou não consegue decifrar.
  - Não precisa de canal seguro para trocar chaves.
  - Exemplos: RSA (Rivest, Shamir e Adleman), ElGamal, Diffie-Hellman (troca de chaves) e curvas elípticas.
- Uma criptografia é computacionalmente segura quando o custo e o tempo para quebrá-la superam o valor e a vida útil da informação.
