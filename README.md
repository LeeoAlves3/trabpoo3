# trabpoo3

Classe: Despesa

Atributos:

    descricao (string): Descrição da despesa.
    valor (float): Valor da despesa.
    data_vencimento (date): Data de vencimento da despesa.
    categoria (CategoriaDespesa): Categoria à qual a despesa pertence.
    paga (booleano): Indica se a despesa foi paga.
    data_pagamento (date): Data em que a despesa foi paga, caso aplicável.

Métodos:

    marcar_como_paga(data_pagamento: date): Marca a despesa como paga
    calcular_atraso() -> int: Calcula a quantidade de dias de atraso da despesa em relação à data de vencimento.

Classe CategoriaDespesa

A classe CategoriaDespesa serve como base para as categorias específicas de despesa.

Atributos:

    nome (string): Nome da categoria.

Métodos:

    get_tipo() -> string: Retorna o tipo da categoria

Classe: Usuario

A classe Usuario representa um usuário do sistema.

Atributos:

    login (string): Nome de usuário.
    senha (string): Senha criptografada do usuário.

Métodos:

    atualizar_senha(nova_senha: string): Atualiza a senha do usuário e a armazena criptografada.


Classe: MenuPrincipal

A classe MenuPrincipal controla a exibição e interação com o menu principal do sistema.

Métodos:

    exibir_menu(): Exibe as opções do menu principal.
    processar_opcao(opcao: int): Processa a opção escolhida pelo usuário.

Classe: Criptografia

A classe Criptografia contém métodos para criptografar e comparar senhas.

Métodos:

    criptografar_senha(senha: string) -> string: Retorna a senha criptografada.
    comparar_senhas(senha_digitada: string, senha_armazenada: string) -> booleano: Compara a senha digitada com a senha armazenada.

Classe: Aplicacao

A classe Aplicacao é a classe principal que coordena as funcionalidades do sistema.

Métodos:

    iniciar(): Inicia a execução da aplicação.
    Métodos para executar cada funcionalidade do menu principal.
