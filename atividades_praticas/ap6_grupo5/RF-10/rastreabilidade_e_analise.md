# Rastreabilidade e Análise de Consistência – HU10: Cadastro de Histórico Médico Pessoal

## Matriz de Rastreabilidade

| Requisito / User Story                          | Relacionado a                                | Descrição / Observações                                                                                                                                                                                                  |
|-------------------------------------------------|----------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| HU10 – Cadastro de Histórico Médico Pessoal     | RF-10 (Requisito Funcional)                  | Implementa a funcionalidade de cadastro e visualização de dados de histórico médico, conforme o RF-10.                                                                                                                  |
| HU10 – Cadastro de Histórico Médico Pessoal     | RNF - Segurança e Privacidade (LGPD)         | Exige que dados sensíveis sejam "armazenados com segurança e criptografia", "conformidade com a LGPD" e "controle do usuário sobre o compartilhamento".                                                                |
| HU10 – Cadastro de Histórico Médico Pessoal     | RNF - Acessibilidade                         | A interface de cadastro e visualização deve ser acessível para garantir que todos os usuários possam gerenciar suas informações de saúde.                                                                               |
| HU10 – Cadastro de Histórico Médico Pessoal     | HU06 – Adaptação de Respostas por Interação  | A IA poderá "utilizar esses dados (com consentimento do usuário) para refinar suas recomendações", conectando-se à HU06 sobre a adaptação das respostas da IA.                                                           |
| HU10 – Cadastro de Histórico Médico Pessoal     | HU07 – Uso de Referências Validadas          | O tratamento de dados médicos deve seguir as "referências validadas e aceitas internacionalmente" na área da saúde.                                                                                                     |
| HU10 – Cadastro de Histórico Médico Pessoal     | UC - Gerenciar Histórico Médico              | Um Caso de Uso que detalha os fluxos de adição, edição, visualização e exclusão de registros do histórico médico pelo usuário.                                                                                       |

---

## Análise de Consistência

- [x] O usuário consegue cadastrar dados de histórico médico em uma seção dedicada do aplicativo?
- [x] O aplicativo permite o registro de diagnósticos, medicamentos, alergias e histórico de tratamentos?
- [x] É possível anexar documentos (PDF, JPG) à seção de histórico médico?
- [x] Somente o usuário autenticado pode visualizar e editar seu histórico médico?
- [x] Os dados do histórico médico são armazenados com segurança e criptografia?
- [x] A IA pode utilizar (com consentimento) o histórico médico para personalizar recomendações?
- [x] O usuário tem controle sobre o compartilhamento do seu histórico médico?
- [ ] Como o sistema valida a integridade e a veracidade dos dados inseridos pelo usuário (ex: dosagens de medicamentos, diagnósticos)?
- [ ] Há um limite de tamanho ou tipo de arquivo para os anexos?
- [ ] Como é feito o tratamento de dados inconsistentes ou incompletos no histórico?
- [ ] Existem regras de negócio para a IA usar esses dados, como alertas sobre possíveis interações medicamentosas?

### Recomendações:

- Detalhar os mecanismos de validação dos dados inseridos pelo usuário, especialmente para informações críticas (ex: formatos de data, listas pré-definidas para diagnósticos/medicamentos).
- Definir limites para o tamanho e tipo de arquivos anexados e como o sistema lida com uploads inválidos.
- Esclarecer o processo de como a IA usará especificamente o histórico médico para refinar as recomendações, incluindo regras de negócio para alertas de interações (se aplicável).
- Considerar a possibilidade de integração futura com prontuários eletrônicos de saúde para importação automatizada de dados (com consentimento).
