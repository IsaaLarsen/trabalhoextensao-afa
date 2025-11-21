LINK VIDEOS:[LINK VIDEOS:](https://drive.google.com/drive/folders/1oAEPwQBpbjFOWliLfzkS8e_A4_Lo-DFy?usp=sharing)

### Caso de Teste 01: Venda concluída com sucesso
| ID       | Descrição                                                        |
| -------- | ---------------------------------------------------------------- |
| C02-CT01 | Venda registrada corretamente, reduzindo estoque e lançando valor no caixa. |

**Pré-condições**  
- Cliente, funcionário e produtos cadastrados.  
- Produto com quantidade suficiente em estoque.

**Passos**  
DADO que o usuário acessa a tela de vendas e clica em **Novo**  
E seleciona cliente, funcionário e data  
E adiciona produtos  
QUANDO finalizar e salvar  
ENTÃO a venda deve ser registrada e aparecer no Livro Caixa.

**Critérios de Aceitação**  
- Estoque atualizado conforme venda.  
- Entrada registrada no caixa.  
- Teste realizado e evidenciado.  
- **COLOCAR LINK AQUI**

---

### Caso de Teste 02: Produto sem estoque suficiente
| ID       | Descrição                                                        |
| -------- | ---------------------------------------------------------------- |
| C02-CT02 | Sistema deve impedir inclusão de produto com estoque insuficiente. |

**Pré-condições**  
- Produto com quantidade disponível = 10.

**Passos**  
DADO que o usuário tenta adicionar o produto  
QUANDO selecionar a quantidade desejada  
ENTÃO o sistema deve exibir a mensagem **“Estoque insuficiente”**.

**Critérios de Aceitação**  
- Produto não deve ser incluído na venda.  
- Teste realizado e reprovado: sistema permitiu finalizar venda mesmo sem estoque.  
- **COLOCAR LINK AQUI**

---

### Caso de Teste 03: Finalizar venda sem selecionar tipo de documento
| ID       | Descrição                                                        |
| -------- | ---------------------------------------------------------------- |
| C02-CT03 | Sistema deve impedir finalização sem escolha do tipo de documento. |

**Pré-condições**  
- Venda preparada para finalizar.

**Passos**  
DADO que o usuário está na tela final  
QUANDO clicar em **Salvar** sem selecionar o tipo de documento  
ENTÃO o sistema deve exibir uma mensagem de erro.

**Critérios de Aceitação**  
- Finalização bloqueada.  
- Teste evidenciado e aprovado.  
- **COLOCAR LINK AQUI**

---

### Caso de Teste 04: Cadastrar venda sem selecionar cliente
| ID       | Descrição                                                        |
| -------- | ---------------------------------------------------------------- |
| C02-CT04 | Sistema deve impedir cadastro de venda sem cliente selecionado. |

**Pré-condições**  
- Campo cliente não preenchido.

**Passos**  
DADO que o usuário está na tela de vendas  
E clica em **Novo**  
E deixa o campo cliente vazio  
QUANDO clicar em **Salvar**  
ENTÃO o sistema deve exibir um erro informando que é obrigatório selecionar um cliente.

**Critérios de Aceitação**  
- Cadastro bloqueado.  
- Teste evidenciado e aprovado.  
- **COLOCAR LINK AQUI**
