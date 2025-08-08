# NutriVision

Analista de Cardápios Escolares

## 📌 Descrição

O NutriVision é uma plataforma completa para análise nutricional de cardápios escolares. A solução é dividida em três módulos principais: API de formatação de cardápios, base de dados nutricional e interface web interativa.

- A API em Flask recebe arquivos de cardápios e os transforma em um formato padronizado, consultando um banco SQLite para mapear ingredientes e receitas.
- A base de dados fornece valores de macro e micronutrientes de ingredientes utilizados nas análises.
- A interface web permite o upload dos cardápios, visualização de etapas de análise e feedback visual com insights.

---

## 🚀 Funcionalidades

- Endpoint GET `/formatar-cardapio` para consultar cardápios já processados.
- Endpoint POST `/formatar-cardapio` para envio e formatação de novos cardápios.
- Conversão de planilhas Excel para JSON com aplicação de regras de negócio.
- Scripts de criação e povoamento do banco de dados nutricional.
- Upload de arquivos (.csv, .xlsx, .xls) com suporte a arrastar e soltar.
- Tema claro/escuro com persistência via localStorage.
- Painel de insights com gráficos analíticos e resumo de regras atendidas/não atendidas.

---

## 🧪 Tecnologias Utilizadas

- **Backend:** Python, Flask, SQLite
- **Frontend:** React 19, Vite 7, TypeScript, Tailwind CSS 4
- **Bibliotecas Auxiliares:** pandas, openpyxl, xlrd, Recharts, Aura Design System, ESLint

---

## 📂 Estrutura de Pastas

```
.
├── app.py
├── cardapio_input/
│   ├── convert_to_json.py
│   ├── PlanilhaTeste.xlsx
│   └── json_outputs/
├── database/
│   ├── cardapios.db
│   ├── db_inserts.py
│   ├── db_operations.py
│   ├── db_populando.py
│   └── InsertTable.xlsx
├── ingredientes.db
├── utils/
│   └── transformador.py
├── requirements.txt
├── Client/
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── aura/
│   │   │   ├── aura-design-system/
│   │   │   └── aura-icons/
│   │   ├── contexts/
│   │   │   └── LayoutContext.tsx
│   │   ├── hooks/
│   │   │   └── useLayout.ts
│   │   ├── shared/
│   │   │   └── components/
│   │   │       ├── AsideWeek.tsx
│   │   │       ├── CardNameSchool.tsx
│   │   │       ├── CardSemana.tsx
│   │   │       ├── Header.tsx
│   │   │       ├── Insight.tsx
│   │   │       ├── MonthlyAverageGraph.tsx
│   │   │       ├── Navbar.tsx
│   │   │       ├── Sidebar.tsx
│   │   │       └── WeekAnalysis.tsx
│   │   ├── App.tsx
│   │   └── main.tsx
│   ├── package.json
│   └── vite.config.ts
```

---

## 🔧 Como Rodar o Projeto

### Backend

#### Pré-requisitos
- Python 3.x
- Dependências listadas em `requirements.txt`

#### Passo a passo
```bash
git clone <URL do repositório>
cd <nome-da-pasta-backend>
pip install -r requirements.txt
python app.py
```

### Banco de Dados

#### Pré-requisitos
- SQLite 3 ou ferramenta para abrir `.db`

#### Passo a passo
```bash
sqlite3 ingredientes.db
```

### Frontend

#### Pré-requisitos
- Node.js e npm

#### Passo a passo
```bash
git clone <URL do repositório>
cd <nome-da-pasta-frontend>
npm install
npm run dev
```

---

## 🔗 Endpoints / Rotas

- `GET /formatar-cardapio` – Lista cardápios já recebidos e processados.
- `POST /formatar-cardapio` – Recebe um cardápio e retorna a versão transformada.

---

## 👥 Equipe do Projeto

| Nome                              | Função            |
|-----------------------------------|-------------------|
| Amanda de Menezes Maidana            | UX/UI             | 
| Arthur Duarte Guedes                 | Desenvolvimento   |
| Diogo Leite Gomes                    | Desenvolvimento   |
| Felipe Pedrozo Ribeiro               | UX/UI             |
| Gabriel Gravena Barros               | Desenvolvimento   |
| Henrique Oliveira Silva              | Desenvolvimento   |
| Jose Lucas Aparecido Rocha           | Desenvolvimento   |
| Kauã Vicente Domingos                | Versionamento     |
| Leandro de Oliveira Candido          | Desenvolvimento   |
| Rhyan Santiago Komm                  | PO & Desenvolvimento   |
| Rodrigo Terra Costa                  | Desenvolvimento   |
| Thiago Olszewski de Carvalho         | PO & UX/UI             |
| Valber Oliveira da Conceição         | Desenvolvimento   |
| Willdanthê Amorim Alaman             | Desenvolvimento   |

<br/>

<div style="display: flex; gap: 10px;">
  <a href="https://github.com/AM-Maidana">
    <img src="https://github.com/AM-Maidana.png" alt="Henrique Oliveira" style="border-radius: 50%; width: 60px; height: 60px; margin: 10%">
  </a>
  <a href="https://github.com/ArthurDuGuedes">
    <img src="https://github.com/ArthurDuGuedes.png" alt="Henrique Oliveira" style="border-radius: 50%; width: 60px; height: 60px; margin: 10%">
  </a>
  <a href="https://github.com/Diogoltt">
    <img src="https://github.com/Diogoltt.png" alt="Henrique Oliveira" style="border-radius: 50%; width: 60px; height: 60px; margin: 10%">
  </a>
  <a href="https://github.com/Holiveira090">
    <img src="https://github.com/Holiveira090.png" alt="Henrique Oliveira" style="border-radius: 50%; width: 60px; height: 60px; margin: 10%">
  </a>
  <a href="https://github.com/joselucas0">
    <img src="https://github.com/joselucas0.png" alt="Henrique Oliveira" style="border-radius: 50%; width: 60px; height: 60px; margin: 10%">
  </a>
  <a href="https://github.com/Kaua676">
    <img src="https://github.com/Kaua676.png" alt="Kauã Vicente" style="border-radius: 50%; width: 60px; height: 60px; margin: 10%">
  </a>
  <a href="https://github.com/Leandro-Oli2">
    <img src="https://github.com/Leandro-Oli2.png" alt="Kauã Vicente" style="border-radius: 50%; width: 60px; height: 60px; margin: 10%">
  </a>
  <a href="https://github.com/olszewskioc">
    <img src="https://github.com/olszewskioc.png" alt="Thiago Olszewski" style="border-radius: 50%; width: 60px; height: 60px; margin: 10%">
  </a>
  <a href="https://github.com/oppsggbarros">
    <img src="https://github.com/oppsggbarros.png" alt="Gabriel Gravena" style="border-radius: 50%; width: 60px; height: 60px; margin: 10%">
  </a>
  <a href="https://github.com/Pedrozo0901">
    <img src="https://github.com/Pedrozo0901.png" alt="Gabriel Gravena" style="border-radius: 50%; width: 60px; height: 60px; margin: 10%">
  </a>
  <a href="https://github.com/RhyanSKomm">
    <img src="https://github.com/RhyanSKomm.png" alt="Rhyan" style="border-radius: 50%; width: 60px; height: 60px; margin: 10%">
  </a>
  <a href="https://github.com/Rodrigo15511">
    <img src="https://github.com/Rodrigo15511.png" alt="Rodrigo Terra" style="border-radius: 50%; width: 60px; height: 60px; margin: 10%">
  </a>
  <a href="https://github.com/ValberOIiveira">
    <img src="https://github.com/ValberOIiveira.png" alt="Willdanthê Amorim" style="border-radius: 50%; width: 60px; height: 60px; margin: 10%">
  </a>
  <a href="https://github.com/Willdanthe">
    <img src="https://github.com/Willdanthe.png" alt="Willdanthê Amorim" style="border-radius: 50%; width: 60px; height: 60px; margin: 10%">
  </a>
  </div>

---

## 🛠 Ferramentas de Trabalho

### 🔄 GitHub Projects
Utilizado para organizar sprints e tarefas.

### 💻 GitHub
Repositório principal:  
[https://github.com/J-A-Digix](https://github.com/J-A-Digix)

---

## 🙋‍♂️ Autor

Mantido pelos times da organização NutriVision.
