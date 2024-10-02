## Componentes e Arquitetura do Azure

### Regiões do Azure, zonas de disponibilidade e pares de regiões
O Azure é composto por datacenters localizados em todo o mundo. Ao usar um serviço ou criar um recurso como um banco de dados ou uma máquina virtual, você está usando uma equipamento físico em um desses locais. O Azure organiza esses datacenters em regiões.

### Regiões do Azure
A região é uma área geográfica que contém pelo menos um, mas potencialmente vários datacenters próximos e conectados em rede com uma rede de baixa latência. O Azure oferece mais regiões globais do que qualquer outra provedor de nuvem com mais de 60 regiões representando mais de 140 países. Essas regiões oferecem a flexibilidade de aproximar os aplicativos de seus usuários , não importa onde eles estejam. As regiões globais fornecem melhor escalabilidade e redundância, além de preservar a residência de dados para seus serviços. Ao implantar um serviço no Azure, muitas vezes precisará escolher a região onde deseja que seu recurso seja implantado.<br/>

<img src="https://www.class365.com.br/wp-content/uploads/2020/10/regions-map-desktop.svg" alt="Regiões do Azure"><br/>

### Zonas de disponibilidade

Zonas de disponibilidade são datacenters fisicamente separados em uma região do Azure. Cada zona de disponibilidade é composta por um ou mais datacenters equipados com energia, refrigeração e rede independentes, são configuradas para ser um limite de isolamento, se uma zona cair a outra continua funcionando. Essas zonas são conectadas por meio de redes privadas de fibra óptica de alta velocidade.

Você pode usar zonas de disponibilidade para executar aplicativos de missão crítica e criar alta disponibilidade em sua arquitetura de aplicativos, colocando seus recursos de computação, armazenamento, rede e dados em uma zona replicando em outras zonas.<br/>

<img src="https://www.class365.com.br/wp-content/uploads/2020/10/zona-de-disponibilidade.png" alt="Zonas de Disponibilidade"><br/>

### Pares de Região
Cada região do Azure está sempre emparelhada com outra região dentro da mesma geografia (como EUA, Europa ou Ásia) a pelo menos 300 milhas de distância. Essa abordagem permite:
- Replicação automática para alguns serviços.
- Recuperação de região priorizada em caso de interrupção
- As atualizações são lançadas sequencialmente para minimizar o tempo de inatividade.<br/>

<img src="https://www.class365.com.br/wp-content/uploads/2020/10/azurepairs.png" alt="Pares de Região"><br/>

### Regiões Soberanas Azure
As regiões soberanas do Azure são áreas geográficas que atendem a requisitos específicos de conformidade e residência de dados.(exemplo)

- US DoD Central, US Gov Virginia, US Gov Iowa e outras: são instâncias físicas e lógicas isoladas de rede do Azure para agências e parceiros do governo dos Estados Unidos. Esses datacenters são operados por pessoas selecionadas dos EUA e incluem certificações de conformidade adicionais.
- Leste da China, Norte da China e outras: essas regiões estão disponíveis por meio de uma parceria exclusiva entre a Microsoft e a 21Vianet, por meio da qual a Microsoft não mantém diretamente os datacenters.

### Referências
[Azure Fundamentals – Quase tudo que você precisa saber](https://www.class365.com.br/azure/azure-fundamentals-sumario/)<br/>
[Arquitetura do Azure: Seus principais Componentes](https://www.linkedin.com/pulse/arquitetura-do-azure-seus-principais-componentes-peixoto-cardoso/)<br/>

## Recursos do Azure
Recursos do Azure são entidades gerenciadas pelo Azure, como máquinas virtuais, redes virtuais e contas de armazenamento. <br/>
Alguns recursos do Azure incluem: <br/>
- Rede Virtual do Azure: Um serviço que permite que vários recursos do Azure se comuniquem com segurança entre si, com a internet e com as redes locais. 
- Azure Resource Manager: Uma ferramenta que facilita o gerenciamento e a visualização de recursos no aplicativo. 
- Provedores de recursos do Azure: Um conjunto de operações REST que habilitam a funcionalidade para um serviço específico do Azure. 
- SAP Hana: Uma combinação de banco de dados otimizado e serviço de nuvem, que aprimora o sistema de gestão ERP (Planejamento de Recursos Empresariais). 
- Azure Lighthouse: Uma ferramenta que permite o gerenciamento de recursos entre locatários. 
- Grupos de Recursos do Azure: Uma ferramenta que ajuda a organizar e segmentar projetos dentro do Azure.

## Grupo de Recursos
Um grupo de recursos do Azure é um contêiner que agrupa recursos relacionados a uma solução do Azure. Os recursos podem ser gerenciados como uma única unidade, o que ajuda na organização e no controle deles.<br/> 
Um grupo de recursos pode incluir todos os recursos para a solução ou apenas os que o usuário deseja gerenciar. <br/>
Alguns exemplos de recursos do Azure são:<br/>
- Máquinas virtuais, Redes virtuais, Contas de armazenamento.
- 
<img src="https://miro.medium.com/v2/resize:fit:866/format:webp/1*aSwyjD1c2BVQta7f-FuNTA.png" alt="Grupo de Recursos"><br/>

## Assinaturas do Azure
As assinaturas do Azure são contratos com a Microsoft que permitem o uso de serviços e plataformas de nuvem da Microsoft. Elas são unidades de gerenciamento, cobrança e escala, e são essenciais para a adoção do Azure em larga escala.<br/> 
As assinaturas do Azure têm várias finalidades, incluindo:<br/>
- Contrato legal: Cada assinatura é associada a uma oferta do Azure, que fornece um plano de tarifa, benefícios e termos e condições.
- Contrato de pagamento: Ao criar uma assinatura, o usuário fornece informações de pagamento, como um número de cartão de crédito.
- Limite de escala: As assinaturas têm limites de escala definidos, que não podem ser excedidos.
- Limite administrativo: As assinaturas servem como limite para administração, segurança e política.<br/>

## Grupos de Gerenciamento
Os grupos de gerenciamento do Azure são contêineres que permitem gerenciar o acesso, a política e a conformidade entre várias assinaturas. Eles oferecem gerenciamento de nível empresarial em grande escala, independentemente do tipo de assinatura.<br/> 
Você pode definir um grupo de gerenciamento como um escopo atribuível em uma definição de função personalizada do Azure. A função personalizada do Azure estará então disponível para atribuição nesse grupo de gerenciamento e em qualquer grupo de gerenciamento, assinatura, grupo de recursos ou recurso abaixo dele<br/>

### Referências
[O que é grupo de recursos do Azure](https://medium.com/@rodrigocameloMCT/o-que-%C3%A9-grupo-de-recursos-do-azure-a03ef0059ad8)<br/>
[Assinatura e Recursos do Azure](https://www.linkedin.com/pulse/assinatura-e-recursos-do-azure-leopoldo-peixoto-cardoso/)<br/>








