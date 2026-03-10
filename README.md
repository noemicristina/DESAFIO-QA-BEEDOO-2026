# DESAFIO-QA-BEEDOO-2026
1. Análise inicial da aplicação:
Durante a análise inicial da aplicação, identifiquei que o sistema é um site de cadastro de cursos, com as funcionalidades principais de:
- Cadastro de cursos, contendo campos obrigatórios como Nome do curso, Instrutor, URL da imagem de capa, Datas de início e fim, Número de vagas, Tipo de curso;
- Diferenciação entre cursos Presenciais e Online, com campos dinâmicos (Endereço para presencial e Link da aula/descrição para online);
- Listagem de cursos, exibindo informações como nome, duração, tipo, imagem, descrição e número de vagas;
- Possibilidade de excluir cursos da lista;
- Mensagens de confirmação após ações como cadastrar curso.


2. Decisões tomadas para criação dos testes:
- Testar todos os campos obrigatórios individualmente: para garantir que cada campo, sozinho ou combinado, seja validado corretamente (ex.: Nome do curso, Instrutor, Número de vagas).
- Validar formatos e tipos de dados: campos como datas, URL e número de vagas foram testados com valores válidos, inválidos, vazios e limites, para evitar entradas incorretas.
- Testar fluxos completos: testes que simulam o cadastro completo de um curso e verificam se ele aparece na lista corretamente, incluindo ordenação dos cursos recém cadastrados.
- Testar ações críticas de usuário: como exclusão de curso, verificando tanto sucesso quanto falha na remoção, garantindo integridade dos dados.
  

3. Explicação do raciocínio durante a análise:
Meu raciocínio seguiu a abordagem de testes de caixa preta, focando no comportamento do sistema do ponto de vista do usuário, sem acesso ao código. Primeiro, identifiquei todas as funcionalidades visíveis da aplicação. Em seguida, listei cenários para cada campo, considerando valores válidos, inválidos, vazios e limites. Para campos dinâmicos, como Tipo de curso, criei testes que garantem que a lógica condicional funciona corretamente (ex.: Endereço aparece só para presencial, Link só para online). Por fim, conectei os testes aos fluxos completos, verificando que ao cadastrar o curso ele é mostrado na lista e que ações críticas como exclusão e mensagens de sucesso funcionam.
