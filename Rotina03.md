### Caso de Teste 01: Compra concluída com sucesso
| ID       | Descrição                                                        |
|----------|------------------------------------------------------------------|
| C03-CT01 | Compra registrada, estoque atualizado e lançamento no caixa.     |

**Pré-condições**
- Fornecedor cadastrado.
- Produto cadastrado.

**Passos**
DADO que o usuário inicia uma nova compra  
E adiciona produtos  
QUANDO finalizar a compra  
ENTÃO o estoque deve ser atualizado corretamente.

**Critérios de Aceitação**
- Compra marcada como CONFIRMADA.  
- Teste evidenciado e aprovado.  
- **COLOCAR LINK AQUI**

---

### Caso de Teste 02: Fornecedor cadastrado com sucesso
| ID       | Descrição                                                        |
|----------|------------------------------------------------------------------|
| C03-CT02 | Fornecedor cadastrado no sistema e redirecionado para listagem.  |

**Pré-condições**
- Nenhuma.

**Passos**
DADO que o usuário acessa a tela de cadastro de fornecedores  
E preenche todos os dados obrigatórios  
QUANDO clicar em **Salvar**  
ENTÃO o sistema deve criar um novo fornecedor.

**Critérios de Aceitação**
- Teste evidenciado e reprovado: erro no campo CEP mesmo informando valor válido.  
- **COLOCAR LINK AQUI**

---

### Caso de Teste 03: Fornecedor não informado
| ID       | Descrição                                                        |
|----------|------------------------------------------------------------------|
| C03-CT02 | Sistema deve impedir criação de compra sem fornecedor.           |

**Pré-condições**
- Nenhuma.

**Passos**
DADO que o usuário tenta criar uma compra sem informar fornecedor  
QUANDO clicar em **Salvar**  
ENTÃO o sistema deve bloquear a ação.

**Critérios de Aceitação**
- Mensagem exibida: “Fornecedor obrigatório”.  
- Teste evidenciado e aprovado.  
- **COLOCAR LINK AQUI**

---

### Caso de Teste 04: Tipo de documento não selecionado
| ID       | Descrição                                                        |
|----------|------------------------------------------------------------------|
| C03-CT03 | Sistema deve impedir finalização da compra sem tipo de documento.|

**Pré-condições**
- Compra sendo finalizada.

**Passos**
DADO que o usuário cria uma nova compra  
E chega à etapa de finalização  
E não seleciona o tipo de documento  
QUANDO clicar em **Salvar**  
ENTÃO o sistema deve exibir uma mensagem de erro.

**Critérios de Aceitação**
- Mensagem: “É necessário informar o tipo de documento”.  
- Teste realizado e evidenciado.  
- **COLOCAR LINK AQUI**
