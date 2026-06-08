<p align="center">
  <img src="https://raw.githubusercontent.com/gusta-ve/gusta-ve/main/banner.svg" alt="gustavo" width="580">
</p>

<p align="center">
  <b>Offensive Security · eJPT</b> &nbsp;|&nbsp; Infra & Produção @ T-Systems &nbsp;|&nbsp; CC @ USCS<br/>
  <sub>Gustavo Almeida · Ribeirão Pires · São Paulo · Brasil</sub>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/gustavo-almeida-moura/"><img src="https://img.shields.io/badge/LinkedIn-0A0A0A?style=flat&logo=linkedin&logoColor=0A66C2"></a>
  <a href="https://gustavoti.com"><img src="https://img.shields.io/badge/gustavoti.com-0A0A0A?style=flat&logo=googlechrome&logoColor=00C2FF"></a>
  <a href="mailto:gustavoalm09@gmail.com"><img src="https://img.shields.io/badge/Email-0A0A0A?style=flat&logo=gmail&logoColor=EA4335"></a>
  <img src="https://img.shields.io/badge/eJPT-Certified-0A0A0A?style=flat&logo=hackthebox&logoColor=9FEF00">
</p>

---

## About

**Segurança ofensiva é o que me move** — exploração web, enumeração, redes, pivoting e Linux
ofensivo. Por trás disso, a base de quem sustenta infraestrutura crítica de produção.

Entrei em TI ainda novo com a mania de abrir tudo pra entender como funciona por dentro — e,
quando quebrava, ir atrás da causa raiz até achar. Esse instinto foi o que me puxou pra segurança.

No dia a dia trabalho com suporte de produção na **T-Systems**, numa linha de montagem de
caminhões: ambiente crítico, problema sob pressão, infra que não pode cair. Em paralelo, fechando
**Ciência da Computação na USCS**.

A eJPT veio como consequência, não como ponto de partida — quando fui atrás dela, já estava com a
chave virada. Hoje empurro a carreira pro lado ofensivo: mapear o alvo, achar a brecha que passou
batido e ir até o fim. Quando não tô em lab, construo sistemas reais em produção.

---

## Featured Projects

Duas ferramentas autorais de segurança ofensiva que jogam **a mesma mão**: o
`wraith` abaixa os ases (recon + detecção), o `hickok` traz os oitos (pós-exploração).
Ases e oitos — a *mão do homem morto*, a que Wild Bill Hickok segurava quando levou
o tiro nas costas em **Deadwood, 1876**. E é numa cidade-alvo com esse nome —
[`deadwood`](https://github.com/gusta-ve/deadwood), um range do primeiro injection trivial
ao quase-impossível — que afio as duas. Tudo em **Python**, núcleo **sem dependências**,
testado, com CI, e publicado no **PyPI**.

<p align="center">
  <a href="https://github.com/gusta-ve/wraith"><img src="https://raw.githubusercontent.com/gusta-ve/gusta-ve/main/wraith.svg" alt="wraith" width="47%"></a>
  &nbsp;
  <a href="https://github.com/gusta-ve/hickok"><img src="https://raw.githubusercontent.com/gusta-ve/gusta-ve/main/hickok.svg" alt="hickok" width="47%"></a>
</p>

### wraith — offensive recon & vulnerability detection

Percorre o recon-até-detecção como um pipeline de **fases componíveis (DAG)**: resolve
o alvo, varre portas, mapeia a superfície web, testa e reporta. Acha **Broken Access
Control, IDOR, XSS, SQLi (error/boolean/time), command injection, SSTI, LFI, open
redirect e CORS** — e **toda detecção é confirmada uma segunda vez** antes de virar
finding (evidência, não chute). Templates declarativos, núcleo **zero-dependência**.

**Python · asyncio · engine de fases em DAG · zero-dep · testes · CI**
**[Repositório](https://github.com/gusta-ve/wraith)** &nbsp;·&nbsp; `pipx install wraith-sec`

### hickok — reverse-shell handler & post-exploitation

A metade da ação: lê um run do `wraith` e age sobre ele. **Handler de reverse shell**
multi-listener com upgrade pra PTY, geração de payloads, e uma **engine de SQL injection
completa** (`hickok sql`: union/boolean/time auto, **SOCKS5/Tor nativo sem dependência**,
cache por alvo com *resume*). Também sem dependências, testado, com CI.

**Python · SQLi engine · SOCKS5/Tor nativo · cache & resume · zero-dep · CI**
**[Repositório](https://github.com/gusta-ve/hickok)** &nbsp;·&nbsp; `pipx install hickok`

Do outro lado da mesa, também construo e sustento software real em produção e na infra:

### Nexus — full-stack em produção

Sistema rodando um negócio real: CRM, portal do cliente e painel admin para suporte de TI.
**.NET 10 / Blazor · PostgreSQL · Docker · Clean Architecture** — multi-tenant com isolamento real,
cofre de senhas **AES-256-GCM** e CI/CD completo.

O código de produção fica em repositório privado (uso diário e dados sensíveis); mantenho um
*showcase* público e a demo no ar pra explorar à vontade.

**[Produção](https://gustavoti.com)** · **[Demo](https://demo.gustavoti.com)** · **[Showcase](https://github.com/gusta-ve/nexus-showcase)**

### vordr — the warden of your servers

Sentinela de infra que **roda em qualquer máquina** (Linux/macOS/Windows) e vigia seus hosts
Linux por **SSH**, respondendo numa tela só — **estão no ar?**, **vou ser cobrado?**
(renovação de server/domínio, gasto/mês) e **estão seguros?**. Descobre servidores pela API do
provedor (integração extensível) ou por config manual — qualquer host —, puxa a expiração de
domínio por **RDAP** e **avisa antes da cobrança chegar** (Telegram/e-mail). Sem agente, sem
banco, sem segredo — só o `~/.ssh/config`.

**Python · zero-dependência (stdlib puro) · testes · CI · PyPI**
**[Repositório](https://github.com/gusta-ve/vordr)** &nbsp;·&nbsp; `pipx install vordr`

---

## Stack

**Ofensiva** &nbsp;
![Kali](https://img.shields.io/badge/Kali-0A0A0A?style=flat&logo=kalilinux&logoColor=557C94)
![Burp Suite](https://img.shields.io/badge/Burp-0A0A0A?style=flat&logo=burpsuite&logoColor=FF6633)
![Metasploit](https://img.shields.io/badge/Metasploit-0A0A0A?style=flat&logo=metasploit&logoColor=2596CD)
![Wireshark](https://img.shields.io/badge/Wireshark-0A0A0A?style=flat&logo=wireshark&logoColor=1679A7)
![Nmap](https://img.shields.io/badge/Nmap-0A0A0A?style=flat&logo=gnometerminal&logoColor=E6EDF3)
![sqlmap](https://img.shields.io/badge/sqlmap-0A0A0A?style=flat&logo=gnometerminal&logoColor=E6EDF3)
![Hydra](https://img.shields.io/badge/Hydra-0A0A0A?style=flat&logo=gnometerminal&logoColor=E6EDF3)
![ffuf](https://img.shields.io/badge/ffuf-0A0A0A?style=flat&logo=gnometerminal&logoColor=E6EDF3)

**Linguagens** &nbsp;
![C#](https://img.shields.io/badge/C%23-0A0A0A?style=flat&logo=dotnet&logoColor=239120)
![Python](https://img.shields.io/badge/Python-0A0A0A?style=flat&logo=python&logoColor=3776AB)
![Java](https://img.shields.io/badge/Java-0A0A0A?style=flat&logo=openjdk&logoColor=E76F00)
![JavaScript](https://img.shields.io/badge/JavaScript-0A0A0A?style=flat&logo=javascript&logoColor=F7DF1E)
![C](https://img.shields.io/badge/C-0A0A0A?style=flat&logo=c&logoColor=A8B9CC)

**Frameworks e Web** &nbsp;
![.NET](https://img.shields.io/badge/.NET-0A0A0A?style=flat&logo=dotnet&logoColor=512BD4)
![Blazor](https://img.shields.io/badge/Blazor-0A0A0A?style=flat&logo=blazor&logoColor=512BD4)
![ASP.NET](https://img.shields.io/badge/ASP.NET-0A0A0A?style=flat&logo=dotnet&logoColor=512BD4)
![Node.js](https://img.shields.io/badge/Node.js-0A0A0A?style=flat&logo=nodedotjs&logoColor=339933)
![React](https://img.shields.io/badge/React-0A0A0A?style=flat&logo=react&logoColor=61DAFB)

**Bancos de Dados** &nbsp;
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-0A0A0A?style=flat&logo=postgresql&logoColor=4169E1)
![MySQL](https://img.shields.io/badge/MySQL-0A0A0A?style=flat&logo=mysql&logoColor=4479A1)
![SQL Server](https://img.shields.io/badge/SQL_Server-0A0A0A?style=flat)
![MongoDB](https://img.shields.io/badge/MongoDB-0A0A0A?style=flat&logo=mongodb&logoColor=47A248)

**Infra & Ferramentas** &nbsp;
![Linux](https://img.shields.io/badge/Linux-0A0A0A?style=flat&logo=linux&logoColor=FCC624)
![Docker](https://img.shields.io/badge/Docker-0A0A0A?style=flat&logo=docker&logoColor=2496ED)
![Bash](https://img.shields.io/badge/Bash-0A0A0A?style=flat&logo=gnubash&logoColor=4EAA25)
![Git](https://img.shields.io/badge/Git-0A0A0A?style=flat&logo=git&logoColor=F05032)

---

<p align="center"><sub>Aberto a oportunidades em segurança ofensiva e infraestrutura.</sub></p>
