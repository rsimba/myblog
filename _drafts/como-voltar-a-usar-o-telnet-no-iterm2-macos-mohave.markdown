---
layout: "post"
title: "Como Voltar A Usar O Telnet No iTerm2 (MacOS Mohave)"
date: "2019-07-25 09:59"
category: Telnet
---
O Telnet é o mais antigo protocolo da suite TCP/IP para acesso remoto e que por razões de seguranca tem sido substituido pelo SSH, mas apesar disso o Telnet é ainda usado ou suportado em muitos sistemas e um dos exemplos sao os varios emuladores de redes em a primeira opcao de ter acesso aos dispostivos é o Telnet.

A Apple é daquelas empresas que faz as coisas de forma diferente e foi mais longe em remover completamente o Telnet do seu último Sistema Operativo, o **macOS Mojave**, por razoes de segurança. Se estivermos a usar o **iTerm2** para aceder um dispositivo via telnet, recebemos a seguinte mensagem:
<img src="/assets/iterm2_telnet_msg.jpg" class="align-center">

A solucao mais simples é instalar o Telnet usando o Homebrew:

{% highlight brew %}

brew install telnet

{% endhighlight %}

Nas versoes anteriores do macOS, o Telnet estava localizado no directorio **/usr/bin/** mas na actual versao, encontramos no **/usr/local/bin/**. É por esta razao que o iTerm2 está a reclamar.

A forma mais simples de dizermos ao iterm2 onde encontrar o Telnet é definirmos o caminho completo da aplicacao (**/usr/local/bin/telnet $$HOST$$ $$PORT$$**) na secção dos perfeis, por exemplo:
<img src="/assets/iterm2_profiles.jpg" class="align-center">

Depois disso teremos o acesso remote usando o iterm2.
<img src="/assets/iterm2_telnet_success.jpg" class="align-center">
