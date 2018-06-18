# RouterSSH
### Roteador para internet móvel desbloqueado via SSH/VPN.
> ### PARA APARELHOS SEM ROOT

![](https://raw.githubusercontent.com/fazendo/RouterSSH/master/imagens/telegram-bot.png)

![](https://img.shields.io/github/stars/fazendo/RouterSSH.svg) ![](https://img.shields.io/github/forks/fazendo/RouterSSH.svg) ![](https://img.shields.io/github/tag/fazendo/RouterSSH.svg) ![](https://img.shields.io/github/release/fazendo/RouterSSH.svg) ![](https://img.shields.io/github/issues/fazendo/RouterSSH.svg)

####Creditos
 - @Marlyson33 (Telegram)
 - GRUPO DAS PAYLOADS (Telegram)
 - Termux.APK - Fredrik Fornwall (PlayStore)
 - seu credito não está aqui? favor solicitar!!! OK

###Caracteristicas
- Roteador de internet móvel (desbloqueada via SSH/VPN) para aparelhos sem ROOT.
- SEM ROOT - PARA APARELHOS SEM ROOT 
- ISSO MESMO PARA VOCÊ QUE NÃO TEM ROOT.

**TABELA DE CONTEÚDO**

[TOCM]

[TOC]

#Requerimentos: O que é necessáario para isso funcionar?
##Que Seu Dispositivo/Aparelho tenha Sistema Operacional Android 5.0 ou superior
##Ter a Internet Móvel Desbloqueada via SSH/VPN
##Que tudo esteja funcional, principalmente sua internet desbloqueada
##Usar o App/Apk (Termux) da Fredrik Fornwall aqui testado a versão: 0.61
###Termux (playstore id: com.termux) link: https://play.google.com/store/apps/details?id=com.termux
###APK INCLUSO! Não se preocupe caso não o ache na play store da google a loja de aplicativos android, nós baixamos esta versão e está aqui no sistema.
##Ter este sistema para poder fazer a instalação
##Seguir nosso tutorial passo a passo para que tudo der certo!
###Não tente adivianhar! LEIA! MANUAL FOI FEITO PARA SER SEGUIDO!
####Se você gosta de perder tempo, blz! SE NÃO! SEGUI O PASSO A PASSO!
###Codigo/Comando que deve ser inserido no terminal

Copie e cole o comando abaixo no terminal e dê enter.

    apt update && apt upgrade -y && apt install wget -y && wget https://raw.githubusercontent.com/fazendo/RouterSSH/master/instalador && bash instalador
    
###Images

Nós Fazemos por você：
[![](https://raw.githubusercontent.com/fazendo/RouterSSH/master/imagens/developer.png)]
> Tamo Junto
                
----


###FlowChart

```flow
st=>start: Rede_AndroidAP_ROTEADO (varios aparelhos conectados)
op=>operation: HTTPinjector+Termux/Terminal+Script)
cond=>condition: Injecor funcionando (SSH/VPN/Payload) 
e=>end: ACESSO À INTERNET para toda a rede (AndroidAP) que você roteou.

st->op->cond
cond(yes)->e
cond(no)->op
```

###Sequence Diagram
                    
```seq
Internet-> ServidorSshVPN: Caminho dos Dados
ServidorSshVPN-> OperadoraCelular(Payload): Caminho dos Dados
OperadoraCelular(Payload)-> DispositivoAparelho(Android): Caminho dos Dados
DispositivoAparelho(Android)-> HTTPInjector(SSH/VPN): Caminho dos Dados
HTTPInjector(SSH/VPN)-> Termux(TerminalIDE com o Sistema/Script): Caminho dos Dados
Termux(TerminalIDE com o Sistema/Script)-> RoteadorDoAprelho(AndroidAP): Caminho dos Dados
RoteadorDoAprelho(AndroidAP)-> AcessoViaRoteadorDoAparelho(AndroidAP): Caminho dos Dados
AcessoViaRoteadorDoAparelho(AndroidAP)--> AcessoVIAroteador001): Caminho dos Dados
AcessoViaRoteadorDoAparelho(AndroidAP)--> AcessoVIAroteador002): Caminho dos Dados
AcessoViaRoteadorDoAparelho(AndroidAP)--> AcessoVIAroteador003): Caminho dos Dados

```

###End