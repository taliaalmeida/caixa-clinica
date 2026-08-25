<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:D01117,50:EC4899,100:F9A8D4&height=180&section=header&text=CAIXA%20CL%C3%8DNICA&fontSize=34&fontColor=FDF2F8&fontAlignY=35&desc=Atendimentos%20%7C%20Despesas%20%7C%20Produtos%20%7C%20Fechamento&descAlignY=58&descSize=15&descColor=F9A8D4" alt="Banner Caixa Clínica" />
</p>

<p align="center">
  <strong>Aplicação web para controle financeiro mensal de clínicas de estética.</strong>
</p>

<p align="center">
  <a href="https://taliaalmeida.github.io/caixa-clinica/"><img src="https://img.shields.io/badge/DEMO-ONLINE-EC4899?style=for-the-badge&labelColor=0D1117" alt="Demo online" /></a>
  <img src="https://img.shields.io/badge/STATUS-FEATURED-F9A8D4?style=for-the-badge&labelColor=0D1117" alt="Status featured" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black" alt="Firebase" />
</p>

> **01 // PROJECT_OVERVIEW**  
> O Caixa Clínica centraliza os lançamentos financeiros de uma clínica em uma interface web simples. A aplicação permite registrar atendimentos, colaboradores, produtos vendidos e despesas, acompanhar o fechamento do mês e exportar resumos.

## 02 // RECURSOS

| Módulo | Funcionalidade |
| --- | --- |
| **Atendimentos** | Registra paciente, procedimento, sessão, valor, forma de pagamento, origem e observações. |
| **Colaboradores** | Mantém os lançamentos relacionados à equipe. |
| **Produtos** | Registra produtos vendidos e seus valores. |
| **Despesas** | Organiza saídas e observações do mês. |
| **Fechamento** | Exibe métricas e saldo do período. |
| **Exportação** | Permite exportar resumos e atendimentos. |
| **Organização mensal** | Detecta registros fora do mês e reorganiza os dados no caminho correspondente. |

## 03 // INTERFACE

A captura abaixo mostra a aplicação publicada com os módulos de **Atendimentos**, **Colaboradores**, **Produtos**, **Despesas** e **Fechamento**, além do formulário para novo atendimento. A tabela de dados foi omitida da captura entregue para não expor nomes de pacientes.

<p align="center">
  <img src="assets/screenshots/caixa-clinica-interface.webp" alt="Interface de lançamento de atendimento do Caixa Clínica" width="920" />
</p>

<p align="center"><sub>Captura real da interface publicada, com o formulário operacional preservado e dados pessoais removidos do enquadramento.</sub></p>

## 04 // STACK E ARQUITETURA

| Camada | Tecnologia/abordagem |
| --- | --- |
| Interface | HTML5, CSS3 e JavaScript no navegador. |
| Dados | Firebase, com sincronização entre usuárias. |
| Entrada | Formulários para atendimentos, colaboradores, produtos e despesas. |
| Período | Seleção de mês com navegação anterior/próximo. |
| Publicação | GitHub Pages. |

## 05 // COMO USAR

### Demo online

Acesse [taliaalmeida.github.io/caixa-clinica](https://taliaalmeida.github.io/caixa-clinica/).

### Execução local

```bash
git clone https://github.com/taliaalmeida/caixa-clinica.git
cd caixa-clinica
python3 -m http.server 8000
```

Abra [http://localhost:8000](http://localhost:8000) no navegador.

### Fluxo recomendado

1. Selecione o mês de trabalho.
2. Configure o Firebase pelo botão de configurações, se for necessário sincronizar os dados.
3. Cadastre atendimentos, colaboradores, produtos e despesas.
4. Acompanhe o saldo e as métricas em **Fechamento**.
5. Exporte os resumos quando precisar compartilhar ou arquivar o período.

## 06 // ORGANIZAÇÃO DOS DADOS

O sistema trabalha com dados mensais. Ao navegar entre os meses, ele verifica registros que estejam em um caminho incorreto e pode migrá-los silenciosamente para a pasta correspondente ao período.

Essa automação facilita a manutenção do histórico, mas deve ser testada com dados de demonstração antes do uso em produção. Faça backup do banco e revise as regras do Firebase antes de habilitar gravações reais.

## 07 // CONFIGURAÇÃO E SEGURANÇA

O `index.html` oferece um modal de configuração do Firebase e salva as configurações no navegador. As credenciais de cliente do Firebase não substituem regras de segurança: configure permissões de leitura e escrita no banco, limite o acesso por ambiente e nunca publique tokens administrativos ou dados identificáveis em commits e screenshots.

## 08 // ESTRUTURA

```text
caixa-clinica/
├── Clinica       # Conteúdo auxiliar publicado no repositório
├── index.html    # Aplicação web
├── README.md     # Documentação
└── TODO.md       # Pendências e ideias de evolução
```

## 09 // ROADMAP

| Prioridade | Evolução sugerida |
| --- | --- |
| Alta | Adicionar autenticação e permissões por clínica/usuária. |
| Alta | Criar rotina explícita de backup e restauração antes das migrações mensais. |
| Média | Extrair CSS e JavaScript para arquivos separados e facilitar manutenção. |
| Média | Adicionar testes para fechamento, exportação e organização por mês. |

## 10 // AUTORIA

Desenvolvido por **Natalia Almeida — By Natalia Dev**.

- [Demo online](https://taliaalmeida.github.io/caixa-clinica/)
- [Perfil no GitHub](https://github.com/taliaalmeida/taliaalmeida)
- [Instagram](https://www.instagram.com/nataliaalmeidatech)

<p align="center">
  <sub>Learn. Build. Automate. Evolve.</sub>
</p>
