# 🧪 Exploratory Testing Findings – KaBuM!

Registro de achados de uma sessão de teste exploratório conduzida no site KaBuM

---

## 📌 Charter 001

| Campo              | Detalhe                                                                                                                           |
| ------------------ | --------------------------------------------------------------------------------------------------------------------------------- |
| ID do Charter      | 001                                                                                                                               |
| Área               | Explorar funcionalidades e o fluxo de adição ao carrinho de compras, assim como a aplicação de cupons de desconto                 |
| Missão             | Explorar comportamentos inesperados na busca de produtos, aplicação de filtros e gestão do carrinho de compras                    |
| Duração            | 20 minutos                                                                                                                        |
| Ambiente           | Chrome 146.0.7680.165 (64 bits)                                                                                                   |
| Data               | 28/03/2026                                                                                                                        |
| Tester             | Renato Paes                                                                                                                       |
| Hipóteses iniciais | O total do carrinho pode não atualizar corretamente ao alterar quantidade, filtros combinados podem retornar dados inconsistentes |

---

## 🔍 Heurísticas utilizadas

* CRUD: criação, leitura, atualização e remoção
* Vazio/Cheio/Limite: estados extremos
* Fluxo interrompido: voltar, recarregar e trocar de aba

---

## 🧪 Observações

### OBS-001 – Botão voltar e avançar

* **Área:** Navegação
* **Heurística:** Fluxo interrompido
* **Ação:** Uso do botão voltar/avançar
* **Resultado esperado:** Preservar compras
* **Resultado obtido:** Funcionamento adequado
* **Classificação:** ✅ Funciona como esperado

---

### OBS-002 – Quantidade no carrinho

* **Área:** Carrinho de compras
* **Heurística:** CRUD / Limite
* **Ação:** Alterar quantidade
* **Resultado esperado:** Atualizar valores corretamente
* **Resultado obtido:** Funciona, porém limite não é claro
* **Classificação:** ⚠️ Sugestão de melhoria

---

### OBS-003 – Refresh (F5)

* **Área:** Navegação
* **Heurística:** Fluxo interrompido
* **Resultado:** Itens preservados
* **Classificação:** ✅ Funciona como esperado

---

### OBS-004 – Cupom de desconto

* **Resultado:** Aplicação correta
* **Classificação:** ✅ Funciona como esperado

---

### OBS-005 – Múltiplos cupons

* **Resultado:** Bloqueio correto com mensagem
* **Classificação:** ✅ Funciona como esperado

---

### OBS-006 – Frete

* **Resultado:** Atualização correta
* **Classificação:** ✅ Funciona como esperado

---

### OBS-007 – Favoritos

* **Resultado:** Produto não sai dos favoritos após ir para o carrinho
* **Classificação:** ⚠️ Sugestão de melhoria

---

### OBS-008 – Ícone carrinho

* **Resultado:** Falta de clareza visual
* **Classificação:** ⚠️ Sugestão de melhoria

---

### OBS-009 – Checkout

* **Resultado:** Informações do carrinho permanecem visíveis
* **Classificação:** ⚠️ Sugestão de melhoria

---

## 📊 Resumo dos Achados

| Classificação          | Quantidade |
| ---------------------- | ---------- |
| Bug                    | 0          |
| Sugestão de melhoria   | 4          |
| Funciona como esperado | 5          |

---

## 📌 Charter 002

| Campo         | Detalhe                                       |
| ------------- | --------------------------------------------- |
| ID do Charter | 002                                           |
| Área          | Cadastro de usuários e busca                  |
| Missão        | Identificar falhas de validação e usabilidade |
| Duração       | 20 minutos                                    |
| Ambiente      | Chrome 146.0.7680.165                         |
| Data          | 29/03/2026                                    |
| Tester        | Renato Paes                                   |

---

## 🔍 Observações

### OBS-001 – Telefone

* **Resultado:** Aceita DDD inválido (00)
* **Classificação:** ⚠️ Sugestão de melhoria

---

### OBS-002 – Data de nascimento

* **Resultado:** Validação tardia
* **Classificação:** ⚠️ Sugestão de melhoria

---

## 📊 Resumo dos Achados

| Classificação          | Quantidade |
| ---------------------- | ---------- |
| Bug                    | 0          |
| Sugestão de melhoria   | 2          |
| Funciona como esperado | 0          |

---

## 🚀 Próximos passos

* Converter observações em bugs formais
* Priorizar itens com impacto de segurança
* Nova sessão focada em login e cadastro

---

## 🛠 Técnicas Aplicadas

* Teste exploratório com charter estruturado
* Heurísticas: CRUD, Vazio/Cheio/Limite, Fluxo interrompido

