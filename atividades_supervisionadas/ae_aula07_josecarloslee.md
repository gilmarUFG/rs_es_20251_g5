## Tarefa: Técnicas para Especificação de Requisitos

### 1. Pesquisa sobre Técnicas de Especificação

A seguir, são descritas duas técnicas comuns para a especificação de requisitos de software: Histórias de Usuário (User Stories) e Casos de Uso (Use Cases).

---

#### Técnica 1: Histórias de Usuário (User Stories)

**Descrição:**
Histórias de usuário são descrições curtas e simples de uma funcionalidade contadas da perspectiva da pessoa que deseja o novo recurso, geralmente um usuário ou cliente do sistema. Elas normalmente seguem um template simples:

* **"Como um `<tipo de usuário>`, eu quero `<realizar alguma ação>` para que `<obtenha algum benefício>`."**

Elas são frequentemente usadas em metodologias ágeis (como Scrum) e são tipicamente escritas em cartões físicos ou digitais, servindo como um lembrete para uma conversa futura sobre os detalhes do requisito.

**Cenários Aplicáveis:**

* Projetos que utilizam metodologias ágeis.
* Quando o foco principal é o valor entregue ao usuário final.
* Para capturar requisitos funcionais de forma rápida e colaborativa.
* Em situações onde os detalhes podem ser definidos posteriormente em conversas com a equipe.

**Vantagens:**

* **Foco no Usuário e Valor:** Mantém a equipe focada nas necessidades e benefícios do usuário.
* **Simplicidade e Clareza:** Fáceis de entender por todos (clientes, desenvolvedores, testers).
* **Facilita a Priorização:** O valor descrito ajuda a ordenar o backlog.
* **Promove a Colaboração:** São "promessas de conversa", incentivando o diálogo entre a equipe e os stakeholders.
* **Flexibilidade:** Permitem que os detalhes sejam definidos mais perto da implementação.

**Desvantagens:**

* **Falta de Detalhes:** Podem ser muito vagas inicialmente, necessitando de conversas adicionais e critérios de aceitação claros.
* **Não Ideais para Não Funcionais:** Menos eficazes para detalhar requisitos não funcionais (desempenho, segurança) ou regras de negócio complexas.
* **Risco de Ambiguidade:** Se não forem bem escritas ou discutidas, podem levar a interpretações diferentes.
* **Escalabilidade:** Gerenciar um grande número de histórias pode ser desafiador sem ferramentas adequadas.

---

#### Técnica 2: Casos de Uso (Use Cases)

**Descrição:**
Casos de uso descrevem a interação entre um ator (usuário ou outro sistema) e o sistema de software para alcançar um objetivo específico. Eles detalham a sequência de passos que ocorrem durante essa interação. Um caso de uso geralmente inclui:

* **Nome:** Um nome claro e conciso para o objetivo do ator.
* **Ator(es):** Quem inicia ou participa da interação.
* **Pré-condições:** O que deve ser verdadeiro antes do caso de uso começar.
* **Pós-condições:** O estado do sistema após a conclusão bem-sucedida.
* **Fluxo Principal (Caminho Feliz):** A sequência normal de passos para atingir o objetivo.
* **Fluxos Alternativos/Exceção:** Sequências que lidam com variações ou erros.

Podem ser representados textualmente (mais comum) ou graficamente usando diagramas de Casos de Uso UML (que mostram a relação entre atores e casos de uso).

**Cenários Aplicáveis:**

* Para detalhar requisitos funcionais, especialmente aqueles com fluxos de interação complexos.
* Quando é importante entender como diferentes atores interagem com o sistema para atingir seus objetivos.
* Em projetos que necessitam de uma documentação mais formal e detalhada das funcionalidades.
* Para derivar casos de teste funcionais.

**Vantagens:**

* **Foco no Objetivo do Ator:** Centrados em como os usuários usarão o sistema para realizar tarefas.
* **Detalhamento:** Capturam a sequência de passos, incluindo alternativas e exceções, reduzindo ambiguidades.
* **Compreensão do Contexto:** Ajudam a entender como a funcionalidade se encaixa no sistema maior.
* **Base para Testes:** Os fluxos descritos são uma ótima base para criar casos de teste.
* **Comunicação:** Podem ser entendidos tanto por usuários de negócio quanto por equipes técnicas (especialmente a descrição textual).

**Desvantagens:**

* **Podem ser Longos e Complexos:** Descrever todos os fluxos pode tornar os casos de uso extensos e demorados para escrever e manter.
* **Foco Funcional:** Assim como as User Stories, não são a melhor forma para capturar requisitos não funcionais detalhadamente.
* **Risco de Focar no Design:** Há uma tentação de incluir detalhes de interface ou implementação nos passos, o que deve ser evitado na especificação de requisitos.
* **Manutenção:** Mudanças nos requisitos podem exigir atualizações em vários fluxos dentro de um caso de uso.

---

### 2. Especificação de Requisitos dos Cenários

A seguir, são especificados dois requisitos, um para cada cenário do grupo, utilizando as técnicas descritas acima.

---

#### Requisito A: Cenário "Aplicativo de Saúde Mental com IA"

* **Técnica Utilizada:** História de Usuário (User Story)

* **ID:** RF-SM-010 (Exemplo)
* **História:**
    * **Como um** usuário do aplicativo de saúde mental,
    * **eu quero** registrar meu humor diariamente selecionando uma opção (ex: Muito Bem, Bem, Neutro, Mal, Muito Mal) e opcionalmente adicionar uma nota,
    * **para que** eu possa acompanhar minhas variações de humor ao longo do tempo e identificar padrões junto com o aplicativo ou meu terapeuta.

* **Critérios de Aceitação (Exemplos - seriam definidos em conversa):**
    * Deve haver uma seção visível na tela principal para registro diário do humor.
    * As opções de humor devem ser apresentadas de forma clara (ícones e/ou texto).
    * Deve ser possível adicionar uma nota de texto livre associada ao registro de humor.
    * O registro deve ser salvo com a data e hora.
    * O histórico de humor deve ser visualizável em um gráfico ou lista.

---

#### Requisito B: Cenário "Sistema de Agricultura Inteligente com IoT"

* **Técnica Utilizada:** Caso de Uso (Use Case - Descrição Textual Simplificada)

* **ID:** RF-AGRO-025 (Exemplo)
* **Nome do Caso de Uso:** Visualizar Histórico de Umidade do Solo por Talhão
* **Ator(es):** Agricultor
* **Pré-condições:**
    * O Agricultor está autenticado no sistema.
    * Sensores de umidade do solo estão instalados e transmitindo dados para os talhões monitorados.
    * O sistema processou e armazenou os dados históricos de umidade.
* **Pós-condições:**
    * O histórico de umidade do talhão selecionado é exibido para o Agricultor.
* **Fluxo Principal (Caminho Feliz):**
    1.  O Agricultor seleciona a opção "Monitoramento de Talhões" no menu principal.
    2.  O sistema exibe a lista ou mapa dos talhões cadastrados.
    3.  O Agricultor seleciona o talhão desejado.
    4.  O sistema exibe as opções de visualização para o talhão selecionado.
    5.  O Agricultor seleciona a opção "Histórico de Umidade do Solo".
    6.  O sistema solicita ao Agricultor que defina o período desejado (ex: últimos 7 dias, último mês, período customizado).
    7.  O Agricultor informa o período e confirma.
    8.  O sistema recupera os dados históricos de umidade do solo para o talhão e período selecionados.
    9.  O sistema exibe os dados históricos em formato de gráfico (ex: linha do tempo) e/ou tabela para o Agricultor.
* **Fluxos Alternativos/Exceção:**
    * **7a. Período Inválido:** Se o Agricultor inserir um período inválido (ex: data final anterior à inicial), o sistema exibe uma mensagem de erro e solicita a correção (retorna ao passo 7).
    * **8a. Dados Não Disponíveis:** Se não houver dados de umidade para o período ou talhão selecionado, o sistema exibe uma mensagem informativa (ex: "Nenhum dado de umidade encontrado para este período/talhão").

---
