# 🧮 Análise Estatística de Desempenho de Estudantes

## 🎯 Objetivo
Este projeto aplica **conceitos de inferência estatística** — testes de hipótese e intervalos de confiança (usando métodos analíticos e bootstrap) — sobre o dataset `Student_performance_data.csv`, que contém informações sobre o desempenho de estudantes.

O trabalho foi desenvolvido em Python, explorando a relação entre variáveis como **gênero**, **horas de estudo semanais** e **GPA (nota média)**.
---

## 📊 Estrutura do Projeto
```bash
├── Inferência Estatística.ipynb # Notebook com toda a análise
├── Student_performance_data.csv # Base de dados utilizada
├── summary_hypothesis_tests_v2.csv # Resumo dos resultados estatísticos
├── README.md # Este arquivo
├── LICENSE # Licença MIT
```

---

## 🧠 Etapas da Análise

1. **Exploração dos dados**
   - Verificação de tipos de variáveis, valores ausentes e distribuições.
   - Identificação das principais variáveis: `Gender`, `StudyTimeWeekly`, `GPA`.

2. **Formulação de hipóteses**
   - **H1**: Diferença de médias de GPA entre gêneros.
   - **H2**: Correlação entre horas de estudo e GPA.

3. **Aplicação dos testes**
   - Testes de normalidade (Shapiro-Wilk) e homogeneidade (Levene).
   - **Mann–Whitney U** para H1 (duas amostras independentes).
   - **Spearman rho** para H2 (correlação não paramétrica).

4. **Intervalos de Confiança (Bootstrap)**
   - Estimativa de IC 95% para diferenças de médias e correlação.

5. **Visualizações**
   - Histogramas e boxplots por gênero.
   - Scatterplot (horas de estudo × GPA).
   - Distribuições bootstrap.

---

## 📈 Principais Resultados

### Hipótese 1 — Diferença entre gêneros
- Teste: **Mann–Whitney U**
- p-value ≈ 0.48 → **não rejeitamos H₀**
- Conclusão: não há diferença estatisticamente significativa entre as médias de GPA dos grupos de gênero.

### Hipótese 2 — Correlação entre horas de estudo e GPA
- Teste: **Spearman rho**
- ρ ≈ 0.17, p < 0.001 → **rejeitamos H₀**
- Conclusão: há uma correlação positiva, embora fraca, entre horas de estudo e desempenho (GPA).

---

## 🧩 Ferramentas Utilizadas
- **Python 3.11+**
- **Pandas**, **NumPy**, **SciPy**, **Seaborn**, **Matplotlib**
- **Bootstrap** para ICs via reamostragem

---

## 🧪 Reproduzindo a Análise

### 1️⃣ Para a execução do projeto, instale as seguintes dependências: 

```bash
pip install pandas
```
```bash
pip install numpy
```
```bash
pip install scipy
```
```bash
pip install matplotlib
```

2️⃣ Executar o notebook:

Abra o arquivo Student_performance_analysis.ipynb no Jupyter Notebook ou VS Code e execute todas as células.

📜 Licença:

Este projeto está licenciado sob a MIT License.

👨‍💻 Autores
<table>
  <tr>
    <td align="center">
         <a href="https://github.com/JoaoDario632">
         <img src="https://avatars.githubusercontent.com/u/134674876?v=4" style="border-radius: 50%" width="100px;" alt="ferreira"/>
         <br />
         <sub><b>João Dário 💻👑</b></sub>
       </a>
     </td>
     <td align="center">
        <a href="https://github.com/FrrTiago">
         <img src="https://avatars.githubusercontent.com/u/132114628?v=4" style="border-radius: 50%" width="100px;" alt="ferreira"/>
         <br />
         <sub><b>Tiago Ferreira 💻👑</b></sub>
       </a>
     </td>
  </tr>
</table>
Desenvolvido como parte de uma atividade prática de inferência estatística e análise de dados.
