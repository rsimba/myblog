---
layout: "post"
title: "Servidor para Lab"
date: "2020-07-21 10:17"
author: Simba, R. H. N.
comments: true
category: ferramentas
---
Já faz algum tempo desde que me desfiz do meu pequeno lab, constituído na altura por uns poucos switches e roteadores da Cisco. Desde então, tenho feito o uso quase exclusivo de plataformas virtuais a partir de um portátil, principalmente para pequenos e rápidos testes.

A tecnologia de virtualização, em particular em redes, está hoje mais desenvolvida e estável. Ao mesmo tempo, os principais fabricantes têm disponível versões dos seus Sistemas Operativos de Redes que são agora facilmente virtualizados, (considerando que os requisitos mínimos dos recursos físicos são atendidos), permitindo o uso ou teste de funcionalidades / tecnologias em um servidor sem a necessidade de um roteador ou switch físico.

Os portáteis são OK para pequenos e rápidos labs mas estaremos sempre limitados aos seus recursos físicos que são no geral mínimos. Tendo em consideração a esta limitação e a necessidade de criar labs que exijam mais da máquina *host*, decidi investir em um servidor segunda mão para este fim e desta forma tirar ainda mais proveito das plataformas virtuais existentes.

## Objectivos

Com este laboratório pretendo alcançar dois principais objectivos:
- O teste de funcionalidades, tecnologias e soluções antes de apresentá-las como funcionais aos clientes com quem eu trabalho
- Como parte do material de estudo para as diversas certificações técnicas

## O Servidor

No geral, os servidores são equipamentos caros, contudo, é possível comprar servidores dos maiores fabricantes em segunda mão à um preço razoável e em bom estado de conservação. De facto, existem empresas especializadas na venda destes tipos de servidores.

Na escolha de servidores para o uso das plataformas virtuais de redes, devemos levar em considerações as seguintes importantes características: CPU (a quantidade de CPUs físicos e a quantidade de cores por CPU, assim como a tecnologia de virtualização usada nestes processadores), memória e armazenamento.

No meu caso, acabei por usar um [IBM System x3650 M4](https://lenovopress.com/tips0850-system-x3650-m4-e5-2600-v2) que tem as seguintes principais características físicas:
- Suporte máximo de 2 CPUs físicos
	- Suporte aos processadores Intel Xeon E5-2600v2, máximo de 12 cores por CPU.
- Suporte para 24 memórias físicas
	- Permitindo ter o máximo do total de 768GB de memória.
- Suporte máximo de 28.4TB de armazenamento
- Suporte mínimo de 4 portas de 1-GigabitEthernet

**Nota**. Boa parte dos processadores Intel (incluindo os da família Xeon E5-2600v2) o suportam a tecnologia *Hyper-Threading* que na pratica duplicate o numero total de cores. Isto é, caso um processador suporte 10 cores, com o *Hyper-Threading* este número é duplicado por dois, 20.

Apesar deste servidor ter o máximo das características listadas acima, a actual configuração dependerá de vários factores. No meu caso, tenho o servidor configurado da seguinte forma:
- 2x CPUs com 10 cores em cada CPU, totalizando 20 cores
- 24x memórias de 8GB cada, totalizando 192GB
- 8x Discos de 600GB cada, totalizando 4.8TB

<img src="/assets/ESXi.jpg" class="align-center">

Ao invés de instalar um Sistema Operativo e usar os recursos da máquina na sua totalidade, optei por usar o VMWare ESXi como o *hypervisor*, para a criação e gestão de várias máquinas virtuais.

## Requisitos Mínimos das Imagens dos Roteadores e Switches

As plataformas como o CML, EVE-NG e GNS3, usam várias imagens que os fabricantes têm disponíveis para virtualização e estas imagens têm requisitos mínimos próprios para o seu funcionamento normal num ambiente virtual.

Por exemplo, a Cisco tem disponível as imagens do Sistema Operativo dos seus principais productos para uso em ambiente virtual e cada uma dessas imagens tem requisitos próprios de CPUs, memória, e armazenamento, por exemplo, para o IOS XRv 9000, os seguintes requisitos mínimos são necessários:
- 1 CPU virtual com o mínimo de 2 cores
- 12GB de memoria virtual, é recomendado o uso de 19GB de memoria caso portas de 10G são usadas para interligar vários roteadores.
- 45GB de armazenamento
- Mínimo de 4 Portas de rede, onde 1 para gestão, 2 reservadas, e 1 para o tráfego normal.

O que quer dizer que com a configuração actual do meu servidor onde tenho disponível o total de 40 cores de processadores (*Hyper-Threading* duplica os números de cores em cada CPU), 192GB de memória… Ao olhar para o processador, é possível simular o total de 20 roteadores (40 / 2 = 20) a correrem o IOS XR. Contudo, temos limitação na memória total disponível, que neste caso nos permite apenas simular 16 roteadores (192GB / 12GB = 16GB) ou 15 para deixarmos algum recurso para a maquina *host* usar.

## Resumo

Tal como referi acima, as tecnologias de virtualização estão mais maduras, confiáveis, e estáveis permitindo a substituição dos caros hardwares para uso em ambientes de produção, testes ou estudos.

Contudo, o processo da escolha de um servidor minimamente perfeito para as nossas necessidades pode ser exaustivo e caro. Por isso, é importante saber primeiro os requisitos mínimos das imagens dos Sistema Operativo que queremos virtualizar e a dimensão da topologia em que queremos testar as várias tecnologias ou funcionalidades.

Por último, considerar os gastos da corrente eléctrica visto que servidores no geral consumem mais que um portátil e claro o barulho, as ventoinhas dos servidores fazem muito mais barulho e num espaço pequeno podem facilmente tirar o sossego a qualquer um.

Abraços,
