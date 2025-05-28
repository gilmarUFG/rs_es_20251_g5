# Rastreabilidade e Análise de Consistência – HU04 Limitação e Encaminhamento Profissional

## Matriz de Rastreabilidade

| Requisito / User Story                     | Relacionado a                      | Descrição / Observações                                                                                     |
|-------------------------------------------|----------------------------------|-------------------------------------------------------------------------------------------------------------|
| HU04 – Limitação e Encaminhamento Profissional | RF - Mensagens de Limitação       | Exibição de mensagens claras sobre as limitações do aplicativo em pontos estratégicos                        |
| HU04                                       | IA - Detecção de Risco            | Acionamento de mensagens em situações de risco ou complexidade identificada pela IA                          |
| HU04                                       | Conteúdo Saúde Mental             | Mensagens em seções específicas reforçando a importância do acompanhamento profissional                      |
| HU04                                       | HU05 - Recomendação de Profissionais | Integração para direcionar o usuário para profissionais qualificados                                        |
| HU04                                       | QA - Validação de Usabilidade    | Testes para garantir clareza, acolhimento e não intrusividade das mensagens                                 |

---

## Análise de Consistência

- [x] A mensagem de limitação é exibida no onboarding?  
- [x] A IA aciona mensagens em níveis de risco ou complexidade altos?  
- [x] As mensagens são claras, acolhedoras e não alarmistas?  
- [x] Há links ou direcionamentos claros para busca de profissionais?  
- [x] A frequência e o teor das mensagens são validados por especialistas em saúde mental?  
- [x] Testes de usabilidade confirmam compreensão e evitam frustração?  
- [ ] Existe tratamento para falhas na exibição das mensagens?  
- [ ] Está definido o fluxo alternativo caso o usuário ignore ou rejeite as mensagens?  
- [ ] A rastreabilidade com outras HUs (como a recomendação de profissionais) está formalizada?  

---

### Recomendações

- Definir fluxo de exceção para falhas na exibição das mensagens.  
- Formalizar a integração com HU de recomendação de profissionais para rastreabilidade completa.  
- Documentar gatilhos e frequência da exibição com base na avaliação dos especialistas em saúde mental.  
- Garantir que as mensagens sejam testadas em múltiplos dispositivos e situações para evitar frustrações.  
