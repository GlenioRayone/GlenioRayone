<h1 align="center">Olá, eu sou Glenio Rayone 👋</h1>

<p align="center">
  <b>Engenheiro Civil • Guarda Civil Municipal • Desenvolvedor Fullstack Autodidata</b>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&pause=1000&color=2F81F7&center=true&vCenter=true&width=600&lines=Desenvolvedor+Fullstack+Autodidata;C%23+%7C+WPF+%7C+Android+%7C+Node.js;Publicado+na+Google+Play+e+Microsoft+Store" alt="Typing SVG" />
</p>

---

### 🧰 Tecnologias que utilizo

<p align="center">
  <img src="https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white" />
  <img src="https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white" />
  <img src="https://img.shields.io/badge/WPF-0C54C2?style=for-the-badge&logo=windows&logoColor=white" />
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white" />
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black" />
</p>

---

### 🧭 Sobre mim

Sou **Guarda Civil Municipal em Contagem/MG desde 2013** e **Engenheiro Civil** formado em 2019. De forma autodidata, me tornei desenvolvedor fullstack e hoje sou responsável por **projetar, desenvolver e manter todo o ecossistema de tecnologia** utilizado pela minha corporação — do aplicativo de campo ao banco de dados que sustenta a operação diária.

Queria desenvolver um sistema para ajudar estudantes e recém-formados em Engenharia Civil, além de pedreiros e mestres de obras, a ter uma ferramenta simples e útil, entregando cálculos e resultados de pequenas edificações de forma prática. Foi isso que me levou a conhecer os princípios de programação e desenvolvimento de software. Juntando essa necessidade de aprendizado com a realidade da Guarda Civil — que começou como uma necessidade prática de digitalizar processos internos — o projeto se tornou um sistema completo, multiplataforma, em produção e usado diariamente por dezenas de agentes e gestores.

- 🛠️ Atuo em **todas as camadas**: aplicativo desktop, aplicativo mobile, API e banco de dados
- 🚓 Meus sistemas cobrem desde controle de escalas e ocorrências disciplinares até banco de horas, patrimônio e comunicação interna
- 📈 Evoluo constantemente a arquitetura, migrando módulos legados para soluções mais robustas e escaláveis
- 🎯 Foco em software que resolve problemas reais de uma operação pública 24/7

---

### 🖥️ Sistema Desktop — Guarda Civil de Contagem

Aplicação **WPF (C#)** que é o núcleo de gestão da corporação e a referência oficial de regras de negócio para os demais módulos (mobile e API).

- 📋 **CCOP / Pendências**: workflow completo de comunicações disciplinares, com geração automática de e-mails com anexos em PDF, controle de status por tipo de ocorrência e trilha de auditoria
- 🔄 **Fluxo de Processos**: linha do tempo visual com etapas coloridas para aprovações multi-nível, com atualização automática de escala mediante aprovação do gestor
- ⏱️ **Banco de Horas**: módulo migrado integralmente para PostgreSQL, com exportação em Excel/PDF, expiração automática de créditos e ferramentas de correção/recuperação a partir de backups
- 🎓 **Centro de Formação**: motor de processos de ATP (Avaliação Técnico-Profissional), gestão de turmas e geração de listas de presença em PDF
- 💬 **GChat/Messenger**: comunicação interna em tempo real com notificações push (FCM) integradas ao app mobile
- 🚗 **Logística/Intendência**: controle de viaturas, cautelas de equipamento e portes de arma
- 🗺️ **Ordem de Serviço**: suporte a múltiplas viaturas com geolocalização reversa e preservação de assinaturas em PDF

---

### 📱 Aplicativo Android — Guarda Civil de Contagem

App nativo publicado na **Google Play**, extensão de campo do sistema desktop, usado pelos agentes em serviço.

- 🔁 **Sincronização API-first**, com cache local em SQLite e política de retry com backoff exponencial
- 🧩 Módulos dedicados: CCOP, Alteração Diária, Histórico de Guarda, Banco de Guardas, Documentos, Portaria, Livro Sentinela, Cautela, Equipamentos, Chat interno
- 🗄️ SQLite tratado como cache descartável — sincronização "wipe-then-repopulate" a partir da API garante consistência com o servidor

---

### 🔗 API e Arquitetura de Dados

- ⚙️ **Node.js + Express**, com rotas dedicadas para cada módulo (escala, banco de guardas, intendência, equipamentos, portaria, centro de formação, veículos, porte de arma, entre outros)
- 🐘 **PostgreSQL** como banco primário, com arquitetura multi-schema (por usuário, por posto, por ano) e tabelas particionadas por mês para dados de alto volume
- 📴 **SQLite** como cache offline no desktop e no mobile, garantindo operação mesmo com instabilidade de rede
- 🔥 **Firebase** (Firestore/FCM) usado para notificações push em tempo real, com lógica de negócio sendo progressivamente migrada para PostgreSQL

---

### 🚀 Projetos em destaque — publicados oficialmente

Meus dois principais sistemas estão **publicados e disponíveis ao público** nas lojas oficiais Android e Windows.

<table>
<tr>
<td width="50%" valign="top" align="center">

**📱 Guarda Civil Contagem — Android**

<a href="https://play.google.com/store/apps/details?id=com.gleniorayone.guardacivil&hl=pt_BR">
  <img src="https://play-lh.googleusercontent.com/XH49i-_-uMyN2N0rnm_RAjzyhh9WXIbFzVAbvNdi0NliCMGYyvVUy8_-lvqfBdfSGRyIlz3kAOKd9e4id2ylkA=w200-h200" width="90" alt="Ícone do app Android" /><br/>
  <img src="https://play-lh.googleusercontent.com/oQ5zD5KFtQbzHYU7V5d0osNrQYe_ULqpxLv1e8dA_yjH7oXY_JD5VwOnfvIemGoKenaKnoa5zrg8yR-3V03g=w526-h296" width="260" alt="Captura de tela do app" />
</a>

<br/><br/>

<a href="https://play.google.com/store/apps/details?id=com.gleniorayone.guardacivil&hl=pt_BR">
  <img src="https://play.google.com/intl/en_us/badges/static/images/badges/pt-br_badge_web_generic.png" height="55" alt="Disponível no Google Play" />
</a>

*App nativo com sincronização em tempo real, publicado sob o desenvolvedor `syseng.corporation`*

</td>
<td width="50%" valign="top" align="center">

**🖥️ Guarda Civil de Contagem — Windows**

<a href="https://apps.microsoft.com/detail/9mv3ccwbk8zn?hl=pt-BR&gl=BR">
  <img src="https://store-images.s-microsoft.com/image/apps.25363.13800944033309045.ede4ef19-15df-4923-90a1-01d44cde53f5.66cfa4ea-53bf-4340-92ef-887fe7367b18" width="90" alt="Ícone do app Windows" />
</a>

<br/><br/>

<a href="https://apps.microsoft.com/detail/9mv3ccwbk8zn?hl=pt-BR&gl=BR">
  <img src="https://get.microsoft.com/images/pt-br%20dark.svg" height="55" alt="Disponível na Microsoft Store" />
</a>

*Sistema completo de gestão operacional e administrativa, distribuído oficialmente via Microsoft Store*

</td>
</tr>
</table>

---

### 📊 Estatísticas do GitHub

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=GlenioRayone&show_icons=true&theme=dark&hide_border=true&count_private=true" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=GlenioRayone&layout=compact&theme=dark&hide_border=true" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=GlenioRayone&theme=dark&hide_border=true" />
</p>

---

### 📫 Contato

<p align="center">
  <a href="https://www.linkedin.com/in/glenio-rayone">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
</p>

<p align="center">
  <i>Desenvolvendo tecnologia de dentro da própria linha de frente da segurança pública.</i>
</p>
