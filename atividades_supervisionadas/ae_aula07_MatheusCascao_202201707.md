# Técnicas para Especificação de Requisitos

## 1. Técnicas de Especificação

### 1.1 Casos de Uso (Use Cases)

**Descrição**:  
Casos de uso são uma técnica da Engenharia de Requisitos baseada na UML (Unified Modeling Language) para descrever como os usuários (atores) interagem com o sistema para atingir um objetivo específico. Cada caso de uso descreve um cenário de interação completa entre um ator e o sistema.

**Cenários de Aplicação**:  
Casos de uso são ideais para sistemas interativos, em que há múltiplos perfis de usuário e diversas funcionalidades dependentes dessas interações. São muito usados em sistemas de informação, ERPs, aplicativos móveis e plataformas web.

**Vantagens**:

- Ajuda a identificar claramente os atores e suas interações com o sistema.
- Facilita a comunicação entre desenvolvedores, analistas e stakeholders.
- Fornece base para o desenvolvimento de testes funcionais.

**Desvantagens**:

- Pode se tornar complexo e extenso em sistemas grandes.
- Nem sempre capta bem requisitos não funcionais.
- Exige entendimento prévio da metodologia UML.

---

### 1.2 Histórias de Usuário (User Stories)

**Descrição**:  
Histórias de usuário são uma técnica ágil que descreve os requisitos a partir da perspectiva do usuário final, normalmente com o seguinte formato:  
**“Como [tipo de usuário], eu quero [ação ou funcionalidade] para que [benefício ou objetivo].”**

**Cenários de Aplicação**:  
Muito utilizadas em metodologias ágeis como Scrum e XP, as histórias de usuário são ideais para projetos com entregas incrementais, com foco no valor ao usuário e constante iteração.

**Vantagens**:

- Foco no valor entregue ao usuário.
- Linguagem simples, que facilita a comunicação com o cliente.
- Permite flexibilidade e adaptação contínua.

**Desvantagens**:

- Pode faltar detalhamento técnico.
- Nem sempre especifica requisitos não funcionais.
- Requer complementariedade com critérios de aceitação para maior clareza.

---

## 2. Especificação de Requisitos dos Cenários do Grupo

### 2.1 Requisito A: "O sistema deve permitir um Modo de emergência: Contato rápido com serviços de ajuda (CVV, emergência médica)."

**Técnica utilizada**: Casos de Uso

**Caso de Uso**:

- **Nome**: Ativar Modo de Emergência
- **Ator Principal**: Usuário
- **Pré-condições**: O usuário está logado no aplicativo e com acesso à internet.
- **Fluxo Principal**:
  1. O usuário acessa o menu principal do aplicativo.
  2. O usuário seleciona a opção “Modo de Emergência”.
  3. O sistema exibe opções de contato: CVV, emergência médica, chat de suporte.
  4. O usuário escolhe o tipo de ajuda desejada.
  5. O sistema inicia o contato (via ligação, mensagem ou redirecionamento).
- **Pós-condições**: O usuário foi conectado ao canal de ajuda apropriado.
- **Extensões**:
  - Caso não haja conexão, o sistema exibe uma mensagem e oferece o número offline.

---

### 2.2 Requisito B: "O sistema deve fazer sugestões de práticas de saúde mental para o paciente."

**Técnica utilizada**: Histórias de Usuário

**História de Usuário**:  
**Como** paciente,  
**eu quero** receber sugestões de práticas de saúde mental personalizadas,  
**para que** eu possa melhorar meu bem-estar emocional de forma contínua.

**Critérios de Aceitação**:

- O sistema deve apresentar pelo menos uma sugestão por dia.
- As sugestões devem variar de acordo com o histórico emocional do usuário.
- O usuário deve poder avaliar a utilidade das sugestões para melhorar recomendações futuras.

---

**Arquivo nomeado**: `ae_aula07_202201680_aline_ayumi_hamano.md`
