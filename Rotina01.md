### Caso de Teste 01: Importação de XML válida e geração da compra
| ------- | ---------------------------------------------------------------- |
| ID      | Descrição                                                        |
| C01-CT01 | Importação de XML correto deve registrar itens e atualizar o estoque. |

#### Pré-condições
- XML íntegro e válido.
- Produtos cadastrados no sistema.

#### Passos
DADO que o usuário acessa **Pedidos > Importar XML de Compra**  
E informa **CFOP, Grupo e ST de Entrada**  
E seleciona um XML válido  
QUANDO clicar em **“Gerar Compra”** e em seguida **“Finalizar”**  
ENTÃO o sistema deve atualizar o estoque e marcar a compra como **“CONFIRMADA”**.

#### Critérios de aceitação
- Compra confirmada.  
- Estoque atualizado com os itens importados.  
- Teste executado e evidenciado.  
- **COLOCAR LINK AQUI**

| ------- | ---------------------------------------------------------------- |

---

### Caso de Teste 02: Validação de campos obrigatórios
| ------- | ---------------------------------------------------------------- |
| ID      | Descrição                                                        |
| C01-CT03 | Bloqueio da importação quando CFOP ou Grupo não forem preenchidos. |

#### Pré-condições
- Nenhuma.

#### Passos
DADO que o usuário acessa a tela  
E deixa **CFOP ou Grupo** sem preenchimento  
QUANDO tentar importar o XML  
ENTÃO o sistema deve exibir mensagens informando que o campo é obrigatório.

#### Critérios de aceitação
- Validação dos campos obrigatórios.  
- Testes executados e evidenciados.  
- **COLOCAR LINK AQUI**

| ------- | ---------------------------------------------------------------- |

---

### Caso de Teste 03: Importação de XML inválido
| ------- | ---------------------------------------------------------------- |
| ID      | Descrição                                                        |
| C01-CT02 | Sistema deve rejeitar XML incorreto ou corrompido. |

#### Pré-condições
- XML com estrutura inválida.

#### Passos
DADO que o usuário acessa a tela de importação  
E seleciona um XML inválido  
QUANDO clicar em **“Importar XML”**  
ENTÃO o sistema deve exibir erro e impedir a continuidade do processo.

#### Critérios de aceitação
- Mensagem clara indicando erro no XML.  
- Não deve permitir prosseguir para gerar compra.  
- Teste realizado e evidenciado.  
- **COLOCAR LINK AQUI**

| ------- | ---------------------------------------------------------------- |

---

### Caso de Teste 04: Compra gerada sem confirmação de entrada
| ------- | ---------------------------------------------------------------- |
| ID      | Descrição                                                        |
| C01-CT04 | Compra deve permanecer pendente enquanto não for confirmada. |

#### Pré-condições
- XML importado com sucesso.

#### Passos
DADO que o usuário gera a compra  
QUANDO sair da tela sem alterar o status para **CONFIRMADA**  
ENTÃO a compra deve permanecer com status **“PENDENTE”** e não alterar o estoque.

#### Critérios de aceitação
- Estoque inalterado.  
- Teste realizado e evidenciado.  
- **COLOCAR LINK AQUI**

| ------- | ---------------------------------------------------------------- |
