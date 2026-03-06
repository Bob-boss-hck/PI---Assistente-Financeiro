<script src="https://gist.github.com/ernestoguimaraes/e691040b8cbe3b362be19aa45b48fcb2.js">http://patorjk.com/software/taag/#p=display&f=Graffiti&t=Type%20Something%20</script>
<p align="center">
  <img src="https://img.shields.io/badge/status-em%20desenvolvimento-yellow?style=for-the-badge" alt="Status: Em Desenvolvimento"/>
  <img src="https://img.shields.io/badge/univesp-projeto%20integrador-blue?style=for-the-badge" alt="Univesp - Projeto Integrador"/>
  <img src="https://img.shields.io/badge/licença-MIT-green?style=for-the-badge" alt="Licença MIT"/>
</p>

<h1 align="center">💰 Finança Fácil</h1>

<p align="center">
  <strong>Sistema web para controle de receitas e despesas pessoais</strong><br>
  Projeto Integrador I — UNIVESP (Universidade Virtual do Estado de São Paulo)
</p>

<p align="center">
  <a href="#-sobre-o-projeto">Sobre</a> •
  <a href="#-problema">Problema</a> •
  <a href="#%EF%B8%8F-tecnologias">Tecnologias</a> •
  <a href="#-funcionalidades">Funcionalidades</a> •
  <a href="#-estrutura-do-projeto">Estrutura</a> •
  <a href="#-como-executar">Como Executar</a> •
  <a href="#-equipe">Equipe</a>
</p>

---

## 📋 Sobre o Projeto

O **Finança Fácil** é uma aplicação web desenvolvida como Projeto Integrador do curso de Tecnologia da Informação da UNIVESP — Polo Aparecida, Caçapava, Jacareí e Redenção da Serra.

O sistema permite que o usuário registre suas receitas e despesas, categorize seus gastos e acompanhe sua saúde financeira por meio de gráficos interativos e relatórios visuais — tudo de forma simples, intuitiva e minimalista.

> **Metodologia:** Aprendizagem Baseada em Problemas e por Projetos (ABPP) + Design Centrado no Ser Humano (HCD)

## 🔍 Problema

A falta de controle financeiro pessoal é um dos principais fatores que levam ao endividamento no Brasil. Segundo pesquisas recentes, a maioria das pessoas não possui o hábito de registrar e acompanhar suas movimentações financeiras, o que dificulta o planejamento e a tomada de decisões.

**Pergunta norteadora:** Como uma ferramenta web simples e acessível pode ajudar pessoas comuns a organizarem suas finanças pessoais e evitarem o endividamento?

## 🛠️ Tecnologias

| Camada | Tecnologia | Descrição |
|--------|-----------|-----------|
| **Back-end** | ![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white) | Microframework Python para rotas e lógica de negócio |
| **Banco de Dados** | ![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white) | Banco de dados embutido, leve e portátil |
| **Front-end** | ![Bootstrap](https://img.shields.io/badge/Bootstrap_5-7952B3?style=flat-square&logo=bootstrap&logoColor=white) | Framework CSS responsivo para interface minimalista |
| **Gráficos** | ![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=flat-square&logo=chartdotjs&logoColor=white) | Biblioteca JavaScript para gráficos interativos |
| **Versionamento** | ![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white) | Controle de versão e colaboração em equipe |

## ✨ Funcionalidades

### Previstas para a versão final

- [ ] 📊 **Dashboard** — Visão geral com cards de saldo, receitas e despesas
- [ ] ➕ **Adicionar transação** — Formulário para registrar receitas e despesas
- [ ] 📋 **Histórico** — Listagem completa com filtros por período, tipo e categoria
- [ ] ✏️ **Editar/Excluir** — Gerenciamento das transações cadastradas
- [ ] 🍩 **Gráfico de rosca** — Distribuição de despesas por categoria
- [ ] 📊 **Gráfico de barras** — Comparativo receitas vs despesas por mês
- [ ] 📈 **Gráfico de linha** — Evolução do saldo ao longo do ano
- [ ] 🏷️ **Categorias** — Categorias pré-cadastradas + criação de novas
- [ ] 🔍 **Filtros** — Seleção por mês/ano em todas as telas
- [ ] 📱 **Responsivo** — Layout adaptável para desktop, tablet e celular

> As funcionalidades serão implementadas progressivamente ao longo das quinzenas do Projeto Integrador.

## 📁 Estrutura do Projeto

```
financa-facil/
│
├── app.py                    # Arquivo principal — rotas Flask e lógica
├── database.py               # Funções do banco de dados (CRUD)
├── models.py                 # Modelos de dados e validações
├── config.py                 # Configurações do projeto
├── requirements.txt          # Dependências Python
├── financas.db               # Banco SQLite (gerado automaticamente)
├── .gitignore                # Arquivos ignorados pelo Git
├── README.md                 # Este arquivo
│
├── templates/                # Templates HTML (Jinja2)
│   ├── base.html             # Template base (navbar + footer + scripts)
│   ├── index.html            # Dashboard com gráficos
│   ├── adicionar.html        # Formulário de nova transação
│   ├── historico.html        # Listagem e filtros de transações
│   ├── relatorios.html       # Página de relatórios com gráficos
│   ├── categorias.html       # Gerenciamento de categorias
│   └── 404.html              # Página de erro
│
└── static/                   # Arquivos estáticos
    ├── css/
    │   └── style.css         # Estilos customizados
    ├── js/
    │   ├── charts.js         # Lógica dos gráficos (Chart.js)
    │   └── main.js           # Interações gerais
    └── img/
        └── logo.png          # Logo do projeto
```

## 🚀 Como Executar

### Pré-requisitos

- [Python 3.8+](https://www.python.org/downloads/)
- [Git](https://git-scm.com/downloads)

### Passo a passo

```bash
# 1. Clone o repositório
git clone https://github.com/seu-grupo/financa-facil.git

# 2. Entre na pasta do projeto
cd financa-facil

# 3. Crie um ambiente virtual
python -m venv venv

# 4. Ative o ambiente virtual
# Windows:
venv\Scripts\activate
# Linux/Mac:
source venv/bin/activate

# 5. Instale as dependências
pip install -r requirements.txt

# 6. Execute a aplicação
python app.py
```

A aplicação estará disponível em: **http://localhost:5000**

### Dependências (`requirements.txt`)

```
Flask==3.1.*
```

## 🗃️ Banco de Dados

O sistema utiliza **SQLite** com duas tabelas principais:

```
┌──────────────────┐       ┌──────────────────────┐
│   categorias     │       │     transacoes        │
├──────────────────┤       ├──────────────────────┤
│ id (PK)          │◄──┐   │ id (PK)              │
│ nome (UNIQUE)    │   │   │ descricao            │
│ tipo             │   │   │ valor                │
│ cor              │   └───│ categoria_id (FK)    │
└──────────────────┘       │ tipo                 │
                           │ data                 │
                           │ criado_em            │
                           └──────────────────────┘
```

O banco é criado automaticamente na primeira execução do `app.py`, junto com categorias padrão pré-cadastradas (Salário, Alimentação, Transporte, etc.).

## 📅 Cronograma do PI

| Quinzena | Etapa | Status |
|----------|-------|--------|
| Q0 | Formação do grupo e setup do GitHub | ✅ Concluída |
| Q1 | Análise do cenário e levantamento bibliográfico | 🔄 Em andamento |
| Q2 | Definição do problema e Plano de Ação | 🔄 Em andamento |
| Q3 | Desenvolvimento — Back-end + Front-end base | ⏳ Pendente |
| Q4 | Dashboard + Gráficos + Relatório Parcial | ⏳ Pendente |
| Q5 | Refinamento da solução com feedback | ⏳ Pendente |
| Q6 | Finalização + Avaliação Colaborativa | ⏳ Pendente |
| Q7 | Entrega do Relatório Final + Vídeo | ⏳ Pendente |

## 👥 Equipe

| Nome | RA | Papel |
|------|----|-------|
| Gabriel Siqueira Silva | 24200844 | Líder / Scrum Master |
| Raoni Kirschner Sava | 24218257 | Dev Back-end |
| Gabriele Cristine Ribeiro Aluvino | 24211510 | Dev Back-end |
| Lucas Rabelo Fabiano | 24219010 | Dev Front-end |
| Nelson de Paula Santos Júnior | 24206410 | Dev Front-end / Gráficos |
| Rafael José Benedito da Conceição | 24204145 | Documentação / QA |
| Reginaldo Francisco Pedrosa | 24217557 | QA / Testes |
| Reinaldo Samuel de Souza Silva | 24211225 | QA / Testes |

> **Polo:** [Aparecida, Caçapava, Jacareí e Redenção da Serra] — **Orientador PI:** [Thiago Vinicius Ribeiro Soeira]

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 🎓 Referências

- UNIVESP — [Manual do Aluno](https://apps.univesp.br/manual-do-aluno/)
- UNIVESP — [Regulamento do Projeto Integrador](https://apps.univesp.br/manual-do-aluno/assets/docs/Regulamento_para_o_Projeto_Integrador_jun_2023.pdf)
- [Documentação Flask](https://flask.palletsprojects.com/)
- [Documentação SQLite](https://www.sqlite.org/docs.html)
- [Documentação Bootstrap 5](https://getbootstrap.com/docs/5.3/)
- [Documentação Chart.js](https://www.chartjs.org/docs/)

---

<p align="center">
  Desenvolvido com ☕ por alunos da <strong>UNIVESP</strong><br>
  Projeto Integrador I — 2025
</p>









