# Simulador de Investimentos e Alocação em Fundos Imobiliários (FIIs)

Projeto prático de um simulador financeiro em Excel desenvolvido durante o meu aprendizado no curso da **Digital Innovation One (DIO)**.

---

## 📋 Resumo do Projeto

### 1. As perguntas que a ferramenta responde e onde aparece cada resposta:
* **Qual a sugestão de investimento com base no salário?** (Aparece na célula `D14`).
* **Qual será o patrimônio acumulado e os dividendos mensais gerados?** (Aparecem nas células `D20` e `D21`).
* **Como evolui o patrimônio e a renda em diferentes prazos de 2 a 30 anos?** (Aparece na tabela de Cenários, linhas 24 a 28).
* **Como alocar os recursos (percentuais e valores) por tipo de FII conforme o perfil?** (Aparece na tabela de alocação, linhas 35 a 41).

### 2. Como o VF e o PROCV entram nos cálculos:
* **VF (Valor Futuro / FV):** Utilizado nas fórmulas financeiras para projetar o crescimento do capital e dos juros compostos ao longo dos anos, presente no cálculo do patrimônio acumulado (`D20`) e na tabela de cenários.
* **PROCV (VLOOKUP):** Utilizado nas células de percentual sugerido (`C35` a `C40`) para buscar dinamicamente os pesos de cada FII com base em uma chave composta (`Perfil-Tipo de FII`) vinda da base de dados (`Planilha2`).

### 3. Intervalos Nomeados criados na planilha:
* `Aporte`, `Patrimonio`, `Qtd_anos`, `Rendimento`, `rendimento_carteira`, `Taxa_mensal`, além de referências de gráficos (`_xlchart.v1.0` e `_xlchart.v1.1`).

### 4. Percentuais de cada perfil e de onde vieram:
Os dados vieram estruturados da `Planilha2` conforme o perfil de risco:
* **Conservador:** 30% Papel, 30% Tijolo, 20% Híbridos, 20% FOFs (0% Desenvolvimento e Hotelarias).
* **Moderado:** 30% Papel, 30% Tijolo, 10% Híbridos, 10% FOFs, 10% Desenvolvimento, 10% Hotelarias.
* **Agressivo:** 40% Papel, 10% Tijolo, 10% Híbridos, 10% FOFs, 20% Desenvolvimento, 10% Hotelarias.

### 5. O que mudou em relação à ferramenta padrão do Expert:
* Uso de chaves compostas para otimizar as buscas no PROCV de forma limpa.
* Adoção de intervalos nomeados para tornar as fórmulas financeiras mais legíveis.
* Automação de múltiplos horizontes de tempo na tabela de cenários vinculada às funções de valor futuro.

---

### ⚠️ Aviso Acadêmico / Disclaimer
Este repositório foi desenvolvido estritamente para fins **educacionais e acadêmicos**, como parte do desafio prático do curso da **Digital Innovation One (DIO)**. As adaptações e parametrizações foram realizadas por mim como estudante em fase de aprendizado.
