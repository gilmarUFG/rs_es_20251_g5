# 🧪 Simulação de Revisão de Requisito

**User Story: HU02 – Sugestões de Práticas de Saúde Mental**

> **Como** paciente em acompanhamento de saúde mental,  
> **Quero** receber sugestões de práticas saudáveis e acessíveis,  
> **Para que** eu possa cuidar do meu bem-estar mental de forma contínua e preventiva.

---

## ✅ Verificação com Checklist
---------------------------------------------------------------------------------------------------------------------------------
| Critério de Verificação                                              | Status | Observações                                                                                                    |
|----------------------------------------------------------------------|-----------------------|----------------------------------------------------------------------------------------------------------------|
| A descrição está clara e compreensível?                              | ✅                    | O card e a conversa são claros e detalham bem a funcionalidade.                                                 |
| O requisito atende a uma necessidade real do usuário?                | ✅                    | Sim, oferece suporte contínuo para o bem-estar mental.                                                 |
| Há valor de negócio claramente definido?                             | ✅                    | Agrega valor ao usuário, incentiva o engajamento e a retenção.                                                  |
| Os critérios de aceitação estão descritos e são objetivos?           | ✅                    | Os critérios são objetivos, cobrindo a existência da seção, formatos, curadoria e interação do usuário. |
| O requisito é testável (permite escrita de casos de teste)?          | ✅                    |              |
| Estão descritos os fluxos principais e alternativos?                 | ✅/❌                | A conversa descreve apenas o fluxo principal (seção dedicada, personalização, formatos). Faltam alguns alternativos de interação. |
| Há tratamento de exceções e erros?                                   | ❌                    | Não há menção sobre o que acontece se não houver sugestões personalizadas ou se o conteúdo externo estiver indisponível. |
| O requisito está alinhado com regras de negócio conhecidas?          | ✅                    |              |
| Existe rastreabilidade com histórias ou regras relacionadas?         | ✅                    | A conversa menciona personalização (relacionado a perfil), curadoria de especialistas e acessibilidade (WCAG / WAI-ARIA). |
| O requisito está consistente com outras funcionalidades existentes?  | ✅                    |              |
| Há viabilidade técnica para entrega no sprint?                       | ✅                    | Sim, com um banco de dados de práticas e um algoritmo de recomendação (mesmo que simples inicialmente).        |
--------------------------------------------------------------------------------------------------------------

**Conclusão:** A HU02 é bem estruturada e clara, com critérios de aceitação que guiam bem o desenvolvimento. Os pontos de aprimoramento residem em detalhar mais os fluxos alternativos de interação (ex: descarte de sugestão) e o tratamento de exceções para garantir uma experiência mais robusta, especialmente em relação à personalização e fontes de conteúdo.