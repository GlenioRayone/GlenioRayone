<h1 align="center">Olá, eu sou Glenio Rayone 👋</h1>

<p align="center">
  <b>Engenheiro Civil • Guarda Civil Municipal • Desenvolvedor Fullstack Autodidata</b>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&pause=1000&color=2F81F7&center=true&vCenter=true&width=600&lines=Desenvolvedor+Fullstack+Autodidata;C%23+%7C+WPF+%7C+Android+%7C+Node.js;Construindo+solu%C3%A7%C3%B5es+reais+para+a+Guarda+Civil" alt="Typing SVG" />
</p>

---

### 🧭 Sobre mim

Sou **Guarda Civil Municipal em Contagem/MG desde 2013** e **Engenheiro Civil** formado em 2019. De forma autodidata, me tornei desenvolvedor fullstack e hoje sou responsável por **projetar, desenvolver e manter todo o ecossistema de tecnologia** utilizado pela minha corporação — do aplicativo de campo ao banco de dados que sustenta a operação diária.

Queria desenvolver um sistema para ajudar estudantes e recem formados em engenharia civil além de pedreiros e mestre de obras, a ter um sistema simples e útil entregando cálculos e resultados de pequenas edificações de forma simples, oque me levou a conhecer os principio de programação e desenvolvimento de softwares, juntando essa necessidade de conhecimento em desenvolvimento e na Guarda Civil que começou como uma necessidade prática — digitalizar processos internos da Guarda Civil — se tornou um sistema completo, multiplataforma, em produção e usado diariamente por dezenas de agentes e gestores.

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

### 📊 Estatísticas do GitHub

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=GlenioRayone&show_icons=true&theme=dark&hide_border=true&count_private=true" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=GlenioRayone&layout=compact&theme=dark&hide_border=true" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=GlenioRayone&theme=dark&hide_border=true" />
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

### 📌 Projeto em destaque

<p align="center">
  <a href="https://github.com/GlenioRayone/variavel">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=GlenioRayone&repo=variavel&theme=dark&hide_border=true" />
  </a>
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
