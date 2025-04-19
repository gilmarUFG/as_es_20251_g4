# Atividade Prática 1 - Aula 2 - 17/04/2025

### Discentes
1. Christopher (201802758);
2. Felipe Moreira Silva (202201689);
3. Frederico Garcez Rodrigues (202201690);
4. Joseppe Pedro Cunha Fellini (202300194);
5. Mauro Sérgio do Nascimento Júnior (202204842);

### Problema
A proposta de sistema é para o desenvolvimento de um software de gerenciamento de reservas de livros em uma biblioteca escolar, com o objetivo de otimizar o processo de empréstimo e devolução de livros, garantindo que o controle seja eficiente e acessível para todos os envolvidos (bibliotecários, alunos, professores e diretores). Este sistema visa melhorar a organização e a experiência do usuário, além de proporcionar maior agilidade e precisão na gestão dos recursos bibliográficos.

### Requisitos Funcionais
**RF001** - O software deve possibilitar a busca de qualquer tipo de título. A busca deve ser abrangente e considerar: nome do livro, autor, editora, edição, categoria e até mesmo descrição.

**RF002** - O software deve possibilitar ao aluno visualizar todos os livros mesmo aqueles que já estão reservados, porém informando-o que o livro visualizado já foi reservado sem informar quem o reservou.

**RF003** - O software deve possibilitar o pagamento de multas pendentes para os locadores de livros, assim como a anexação de pagamentos presenciais.

**RF004** - O software deve possibilitar o registro de livros com título, autor, editora, categoria.

**RF005** - O software deve possibilitar autenticação para identificação de ação de locadores e administradores.

**RF006** - O sistema deve notificar o sucesso das operações de reserva.

### Requisitos de Qualidade:
**RQ001** - O sistema deve funcionar de forma consistente em dispositivos móveis.

**RQ002** - O sistema deve garantir a integridade dos dados.

**RQ003** - O sistema deve possuir uma interface intuitiva e acessível para diferentes perfis de usuários.

**RQ004** - O sistema deve manter a segurança dos dados de acordo com regras de compliance vigentes.

**RQ005** - O sistema deve ser tolerante a falhas, conseguindo manter os dados mesmo em contextos adversos de hardware ou software, minimizando o downtime.

**RQ006** - A busca por livros deve ter um tempo de resposta limite de 200 ms.

### Matriz de Mapeamento de Requisitos de Qualidade

|Requisito Funcional|Requisito de Qualidade|
|--|--|
|RF001|RQ003|
|RF002|RQ002|
|RF003|RQ004|
|RF005|RQ004|
|RF001|RQ006|
|RF006|RQ002|
|RF006|RQ003|
