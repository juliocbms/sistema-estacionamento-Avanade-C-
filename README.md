# Sistema de Estacionamento

Este é um projeto simples de sistema de estacionamento em C#, criado para gerenciar veículos estacionados. O sistema permite adicionar, remover e listar veículos, além de calcular o valor a ser pago com base no tempo de permanência.

### Funcionalidades
- **Adicionar Veículo:** Cadastra a placa de um novo veículo no sistema.
- **Remover Veículo:** Remove um veículo, calcula o valor total a ser pago com base no preço por hora e no preço inicial, e exibe o resultado.
- **Listar Veículos:** Exibe a lista de todos os veículos atualmente estacionados.
- **Encerrar:** Sai do programa.

### Tecnologias Utilizadas
- C#
- .NET

### Como Executar o Projeto
1.  **Clone o repositório:**
    ```sh
    git clone [https://github.com/juliocbms/sistema-estacionamento-Avanade-C-.git](https://github.com/juliocbms/sistema-estacionamento-Avanade-C-.git)
    ```
2.  **Navegue até o diretório do projeto:**
    ```sh
    cd sistema-estacionamento-Avanade-C-
    ```
3.  **Rode o projeto:**
    ```sh
    dotnet run
    ```

### Estrutura do Código
O projeto é composto por duas classes principais:
-   `Estacionamento.cs`: Contém a lógica principal do estacionamento, incluindo os métodos para adicionar, remover e listar veículos.
-   `Program.cs`: É o ponto de entrada do programa, responsável por exibir o menu interativo e chamar os métodos da classe `Estacionamento` com base na escolha do usuário.

<img width="440" height="358" alt="diagrama_classe_estacionamento" src="https://github.com/user-attachments/assets/b93f906e-0d63-4ebe-bb93-fe6f424c6ac0" />

A classe contém três variáveis, sendo:

**precoInicial:** Tipo decimal. É o preço cobrado para deixar seu veículo estacionado.

**precoPorHora:** Tipo decimal. É o preço por hora que o veículo permanecer estacionado.

**veiculos:** É uma lista de string, representando uma coleção de veículos estacionados. Contém apenas a placa do veículo.

A classe contém três métodos, sendo:

**AdicionarVeiculo:** Método responsável por receber uma placa digitada pelo usuário e guardar na variável veiculos.

**RemoverVeiculo:** Método responsável por verificar se um determinado veículo está estacionado, e caso positivo, irá pedir a quantidade de horas que ele permaneceu no estacionamento. Após isso, realiza o seguinte cálculo: precoInicial * precoPorHora, exibindo para o usuário.

**ListarVeiculos:** Lista todos os veículos presentes atualmente no estacionamento. Caso não haja nenhum, exibir a mensagem "Não há veículos estacionados".
