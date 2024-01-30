README - Controle Financeiro Simples
Este é um projeto simples de sistema de gerenciamento de transações que permite criar, editar e excluir transações financeiras. O sistema é construído utilizando HTML, JavaScript e faz uso de uma API RESTful para persistência de dados.

Funcionalidades
1. createTransactionContainer(id)
Esta função cria um contêiner HTML para uma transação com base no ID fornecido. O contêiner recebe a classe "transaction" e um ID único composto por "transaction-" seguido do ID fornecido.

2. createTransactionTitle(name)
Cria um elemento HTML span para representar o título de uma transação. O texto do título é definido com base no nome da transação.

3. createTransactionAmount(amount)
Cria um elemento HTML span para representar o valor de uma transação. O valor é formatado como moeda brasileira (BRL) e exibe "C" para créditos e "D" para débitos.

4. createEditTransactionBtn(transaction)
Cria um botão de edição para uma transação específica. Ao ser clicado, preenche os campos do formulário com os detalhes da transação para edição.

5. createDeleteTransactionBtn(id)
Cria um botão de exclusão para uma transação específica. Ao ser clicado, realiza uma requisição para a API RESTful para excluir a transação e atualiza a interface.

6. renderTransaction(transaction)
Renderiza visualmente uma transação, criando e adicionando os elementos HTML correspondentes ao contêiner de transação.

7. saveTransaction(ev)
Função chamada ao enviar o formulário de transação. Realiza uma requisição à API RESTful para salvar ou editar uma transação, e atualiza a interface de acordo.

8. fetchTransactions()
Realiza uma requisição à API RESTful para obter a lista de transações existentes.

9. updateBalance()
Calcula e atualiza o saldo total com base nas transações existentes, exibindo-o na interface.

10. setup()
Função de inicialização que obtém as transações existentes e as renderiza na interface.

Instruções de Uso
Abra o arquivo index.html em um navegador web.
O sistema carregará as transações existentes da API e exibirá na interface.
Utilize o formulário para adicionar ou editar transações.
Cada transação exibirá botões de edição e exclusão para ações adicionais.
Certifique-se de configurar uma API RESTful para manipular as operações CRUD do sistema. No exemplo fornecido, a API está configurada localmente em http://localhost:3000/transactions.

Lembre-se de adaptar o código para atender às necessidades específicas do seu projeto, como o endpoint da API, estilos e outras personalizações desejadas.
