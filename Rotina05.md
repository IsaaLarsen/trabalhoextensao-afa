LINK VIDEOS: https://drive.google.com/drive/folders/1rPAU-DbDQ_1Cya_PgiDzbE0YH7vf6NkQ?usp=drive_link


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

VIDEO CASO 01: https://drive.google.com/file/d/1u7kaWDCkIrKdpTILDo9ok8uDynsUNchh/view?usp=drive_link
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

VIDEO CASO 02: https://drive.google.com/file/d/1SgQ-dv_pq6uvY00MsnB-UAf7MjvjwYeB/view?usp=drive_link
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

VIDEO CASO 03: https://drive.google.com/file/d/1w2Jz-ZPw8MFFhPZxvsHg4FaWPEbITZtn/view?usp=drive_link 
