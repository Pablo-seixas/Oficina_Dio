# Sistema de Gerenciamento de Oficina Mecânica

Este projeto é um sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica.

![Diagrama do Banco de Dados](https://github.com/Pablo-seixas/Escola_Dio/blob/main/escola.png)

## Descrição

Clientes levam veículos à oficina mecânica para serem consertados ou para passarem por revisões periódicas. Cada veículo é designado a uma equipe de mecânicos que identifica os serviços a serem executados e preenche uma Ordem de Serviço (OS) com data de entrega. A partir da OS, calcula-se o valor de cada serviço, consultando-se uma tabela de referência de mão-de-obra. O valor de cada peça também irá compor a OS. O cliente autoriza a execução dos serviços e a mesma equipe avalia e executa os serviços.

## Entidades

- `Cliente`: Representa um cliente que leva seu veículo à oficina. Cada cliente tem um nome e um endereço, e pode ter vários veículos.
- `Veiculo`: Representa um veículo que é levado à oficina para conserto ou revisão. Cada veículo tem um modelo e um ano, e pode ter várias ordens de serviço associadas a ele.
- `Mecanico`: Representa um mecânico que trabalha na oficina. Cada mecânico tem um código, um nome, um endereço e uma especialidade.
- `OrdemDeServico`: Representa uma ordem de serviço que é criada para cada veículo. Cada ordem de serviço tem um número, uma data de emissão, um valor, um status e uma data para conclusão dos trabalhos. Cada ordem de serviço pode ter vários mecânicos e vários serviços associados a ela.
- `Servico`: Representa um serviço que é executado em um veículo. Cada serviço tem uma descrição e um valor.
- `Peca`: Representa uma peça que é usada em uma ordem de serviço. Cada peça tem um nome e um valor.

## Observações

Este projeto foi criado como parte de um desafio de projeto. As entidades e relacionamentos foram criados com base em uma narrativa fornecida. Algumas suposições foram feitas para preencher lacunas na narrativa.
