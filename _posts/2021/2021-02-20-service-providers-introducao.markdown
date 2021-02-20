---
layout: "post"
title: "Service Providers: Introdução"
date: "2021-02-20 07:27"
author: Simba, R. H. N.
comments: true
category: Service Provider
---
Do ponto de vista estrutural, a Internet é organizada de forma hierárquica e composta por vários componentes fundamentais interligados entre si, um desses componentes são os Operadores de Serviços de Internet ou **Internet Service Provider **(ISPs) como são tradicionalmente chamados em Inglês.

**Nota. ** Hoje, estes Operadores são simplesmente chamados de Operadores de Serviços ou _Service Providers_(SP). Por esta razão, preferi usar a abreviação _SP_ na maior parte do artigo ao invés de Operador de Serviços de Telecomunicações para não confundir o leitor, porque geralmente as diferentes soluções de fabricantes para este seguimento, os treinamentos, as certificações, etc., estão sempre descritos _SPs_ e não por outro nome.

Na visão clássica da Internet, existem três (3) diferentes classes de SPs e esta classificação tem como base factores como o tamanho e a cobertura das suas redes:
- **SPs Globais**. Constituem o Backbone da Internet e pelo alcance global das suas redes, são classificados de _Tier 1_ e estão no topo da hierarquia.
- **SPs Regionais**. A rede desta categoria de SPs têm uma cobertura regional e são classificadas de _Tier 2_. Na hierarquia, são o ponto intermédio entre os _Tiers 1_ e _Tiers 3_.
- **SPs Locais**. Também conhecidos por SP de Acesso, _Edge_ ou _Tier 3_, são SPs em que tradicionalmente os clientes finais ligam-se para ter acesso à Internet.

SPs não operam de forma independente, as suas redes são interligadas (processo conhecido por _Peering_) entre si para então constituir a infra-estrutura da Internet (a rede de redes) e existem certos requisitos, padrões, e custos a considerar para que esta interligação seja possível.

<img src="/assets/Canvas1.jpg" class="align-center">

No passado a classificação do SPs em termos funcionais foi mais exclusiva, hoje com a existência dos Operadores de Conteúdos como a Amazon, Netflix, e outros, existe uma remodelação em curso na estrutura da Internet em que o objectivo é oferecer uma melhor experiência de serviços aos clientes finais e isto obriga muitos dessas empresas a ter as suas infra-estruturas mais próximas do cliente. E não apenas isto, hoje vemos SPs globais e regionais a oferecerem também serviços aos clientes finais e operarem em simultâneo, como SPs de acesso.

Do ponto de vista técnico, a Internet é um sistema complexo e existem muitos outros componentes fundamentais e que foram propositadamente excluídos deste artigo, mas que serão parte de futuros artigos, por exemplo: as CDNs, os IXPs, e as várias organizações que mantêm importantes serviços como DNS, domínios, IPs e Números Autónomos públicos, e outros.

# O que é um SP?
Em telecomunicações, um SP não é nada mais que uma empresa pública ou privada que oferece aos seus clientes diferentes serviços, tais como o acesso à Internet, serviços de Voz, Vídeo, Nuvem, Conectividade, e outros, usando diferentes meios de comunicação (Cabo, Wireless, Fibra, Satélite, etc.).
 
Hoje, independente do serviço oferecido, estas empresas de telecomunicações são simplesmente chamadas ou classificadas de Operadores de Serviços Telecomunicações, ou _Service Provider_ e todos podem oferecer os mesmos serviços, desde que as suas infra-estruturas permitam. No entanto, nem sempre foi assim, no passado estas empresas eram classificadas de acordo ao serviço fornecido, por exemplo, existiam os Operadores de Serviços de Telefonia Fixa (tradicionalmente chamados de _Telcos_), os de Telefonia Móvel, Operadores de Serviços de TV por Cabo, Operadores de Serviços de Internet (_ISPs_), e outros. Cada um desses operadores, tinham infra-estruturas criadas e optimizadas especificamente para suportar um determinado serviço e quem quisesse oferecer mais de um serviço, tinha de obrigatoriamente criar e suportar mais de uma infra-estrutura rede, por exemplo, uma de voz e uma de dados e ai fora.
 
Esta situação não só limitava a capacidade de crescimento e a diversificação de serviços dos Operadores existentes na altura como também limitava a entrada de novas empresas no sector ou empurrava outras para a falência devido ao monopólio natural que muitos desses operadores tinham (principalmente os Operadores estatais). Do ponto de vista de um cliente, havia também um grande transtorno devido aos diferentes equipamentos de diferentes Operadores que era obrigado a ter instalado, assim como o cliente era obrigado a lidar com mais de um Operador. Contudo, com o andar do tempo e com a evolução / maturidade das tecnologias, isto ainda na década de 1990, as coisas começaram a mudar para melhor e houve necessidade de acelerar o processo de convergência de serviços em uma única infra-estrutura, dois principais factores estiveram no centro deste processo:
1. **Convergência de serviços para uma única Infra-estrutura**. Muitos dos diferentes serviços fornecidos por vários operadores, passaram a ser suportados por uma única tecnologia que é o IP/MPLS e tecnologias como o ATM que suportavam um serviço específico, tornaram-se obsoletas. Este processo permitiu que uma única infra-estrutura fosse necessária para suportar diferentes serviços.
2. **Abertura de mercados de telecomunicações**. Ao mesmo tempo, foram criados em muitos países regulamentos que permitiram a abertura do mercado de telecomunicações, permitindo a convergência digital no seu todo e um ambiente mais competitivo.
 
Por estas e outras razões, hoje temos serviços como Voz, Vídeo, e outros, todos a serem fornecidos por cima de uma infra-estrutura baseada em IP, o que fez com que mais empresas do género surgissem e com um portefólio de serviços de telecomunicações diferenciado e competitivo. E por fim, com esta convergência, os diferentes Operadores passaram a ser simplesmente denominadas de Operadores de Serviços ou _Service Providers_ ao invés de serem caracterizadas com base ao serviço oferecido.

## O que difere um SP de outras Empresas?
Como vimos acima, um SP pode ser uma empresa com actividades comerciais como qualquer outra a operar num sector diferente e hoje as TICs estão presentes virtualmente em todas as empresas, independente da sua actividade de negócio. Contudo, diferente de outras empresas em que as TICs ou rede em particular é vista como um elemento facilitador e na inexistência da mesma a empresa poderá continuar a gerar receitas, para um SP a rede é o seu primeiro produto e a sua principal fonte de rendimento, é a partir dela onde vários serviços são criados e comercializados ao cliente final. 
 
Sem uma infra-estrutura de rede não há SP, por esta razão, estas redes têm e devem ter maior atenção assim como são naturalmente planeadas, desenhadas, e implementadas em grande escala com o objectivo de cobrir áreas maiores.

## Plano e Desenho da Rede
O mercado das telecomunicações é altamente competitivo e há mais hipóteses em um SP não sobreviver se não fizer investimentos inteligentes na sua rede e na capacitação do pessoal que opera a mesma. Na altura do planeamento e desenho da rede, um SP deve decidir quem será o cliente alvo (empresarial ou residencial) e aonde estes estão geograficamente organizados. Com esta informação e com base a tecnologia de acesso a ser usada, o é possível traçar um plano de cobertura e construir a rede de acordo a estes dados obtidos durante o planeamento.
 
Do ponto de visto físico e lógico as redes geralmente são compostas por duas camadas: de Transmissão e Serviços. A camada de transmissão pode ser composta por qualquer meio de comunicação usado para interligar os equipamentos de rede; e a camada de serviços (também conhecida de _overlay_) é composta por equipamentos e protocolos (IP/MPLS) que permitam a criação de diferentes serviços.
 
Pelo seu requisito de possibilitar possíveis clientes localizados em diferentes pontos geográficos de uma cidade, pais, ou continentes, existem determinados princípios fundamentais a considerar quando as mesmas são planeadas e desenhadas para evitar complexidades durante a implementação e operação. Exemplo desses princípios são: modular, redundância, simplicidade, hierarquia e outros. 

<img src="/assets/Canvas2.jpg" class="align-center">

Vemos na seguinte imagem a exemplo de um desenho de rede modular e hierárquico e que é um desenho tradicional de redes de grande escala tal como a de um SP.  Para facilitar a operação, o funcionamento, a gestão e outros, a rede segmentada em três (3) diferentes domínios e cada um com funções especificas:
- **Acesso**. Que tem a ver a com os vários equipamentos de rede, meios de comunicação, e protocolos que possibilitam um cliente ligar-se na rede do SP para posteriormente consumir os serviços contratados,
- **Agregação**. Que tem a ver com os vários equipamentos de rede, meios de comunicação, e protocolos com o objectivo de agregar o tráfego de vários clientes numa determinada localização geográfica,
- **Core**. Que tem a ver com os vários equipamentos de rede, meios de comunicação, e protocolos com o objectivo de facilitar o tráfego entre clientes localizados em diferentes zonas e facilitar o consumo generalizados de serviços fornecidos aos clientes,

## Receitas e Despesas
Do ponto de vista de negócio tal como qualquer outra empresa comercial, um SP deve considerar dois importantes aspectos ligados à contabilidade da empresa: receitas e despesas. É importante que existam várias opções para gerar receitas financeiras que permitam a empresa cobrir as suas despesas e em simultâneo ter algum rendimento; da mesma forma e como em qualquer negócio, haverão sempre despesas e estas nunca devem ser maiores que as receitas para que uma empresa seja rentável.

<img src="/assets/Canvas3.jpg" class="align-center">

### Opções de Receitas
Tal como já frisei, a fonte principal de receitas de um SP é a infra-estrutura de rede que pode suportar vários serviços. Contudo, é possível existirem outras opções de receitas tais como as quatro (4) listadas a baixo:
1. **Rede**. Considerando as duas camadas discutidas acima (transmissão e serviços), geralmente é possível um SP criar serviços em cada uma dessas camadas. Por exemplo, consideremos a fibra Óptica (DWDM) como parte da transmissão e claro por cima temos a camada de serviços suportada pelo IP/MPLS, é possível dividirmos os possíveis serviços oferecidos em duas partes:
     1. Serviços oferecidos na camada IP/MPLS: residências (Internet, IPTV, voz, conteúdo, etc.), empresarial (L3VPN, L2VPN, etc.) Móvel, _Peering_, transito, e outros.
     2. Serviços oferecidos na transmissão: linhas privadas OTN, TDM, DWDM, etc.
2. **Data Center**. Muitos SPs constroem DCs em zonas estratégicas onde muitos dos seus equipamentos são instalados e a partir do qual serviços de Nuvem podem ser oferecidos. Em simultâneo, é possível arrendar espaços nestes DCs às clientes interessados.
3. **Serviços geridos** (MSP na sigla Inglesa). Outra opção de receitas  e são os serviços geridos oferecidos aos seus clientes em forma de suporte ou produtos.
4. **Revenda**. Em alguns casos um SP pode funcionar também como um revendedor, vendendo equipamentos de rede directamente aos seus clientes.  

### Despesas
Para que um SP continue a ser competitivo e a oferecer serviços ou suporte de qualidade, investimentos devem ser feitos na rede e no capital humano, e isto significa despesas. Para além dessas despesas óbvias, podemos resumir em três (3) diferentes formas de despesas que quase sempre farão parte de um SP: 
1. **Rede**. É importante um plano de investimento um investimento equilibrado na infra-estrutura de rede para manter um alto nível de serviços, por exemplo, avaliar e actualizar a largura de banda interna e externa, investir em equipamento físico próprio para a classe de SPs, arrendar ou comprar locais que funcionem como PoPs, etc.
2. **Pessoas**. SPs precisam de engenheiros capacitados para operar, monitorizar a rede interna e oferecer um suporte de primeira classe aos seus clientes, para tal, é importante que estes profissionais sejam remunerados de forma aceitável. Não apenas salários, um SP precisa de criar incentivos assim como criar e manter um plano continuo de treinamento do seu pessoal.
3. **Licenças** e outros. Outras despesas têm a ver com questões legais, por exemplo, o pagamento de licença de SP que o permitam operar num determinado país ou área.

# Operação Normal
Tal como qualquer outra organização comercial e de acordo a certos critérios, um SP é dividido em vários departamentos e funções para facilitar gestão de certas actividades e operações que em condições normais seriam complexas devido ao tamanho  natural da rede  e das várias tecnologias usadas. Estes são os departamentos normalmente encontrados num SP: 
- **Vendas**. Normalmente o primeiro ponto de contacto quando um possível cliente mostra interesses nos serviços de um determinado SP.
- **Apoio ao cliente**. Responsável em gerir as chamadas de clientes com problemas e encaminhar certos problemas a outras áreas.
- **Engenharia**. Este departamento tem principalmente a ver com questões relacionadas a rede e pode ser subdivido em vários outros departamentos:
     -  **Activação**. Responsável em criar, com base a informação obtida pela área de vendas, o perfil de um cliente para a posterior activação ou desactivação do mesmo.
     - **Backbone** ou **Core**. Responsável em manter rede IP do SP 
     - **NOC**. Responsáveis em monitorizar a rede e notificar outros departamentos sobre possíveis problemas ou pedir a resolução de um problema identificado.
     - **Infra-estrutura**. Responsável instalar novos sites na rede ou resolver problemas pontuais que possam surgir. 
     - **instalação**. Responsável em instalar novos cliente ou resolver problemas nos clientes ao nível de transmissão.
- **Finanças**. Responsável pela gestão das receitas e despesas do SP.

Outros departamentos não técnicos mas também importantes podem ser o **RH**, _marketing_, treinamento, e outros.

## Interacção entre Departamentos
Os departamentos acima descritos operam de formas independente e, em simultâneo, dependente de outros departamentos, e podemos ilustrar esta operação usando dois exemplos.

<img src="/assets/Canvas4.jpg" class="align-center">

### Novo Cliente
Por norma, o ponto inicial de comunicação para possíveis clientes é o departamento de **vendas** e a mesma é feita principalmente a partir de números telefónicos ou email. Durante este contacto, o cliente é informado das várias opções de serviços, preços, uma explicação do contracto de serviços que posteriormente devera ser aceite pelas duas partes. No que lhe concerne, a equipa de vendas, usando ferramentas próprias, cria o perfil do cliente que é partilhado com outros departamentos: **activação**, para a criação do perfil de serviço do cliente com os requisitos de largura de banda, QoS, e outros detalhes tal como foram estipulados pelo contracto de serviço; **finanças**, para a criação do mesmo perfil nos seus sistemas e ter o controle financeiro dos pagamentos ou não pagamentos; **instalação**, para o agendamento da instalação dos equipamentos no cliente.
 
Dependendo de muitos factores como a seriedade do SP e do cliente (residencial ou empresarial), o processo todo desde o primeiro contacto até o cliente ter os devidos equipamentos instalados e poder consumir os serviços contratados, pode levar horas, dias ou mesmo semanas.

Quando estiver tudo estiver ultrapassado e o cliente estiver feliz e consumir os serviços contratados, é normal existirem problemas técnicos e que mereçam atenção do SP. Quando isso acontece, o cliente tem como a primeira linha de contacto o departamento de Apoio ao Cliente que irá receber a chamada do cliente, fazer alguns despistes por telefone, criar um _ticket_,  e caso o problema não for resolvido, o operador devera encaminhar uma ocorrência do problema ao departamento mais apropriado para resolver o mesmo.

### Infra-estrutura
A rede precisa ser monitorada constantemente para ser protegida de possíveis problemas que possam surgir e que possam interromper o normal funcionamento dos serviços fornecidos aos clientes. Quando a rede estiver operacional é preciso que se tenha visibilidade e monitorizar de formas a estar notificado de problemas existentes ou que possam existir, o **NOC** é o responsável por esta tarefa em manter a rede em constante monitorização assim como a ligacao de determinados clientes considerados cruciais para a empresa ou que tenham uma clausula no seu contracto que permita este serviço. Em termos técnicos, geralmente irão existir dois problemas: IP e transmissão. Na eventualidade de existir um problema considerado de nível IP, o NOC tem como tarefa em notificar o departamento **Core** ou **Backbone**; ao passo que se o problema for de nível de transmissão, o NOC irão notificar o departamento de **infra-estrutura** para a resolução do mesmo.
 
Quando consideramos o crescimento e expansão da rede, muitos novos sites ou PoPs deverão ser instalados com os devidos equipamentos de rede: transmissão e IP, e os dois departamentos devem trabalhar em conjunto para que o novo PoP esteja operacional.

# Resumo
Existem SPs de vários tipos, uns maiores e outros menores e de uma forma geral qualquer empresa que comercialize serviços de telecomunicações tais como a Internet é considerado um SP. Levando isto em consideração, neste _post_ falei de forma resumida os conceitos básicos, a operação, e outros, que podem se aplicar a qualquer SPs independente do tamanho ou da tecnologia de transmissão a usar. Quanto a organização e nomes de departamentos, muitos SPs usam uma nomenclatura diferente que vá de acordo aos seus objectivos e funções, no entanto, a função será a mesma comparando a outros SPs que tenham um nome diferente para um certo departamento. 

 
Abraços,
