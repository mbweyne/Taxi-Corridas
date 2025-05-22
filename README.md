![Banner do Projeto](Banner.png)
# 🚖 Projeto 7 - RideWise – Explorando Corridas de Táxi em Chicago

Este projeto tem como objetivo identificar padrões de comportamento dos passageiros da empresa de caronas **Zuber**, em **Chicago**, e verificar o impacto de fatores externos como **clima** e **localização** nas corridas.

---

## 📊 Objetivo do Projeto

- Analisar os dados de corridas de táxi por empresa e por destino.
- Identificar os bairros com maior volume de desembarque.
- Investigar o impacto do clima, especialmente nos **sábados chuvosos**, na duração das corridas entre o Loop e o Aeroporto Internacional O'Hare.

---

## 🗂 Esquema do Banco de Dados

A base de dados é composta por cinco tabelas principais interligadas, conforme o esquema a seguir:

![Esquema do Banco de Dados](Banner.png)

### Tabelas:

#### `trips`
- `trip_id`: ID da corrida
- `cab_id`: táxi responsável
- `start_ts`, `end_ts`: horários da corrida
- `duration_seconds`: duração
- `distance_miles`: distância
- `pickup_location_id`, `dropoff_location_id`: locais de origem e destino

#### `cabs`
- `cab_id`: ID do táxi
- `vehicle_id`: ID do veículo
- `company_name`: empresa de táxi

#### `neighborhoods`
- `neighborhood_id`: ID do bairro
- `name`: nome do bairro

#### `weather_records`
- `record_id`: ID do registro climático
- `ts`: data/hora do registro
- `description`: condição do clima
- `temperature`: temperatura

---

## 🧪 Etapas do Projeto

### 📌 Etapa 1: Análise Exploratória de Dados
- Visualização do número de corridas por empresa
- Identificação dos 10 bairros com maior média de corridas
- Criação de gráficos para apoiar as análises

### 📌 Etapa 2: Teste de Hipótese
**Hipótese:**  
> "A duração média das corridas do Loop para o Aeroporto O'Hare é diferente aos sábados chuvosos."

**Etapas executadas:**
- Filtragem das corridas de sábado
- Identificação de corridas em dias chuvosos
- Aplicação do **Teste de Mann-Whitney** para comparação de médias

---

## 📌 Tecnologias Utilizadas

![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white&style=flat)
![Pandas](https://img.shields.io/badge/-Pandas-150458?logo=pandas&logoColor=white&style=flat)
![Matplotlib](https://img.shields.io/badge/-Matplotlib-11557C?logo=matplotlib&logoColor=white&style=flat)
![SciPy](https://img.shields.io/badge/-SciPy-8CAAE6?logo=scipy&logoColor=white&style=flat)

---

## 📈 Resultados e Conclusões

- Identificamos as empresas com maior volume de corridas e os bairros mais movimentados de Chicago.
- O clima impacta sim a duração média das corridas nos sábados, segundo o teste estatístico.
- As análises ajudam a Zuber a tomar decisões estratégicas sobre alocação de recursos e campanhas promocionais.

---

## 👩‍💻 Desenvolvido por

**Marcia Bayardino Weyne**  
[Cientista de Dados em Transição de Carreira](https://www.linkedin.com/in/marcia-bayardino-weyne)  
📫 mbweyne@gmail.com  
🌐 [GitHub](https://github.com/mbweyne)

