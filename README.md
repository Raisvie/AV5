# AV5
Programa em Python para calcular as frequências naturais de vibração e os modos normais (deslocamentos relativos) de uma cadeia circular (primeira massa conectada a última) composta por N átomos conectados por molas idênticas de constante elástica k .

# 📊 Modelo de Cadeia Vibratória com Matrizes Esparsas (SciPy)

Este repositório contém um notebook interativo que demonstra a construção e análise modal de cadeias de massas e molas utilizando **matrizes esparsas com SciPy**.

## 📌 Objetivo

Explorar o comportamento vibracional de dois sistemas:

- 🟦 **Cadeia homogênea com pontas livres**
- 🟨 **Cadeia ternária com ligação circular**

A análise foca na **densidade de estados vibracionais** e nos **modos normais**, revelando efeitos físicos como *band gaps* e *modos localizados*.

Além disso, o notebook explora o efeito do tamanho da cadeia variando **N = 100, 1.000 e 10.000**, demonstrando como o aumento do número de massas intensifica os fenômenos observados.

---

## 🧪 Principais Conceitos Abordados

### 🔹 Distribuição das Frequências Naturais
- **Homogênea:** Distribuição contínua e suave.
- **Ternária:** Lacunas (band gaps) na densidade de estados, refletindo periodicidade.

### 🔹 Padrões de Modos Vibracionais
- **Baixa frequência:**
  - Homogênea → ondas suaves e estendidas.
  - Ternária → padrões modulados e alternados.
- **Alta frequência (Ternária):**
  - Modos localizados → confinamento vibracional em regiões específicas.

### 🔹 Efeito do Tamanho da Cadeia (N)
- Testado para N = 100, 1.000 e 10.000.
- Quanto maior o sistema, mais evidentes ficam os:
  - **Band gaps**
  - **Modos localizados**
  - **Modulações periódicas**

---

## ⚙️ Tecnologias Utilizadas

- `Python 3.11.7`
- `NumPy`
- `SciPy (sparse.linalg)`
- `Matplotlib`

---

## 🧠 Observação Técnica

Durante os testes com a função `eigsh()` do SciPy, observou-se que o uso de:

```python
which='SM'  # Smallest Magnitude

