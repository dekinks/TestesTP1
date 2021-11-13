# Cliente - Testes TP1

O cliente de testes realiza alguns dos testes básicos que serão executados durante a avaliação do seu trabalho. Observe que durante a avaliação, poderão ser executados testes adicionais.

A entrada e saída de cada caso de teste executado se encontram nos diretórios tests/in/ e tests/out/, respectivamente.

Cada caso de teste é executado usando tanto IPv4 quanto IPv6. Além disso, são avaliados dois possíveis cenários:

- single_msg_single_pkg: cenário onde cada mensagem é, provavelmente, enviada em apenas um pacote (pode ser recebida pelo servidor em apenas um recv).
- single_msg_multiple_pkg: cenário onde cada mensagem será enviada em mais de um pacote (a mensagem deve ser recebida pelo servidor por mais de um recv).

## Execução

O programa de testes foi desenvolvido em Python3. Para executá-lo:

`python3 run_tests.py <server> <port>`

onde <server> é o caminho para o executável do seu servidor e <port> é a porta na qual ele deve ser executado.

Exemplo:

`python3 run_tests.py /home/aluno/servidor 9999`
