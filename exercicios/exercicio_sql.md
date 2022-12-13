Exercício 1

Criar um banco de dados com as 3 tabelas:
1. Cliente
   Campos
      - Nome
      - Sobrenome
      - CPF
      - EnderecoID

2. Endereco
   Campos
     - Tipo (rua, avenida, quadra)
     - Logradouro
     - Numero
     - Bairro
     - CEP
     - Cidade
     - Estado
     - ClienteID

3. Produto
   Campos
     - Produto
     - Preco
     - ClienteID

## Premissas
- As tabelas devem ser de primary id auto incrementado;
- Deve existir um relacionamento de 1->N (de 1 para muitos) entre a tabela Cliente e a tabela Endereco (ou seja, um cliente pode ter vários endereços);
- Deve existir um relacionamento de 1->N (de 1 para muitos) entre a tabela Cliente e a tabela Produto (ou seja, um cliente pode ter vários produtos);
- Um produto só pode ter um cliente vinculado a ele;
- Um endereço só pode ter um cliente vinculado a ele;
- O CPF da tabela Cliente deve ser único nela (ou seja, não podemos ter 2 clientes com o mesmo CPF);
- O preço do produto não pode ser negativo;
- O campo Tipo da tabela Endereco só pode receber dados como rua, avenida ou quadra; algo diferente disso não pode permitir persistir na tabela.

## Vocabulários
Persistir = salvar, armazenar, guardar na tabela, etc.
Constraints = validação de dados, verificar se um dado está de acordo com a regra implementada;
1->N = relação 1 para muitos
1->1 = relação 1 para 1
N->N = relação muitos para muitos (ver imagem)
