# 🎁 Lista de Presentes Web (Integração Supabase & AI-Assisted Dev)

Uma aplicação web funcional de ponta a ponta desenvolvida para resolver uma necessidade real de negócio: o gerenciamento dinâmico de uma lista de presentes (Chá de Casa Nova), evitando presentes duplicados e facilitando a experiência do usuário final.

Mais do que um projeto de código, este repositório é uma demonstração de **Análise Funcional, Arquitetura de Integrações e Engenharia de Prompt**.

## 🎯 O Desafio de Negócio
Criar uma plataforma leve, responsiva e sem atrito para os convidados (sem necessidade de criação de contas complexas), garantindo ao mesmo tempo a integridade dos dados no banco e uma área de administração ágil para a gestão do catálogo.

## 🧠 Minha Atuação: A Ponte Técnica
Em vez de focar apenas na digitação de código bruto, atuei como um verdadeiro **Analista de Sistemas e Arquiteto da Solução**, utilizando IA como ferramenta de desenvolvimento:

1. **Levantamento de Requisitos e Modelagem:** Mapeamento do fluxo do usuário (leitura de catálogo público vs. atualização de status de compra).
2. **Orquestração com IA:** Utilização avançada de Engenharia de Prompt para gerar a estrutura de Front-End (HTML/JS/Tailwind), traduzindo as regras de negócio em instruções lógicas para a máquina.
3. **Integração de Back-End (BaaS):** Configuração manual e integração com o banco de dados PostgreSQL via **Supabase**.
4. **Segurança e Maturidade Técnica:** Implementação de isolamento de credenciais e políticas de segurança no banco de dados.

## 🛡️ Destaques de Arquitetura e Segurança

* **Isolamento de Ambiente (Environment Variables):** As credenciais de acesso ao banco de dados não são expostas no código-fonte. Foi implementada uma arquitetura com `config.js` isolado via `.gitignore`, utilizando um `config.example.js` para documentação do repositório.
* **Row Level Security (RLS) no Supabase:** Configuração de políticas explícitas de banco de dados para gerenciar as permissões de leitura, inserção e atualização, garantindo a integridade do esquema público.
* **Segurança por Obscuridade e Painel Admin:** Separação das rotas de interação pública (`index.html`) da rota de administração do banco (`painel-secreto.html`).

## 🛠️ Stack Tecnológica
* **Front-End:** HTML5, Vanilla JavaScript, Tailwind CSS (via CDN para leveza e deploy ágil).
* **Back-End / Banco de Dados:** Supabase (PostgreSQL).
* **Fluxo de Trabalho:** Linux (Zorin OS), Git/GitHub e AI-Assisted Development.

🚀 Como testar este projeto localmente

1. Clone o repositório:
```bash
git clone [https://github.com/MTaranto/ListaRenata.git](https://github.com/MTaranto/ListaRenata.git)
```

2. Configure as Variáveis de Ambiente:
O projeto utiliza um arquivo `.gitignore` para proteger credenciais sensíveis. Para rodar localmente, você precisará criar o seu próprio arquivo de configuração:
- Renomeie o arquivo de demonstração `config.example.js` para `config.js`.
- Insira as suas credenciais reais do Supabase (URL e Chave Pública) dentro do novo `config.js`.

3. Execute a aplicação:
Abra o arquivo `index.html` em qualquer navegador moderno. Não é necessário processo de build ou servidor local (Node.js/npm) graças à arquitetura serverless.
