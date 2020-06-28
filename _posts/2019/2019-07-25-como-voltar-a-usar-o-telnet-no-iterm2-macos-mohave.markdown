---
layout: "post"
title: "Como Voltar A Usar O Telnet Com O iTerm2 No macOS Mojave"
date: "2019-07-25 09:59"
categories: Ferramentas
comments: true
author: Ricardo Simba
---
O Telnet é o mais antigo protocolo da suite TCP/IP usado para o acesso remoto aos dispositivos de rede e que por razões de segurança tem sido substituído pelo SSH. Mas apesar disso, o Telnet é ainda usado ou suportado em muitos sistemas e um dos exemplos são os vários emuladores de redes em que a primeira opção de ter acesso aos roteadores e switches dos labs é usando o Telnet.

Os Sistemas Operativos da Apple são também conhecidos pelo seu nível de segurança e foi por esta razão que decidiram remover completamente o Telnet do **macOS Mojave**. Vamos a seguir ver como trazemos de volta o Telnet neste sistema e usa-lo com o iTerm2.

O **iTerm2** é um dos terminais *Open Source* para os Macs e podemos ver pela mensagem abaixo o que acontece quando o iTerm2 é instruído em usar o Telnet mas não encontra o mesmo:
<img src="/assets/iterm2_telnet_msg.jpg" class="align-center">

Existem diferentes soluções para este problema e vamos aqui ver a mais simples. Independente da solução, começamos com a instalação do Telnet usando o **Homebrew**:

{% highlight brew %}

brew install telnet

{% endhighlight %}

Nas versões anteriores do macOS, o Telnet estava localizado no directório **/usr/bin/** e já na actual versão, encontramos no **/usr/local/bin/** e é por esta razão que o iTerm2 está a reclamar.

Feita a instalação e o Telnet testado com sucesso, a seguir instruimos o iTerm2 aonde deve procurar pelo Telnet e executar, para isso usamos a seguinte linha na secção dos perfis: **/usr/local/bin/telnet $$HOST$$ $$PORT$$**:
<img src="/assets/iterm2_profiles.jpg" class="align-center">

E feito isto, temos novamente acesso aos nossos dispositivos usando o Telnet:
<img src="/assets/iterm2_telnet_success.jpg" class="align-center">

## Conclusão
O que descrevi aqui é principalmente verdade para casos em que estamos a usar um programa que para executar uma determinada tarefa, tem de chamar uma terceira aplicação. Por exemplo, no EVE-NG, usamos um navegador para interagirmos com os nossos labs e sempre que tentamos aceder um dispositivo, o nevegador aciona uma terceira aplicação (terminais para roteadores e switches, VNC para servidores e desktops e etc).

Para casos em que precisamos apenas de fazer uma sessão de Telnet a partir do nosso computador, basta apenas instalar o Telnet e executarmos o comando a partir do terminal da nossa preferência.


Abraços,
