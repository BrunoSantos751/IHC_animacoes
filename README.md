# Atividade: Uma interface que se comunica
**Disciplina:** Interação Humano-Computador (IHC) • AFYA / UNIMA Maceió  
**Integrantes:** Bruno Moraes, João Honorio, Fabio Fernandes  
**Tema da interface:** Agendamento de consulta médica  

---

### Registro das Animações

| Animação / função | Benefício observado | Risco ou problema | Ajuste realizado |
| :--- | :--- | :--- | :--- |
| **Destaque visual e micro-escala ao clicar no horário** *(ação realizada)* | Deixa claro qual opção foi selecionada pelo usuário através da mudança de cor e borda no card, além de confirmar na hora que o clique foi recebido. | Se o feedback fosse apenas transitório, o usuário poderia ter dúvidas de qual horário ficou ativo ou achar que a consulta já tinha sido agendada direto. | O card escolhido permanece com fundo e borda destacados, acompanhado de uma mensagem de texto logo abaixo confirmando a opção selecionada. |
| **Barra de progresso animada com texto de status** *(operação em andamento)* | Mostra com clareza que a requisição está sendo carregada e processada pelo sistema, informando ao usuário que ele precisa aguardar. | Se não mostrar que está carregando ou se o tempo for longo demais (como testado com 1200 ms), o usuário pensa que o sistema travou e tenta clicar várias vezes. | O botão de confirmação fica desabilitado exibindo "Agendando..." enquanto a barra preenche visualmente e o texto avisa que está carregando ("Reservando horário..."). |
| **Fade e slide curto na tela de confirmação** *(resultado)* | A troca de tela fica suave e o usuário entende que a tarefa terminou. | Movimento grande pode desorientar ou incomodar quem é sensível a movimento. | Deslocamento de apenas 12 px, com os dados (médico, horário, protocolo) escritos na tela. |
| **Tremor no campo de nome vazio** *(erro)* | Chama a atenção para o campo que precisa ser corrigido. | O tremor sozinho não explica o erro. | Borda vermelha e mensagem escrita; com "Reduzir movimento" o tremor é removido. |
