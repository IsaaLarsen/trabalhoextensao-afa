LINK VIDEOS:https://drive.google.com/drive/folders/1oAEPwQBpbjFOWliLfzkS8e_A4_Lo-DFy?usp=sharing 


### Caso de Teste 01: Fechar caixa com sucesso

| ID       | Descrição                        |
|----------|----------------------------------|
| C05-CT01 | Caixa do dia fechado e registrado.|

**Pré-condições**
- Haver pelo menos uma venda no dia.

**Passos**
DADO que o usuário abre o **Livro Caixa**  
QUANDO clicar em **“Fechar Caixa”**  
ENTÃO o caixa deve ser finalizado.

**Critérios de Aceitação**
- O dia fica bloqueado para novas movimentações.  
- Teste evidenciado e aprovado.  


---

### Caso de Teste 02: Tentar fechar caixa sem vendas no dia
| ID       | Descrição                              |
|----------|----------------------------------------|
| C05-CT02 | Sistema deve impedir fechamento vazio. |

**Pré-condições**
- Nenhuma venda registrada.

**Passos**
DADO que o usuário tenta fechar o caixa  
QUANDO clicar em **Fechar**  
ENTÃO deve exibir alerta informando **nenhuma movimentação**.

**Critérios de Aceitação**
- Bloqueio do fechamento.  
- Teste evidenciado e reprovado: sistema permitiu fechar mesmo sem vendas.  


---

### Caso de Teste 03: Retirada de valor maior que o saldo atual
| ID       | Descrição                                          |
|----------|----------------------------------------------------|
| C05-CT04 | Bloqueio de retirada com valor acima do saldo atual.|

**Pré-condições**
- Nenhuma.

**Passos**
DADO que o usuário acessa a opção **Retirar Valores**  
E informa um valor maior que o saldo disponível  
QUANDO tentar salvar  
ENTÃO o sistema deve exibir um alerta indicando que o valor não pode ser maior que o saldo atual.

**Critérios de Aceitação**
- Retirada não registrada.  
- Teste evidenciado e aprovado.  
