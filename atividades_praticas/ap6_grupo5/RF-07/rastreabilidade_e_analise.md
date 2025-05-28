# Rastreabilidade e Análise de Consistência – HU07: Referências Validadas para Suporte em Saúde Mental

## Matriz de Rastreabilidade

| Requisito / User Story          | Relacionado a                               | Descrição / Observações                                                                                     |
|---------------------------------|----------------------------------------------|--------------------------------------------------------------------------------------------------------------|
| HU07 - Referências Validadas    | RF03 - Curadoria por especialistas          | Depende da validação e análise de psicólogos e psiquiatras para garantir que as fontes sejam adequadas.     |
| HU07                            | RF04 - Aviso sobre limitações               | Alinha-se ao requisito de sempre informar que o app não substitui acompanhamento profissional.              |
| HU07                            | RF06 - Aprendizado com histórico emocional  | As referências validadas também devem ser consideradas no processo de adaptação das respostas.              |
| HU07                            | RNF05 - Segurança e LGPD                    | A rastreabilidade das fontes não pode comprometer dados sensíveis, seguindo criptografia e segurança.       |
| HU07                            | RF08 - Feedback de usuários                 | Feedbacks podem ajudar na identificação de respostas inconsistentes com as referências validadas.           |

---

## Análise de Consistência

- [x] As fontes utilizadas são reconhecidas e validadas internacionalmente?
- [x] Existe controle para impedir que a IA gere diagnósticos?
- [x] As respostas da IA incluem avisos de que não substituem profissionais?
- [ ] As referências são sempre apresentadas de forma rastreável para o usuário?
- [x] Há processo definido de curadoria e validação por especialistas?
- [ ] Existe processo automatizado ou alerta para revisão e atualização de fontes?

### Recomendações:

- Avaliar a possibilidade técnica de exibir a fonte específica na resposta da IA sempre que aplicável.
- Definir claramente um processo recorrente de curadoria para garantir que as fontes estejam atualizadas.
- Integrar validações que impeçam a utilização de conteúdos fora do escopo das referências definidas.
- Incluir no frontend ou na documentação do app uma seção que liste as principais fontes utilizadas (ex.: DSM-5, CID-11, OMS) e a data da última revisão.
- Considerar um mecanismo de controle para alertar quando uma fonte se tornar obsoleta ou desatualizada.
