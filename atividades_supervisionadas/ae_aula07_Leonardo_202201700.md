# :pushpin: Atividade Extraordinária

## :books: Técnicas para Especificação
### :pencil: Entrevista

**Descrição:**

* A entrevista é uma técnica de elicitação de requisitos baseada na interação direta entre o analista de requisitos e os stakeholders (usuários, gerentes, especialistas de domínio, etc.). Consiste em conversas estruturadas (com perguntas definidas), semiestruturadas (com tópicos a abordar) ou não estruturadas (mais aberta e exploratória), onde o analista faz perguntas para compreender o domínio do problema, identificar as necessidades, expectativas e restrições relacionadas ao futuro sistema.

**Cenários de Aplicabilidade:**

* Baixo número de stakeholders: Onde é possível dedicar tempo individual para cada entrevistado.
* Busca por uma compreensão mais profunda: A interação direta permite explorar nuances e tópicos implícitos que dificilmente seriam obtidos por outros meios.
* Para esclarecer informações: Pode ser usada como complemento a questionários ou análise de documentos para aprofundar em pontos específicos.
* Como ponto de partida: As entrevistas exploratórias podem ajudar a delimitar o escopo e identificar os principais desafios.

**Vantagens:**

* Profundidade na coleta de informações: Permite explorar detalhes e obter um entendimento rico do contexto.
* Flexibilidade: O entrevistador pode adaptar as perguntas com base nas respostas, explorando áreas inesperadas.
* Identificação de requisitos implícitos: Conhecimentos não formalizados pelos usuários podem ser descobertos através da conversa.
* Estabelecimento de relacionamento: A interação face a face pode fortalecer a relação entre a equipe de desenvolvimento e os stakeholders.

**Desvantagens:**

* Alto custo e tempo demandado: Especialmente em projetos com muitos stakeholders.
* Subjetividade: A interpretação das respostas pode ser influenciada pela experiência e viés do entrevistador.
* Inconsistências entre entrevistados: Diferentes pessoas podem fornecer informações conflitantes.
* Dificuldade em lidar com um grande volume de informações: A organização e análise das notas de entrevista podem ser trabalhosas.
* Dependência da habilidade do entrevistador: A qualidade dos requisitos obtidos está diretamente ligada à capacidade do analista em conduzir a entrevista.

### :pencil: Casos de Uso

**Descrição:**

* A técnica de Casos de Uso foca na descrição das interações entre os atores (pessoas ou outros sistemas que interagem com o sistema) e o sistema em desenvolvimento para alcançar um objetivo específico. Um Caso de Uso descreve uma funcionalidade completa do sistema do ponto de vista do usuário. É composto por um nome, um ator principal, pré-condições, pós-condições e uma sequência de passos (fluxo principal e fluxos alternativos/de exceção) que detalham a interação.

**Cenários de Aplicabilidade:**

* Especificar requisitos funcionais: Descrevem claramente o que o sistema deve fazer em resposta às ações dos atores.
* Projetos de qualquer tamanho e complexidade: A técnica é escalável e pode ser adaptada a diferentes portes de projeto.
* Facilitar a comunicação: A linguagem dos casos de uso é geralmente mais acessível para usuários sem conhecimento técnico aprofundado.
* Base para os testes: Os fluxos dos casos de uso servem como base para a criação e especificação dos cenários de testes.
* Documentar o comportamento do sistema: Oferece uma maneira organizada de especificar as funcionalidades.

**Vantagens:**

* Orientação ao usuário: Descreve as funcionalidades do ponto de vista de quem utilizará o sistema.
* Clareza e compreensibilidade: A estrutura narrativa facilita o entendimento das funcionalidades.
* Abrangência das funcionalidades: Permite descrever o comportamento do sistema em diversas situações (fluxos alternativos e de exceção).
* Validação: Os stakeholders podem validar se o sistema implementa o comportamento esperado descrito nos casos de uso.
* Identificação do escopo: Ajuda a definir os limites do sistema.

**Desvantagens:**

* Especificar requisitos não funcionais: Aspectos como performance, segurança e usabilidade são mais difíceis de serem totalmente especificados apenas com casos de uso.
* Risco de incompletude: É possível que alguns cenários ou fluxos de exceção não sejam identificados durante o levantamento.
* Podem se tornar extensos e complexos: Casos de uso muito detalhados ou com muitos fluxos alternativos podem ser difíceis de gerenciar.
* Foco no "o quê" e não no "como": Casos de uso descrevem o comportamento externo, mas não especificam os detalhes internos da implementação.

## :books: Especificação dos Requisitos

### 1 - Especificação por Entrevista

* **Requisito selecionado:**  

  _Aluno: ABRAAO SANTIAGO MOREIRA  
  Sugestão: O sistema deve permitir um Modo de emergência: Contato rápido com serviços de ajuda (CVV, emergência médica).  
  Prioridade: ALTA_  

* **Entrevista com o stakeholder (usuário)**
  
  Entrevistado: ABRAAO SANTIAGO MOREIRA
     
  Entrevistador: Analista de Requisitos  
  
  Objetivo da entrevista: Entender a motivação, contexto e expectativas para a funcionalidade de "modo de emergência".
  
  Perguntas e respostas (entrevista hipotética):
  
  **P:** Em que situações você acredita que o modo de emergência será utilizado?  
  **R:** Em momentos de crise emocional, ataques de pânico ou quando a pessoa está em risco de cometer algum ato contra si mesma.
  
  **P:** Que tipo de ajuda espera que o sistema forneça nesse modo?  
  **R:** Acesso rápido a serviços como o CVV (Centro de Valorização da Vida), números de emergência médica ou contato com pessoas de confiança.
  
  **P:** Esse modo deve estar disponível em qualquer parte do aplicativo?  
  **R:** Sim, deveria ser acessível de forma fácil e imediata, sem precisar navegar por muitas telas.
  
  **P:** Você gostaria que fosse enviado algum tipo de alerta a contatos cadastrados?  
  **R:** Seria bom, principalmente se o usuário autorizasse previamente. Pode ser uma notificação ou SMS.
  
* **Especificação resumida do requisito a partir da entrevista:**  
  
  O sistema deve disponibilizar um modo de emergência, visível em todas as telas, que permita o contato rápido com o CVV, serviços de emergência médica e contatos de confiança previamente cadastrados. O botão deve ser facilmente acessível e, ao ser acionado, apresentar as opções de ajuda imediata com apenas um clique.

### 2 - Especificação por Caso de Uso

* **Requisito selecionado:**
  
  _Aluno: ALINE AYUMI SOMA HAMANO  
  Sugestão: O sistema deve fazer sugestões de práticas de saúde mental para o paciente.  
  Prioridade: ALTA_  

* **Caso de Uso: UC01 – Sugerir Práticas de Saúde Mental**

  | **Item**             | **Descrição**                                                                                                                                         |
  |----------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|
  | **Nome**             | Sugerir Práticas de Saúde Mental                                                                                                                     |
  | **Ator Principal**   | Usuário do aplicativo                                                                                                                                 |
  | **Atores Secundários** | Sistema de recomendação                                                                                                                             |
  | **Pré-condições**    | O usuário está logado e possui um perfil mínimo com informações cadastradas (idade, histórico emocional ou respostas iniciais).                      |
  | **Descrição**        | O sistema analisa o perfil do usuário e sugere práticas de bem-estar mental, como técnicas de respiração, meditação guiada, caminhadas, etc.        |
  | **Fluxo Principal**  | 1. Usuário acessa a área de recomendações  <br> 2. O sistema avalia os dados do usuário  <br> 3. O sistema apresenta uma lista de sugestões  <br> 4. O usuário pode marcar as práticas realizadas |
  | **Fluxos Alternativos** | - Se o perfil não tiver dados suficientes, o sistema solicita ao usuário que responda a um questionário breve. <br> - Práticas já realizadas podem ser reapresentadas com novas variações. |
  | **Pós-condições**    | As sugestões são armazenadas para avaliação futura da efetividade das práticas recomendadas.                                                         |
