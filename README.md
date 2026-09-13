# AURORA-01 — Sistema de Telemetria

## Sobre o projeto

O AURORA-01 é um projeto acadêmico desenvolvido para a Atividade Integradora do curso de Ciência da Computação.

O projeto simula um sistema de telemetria responsável por analisar as condições de segurança de uma nave espacial antes da decolagem.

O sistema recebe dados simulados e verifica parâmetros como:

-  Temperatura interna;
-  Temperatura externa;
-  Integridade estrutural;
-  Nível de energia;
-  Pressão dos tanques;
-  Status dos módulos críticos.

Com base nesses dados, o algoritmo determina se a nave está:

>  PRONTO PARA DECOLAR

ou

>  DECOLAGEM ABORTADA

---

##  Funcionamento

Para autorizar a decolagem, todos os parâmetros precisam estar dentro das condições de segurança definidas para a simulação.

| Parâmetro | Condição segura |
|---|---|
| Temperatura interna | 18 °C a 30 °C |
| Temperatura externa | -120 °C a 0 °C |
| Integridade estrutural | 1 |
| Nível de energia | ≥ 70% |
| Pressão dos tanques | ≥ 80% |
| Módulo crítico | OK |

Os valores utilizados são simulados e foram definidos exclusivamente para fins acadêmicos.

---

##  Tecnologias utilizadas

- Python
- Jupyter Notebook
- Visual Studio Code
- Git
- GitHub

---

##  Análise energética

A simulação considera uma capacidade energética total de **500 kWh**.

A nave inicia com **87% de carga**, correspondendo a:

**500 × 0,87 = 435 kWh**

Considerando um consumo estimado de **120 kWh** durante a decolagem e perdas energéticas de **10%**, o consumo efetivo é:

**120 + 12 = 132 kWh**

Energia restante:

**435 - 132 = 303 kWh**

Isso corresponde a aproximadamente **60,6% da capacidade total** após a decolagem.

---

##  Análise assistida por IA

A análise dos dados permite classificar os parâmetros como normais ou anômalos e identificar possíveis riscos.

No cenário de teste, foram simuladas condições de risco:

- Temperatura interna: **34 °C**
- Energia: **62%**
- Pressão dos tanques: **76%**

Esses valores estão fora dos limites definidos, fazendo com que o sistema determine:

>  DECOLAGEM ABORTADA

Como medidas de segurança, recomenda-se verificar o sistema térmico, recarregar os sistemas de energia, verificar a pressurização e realizar uma nova leitura da telemetria antes de autorizar a decolagem.

---

##  Reflexão crítica

Sistemas automatizados podem aumentar a segurança de uma missão espacial ao identificar rapidamente situações de risco. Entretanto, decisões relacionadas à segurança não devem depender exclusivamente de sistemas automatizados.

É necessário manter procedimentos de validação, supervisão humana e mecanismos de segurança capazes de interromper uma operação em caso de falhas ou informações inconsistentes.

A exploração espacial também pode proporcionar avanços científicos e tecnológicos, mas envolve custos elevados e impactos ambientais relacionados à fabricação de equipamentos, consumo energético e lançamentos.

Por isso, o desenvolvimento tecnológico deve considerar princípios de responsabilidade, segurança e sustentabilidade.

---

##  Como executar

### 1. Clonar o repositório

```bash
git clone https://github.com/RaulGDev1/projetopythonfiap.git
