# Caixa Clínica

Aplicação web (frontend) para controle de caixa do mês.

## Recursos

- Lançamento de **atendimentos** (paciente, procedimento, sessão, valor, forma de pagamento e origem)
- Lançamento de **colaboradores**
- Registro de **produtos vendidos**
- Registro de **despesas**
- **Tela de fechamento** com métricas e saldo do mês
- Exportação de resumo e atendimentos

## Firebase (sync)

O arquivo `index.html` permite configurar o Firebase Realtime Database via modal. As configurações ficam salvas no navegador.

> Dica: em "Realtime Database" configure permissões com `.read` e `.write` conforme seu projeto.

## Como usar

1. Abra `index.html` no navegador.
2. (Opcional) Configure o Firebase para sincronizar dados.
3. Insira os lançamentos e acompanhe o fechamento.
