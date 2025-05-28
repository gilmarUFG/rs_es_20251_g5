# Rastreabilidade e Análise de Consistência – HU01: Modo de Emergência

## Matriz de Rastreabilidade

| Requisito / User Story                     | Relacionado a                                | Descrição / Observações                                                               |
|--------------------------------------------|----------------------------------------------|---------------------------------------------------------------------------------------|
| HU01 – Modo de Emergência                  | RF-1 (Requisito Funcional)                   | Implementa a funcionalidade de "Modo de emergência" do RF-1.                          |
| HU01 – Modo de Emergência                  | RNF - Usabilidade                            | "A interface deve ser acessível e rápida de acionar (ex: 2 toques no máximo)." |
| HU01 – Modo de Emergência                  | RNF - Acessibilidade                         | "Considerar acessibilidade (ex: contraste, leitores de tela)." e "Testes de acessibilidade aprovados (WAI-ARIA / WCAG)." |
| HU01 – Modo de Emergência                  | RNF - Privacidade e Segurança (LGPD)         | "A funcionalidade não deve registrar logs de uso pessoal para garantir anonimato (segurança e privacidade)." e "Logs pessoais não são armazenados (conformidade com LGPD)." |
| HU01 – Modo de Emergência                  | Política de Monitoramento / Métricas         | "Após lançamento, será ativado monitoramento de cliques e falhas (Shift Right)." e "Há monitoramento de uso anônimo para métricas de acionamento." |
| HU01 – Modo de Emergência                  | UC (Caso de Uso) - Acionar Emergência        | Detalha a interação do usuário para acionar os serviços de emergência.                |
| HU01 – Modo de Emergência                  | RNF - Confiabilidade (Implícita)             | O sistema deve garantir a operação da funcionalidade em momentos críticos.            |

---

## Análise de Consistência

- [x] O botão de emergência está visível na tela inicial (mesmo sem login)?
- [x] Ao clicar, exibe opções de contato com CVV e emergência médica?
- [x] O botão funciona em menos de 2 interações?
- [x] Testes de acessibilidade aprovados (WAI-ARIA / WCAG)?
- [x] Logs pessoais não são armazenados (conformidade com LGPD)?
- [x] Há monitoramento de uso anônimo para métricas de acionamento?
- [ ] Existe um plano de contingência para falha na conexão ou indisponibilidade dos serviços externos (CVV/SAMU)?
- [ ] Como o sistema informa o usuário sobre o status da ligação/redirecionamento?

### Recomendações:

- Detalhar o tratamento de exceções para cenários onde a ligação ou o redirecionamento para os serviços de emergência falha (ex: sem conexão, serviço indisponível).
- Especificar o feedback visual e/ou sonoro para o usuário ao acionar o modo de emergência e durante a tentativa de contato.
- Confirmar se a equipe de QA realmente definirá os "fluxos críticos" e se isso será documentado como parte dos critérios de aceitação.