<!--
# Análise de Estados Quânticos em Sistemas de Spin: Modelagem de Qubit Aplicado como Sensor de Rotação
-->
# Hamiltoniano

## Fundamentação Teórica e Modelagem

A forma do Hamiltoniano de interação dos momentos de spin com o campo magnético é baseada em trabalhos experimentais de espectroscopia em núcleos, e o termo de rotação baseia-se em resultados de interferometria de nêutrons e sistemas rotativos:

$$
H_{\text{magnético}} = H_{\text{elétron}} + H_{\text{núcleo}} + H_{\text{rotação}} + H_{\text{hiperfino}}
$$

Onde:

$$
H_{\text{elétron}} = D (S_z)^2 + \gamma_e B_0 S_z
$$
$$
H_{\text{núcleo}} = Q (I_z)^2 + \frac{f_{DQ}}{2.0} I_z
$$
$$
H_{\text{rotação}} = -\mathbf{\Omega}_{\text{rotação}} \cdot \mathbf{I}
$$
$$
H_{\text{hiperfino}} = \mathbf{S} \cdot \mathbf{A} \cdot \mathbf{I} = A_z S_z I_z + A_{\perp,z}(S_x I_x + S_y I_y)
$$

### Pulsos de Radiofrequência (RF)

Os pulsos $P$ são modelados como senoides, 

$$
$g(t, f) = A \cos(2 \pi f t)$, 
$$

e o fator de desdobramento $f_{DQ}$ é definido como:

$$
f_{\text{DQ}} = 2 B_0 \gamma_{\text{n}} \left( 1 - \frac{\gamma_{\text{e}} A_{\perp}^2}{\gamma_{\text{n}} (D^2 - \gamma_{\text{e}}^2 B_0^2)} \right).
$$

Os pulsos são modelados como:

$$
P_{\pi/2}(t) = g(t,Q - \frac{f_{DQ}}{2})
$$
$$
P_{\pi/\sqrt{2}} = g(t,Q - \frac{f_{DQ}}{2}) + g(t,Q + \frac{f_{DQ}}{2})
$$

### Parâmetros da Simulação

| Parâmetro | Valor | Descrição |
| :--- | :--- | :--- |
| $Q$ | $-4,94$ MHz | Interação quadrupolar nuclear |
| $D$ | $2870,0$ MHz | Desdobramento em campo zero (Zero-field splitting) |
| $\gamma_e$ | $28024,9$ MHz/Tesla | Razão giromagnética do eletrão |
| $\gamma_n$ | $3,077$ MHz/Tesla | Razão giromagnética do núcleo de $^{14}\text{N}$ |
| $A_{\perp}$ | $2,7$ MHz | Constante hiperfina magnética transversa |
| $A_z$ | $-2,14$ MHz | Componente longitudinal da constante hiperfina |
| $B_0$ | $482$ Gauss | Campo magnético estático |

---
*Este projeto utiliza o framework **QuTiP** para a simulação da dinâmica quântica.*
[Link para o Notebook no Google Colab](https://colab.research.google.com/github/ryo-comp/nv-center-rotation-sensor/blob/main/seu_notebook.ipynb)


# Estudo de QuTiP e QS

<!--
Este repositório contém o código-fonte e as simulações utilizadas no artigo submetido ao **Simpósio Brasileiro de Computação Quântica (SBCCQ) 2026**. O projeto foca na modelagem de um sensor de rotação, inspirado em centros NV, controlando a população dos estados quânticos.
-->
Este repositório contém o código-fonte e as simulações para evento específico. O projeto foca na modelagem de um sensor de "***", inspirado em "---", controlando ... estados quânticos.

## Como Rodar o Projeto

Para facilitar a reprodutibilidade, o código principal pode ser executado diretamente no navegador via Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ryo-comp/nv-center-rotation-sensor/blob/main/sensorRotQuantico.ipynb)

### Pré-requisitos (Local)
Caso prefira rodar localmente, você precisará de:
- Python 3.8+
- [QuTiP](https://qutip.org/) (Quantum Toolbox in Python)
- NumPy e Matplotlib

```bash
pip install qutip numpy matplotlib
