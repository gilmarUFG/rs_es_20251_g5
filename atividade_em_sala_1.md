# Aplicativo de Delivery  
## Requisitos Funcionais
RF-001: Permitir que o usuário selecione a quantidade de produtos  
RF-002: O usuário pode cancelar o pedido  
RF-003: O usuárto pode rastrear seu pedido durante a entrega  
RF-004: A empresa deve poder escolher entre entregadores particulares ou da plataforma  
RF-005: O usuário deve ser capaz de salvar métodos de pagamento (como cartões de crédito)
## Requisitos não funcionais
RNF-001: A aplicação deve ser multiplataforma  
RNF-002: A aplicação deve possuir recursos de acessibilidade  
RNF-003: A aplicação deve se comunicar com API's de pagamento de terceiros  
RNF-004: O tempo de carregamento ao navegar entre as telas não deve ultrapassar 1 segundo  
RNF-005: Os dados pessoais do usuárto deven ser criptografados  
## Regras de negócio
18/1 - A quantidade de produtos selecionada não pode ultrapassar o estoque da loja  
192 - O usuárlo não pode cancelar o pedido se já tiver saído para a entrega  
203 - Pedidos não poden ser efetuados fora do horário de funcionamento da loja  
214 - Entregadores afiliados à plataforma deven compartilhar sua localização com a aplicação  
RN-5 Uma empresa não pode ter dois cadastros com o mesmo endereço
