---
layout: "post"
title: "Migração do DS214Se para o RS820+"
date: "2021-02-24 06:53"
category: Geral
comments: true
author: Simba, R. H. N.
---
Quando se trata de dispositivos para armazenamento de dados e ‘backups’, o Synology é a minha escolha. Desde 2017 que usava o Synology DS214Se, mas no fim do ano passado começou a mostrar sinais de cansaço e num desses dias deixou simplesmente de funcionar. Decidi actualizar o DS por uma opção mais potente e com mais espaço de armazenamento, o Synology RS820+.

## Especificações
O RS820+ é considerado um dispositivo de armazenamento de classe empresarial e tem as seguintes especificações técnicas:
- Suporta o máximo de 56TB de disco divididos em 4, cada disco com 14TB
- 4x Portas Gigabit com opção de instalar uma carta de 10Gbps 
- CPU com 4-core 2.1 GHz
- 2GB de memória DDR4 e extensível até 18GB

De momento estou com 3TB num único disco e com planos de aumentar a capacidade com o tempo.

## Software
Uma das partes que mais gosto nos Synology é o básico e rápido Sistema Operativo, chamado DSM e que para além de básico, traz consigo muitas inovações e suporte de muitas funcionalidades.

## Migração do DS214Se para RS820+
Geralmente, a instalação dos produtos Synalogy são feitos de forma simples é rápida. Para começar, as portas de rede destes dispositivos vêm configurados como servidores de DHCP atribuem automaticamente o IP 169.254.129.70 e que será reconhecido ao usar o Synology Assistant a partir do computador. Segue a baixo o passo a passo da minha migração:

1. Ligar o computador ao Synology e configurar de formas a receber o IP automaticamente. Fazer a transferência e instalar o Synology Assistant que irá ajudar-nos a identificar o Synology e fazer as configurações básicas.
<img src="/assets/Syno1.jpg" class="align-center">
<img src="/assets/Syno2.jpg" class="align-center">
2. Como instalei um dos discos do DS214Se no RS820+, automaticamente foi reconhecido e o RS820+ apresenta a opção de migração dos dados  ao invés da formatar o disco.
<img src="/assets/Syno3.jpg" class="align-center">
<img src="/assets/Syno4.jpg" class="align-center">
3. A seguir, precisamos instalar a versão actual do DSM que deve ser transferido da página da Synology.
<img src="/assets/Syno5.jpg" class="align-center">
<img src="/assets/Syno6.jpg" class="align-center">
<img src="/assets/Syno7.jpg" class="align-center">
4. A instalação  do Sistema Operativo leva cerca de 10 minutos para concluir e irá reiniciar assim que terminar.
<img src="/assets/Syno8.jpg" class="align-center">
<img src="/assets/Syno9.jpg" class="align-center">
5. Depois de reiniciar, temos de criar um usuario admin a palavra passe para termos acesso ao sistema.
<img src="/assets/Syno10.jpg" class="align-center">
6. Opcionalmente, criamos ou adicionamos uma conta Quickconnect que nos permite ter acesso ao dispositivo a partir da Internet.
<img src="/assets/Syno11.jpg" class="align-center">
7. E com este último passo, finalmente temos acesso ao dispositivo pronto para ser usado e para configurações adicionais.
<img src="/assets/Syno12.jpg" class="align-center">

## Conclusão
Há muitas possibilidades de uso deste dispositivo de armazenamento que explorarei com o tempo assim como diminuir a minha dependência de algumas opções de armazenamento na Nuvem. Os Synology funcionam e fazem bem o seu serviço e não precisamos ser especialistas para instalar e fazer funcionar.
 
Seguem aqui alguns links interessantes:

[Synology DS214Se](https://www.amazon.com/gp/product/B0855LMP81/ref=as_li_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=B0855LMP81&linkCode=as2&tag=rsimba-20&linkId=20e3b99fb6b464ab19b1b5151f588623)

[Synology RS820+](https://www.amazon.com/gp/product/B07YBX86C2/ref=as_li_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=B07YBX86C2&linkCode=as2&tag=rsimba-20&linkId=3e4d6e4408580a2bbef70cea4d0069e6)

[Synology RS820+ Especificações](https://www.synology.com/en-global/products/RS820+)

[Synology RS820+ guia de instalação](https://global.download.synology.com/download/Document/Hardware/HIG/RackStation/20-year/RS820+/enu/Syno_HIG_RS820_Plus_RS820RP_Plus_enu.pdf)


Abraços,
