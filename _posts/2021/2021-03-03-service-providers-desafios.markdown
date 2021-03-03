---
layout: "post"
title: "Service Providers: Desafios"
date: "2021-03-03 13:12"
category: Service Provider
comments: true
author: Simba, R. H. N.
---
Os _ISPs_ começaram a ganhar popularidade na década de 1990 quando a Internet passou a ser usado para fins comerciais. Nesta mesma fase, a maior competição dos _ISPs_ vinham das grandes empresas de Telefonia que tinham equipamentos e tecnologias maduras que os permitia oferecer serviços diferenciados tais como  Voz e VPN, ao contrário dos _ISPs_ que apenas ofereciam acesso à Internet.

Desde o seu princípio nos anos 1980, a Internet evoluiu para um meio de comunicação inovador e com muitas possibilidades. No centro destas inovações estão os [_ISPs_](https://www.ricardosimba.com/service%20provider/2021/02/20/service-providers-introducao.html) por serem um dos elementos que asseguram a infra-estrutura da Internet. É dentro destas inovações e possibilidades que surgiram os operadores de serviços Web e de conteúdo, e passamos a ver outra categoria de operadores (cloud) com infra-estrutura a partir da qual muitos desses novos serviços funcionam, e hoje são responsáveis por gerar a maior parte do tráfego global da Internet.

A indústria criada pelos SP de cloud é tão forte que está a influenciar virtualmente todas as tecnologias e soluções neste ramo, alterando a estrutura clássica da Internet, e afectando também modelo de negócios.

## _ISPs_ e Concorrência
Se no passado a maior concorrência para os _ISPs_ vinha das grandes empresas de telefonia (Telcos), hoje os seus maiores concorrentes são os Operadores de Serviços de Cloud. Por dois principais motivos: primeiro por forcarem os _ISPs_ numa posição de acesso; segundo pela agilidade natural do seu modelo de negócio.

### O Papel dos ISPs
Para termos uma ideia, hoje, a maior parte do tráfego global da Internet é o vídeo e isto tende a aumentar a medida que novas tecnologias de acesso como o 5G forem surgindo e muitos mais dispositivos ligarem à Internet. Isto quer dizer que, mais e mais usuários deverão  consumir  conteúdos de empresas como o Youtude, Netflix, Amazon Prime Video, e muitos outros. Estas empresas de gestão de conteúdos têm uma coisa em comum, todas funcionam a partir de uma infra-estrutura de Cloud, isto é, são quase todas clientes da AWS, Azure, GCP, etc., é também por esta razão que estas empresas são chamados de OTT (_Over_The_Top Providers_). E como o tráfego precisa chegar ao cliente final de uma forma eficiente, as CDNs como a Akamai, Limelight, etc., são usadas para a distribuição destes conteúdos (tópico para outro artigo).

Do ponto de vista dos SP de Cloud, os _ISPs_ têm dois (2) principais papeis: de manter a infra-estrutura da Internet e por trazerem clientes as suas redes. Podemos entender melhor olhando para a topologia de rede desses _SPs_. Tal como a Internet, estas redes são construidas de forma distribuída e redundante: primeiro são criados vários _Data Centers_ (DCs) em diferentes pontos geográficas chamados regiões ou zonas, a seguir é criada uma rede (core ou backbone) para interligar todos esses DC, por fim, é preciso possibilitar diferentes clientes consumirem os serviços disponíveis nos DC (preferencialmente no DC mais próximo geograficamente) e isto é feito a partir do acesso ou Edge, conforme ilustrado:
<img src="/assets/Cloud1.jpg" class="align-center">

Conseguimos ver no desenho que do ponto de vista da Cloud, os _ISPs_ são simplesmente o meio pelo qual clientes de várias partes do mundo ligam-se à sua rede e consumem os seus serviços. Para possibilitar que mais possíveis clientes estejam ligados à Internet, tem havido varias iniciativas por parte dos SP de cloud em oferecer incentivos ou tecnologias aos _ISPs_ para permitir mais conectividade de pessoas à Internet, exemplo dessas iniciativas são o Google Fibra, Facebook Teragraph, e os vários cabos submarinos iniciados ou patrocinados por um ou vários SPs de cloud.

### Operações Baseadas em Cloud
Uma das características interessantes das redes Cloud é que são uma mistura de processos e tecnologias de sistemas e de redes. Ao tirar o melhor dos dois mundos, adoptaram processos e tecnologias e processos únicos que lhes permite ter maior agilidade, flexibilidade, facilidade, e muita automação, para puder gerir aquando de informação que é esperado dos seus vários serviços. A Cloud si, é muito mais do que o tipo de serviço (IaaS, PaaS, SaaS) ou arquitectura em geral, é também sobre como as suas redes são operadas e testadas continuamente em grande escala, ou como pensamos sobre estas redes e que processos usados para realizar uma actividade, é sobre a agilidade e rapidez, sobre as ferramentas certas a usar.

É pelas razões citadas no parágrafo anterior que soluções baseadas em Cloud conseguem atender melhor as necessidades imediatas do cliente porque hoje todos nós queremos serviços o mais rápido possível. Por exemplo, quando queremos usar os serviços da AWS basta usarmos um portal e em menos de minutos temos o serviço disponível, o mesmo acontece quando queremos comprar algum artigo online, bastam alguns cliques e dias depois temos o artigo, em nenhum momento temos de ligar para algum operador para facilitar a venda ou a configuração do serviço - é tudo automatizado.

O mesmo não acontece com os _ISPs_, muitos continuam a operar as suas redes tal como operavam décadas atrás. Por exemplo: recentemente mudei de uma residência para outra e uma das minhas prioridades era ter acesso à Internet o mais rápido possível. A nova residência já tinha instalações prontas para a Internet mas em nome do antigo residente. Com esses dados, bastava apenas fazer um contracto com o SP e eles poderem associar todos os dados técnicos e serviços necessários em meu nome. Para a minha surpresa, fui informado de que a migração dos dados de um cliente para o outro leva o máximo de 96 horas e o roteador levaria 2-5 dias para ser entregue, 1-2 semanas caso me encontrasse numa outra província. Parte destes tempos é a forma que os SPs estão organizados, existe um SP responsável pela infra-estrutura e muitos outros SPs responsáveis pelos serviços. No meu caso, levou-me cerca de um (1) dia para ter acesso à Internet, primeiro porque tinha o meu próprio roteador e não tinha de esperar os 2-5 dias e segundo porque tive de fazer várias chamadas e enviar vários emails ao SP.

Este é um exemplo de quanto tempo pode levar para um cliente residencial ter finalmente o serviço de Internet activo, claro para um cliente empresarial os tempos são geralmente mais curtos.

## Como Ultrapassar Estes Desafios
Independente do serviço oferecido, os _ISPs_ precisam um modelo de negócio baseado na cloud, implementar princípios como DevOps e tecnologias como o SDN ou NFV. _ISPs_ devem adoptem soluções baseadas em Cloud e usar os mesmos processos e ferramentas usadas pelo SP Cloud de para mais agilidade e rapidez na operação da rede e oferta de serviços. Além disso, ISPs precisam também diferenciar o seu portefólio de serviços e não estar apenas limitado no simples acesso à Internet, é preciso passar a criar outras fontes de rendimentos tais como conteúdos ou Clouds (publicas, privadas, ou híbridas), para tal é importante que ISP invistam em DCs e outra tecnologias.

Hoje já existem soluções de fabricantes que permitem um _ISP_ adoptar implementar solução baseadas em cloud em que o cliente tem acesso a um portal e a partir do mesmo activar/desactivar serviços conforme quiser.

E claro, além da tecnologia, é importante que engenheiros a operar tais redes, sejam treinados nas mesmas tecnologias.

# Resumo
O cliente que consume os vários serviços está hoje mais exigente e estará ainda mais amanha e não ira tolerar longos tempos de espera para a activação de serviços, e querem maior autonomia sem ter que lidar com muitas pessoas. Os ISPs no que lhe concerne, devem entender isso e  procurar adoptar soluções baseadas em cloud para melhor atender as exigências dos clientes e manter-se em frente da concorrência ou ver a sua existência ameaçada.


Abraços,
