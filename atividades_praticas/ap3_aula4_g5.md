# RF-03
### 1. Descrição Detalhada

O objetivo desta funcionalidade é permitir que o usuário acompanhe, em tempo real, a localização do entregador assim que o pedido sai para a entrega. Isso será feito por meio de um mapa no aplicativo, exibindo a rota do entregador e uma estimativa de tempo para a chegada do pedido.

Assim que o status do pedido for alterado para "Em rota de entrega", o usuário visualizará no aplicativo a opção "Acompanhar Entrega". Ao clicar nessa opção, um mapa será aberto mostrando a localização atual do entregador, sua rota e o tempo estimado para a chegada ao destino.

A atualização da localização será feita em intervalos regulares, sem a necessidade de rastreamento em tempo real a cada segundo, garantindo um equilíbrio entre precisão e desempenho do sistema. Caso ocorra algum imprevisto significativo, como um congestionamento ou um acidente, o sistema poderá recalcular a rota ou notificar o usuário sobre possíveis atrasos.

Adicionalmente, para proporcionar maior segurança ao usuário, poderão ser exibidas informações do entregador, como nome e foto. Além disso, será disponibilizada uma opção para que o usuário retorne à tela de detalhes do pedido caso deseje revisá-lo.

### 2. Identificação das Fontes dos Requisitos

A necessidade dessa funcionalidade surge de diversas fontes:

- **Usuários**: Acompanhamento da entrega;
  - **Técnica de Aquisição**: Entrevista - _Foram realizadas entrevistas com usuários reais ou potenciais para entender como eles se sentem em relação ao processo de entrega
    e se gostariam de acompanhar a localização em tempo real ou simplesmente o status do pedido. Durante as entrevistas, foi questionado também sobre suas expectativas em termos de
    precisão do mapa, tempo de atualização e informações adicionais que gostariam de ver no aplicativo._
- **Concorrentes**: Concorrentes já implementam funcionalidades semelhantes. Para manter a competitividade, é fundamental que o nosso aplicativo também tenha esse recurso;
  - **Técnica de Aquisição**: Pesquisa de mercado - _Foi feita uma análise sobre funcionalidades oferecidas por concorrentes, identificando como eles
  implementam o rastreamento de entregas, o nível de detalhes oferecido no mapa, o tipo de informações sobre o entregador (nome, foto, etc.) e as
  opções de personalização (como escolher ver ou não a rota). A partir dessa análise, podemos identificar lacunas ou oportunidades de melhoria no nosso
  próprio sistema._ 
- **Empresa (Logística)**: A disponibilidade do rastreamento pode reduzir a quantidade de chamados ao suporte com dúvidas sobre a localização do pedido;
  - **Técnica de Aquisição**: Brainstorming - _Foram realizados encontros com a equipe de logística de potenciais afiliados para entender como o sistema poderia otimizar o fluxo de entregas.
    A equipe ofereceu insights sobre como a funcionalidade de rastreamento poderia ser integrada com o fluxo de trabalho atual de entregas,
    como a exibição de tempos estimados e a detecção de imprevisto, reduzindo a quantidade de chamados de suporte._
- **Entregadores**: A funcionalidade também pode beneficiar os entregadores, pois os clientes estarão preparados para recebê-los, agilizando a finalização das entregas;
  - **Técnica de Aquisição**: Entrevista - _Foram realizadas entrevistas com entregadores para entender como o sistema poderia melhorar o fluxo do processo e
    a experiência de entrega dos produtos, tanto para o entregador quanto para o cliente._

### 3. Fluxos de Execução

#### Fluxo Principal (Acompanhamento Normal)

1. O usuário realiza um pedido no aplicativo.
2. O pedido é preparado e sai para entrega (status alterado para "Em rota de entrega").
3. O usuário recebe uma notificação informando que a entrega está a caminho e oferecendo a opção de acompanhamento.
4. Na tela de "Meus Pedidos" ou na tela de detalhes do pedido, é exibido um botão "Acompanhar Entrega" ou um mapa em miniatura com a rota do entregador.
5. O usuário clica na opção de acompanhamento.
6. O sistema exibe um mapa com as seguintes informações:
   - Localização atual do entregador (atualizada periodicamente);
   - Endereço de entrega do usuário;
   - Rota entre o ponto de partida e o destino;
7. O mapa é atualizado regularmente para refletir o movimento do entregador.
8. Quando a entrega é concluída, o status do pedido é alterado para "Entregue" e a tela de rastreamento exibe uma confirmação.

#### Fluxo Alternativo (Problema na Entrega)

1. O usuário segue os passos 1 a 7 do fluxo principal.
2. O sistema detecta que o entregador está parado por um período prolongado ou que a estimativa de entrega foi significativamente excedida.
3. O sistema pode:
   - Enviar uma notificação ao usuário informando sobre a possibilidade de atraso;
   - Exibir um aviso na tela de rastreamento;
   - Disponibilizar uma opção para que o usuário entre em contato com o suporte.

### 4. Perfis de Usuários com Permissão de Execução

- **Usuário Comprador**: Principal beneficiado da funcionalidade, pois precisa acompanhar a entrega do pedido.
- **Administrador/Suporte** (opcional): Pode ter acesso ao rastreamento para auxiliar na resolução de problemas em caso de imprevistos
