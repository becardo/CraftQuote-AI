# 🧶 CraftQuote AI — Sistema Inteligente de Orçamentos para Produtos Artesanais

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![AI](https://img.shields.io/badge/AI-LLM-purple)
![Automation](https://img.shields.io/badge/Automation-Web%20Scraping-green)
![Database](https://img.shields.io/badge/Database-SQLite-orange)

## 📌 Sobre o projeto

O **CraftQuote AI** é um sistema inteligente desenvolvido para automatizar a criação de orçamentos de produtos artesanais, especialmente peças produzidas em crochê e amigurumi.

A proposta do projeto é utilizar **Inteligência Artificial e processamento de linguagem natural** para interpretar solicitações feitas pelo usuário, extrair informações importantes do pedido e gerar automaticamente um orçamento considerando:

- Materiais utilizados;
- Quantidade de insumos;
- Tempo de produção;
- Custos de fabricação;
- Frete;
- Margem de lucro;
- Taxas adicionais.

O objetivo é transformar um processo manual de precificação em uma solução automatizada, organizada e escalável.

---

# 💡 Como funciona

O usuário informa o pedido utilizando linguagem natural:

> "Vou fazer um polvo grande usando 4 linhas Pelúcia da Círculo. Vou entregar em Belo Horizonte e acredito que vou gastar 4 dias para produzir."

A Inteligência Artificial interpreta a mensagem e transforma as informações em dados estruturados:

```json
{
  "produto": "Polvo Grande",
  "materiais": [
    {
      "nome": "Linha Pelúcia Círculo",
      "quantidade": 4
    }
  ],
  "tempo_producao": "4 dias",
  "local_entrega": "Belo Horizonte"
}
```

Após isso, o sistema realiza os cálculos necessários e gera um orçamento completo:

```
Produto: Polvo Grande

Materiais:
4x Linha Pelúcia Círculo ........ R$ 87,60
Olhos de segurança .............. R$ 3,20
Fibra siliconada ................ R$ 8,40

Frete ........................... R$ 14,50

Mão de obra (4 dias) ............ R$ 240,00

Lucro ........................... R$ 60,00

---------------------------------
TOTAL ........................... R$ 413,70
```

---

# 🏗️ Arquitetura do sistema

Fluxo geral:

```
Usuário
   |
   v
Chatbot com IA
   |
   v
Extração de informações
   |
   v
Sistema de orçamento
   |
   +----------------+
   |                |
   v                v
Banco de dados   APIs/Web Scraping
   |
   v
Cálculo de custos
   |
   v
Orçamento final
   |
   v
PDF / WhatsApp
```

---

# ⚙️ Funcionalidades

## Planejadas

- [ ] Chatbot para receber pedidos em linguagem natural
- [ ] Extração automática de informações utilizando IA
- [ ] Cadastro de materiais
- [ ] Cadastro de produtos e receitas
- [ ] Banco de dados de fornecedores
- [ ] Cálculo automático de custos
- [ ] Cálculo de mão de obra
- [ ] Cálculo de lucro
- [ ] Geração de orçamento em PDF
- [ ] Integração com WhatsApp

---

# 🗄️ Banco de dados

O sistema utiliza um banco de dados para armazenar informações importantes:

## Materiais

- Nome do material;
- Fornecedor;
- Preço;
- Quantidade disponível;
- Unidade de medida.

## Produtos

- Nome do produto;
- Materiais necessários;
- Quantidade utilizada;
- Tempo médio de produção.

## Clientes

- Nome;
- Contato;
- Histórico de pedidos.

---

# 🌐 Consulta de preços

Uma das funcionalidades futuras é automatizar a obtenção dos preços dos materiais.

## Integração via API

Quando o fornecedor disponibilizar uma API:

```
Sistema
   |
   v
API do fornecedor
   |
   v
Preço atualizado
```

## Web Scraping

Caso não exista API, será possível utilizar automação para consultar informações:

```
Python
 |
 +-- BeautifulSoup
 +-- Selenium
 +-- Playwright

        |
        v

Captura de preços
```

---

# 🛠️ Tecnologias utilizadas

## Backend

- Python

## Banco de dados

- SQLite

## Inteligência Artificial

- Large Language Models (LLMs)
- Processamento de linguagem natural
- Extração estruturada de dados

## Automação

- Web Scraping
- Integração com serviços externos

## Interface

- Em desenvolvimento

---

# 🎯 Objetivos do projeto

O CraftQuote AI busca explorar aplicações práticas de:

- Inteligência Artificial;
- Automação de processos;
- Desenvolvimento de sistemas inteligentes;
- Banco de dados;
- Integração entre diferentes tecnologias.

Além disso, o projeto busca resolver um problema real de pequenos empreendedores artesanais: a dificuldade de calcular preços de venda considerando todos os custos envolvidos.

---

# 👩‍💻 Autora

**Ana Beatriz**

Estudante de Engenharia de Controle e Automação.

Áreas de interesse:

- Inteligência Artificial;
- Automação;
- Desenvolvimento de sistemas;
- Aplicações de tecnologia para problemas reais.

---

⭐ Projeto em desenvolvimento como estudo prático envolvendo Inteligência Artificial, automação e desenvolvimento de software.
