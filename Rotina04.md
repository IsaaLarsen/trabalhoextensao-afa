LINK VIDEOS:[LINK VIDEOS:](https://drive.google.com/drive/folders/1vbQNf6b-eGDcT7QbNSy8M2_uabqg7QHf?usp=sharing)

### Caso de Teste 01: Cadastro de cliente PF com sucesso
| ID       | Descrição                                  |
|----------|--------------------------------------------|
| C04-CT01 | Cadastro básico deve ser salvo corretamente.|

**Pré-condições**
- Nenhuma.

**Passos**
DADO que usuário clica em **“Novo”**  
E preenche os campos obrigatórios  
QUANDO clicar em **Salvar**  
ENTÃO o cliente deve aparecer na lista.

**Critérios de Aceitação**
- Cadastro salvo.  
- Teste evidenciado e aprovado.  
- **VIDEO CASO01 https://drive.google.com/file/d/18oglXn7CxsaB4T_e4uH_dmrehP_SnMjB/view?usp=drive_link**

---

### Caso de Teste 02: Tentativa de salvar cliente sem campos obrigatórios
| ID       | Descrição                                  |
|----------|--------------------------------------------|
| C04-CT02 | Sistema deve impedir cadastro incompleto.  |

**Pré-condições**
- Nenhuma.

**Passos**
DADO que o usuário deixa Nome ou CEP vazio  
QUANDO tentar salvar  
ENTÃO o sistema deve exibir um alerta.

**Critérios de Aceitação**
- Cadastro bloqueado.  
- Teste evidenciado e aprovado.  
- **VIDEO CASO02 https://drive.google.com/file/d/1wJ-V64zR-vHD5ZvnDZHO8lcAmivEc5Bl/view?usp=drive_link**

---

### Caso de Teste 03: Exclusão de cliente cadastrado
| ID       | Descrição                                                   |
|----------|-------------------------------------------------------------|
| C04-CT03 | Sistema exclui cliente e redireciona para a listagem.       |

**Pré-condições**
- Cliente cadastrado no sistema.

**Passos**
DADO que o usuário acessa a tela de clientes  
E seleciona o cliente que deseja excluir  
QUANDO clicar em **Excluir**  
ENTÃO o sistema remove o cliente selecionado.

**Critérios de Aceitação**
- Alerta exibido.  
- Teste evidenciado e aprovado.  
- **VIDEO CASO03 https://drive.google.com/file/d/1_Lv9tKrQ_7jf9DuLhNB7AHMWUuvK8NOK/view?usp=drive_link**

---

### Caso de Teste 04: Habilitar limite para o cliente
| ID       | Descrição                                                       |
|----------|-----------------------------------------------------------------|
| C04-CT03 | Sistema habilita limitações e redireciona para a tela correta. |

**Pré-condições**
- Cliente já cadastrado.

**Passos**
DADO que o usuário está na tela de clientes  
E seleciona o cliente desejado  
E clica no ícone de configurações  
E habilita as opções **Dados Financeiros** e **Dependentes**  
QUANDO clicar em **Salvar**  
ENTÃO o sistema solicita credenciais e nome para confirmação.

**Critérios de Aceitação**
- Alterações salvas.  
- Campos financeiros passam a aparecer.  
- Teste evidenciado e aprovado.  
- **VIDEO CASO04 https://drive.google.com/file/d/1-eviWqqhdlhAsaiRHG9wIsD9vYwjIdJu/view?usp=drive_link**

---

### Caso de Teste 05: Realizar uma venda a prazo sem limite de crédito
| ID       | Descrição                                                   |
|----------|-------------------------------------------------------------|
| C04-CT04 | Sistema alerta e não permite venda a prazo para o cliente.  |

**Pré-condições**
- Cliente cadastrado com limite inferior ao valor da venda.

**Passos**
DADO que o usuário acessa a aba **Vendas**  
E clica em **Novo**  
E preenche todos os campos  
E seleciona um cliente com limite baixo  
QUANDO finalizar a compra e selecionar **A Prazo**  
ENTÃO o sistema deve alertar que o cliente não possui limite suficiente.

**Critérios de Aceitação**
- Cliente é exibido na listagem.  
- Teste evidenciado e aprovado.  
- **VIDEO CASO05 https://drive.google.com/file/d/1TZpebA1B0t9I0B1jGT6762Rb94BGHuNA/view?usp=drive_link**

