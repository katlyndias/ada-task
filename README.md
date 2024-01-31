# Projeto final do módulo de Programação Orientada a Objetos II do B3 Programa Devª da Ada Tech.
--- 
# Instruções de Execução - AdaTask
Para utilizar o AdaTask, siga as instruções abaixo:

## Pré-requisitos
Certifique-se de que você possui o Java instalado em seu sistema. Você pode baixar a versão mais recente em https://www.java.com/en/ 

## Passos para Execução
- Clone o Repositório;
- Acesse o Diretório do Projeto;
- Compile o Código;
- Execute o Aplicativo;
- Interaja com o AdaTask, seguindo as instruções exibidas no console para criar, editar, excluir e visualizar tarefas. Utilize os comandos fornecidos para navegar pelas opções disponíveis.
- Encerre a Execução seguindo as instruções no console ou utilize o comando apropriado.
  
## Observações
- Certifique-se de inserir as informações solicitadas de acordo com o formato especificado durante a interação com o aplicativo.
- O aplicativo funciona em um ambiente de console, proporcionando uma experiência simples e direta.
- Aproveite o AdaTask para um gerenciamento eficiente e organizado de suas tarefas pessoais e profissionais!

--- 
# AdaTask - Aplicativo de Gerenciamento de Tarefas via Console
## Descrição Geral
O AdaTask é um aplicativo de console desenvolvido para facilitar o gerenciamento de tarefas, permitindo aos usuários criar, editar, excluir e visualizar suas tarefas pessoais e profissionais. O aplicativo realiza a simulação de um banco de dados por meio de listas em memória, proporcionando uma experiência simples, intuitiva e eficiente, e não permite a criação de tarefas com datas no passado.

## Estrutura do Projeto
- Camada de Domínio: No núcleo do projeto, a camada de domínio contém classes essenciais, como BaseTask, PersonalTask, WorkTask e StudyTask. Essas classes definem a estrutura e as regras de negócios que envolvem as tarefas gerenciadas pelo aplicativo.

- Camada de Repositório: A camada de repositório é responsável pela "persistência" dos dados, utilizando listas para armazenar as informações das tarefas. Esta camada oferece métodos para adicionar, remover, atualizar e buscar tarefas, garantindo a integridade e a eficiência na manipulação dos dados.

- Camada de Serviço: Com a lógica de aplicação concentrada na camada de serviço, as operações de manipulação de tarefas são gerenciadas de forma eficaz. Essa camada interage diretamente com o repositório, executando as operações necessárias para garantir a consistência dos dados.

- Camada de Controlador: O controlador atua como intermediário entre o usuário e o sistema, possibilitando a interação via console. Ele processa os comandos inseridos pelo usuário e utiliza a camada de serviço para realizar as operações correspondentes, garantindo uma experiência de usuário fluida e intuitiva.

## Principais Funcionalidades
- Criação de Tarefas: Adicione novas tarefas com os seguintes detalhes personalizados: id, título, descrição, prazo.
- Edição de Tarefas: Atualize os detalhes de tarefas já existentes.
- Remoção de Tarefas: Exclua as tarefas que não são mais necessárias.
- Visualização de Tarefas: Liste todas as tarefas disponíveis e filtra a que você deseja ver os detalhes pelo id.
- Visualização de Tarefas que vencem no dia de hoje: Liste todas as tarefas que expiram no dia de hoje, caso existentes.

## Implementação Técnica
- Interface de Console: Uma interface de linha de comando simples para facilitar a interação do usuário.
- Classes de Entidade: Utilização da classe BaseTask e suas subclasses para representar diferentes tipos de tarefas.
- Classe de Repositório: Implementação de uma lista para simular o armazenamento de dados.
- Classe de Serviço: Responsável por implementar a lógica de negócios necessária para manipular as tarefas.
- Classe de Controlador: Processa as entradas do usuário e coordena as operações correspondentes.

## Considerações Adicionais
O projeto adere aos princípios SOLID para garantir um design limpo e extensível. Além disso, a aplicação de herança e generics é evidente nas estruturas de dados e nas operações de manipulação de tarefas, proporcionando uma arquitetura flexível e adaptável.
