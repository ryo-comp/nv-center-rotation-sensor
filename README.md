<!--
# Análise de Estados Quânticos em Sistemas de Spin: Modelagem de Qubit Aplicado como Sensor de Rotação
-->
# Hamiltoniano
A forma do Hamiltoniano de interação dos momentos de spin com o campo magnético é baseada em trabalhos experimentais de espectroscopia em núcleos, e o termo de rotação baseia-se em resultados de interferometria de nêutrons e sistemas rotativos:$$H_{\text{magnético}} = H_{\text{elétron}} + H_{\text{núcleo}} + H_{\text{rotação}} + H_{\text{hiperfino}}$$Onde os termos individuais são definidos como:$$H_{\text{elétron}} = D (S_z)^2 + \gamma_e B_0 S_z, \quad H_{\text{núcleo}} = Q (I_z)^2 + \frac{f_{DQ}}{2.0} I_z, \quad H_{\text{rotação}} = -\mathbf{\Omega}_{\text{rotação}} \cdot \mathbf{I}$$$$H_{\text{hiperfino}} = \mathbf{S} \cdot \mathbf{A} \cdot \mathbf{I} = A_z S_z I_z + A_{\perp,z}(S_x I_x + S_y I_y)$$

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
