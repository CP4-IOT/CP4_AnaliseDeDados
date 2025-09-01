# CP4 Análise de Dados de Consumidores de Energia
Repositório para realização da atividade do cp4 na disciplina de IoT.

## Alunos
-  Gustavo de Aguiar Lima Silva  -  RM557707
-  Julio Cesar Conceição Rodrigues -  RM557298
-  Matheus de Freitas Silva -  RM552602
 
---

## ORIENTAÇÕES GERAIS:

- Link dos datasets:
- Questão 1 a 25: https://fiapcom-my.sharepoint.com/:t:/g/personal/pf1745_fiap_com_br/EYxjAa7H-8FBtku44iW24e4BmYU_XszbVi32oyLGJYodOg?e=w1A4ob
- Questão 26 a 40: https://archive.ics.uci.edu/dataset/374/appliances+energy+prediction
- Ao rodar o notebook no colab, upar os arquivos para manipulação dos dados.

---
## DESCRIÇÃO:

Este notebook utiliza dois datasets relacionados ao consumo de energia elétrica:

Individual Household Electric Power Consumption

Nome do arquivo: household_power_consumption.txt
Descrição: Este dataset contém medições horárias de consumo de energia elétrica de um único domicílio na França ao longo de quase quatro anos (dezembro de 2006 a novembro de 2010).
Conteúdo: As colunas incluem data, hora e várias métricas de consumo e medição, como Global_active_power, Global_reactive_power, Voltage, Global_intensity, Sub_metering_1, Sub_metering_2 e Sub_metering_3.
Observações da Análise: Durante a análise, foram identificados valores ausentes, particularmente na coluna Sub_metering_3. A coluna Date foi convertida para o tipo datetime para análise temporal. A análise exploratória revelou padrões de consumo diário e sazonalidade.
Energy Data Complete

Nome do arquivo: energydata_complete.csv
Descrição: Este dataset contém medições a cada 10 minutos de consumo de energia de eletrodomésticos (Appliances) e luzes (lights), juntamente com várias variáveis de temperatura e umidade em diferentes cômodos da casa e condições meteorológicas externas. Os dados cobrem um período de janeiro a maio de 2016.
Conteúdo: As colunas incluem date, Appliances (consumo em Wh), lights (consumo em Wh), temperaturas e umidades internas (T1 a T9, RH_1 a RH_9), e variáveis meteorológicas externas (T_out, RH_out, Press_mm_hg, Windspeed, Visibility, Tdewpoint).
Observações da Análise: Este dataset não apresentou valores ausentes nas colunas principais utilizadas. A análise exploratória mostrou que o consumo de Appliances tende a se concentrar em valores baixos com alguns picos. Foram exploradas as correlações entre Appliances e variáveis ambientais, e a normalização dos dados foi aplicada para modelagem. O clustering com K-Means em Appliances e lights revelou padrões distintos de consumo.

