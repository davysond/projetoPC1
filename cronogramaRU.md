### **Projeto de Software: Sistema de Pagamento RU**

### **1. Introdução**

O Sistema de Pagamento RU é um software destinado à gestão de compra de tickets do Restaurante Universitário (RU). Ele oferece a conveniência de ser acessado pelo aplicativo e permite a compra de tickets de refeição. O usuário pode efetuar o pagamento através de diversas opções, como Pix, cartão, entre outras, é uma solução inovadora dedicada à administração eficiente da aquisição de tickets do Restaurante Universitário (RU), visando atender de maneira ágil e prática às necessidades dos usuários desse serviço. Este software, que prioriza a comodidade, está especialmente desenvolvido para atender ao público diversificado do RU, abrangendo alunos, funcionários e visitantes que frequentam o ambiente acadêmico. Ao possibilitar o acesso por meio de um aplicativo intuitivo, o sistema visa simplificar o processo de compra de tickets de refeição, proporcionando aos usuários uma experiência dinâmica e adaptada às demandas variadas de pagamento, incluindo opções como Pix, cartão, e outras modalidades. Nesse contexto, o Sistema de Pagamento RU destaca-se como uma ferramenta essencial para otimizar a gestão e garantir a satisfação de todos os envolvidos na comunidade acadêmica.

### **2. Requisitos Funcionais**

#### **2.1 Autenticação e Autorização**
- Login seguro para os usuários.
- Diferenciação de perfis (estudante, funcionário) com diferentes permissões.
  
#### **2.2 Compra de Tickets**
- Interface intuitiva para compra de tickets.
- Opções de pagamento: Pix, cartão, entre outras.
- Geração de QR code para validação da compra.

#### **2.3 Histórico de Transações**
- Registro detalhado das transações efetuadas.
- Consulta de histórico para os usuários.

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

### **4. Backlog do Projeto - Sistema de Pagamento RU Pay**

- Épico: Autenticação e Autorização

   - História de Usuário 1: Como um usuário, quero poder me autenticar de forma segura no sistema para acessar minha conta.
   - História de Usuário 2: Como um usuário, quero que o sistema diferencie entre os perfis de estudante e funcionário para garantir diferentes permissões de acesso.
   - História de Usuário 3: Como um usuário, quero poder recuperar minha senha caso eu a esqueça.

- Épico: Compra de Tickets

  - História de Usuário 4: Como um usuário, quero uma interface intuitiva para comprar tickets de refeição.
  - História de Usuário 5: Como um usuário, quero opções de pagamento como Pix, cartão, entre outras.
  - História de Usuário 6: Como um usuário, quero receber um QR code/comprovante após a compra para validar minha transação.

- Épico: Histórico de Transações

  - História de Usuário 7: Como um usuário, quero ter acesso a um registro detalhado das transações efetuadas.
  - História de Usuário 8: Como um usuário, quero poder consultar meu histórico de transações.

- Requisitos Não Funcionais

  - História de Usuário 9: Como um usuário, quero que meus dados sensíveis sejam criptografados para garantir segurança.
  - História de Usuário 10: Como um usuário, quero que o sistema proteja contra acesso não autorizado.
  - História de Usuário 11: Como um usuário, quero que o sistema responda rapidamente às minhas solicitações.
  - História de Usuário 13: Como um usuário, quero que o sistema faça backup e recuperação de dados em caso de falhas.
  - História de Usuário 14: Como um usuário, quero uma interface intuitiva e amigável.
  - História de Usuário 15: Como um usuário, quero que o sistema ofereça suporte a diferentes tamanhos de tela.

### **5. Arquitetura do Sistema**

#### **5.1 Frontend**
- Desenvolvimento de aplicativo web resposivo (JavaScript/React e Java/Spring Boot).
- Interface amigável para facilitar a compra de tickets.

#### **5.2 Backend**
- Servidor seguro para autenticação e autorização.
- Sistema de gestão de transações e sincronização offline.

#### **5.3 Banco de Dados**
- Banco de dados relacional para armazenar dados de transações e usuários. (Relacional com PostgreSQL).

### **6. Fluxo de Funcionamento**

1. **Login**: O usuário faz login no aplicativo.

2. **Escolha do Ticket**: Seleção do tipo de refeição e quantidade desejada.

3. **Pagamento**: Escolha da forma de pagamento (Pix, cartão, etc.) e confirmação.

4. **Geração do QR Code**: Um QR code é gerado para validar a compra.

5. **Sincronização**: Quando o dispositivo volta online, as transações offline são sincronizadas.

6. **Histórico**: O usuário pode consultar seu histórico de transações a qualquer momento.

### **7. Testes**

- Testes unitários e de integração para garantir a robustez do sistema.

### **8. Implementação**

- Desenvolvimento do frontend, backend e integração do banco de dados.

### **9. Deploy e Manutenção**

- Implementação do sistema em ambiente de produção (plataformas viáveis para o processo, tais como Vercel ou Heroku).
- Monitoramento constante e atualizações de segurança.

### **10. Considerações Finais**

O Sistema de Pagamento RU proporcionará uma experiência eficiente e conveniente para os usuários, garantindo segurança nas transações e facilidade de uso tanto online quanto offline.

### **11. Cronograma de Sprints**

| Sprint | Atividades                                                     | Tempo Estimado | Reuniões                                           |
|--------|-----------------------------------------------------------------|----------------|----------------------------------------------------|
| 1      | Desenvolvimento do Front-end e Back-end                        | 2 semanas      | Revisão de Meio de Sprint                         |
| 2      | Desenvolvimento do Backend                                     | 2 semanas      | Revisão de Meio de Sprint                         |
| 4      | Integração e Deploy                                           | 2 semanas      | Revisão de Meio de Sprint                         |
| 5      | Testes e Correções                                             | 2 semanas      | Revisão de Testes                                 |

| Sprint | Duração | Épico                        | História de Usuário                            |
|--------|----------|------------------------------|-----------------------------------------------|
| 1      | 2 semanas| Autenticação e Autorização   | - Autenticação de usuários 
|        |           |                              | - Diferenciação de perfis 
|        |           |                              | - Recuperação de senha
| 2      | 2 semanas| Compra de Tickets             | - Interface para compra de tickets 
|        |           |                              | - Opções de pagamento 
|        |           |                              | - Geração de QR code
| 3      | 2 semanas| Histórico de Transações       | - Registro detalhado de transações 
|        |           |                              | - Consulta de histórico de transações
| 4      | 2 semanas| Integração e Deploy           | - Integração de todas as funcionalidades 
|        |           |                              | - Preparação para o deploy do sistema
| 5      | 2 semanas| Requisitos Não Funcionais e Entrega| - Criptografia de dados sensíveis 
|        |           |                              | - Proteção contra acesso não autorizado 
|        |           |                              | - Resposta rápida às solicitações 
|        |           |                              | - Interface intuitiva e amigável 
|        |           |                              | - Suporte a diferentes tamanhos de tela

| Sprint | Duração | Épico                        | História de Usuário                            |
|--------|----------|------------------------------|-----------------------------------------------|
| 1      | 2 semanas| Autenticação e Autorização   | 1. Autenticação de usuários, 2. Diferenciação de perfis, 3. Recuperação de senha |
| 2      | 2 semanas| Compra de Tickets             | 1. Interface para compra de tickets, 2. Opções de pagamento, 3. Geração de QR code |
| 3      | 2 semanas| Histórico de Transações       | 1. Registro detalhado de transações, 2. Consulta de histórico de transações |
| 4      | 2 semanas| Integração e Deploy           | 1. Integração de todas as funcionalidades, 2. Preparação para o deploy do sistema |
| 5      | 2 semanas| Requisitos Não Funcionais e Entrega| 1. Criptografia de dados sensíveis, 2. Proteção contra acesso não autorizado, 3. Resposta rápida às solicitações, 4. Interface intuitiva e amigável, 5. Suporte a diferentes tamanhos de tela |

### **12. Gestão de Riscos**
- Risco: Problemas de integração entre as partes do sistema.
  - Mitigação: Realizar testes de integração frequentes durante o desenvolvimento.
- Risco: Dificuldades técnicas na implementação de métodos de pagamento.
  - Mitigação: Iniciar com métodos de pagamento mais simples e escalonáveis.
- Risco: Limitações na escalabilidade do banco de dados.
  - Mitigação: Monitoramento contínuo e otimização conforme necessário.
- Risco: Problemas de segurança devido à criptografia básica.
  - Mitigação: Atualizar a criptografia conforme necessário e realizar auditorias de segurança regulares.

### **13. Funções - Membros**

- Anderson de Lima Leite - anderson.leite@ccc.ufcg.edu.br: Desenvolvedor Back-end.
- Cleciana Maria de Santana - cleciana.santana@ccc.ufcg.edu.br: Desenvolvedor Back-end.
- Davyson Douglas Gomes Guimarães - davyson.guimaraes@ccc.ufcg.edu.br: Desenvolvedor Back-end/Scrum Master.
- Felipe Jerônimo Bernardo da Silva - felipe.jeronimo.silva@ccc.ufcg.edu.br: Desenvolvedor Front-end
- José Arthur Neves de Brito -  jose.arthur.brito@ccc.ufcg.edu.brs: Desenvolvedor Front-end
- Luiz Antonio Correia Costa Cardozo - luiz.cardozo@ccc.ufcg.edu.br: Desenvolvedor Back-end.
- Marcos Vinícius Santos Silva - marcos.silva@ccc.ufcg.edu.br: Desenvolvedor Front-end.

