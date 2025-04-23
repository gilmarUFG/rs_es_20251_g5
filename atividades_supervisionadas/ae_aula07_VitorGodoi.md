# Técnicas para Especificação de Requisitos

## Técnica 1: Histórias de Usuário

**Descrição:**  
As histórias de usuário são sentenças simples que capturam uma necessidade do ponto de vista do usuário, frequentemente no formato:

> *Como [tipo de usuário], eu quero [ação], para que [benefício].*

Elas são complementadas com critérios de aceitação que definem as condições mínimas para considerar a funcionalidade concluída.

**Cenários de Aplicação:**
- Projetos com metodologias ágeis.
- Sistemas que focam na experiência do usuário.
- Funcionalidades que evoluem com o tempo.

**Vantagens:**
- Linguagem simples e compreensível por todos os envolvidos.
- Facilita o alinhamento com o valor entregue ao usuário.
- Ajuda na priorização de funcionalidades.

**Desvantagens:**
- Pode ser ambígua se mal escrita.
- Requer acompanhamento constante com stakeholders.
- Nem sempre fornece nível técnico suficiente.

---

## Técnica 2: Prototipação

**Descrição:**  
A prototipação envolve a criação de versões preliminares da interface do sistema para validar e refinar os requisitos com os usuários finais.

**Cenários de Aplicação:**
- Funcionalidades críticas ou sensíveis (ex: segurança, emergência).
- Quando é necessário validar o fluxo com o usuário antes da implementação.
- Sistemas voltados à experiência do usuário (UX).

**Vantagens:**
- Rápido feedback dos usuários.
- Permite identificar falhas de usabilidade antes do desenvolvimento completo.
- Facilita a comunicação entre desenvolvedores e stakeholders.

**Desvantagens:**
- Pode gerar expectativa de que o protótipo é a versão final.
- Protótipos muito detalhados podem consumir muito tempo.
- Nem todos os aspectos técnicos são representados visualmente.

---

# Aplicação das Técnicas: App de Saúde Mental com IA

## Especificação do requisito A - **“Os usuários devem poder fornecer feedbacks para as respostas.”**
**Técnica aplicada: _História de Usuário_**

### História de Usuário
> **Como** um usuário do aplicativo,  
> **eu quero** poder avaliar as respostas geradas pela IA,  
> **para que** o sistema possa melhorar a qualidade dos atendimentos.

### Critérios de Aceitação
- [x] O usuário pode marcar uma resposta como “útil” ou “não útil”.
- [x] O usuário pode adicionar um comentário opcional explicando o motivo.
- [x] O feedback é vinculado à resposta específica e armazenado com timestamp.
- [x] O sistema deve registrar o feedback de forma assíncrona (sem travar o app).
- [x] Se a resposta for marcada como “não útil”, o app oferece sugestões adicionais de ajuda.

---

## Especificação do requisito B - **“O aplicativo deve contar com um modo de emergência, onde o usuário pode acionar rapidamente contatos de confiança.”**   
**Técnica aplicada: _Prototipação_**

### Processo de Prototipação
1. **Objetivo do protótipo:**  
   Validar a experiência de ativação rápida do modo de emergência, com foco em acessibilidade e rapidez.

2. **Protótipo criado:**  
   Uma maquete interativa de baixa fidelidade (ex: Figma ou Adobe XD), com os seguintes elementos:
   - Botão “Modo de Emergência” visível na tela inicial.
   - Tela de confirmação da ação.
   - Tela de notificação de envio com status.
   - Configuração prévia de contatos de confiança.

3. **Feedback dos usuários:**  
   Durante testes com um grupo-alvo, foi identificado:
   - O botão precisa ter cor destacada (vermelho) e estar acessível mesmo com o app bloqueado.
   - A confirmação precisa ter opção de cancelamento imediato.
   - A notificação enviada aos contatos deve conter nome, localização e mensagem clara.

4. **Ajustes baseados no protótipo:**
   - Implementar acesso ao botão via notificação persistente ou widget.
   - Adicionar campo de mensagem customizável.
   - Incluir teste de envio durante a configuração dos contatos.
