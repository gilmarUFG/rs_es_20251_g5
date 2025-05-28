# Rastreabilidade e Análise de Consistência – HU02: Sugestões de Práticas de Saúde Mental

## Matriz de Rastreabilidade

| Requisito / User Story                     | Relacionado a                                | Descrição / Observações                                                               |
|--------------------------------------------|----------------------------------------------|---------------------------------------------------------------------------------------|
| HU02 – Sugestões de Práticas de Saúde Mental | RF-2 (Requisito Funcional)                   | Implementa a funcionalidade de "sugestões de práticas de saúde mental" do RF-2.        |
| HU02 – Sugestões de Práticas de Saúde Mental | RNF - Usabilidade                            | "As sugestões serão exibidas em uma seção dedicada", "diferentes formatos" e "marcar como 'favorita' ou 'já tentei'". |
| HU02 – Sugestões de Práticas de Saúde Mental | RNF - Acessibilidade                         | "Acessibilidade será garantida (descrições de imagem, leitura por voz, contraste)." e "Testes de acessibilidade aprovados (WCAG / WAI-ARIA)." |
| HU02 – Sugestões de Práticas de Saúde Mental | RNF - Privacidade e Segurança (LGPD)         | "A funcionalidade respeitará a privacidade dos usuários, com dados anonimizados caso haja coleta de uso." e "Dados de uso, se coletados, são anonimizados e seguem a LGPD." |
| HU02 – Sugestões de Práticas de Saúde Mental | RNF - Confiabilidade (Curadoria)             | "As práticas devem ter embasamento profissional (psicologia/psiquiatria)." e "A curadoria será feita com apoio de especialistas." |
| HU02 – Sugestões de Práticas de Saúde Mental | US (User Story) - Gerenciamento de Perfil   | As recomendações serão "personalizadas com base em perfil, histórico ou estado atual do usuário". |
| HU02 – Sugestões de Práticas de Saúde Mental | UC (Caso de Uso) - Receber Sugestões        | Detalha a interação do usuário para visualizar e interagir com as sugestões.          |

---

## Análise de Consistência

- [x] Há uma seção dedicada com sugestões de práticas de saúde mental?
- [x] As sugestões são exibidas em formatos acessíveis (ex: texto, áudio, vídeo)?
- [x] As práticas são baseadas em fontes confiáveis com curadoria profissional?
- [x] O usuário pode marcar sugestões como "favoritas" ou "já tentei"?
- [x] Testes de acessibilidade aprovados (WCAG / WAI-ARIA)?
- [x] Dados de uso, se coletados, são anonimizados e seguem a LGPD?
- [x] A funcionalidade está disponível para usuários autenticados e oferece sugestões genéricas sem login?
- [ ] Existe um critério claro para a "personalização" das sugestões? Quais dados do usuário serão usados para isso?
- [ ] Como o sistema garante a atualização e diversidade contínua das sugestões?
- [ ] Há um processo definido para a revisão e validação do conteúdo das sugestões por parte dos especialistas?

### Recomendações:

- Detalhar o algoritmo ou lógica de personalização das sugestões (ex: com base no humor, atividades registradas, preferências marcadas).
- Esclarecer o processo de curadoria e atualização do banco de dados de práticas, incluindo periodicidade e responsáveis.
- Considerar mecanismos para lidar com a "fadiga de sugestões", oferecendo novas opções ou adaptando a frequência.
- Definir o comportamento do sistema quando não houver sugestões personalizadas relevantes para o perfil do usuário.