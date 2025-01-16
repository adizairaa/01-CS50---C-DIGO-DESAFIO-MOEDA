# 💰 Algoritmo Guloso para Troco Mínimo  

Este repositório contém a solução para o problema de calcular o número mínimo de moedas necessárias para fornecer troco usando um **algoritmo guloso**. A implementação é feita em C e considera as moedas disponíveis de 25, 10, 5 e 1 centavo(s).  

---

## 🧠 **Descrição do Problema**  

Dado um valor de troco devido ao cliente, o objetivo do programa é determinar o menor número de moedas necessárias para fornecer o troco, utilizando uma abordagem gulosa.  

### **Regras do Algoritmo Guloso:**  
1. Selecionar a maior moeda possível que se ajuste ao valor restante do troco.  
2. Subtrair o valor da moeda escolhida do valor restante.  
3. Repetir o processo até que o troco restante seja 0.  

Por exemplo, para um troco de 41 centavos:  
- Selecionar uma moeda de 25 centavos (restam 16 centavos).  
- Selecionar uma moeda de 10 centavos (restam 6 centavos).  
- Selecionar uma moeda de 5 centavos (resta 1 centavo).  
- Selecionar uma moeda de 1 centavo (restam 0 centavos).  

Resultado: 4 moedas no total.  

---

## ⚙️ **Como Funciona o Programa**  

1. O programa solicita ao usuário um valor de troco em reais.  
   - Aceita valores como `0.41`, `9.75` ou `10.00`.  
   - Rejeita valores negativos, palavras ou caracteres não numéricos.  

2. Converte o valor de reais para centavos para evitar imprecisões de ponto flutuante.  

3. Calcula o número mínimo de moedas utilizando o algoritmo guloso.  

4. Exibe o resultado como um número inteiro indicando a quantidade mínima de moedas.  

---

## 🚀 **Como Rodar o Programa**  

1. Clone este repositório:  
   ```bash
   git clone https://github.com/seuusuario/algoritmo-troco.git
   cd algoritmo-troco
   ```

2. Compile o código:  
   ```bash
   make cash
   ```

3. Execute o programa:  
   ```bash
   ./cash
   ```

4. Insira o valor do troco quando solicitado.  

---

## ✅ **Exemplos de Entrada e Saída**  

### Exemplo 1:  
```bash
$ ./cash
Troca devida: 0.41
4
```

### Exemplo 2:  
```bash
$ ./cash
Troca devida: -0.50
Troca devida: foo
Troca devida: 0.99
9
```

---

## 🛠️ **Ferramentas e Testes**  

- **Bibliotecas Utilizadas:**  
  - `math.h`: Para arredondar valores de ponto flutuante.  
  - `cs50.h`: Para facilitar a entrada de dados.  

- **Testes Manuais:**  
  - Insira valores negativos, palavras, ou pressione Enter sem entrada.  
  - Teste com valores como `0.01`, `9.99` ou `0.00`.  

- **Validação de Estilo:**  
  ```bash
  style50 cash.c
  ```

---

## 🌟 **Contribuições**  

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests com melhorias ou sugestões.  

---

## 📜 **Licença**  

Este projeto está licenciado sob a [MIT License](LICENSE).  

