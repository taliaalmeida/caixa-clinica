💰 Caixa Clínica
Aplicação web (frontend) para controle de caixa mensal.

🧩 Recursos
Lançamento de atendimentos (paciente, procedimento, sessão, valor, forma de pagamento e origem)

Lançamento de colaboradores

Registro de produtos vendidos

Registro de despesas

Tela de fechamento com métricas e saldo do mês

Exportação de resumos e atendimentos

Firebase (sincronização)

Organização Automática de Dados: o sistema detecta registros fora do mês correto e realiza a migração silenciosa para a pasta correspondente no Firebase, garantindo que todos os dados fiquem organizados automaticamente.

💡 Dica: ao navegar entre os meses, o sistema faz uma verificação completa e reorganiza os atendimentos “presos” em pastas erradas. Basta abrir o mês com dados misturados (ex: Junho) para ver a limpeza acontecer em segundo plano.

⚙️ Configuração
O arquivo index.html permite configurar o Firebase Realtime Database via modal.
As configurações ficam salvas no navegador.

Em "Realtime Database", configure as permissões com .read e .write conforme seu projeto.

🚀 Como usar
Abra index.html no navegador.

(Opcional) Configure o Firebase para sincronizar dados.

Insira os lançamentos e acompanhe o fechamento.

Navegue pelos meses para que o sistema organize automaticamente os registros.
