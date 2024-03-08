### **Projeto de Software: Sistema de Pagamento RU Pay**

### **1. Introdução**

O Sistema de Pagamento RU Pay é um software destinado à gestão de compra de tickets do Restaurante Universitário (RU). Ele oferece a conveniência de ser acessado pelo celular e permite a compra de tickets de refeição. Nele, o usuário pode efetuar o pagamento através de diversas opções, como Pix, cartão de débito ou crédito. Esta é uma solução inovadora dedicada à administração eficiente da aquisição de tickets do Restaurante Universitário (RU), visando atender de maneira ágil e prática às necessidades dos usuários desse serviço. Este software, que prioriza a comodidade, está especialmente desenvolvido para atender ao público diversificado do RU, abrangendo alunos, funcionários e visitantes que frequentam o ambiente acadêmico. Ao possibilitar o acesso por meio de um site intuitivo, o sistema visa melhorar a experiência dos consumidores do Restaurante Universitário, acelerando o processo para entrada no mesmo, diminuindo filas e transtornos na entrada. Nesse contexto, o Sistema de Pagamento RU destaca-se como uma ferramenta essencial para otimizar a gestão e garantir a satisfação de todos os envolvidos na comunidade acadêmica.

### **2. Requisitos Funcionais**

#### **2.1 Autenticação e Autorização**
- Cadastro simples com email e senha para armazenar os tickets do usuário.
- Opção de inserir a matrícula caso o usuário seja estudante.
- Login seguro e rápido para os usuários.
  
#### **2.2 Compra de Tickets**
- Interface intuitiva para compra de tickets.
- Opções de pagamento: Pix, cartão de débito e crédito.
- A realização da compra gera nota fiscal e comprovante.

#### **2.3 Tela de Comprovante**
- Gerada após a compra é confirmada.
- Contém um QR Code e um texto abaixo informando o tipo do ticket (almoço ou jantar e inteira ou meia).
- Ao ser lido pelo funcionário na entrada do RU, o comprovante é marcado e não pode ser utilizado mais.

#### **2.4 Histórico de Transações**
- Há um histórico simplificado das compras do usuário que pode ser filtrado.
- Também é armazenado todas as notas fiscais das compras, contendo informações detalhadas da transação.
- Para o usuário funcionário é disponibilizado o histórico de todas as compras de todos os usuários e suas notas fiscais.

### **3. Requisitos Não Funcionais**

#### **3.1 Segurança**
- Criptografia de dados sensíveis.
- Proteção contra acesso não autorizado.

#### **3.2 Desempenho**
- Resposta rápida às solicitações.
- Otimização para funcionar em modo offline.

#### **3.3 Confiabilidade**
- Backup e recuperação de dados em caso de falhas.

#### **3.4 Usabilidade**
- Interface intuitiva e amigável.
- Suporte a diferentes tamanhos de tela.

### **4. Backlog do Projeto**

- Épico: Autenticação e Autorização

   - História de Usuário 1: Como um usuário, quero poder me autenticar de forma segura no sistema para acessar minha conta.
   - História de Usuário 2: Como um usuário, quero poder colocar minha matrícula na minha conta.
   - História de Usuário 3: Como um usuário, quero poder recuperar minha senha caso eu a esqueça.

- Épico: Compra de Tickets

  - História de Usuário 4: Como um usuário, quero uma interface intuitiva para comprar tickets de refeição.
  - História de Usuário 5: Como um usuário, quero opções de pagamento como Pix, cartão de débito e crédito.
  - História de Usuário 6: Como um usuário, quero receber um comprovante após a compra para validar minha transação.
  - História de Usuário 7: Como um usuário, quero receber uma nota fiscal após a compra para validar minha transação.
 
- Épico: Tela de Comprovante

  - História de Usuário 8: Como um usuário, quero ter acesso a um comprovante que me permita acessar o RU.
  - História de Usuário 9: Como um usuário, quero que o meu comprovante informe o tipo do meu ticket de acordo com o que eu paguei.
  - História de Usuário 10: Como um funcionário, quero poder realizar a leitura de um comprovante.
  - História de Usuário 11: Como um funcionário, quero que um comprovante que tenha sido lido não possa ser utilizado novamente.

- Épico: Histórico de Transações

  - História de Usuário 12: Como um usuário, quero ter acesso a um registro detalhado das notas fiscais que eu gerei.
  - História de Usuário 13: Como um usuário, quero poder consultar meu histórico de transações e conseguir filtrá-lo.
  - História de Usuário 14: Como um funcionário, quero ter acesso a um registro com todas as notas fiscais geradas por todos os usuários.
  - História de Usuário 15: Como um funcionário, quero ter acesso a um registro com todas as transações feitas por todos os usuários e conseguir filtrá-las.

- Requisitos Não Funcionais

  - História de Usuário 16: Como um usuário, quero que meus dados sensíveis sejam criptografados para garantir segurança.
  - História de Usuário 17: Como um usuário, quero que o sistema proteja contra acesso não autorizado.
  - História de Usuário 18: Como um usuário, quero que o sistema responda rapidamente às minhas solicitações.
  - História de Usuário 19: Como um usuário, quero que o sistema faça backup e recuperação de dados em caso de falhas.
  - História de Usuário 20: Como um usuário, quero uma interface intuitiva e amigável.
  - História de Usuário 21: Como um usuário, quero que o sistema ofereça suporte a diferentes tamanhos de tela.

### **5. Arquitetura do Sistema**

#### **5.1 Frontend**
- Desenvolvimento de aplicativo web resposivo (JavaScript/React e Java/Spring Boot).
- Interface amigável para facilitar a compra de tickets.

#### **5.2 Backend**
- Servidor seguro para autenticação e autorização.
- Sistema de gestão de transações e sincronização offline.

#### **5.3 Banco de Dados**
- Banco de dados relacional para armazenar dados de transações e usuários. (Relacional com PostgreSQL).

### **6. Fluxos de Funcionamento**

- Fluxo padrão do usuário:

1. **Cadastro**: O usuário se cadastra no aplicativo.

2. **Login**: O usuário faz login no aplicativo.

3. **Escolha do Ticket**: Seleção do tipo de refeição.

4. **Pagamento**: Escolha da forma de pagamento e confirmação da compra.

5. **Geração do QR Code**: Um comprovante é gerado para validar a compra.

6. **Histórico**: O usuário pode consultar seu histórico de transações e notas fiscais a qualquer momento.

- Fluxo do funcionário:

2. **Login**: O usuário faz login no aplicativo.

3. **Leitura de comprovante**: O funcionário pode ler um comprovante.

4. **Marcação do comprovante**: Um comprovante lido se torna inativo e não pode mais ser utilizado.

5. **Histórico**: O usuário pode consultar o histórico de transações e as notas fiscais de todos os usuários a qualquer momento.

### **7. Testes**

- Testar o fluxo crítico do sistema:

1. **Cadastro**: O usuário se cadastra no aplicativo.

2. **Login**: O usuário faz login no aplicativo.

3. **Escolha do Ticket**: Seleção do tipo de refeição.

4. **Pagamento**: Escolha da forma de pagamento e confirmação.

5. **Geração do QR Code**: Um comprovante é gerado para validar a compra.

### **8. Deploy e Manutenção**

- Implementação do sistema em ambiente de produção a ser escolhido, provavelmente Vercel.
- Monitoramento constante e atualizações de segurança.

### **9. Considerações Finais**

O Sistema de Pagamento RU proporcionará uma experiência eficiente e conveniente para os usuários, garantindo segurança nas transações e facilidade de uso.

### **10. Cronograma de Sprints**

| Sprint | Duração | Épico                        | História de Usuário                            |
|--------|----------|------------------------------|-----------------------------------------------|
| 1      | 2 semanas| Autenticação e Autorização   | 1. Autenticação de usuários, 2. Inserção da matrícula, 3. Recuperação de senha |
| 2      | 2 semanas| Compra de Tickets             | 1. Interface para compra de tickets, 2. Opções de pagamento, 3. Geração de comprovante, 4. Geração de nota fiscal |
| 3      | 2 semanas| Tela de Comprovante e Histórico de Transações | 1. Acesso ao comprovante, 2. Tipo do comprovante, 3. Leitura do comprovante, 4. Marcação do comprovante, 5. Acesso ao histórico de transações do usuário, 6. Acesso ao histórico de notas fiscais do usuário, 7. Acesso à todas as transações de todos os usuários para o funcionário, 8. Acesso à todas as notas fiscais de todos os usuários para o funcionário |
| 4      | 2 semanas| Integração e Deploy           | 1. Integração de todas as funcionalidades, 2. Preparação para o deploy do sistema |
| 5      | 2 semanas| Requisitos Não Funcionais e Entrega | 1. Criptografia de dados sensíveis, 2. Proteção contra acesso não autorizado, 3. Resposta rápida às solicitações, 4. Interface intuitiva e amigável, 5. Suporte a diferentes tamanhos de tela |

### **11. Gestão de Riscos**

- Risco: Problemas de integração entre as partes do sistema.
  - Mitigação: Realizar testes de integração frequentes durante o desenvolvimento.
- Risco: Dificuldades técnicas na implementação de métodos de pagamento.
  - Mitigação: Iniciar com métodos de pagamento mais simples e escalonáveis.
- Risco: Limitações na escalabilidade do banco de dados.
  - Mitigação: Monitoramento contínuo e otimização conforme necessário.
- Risco: Problemas de segurança devido à criptografia básica.
  - Mitigação: Atualizar a criptografia conforme necessário e realizar auditorias de segurança regulares.

### **12. Funções - Membros**

- Anderson de Lima Leite - anderson.leite@ccc.ufcg.edu.br: Desenvolvedor Back-end.
- Davyson Douglas Gomes Guimarães - davyson.guimaraes@ccc.ufcg.edu.br: Desenvolvedor Back-end/Scrum Master.
- Felipe Jerônimo Bernardo da Silva - felipe.jeronimo.silva@ccc.ufcg.edu.br: Desenvolvedor Front-end
- José Arthur Neves de Brito -  jose.arthur.brito@ccc.ufcg.edu.brs: Desenvolvedor Front-end
- Luiz Antonio Correia Costa Cardozo - luiz.cardozo@ccc.ufcg.edu.br: Desenvolvedor Back-end/Product Owner.
- Marcos Vinícius Santos Silva - marcos.silva@ccc.ufcg.edu.br: Desenvolvedor Front-end.

