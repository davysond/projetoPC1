### **Projeto de Software: Sistema de Pagamento RU**

### **1. Introdução**

O Sistema de Pagamento RU é um software destinado à gestão de compra de tickets do Restaurante Universitário (RU). Ele oferece a conveniência de ser acessado pelo aplicativo e permite a compra de tickets de refeição. O usuário pode efetuar o pagamento através de diversas opções, como Pix, cartão, entre outras.

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

### **4. Arquitetura do Sistema**

#### **4.1 Frontend**
- Desenvolvimento de aplicativo web resposivo (JavaScript/React e Java/Spring Boot).
- Interface amigável para facilitar a compra de tickets.

#### **4.2 Backend**
- Servidor seguro para autenticação e autorização.
- Sistema de gestão de transações e sincronização offline.

#### **4.3 Banco de Dados**
- Banco de dados relacional para armazenar dados de transações e usuários.

### **5. Fluxo de Funcionamento**

1. **Login**: O usuário faz login no aplicativo.

2. **Escolha do Ticket**: Seleção do tipo de refeição e quantidade desejada.

3. **Pagamento**: Escolha da forma de pagamento (Pix, cartão, etc.) e confirmação.

4. **Geração do QR Code**: Um QR code é gerado para validar a compra.

5. **Sincronização**: Quando o dispositivo volta online, as transações offline são sincronizadas.

6. **Histórico**: O usuário pode consultar seu histórico de transações a qualquer momento.

### **6. Testes**

- Testes unitários e de integração para garantir a robustez do sistema.

### **7. Implementação**

- Desenvolvimento do frontend, backend e integração do banco de dados.

### **8. Deploy e Manutenção**

- Implementação do sistema em ambiente de produção.
- Monitoramento constante e atualizações de segurança.

### **9. Considerações Finais**

O Sistema de Pagamento RU proporcionará uma experiência eficiente e conveniente para os usuários, garantindo segurança nas transações e facilidade de uso tanto online quanto offline.

### **10. Cronograma de Sprints**

| Sprint | Atividades                                                     | Tempo Estimado | Reuniões                                           |
|--------|-----------------------------------------------------------------|----------------|----------------------------------------------------|
| 1      | Definição de requisitos, arquitetura e planejamento tecnológico | -      | Reunião Inicial                                   |
| 2      | Desenvolvimento do Frontend                                    | 3 semanas      | Revisão de Meio de Sprint                         |
| 3      | Desenvolvimento do Backend                                     | 4 semanas      | Revisão de Meio de Sprint                         |
| 4      | Funcionalidades de Compra e Pagamento                          | 3 semanas      | Revisão de Meio de Sprint                         |
| 5      | Funcionalidades Offline e Sincronização                       | 3 semanas      | Revisão de Meio de Sprint                         |
| 6      | Histórico de Transações e Notificações                         | 2 semanas      | Revisão Final de Sprint                           |
| 7      | Testes e Correções                                             | 3 semanas      | Revisão de Testes                                 |
| 8      | Implementação e Deploy                                         | 2 semanas      | Reunião de Planejamento Final                     |
| 9      | Monitoramento e Manutenção                                    | Em andamento   | Reuniões periódicas de Manutenção (a cada duas semanas) |

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

- Anderson de Lima Leite - anderson.leite@ccc.ufcg.edu.br: 
- Cleciana Maria de Santana - cleciana.santana@ccc.ufcg.edu.br: 
- Davyson Douglas Gomes Guimarães - davyson.guimaraes@ccc.ufcg.edu.br: 
- Felipe Jerônimo Bernardo da Silva - felipe.jeronimo.silva@ccc.ufcg.edu.br: 
- José Arthur Neves de Brito -  jose.arthur.brito@ccc.ufcg.edu.brs: 
- Luiz Antonio Correia Costa Cardozo - luiz.cardozo@ccc.ufcg.edu.br: 
- Marcos Vinícius Santos Silva - marcos.silva@ccc.ufcg.edu.br: 
