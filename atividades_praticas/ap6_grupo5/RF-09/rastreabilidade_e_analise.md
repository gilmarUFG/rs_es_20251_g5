# Rastreabilidade e Análise de Consistência – HU09: Detecção e Notificação de Tendências Autodestrutivas

## Matriz de Rastreabilidade

| Requisito / User Story                          | Relacionado a                                | Descrição / Observações                                                                                                                                                                                                  |
|-------------------------------------------------|----------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| HU09 – Detecção e Notificação de Tendências Autodestrutivas | RF-9 (Requisito Funcional)                   | Implementa a funcionalidade principal de detecção de tendências autodestrutivas e comunicação de emergência do RF-9.                                                                                                    |
| HU09 – Detecção e Notificação de Tendências Autodestrutivas | RNF - Segurança e Privacidade (LGPD)         | O requisito exige "consentimento explícito", "segurança e privacidade dos dados rigorosamente garantidas", e "conformidade com a LGPD" para um tema altamente sensível.                                                   |
| HU09 – Detecção e Notificação de Tendências Autodestrutivas | RNF - Confiabilidade e Precisão              | A IA deve "detectar padrões" e "classificar" riscos, o que implica alta confiabilidade e precisão para evitar falsos positivos/negativos.                                                                                  |
| HU09 – Detecção e Notificação de Tendências Autodestrutivas | RNF - Ética e Responsabilidade               | O requisito aborda a responsabilidade de "comunicar autoridades" e a necessidade de "validação profissional da lógica de detecção e protocolos de intervenção".                                                           |
| HU09 – Detecção e Notificação de Tendências Autodestrutivas | HU01 – Modo de Emergência                     | HU09 pode acionar o protocolo do "Modo de Emergência" (HU01) de forma proativa pela IA, complementando o acionamento manual do usuário.                                                                                |
| HU09 – Detecção e Notificação de Tendências Autodestrutivas | HU06 – Adaptação de Respostas por Interação  | A detecção da IA se baseia na "análise de padrões nas interações do usuário" (texto, respostas), alinhando-se com a HU06 que trata da capacidade da IA de aprender com as interações.                                    |
| HU09 – Detecção e Notificação de Tendências Autodestrutivas | HU07 – Uso de Referências Validadas          | A lógica de detecção e os protocolos de intervenção da IA devem ser validados por profissionais, baseando-se em referências aceitas (como na HU07).                                                                  |
| HU09 – Detecção e Notificação de Tendências Autodestrutivas | UC - Análise de Comportamento do Usuário     | Um Caso de Uso que detalha o fluxo de coleta e análise de dados comportamentais (ex: texto do diário, voz) para a detecção de padrões de risco.                                                                        |

---

## Análise de Consistência

- [x] A IA detecta tendências autodestrutivas com base nos padrões de interação do usuário?
- [x] Critérios para classificação de risco e emergência são definidos e validados por profissionais?
- [x] O usuário fornece consentimento explícito para o acionamento de contatos/autoridades em caso de emergência?
- [x] O sistema tenta intervenções diretas no aplicativo antes de escalar para contatos externos?
- [x] Contatos de confiança pré-definidos são notificados em situações de emergência, conforme o consentimento do usuário?
- [x] Protocolo para contato com autoridades (ex: SAMU/Polícia) é estabelecido para casos de risco iminente?
- [x] A privacidade e a segurança dos dados são garantidas durante todo o processo?
- [x] O usuário é informado quando um contato de emergência é acionado?
- [ ] Como o sistema gerencia a atualização dos contatos de emergência e sua validade?
- [ ] Há um limite de tentativas de intervenção direta antes da escalada? Qual é esse limite?
- [ ] Como o sistema lida com falsos positivos ou falsos negativos na detecção da IA?
- [ ] Qual o tempo de resposta esperado entre a detecção e a notificação de emergência?

### Recomendações:

- Detalhar o processo de gestão dos contatos de emergência (cadastro, edição, remoção) e a periodicidade de validação.
- Definir com clareza os limites e a lógica para a transição da intervenção direta para a escalada da notificação de emergência.
- Esclarecer os protocolos de segurança e privacidade para o compartilhamento de informações com contatos e autoridades em situações de emergência.
- Considerar mecanismos de feedback para a IA em relação à eficácia das detecções e intervenções (ex: feedback dos profissionais ou de contatos de confiança, com consentimento).
