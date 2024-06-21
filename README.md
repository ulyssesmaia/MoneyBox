<h1>MoneyBox </h1> 

<p align="center">
  <img src="https://img.shields.io/static/v1?label=react&message=framework&color=blue&style=for-the-badge&logo=REACT"/>
  <img src="https://img.shields.io/static/v1?label=Netlify&message=deploy&color=blue&style=for-the-badge&logo=netlify"/>
  <img src="http://img.shields.io/static/v1?label=License&message=MIT&color=green&style=for-the-badge"/>
  <img src="http://img.shields.io/static/v1?label=Ruby&message=2.6.3&color=red&style=for-the-badge&logo=ruby"/>
  <img src="http://img.shields.io/static/v1?label=Ruby%20On%20Rails%20&message=6.0.2.2&color=red&style=for-the-badge&logo=ruby"/>
  <img src="http://img.shields.io/static/v1?label=TESTES&message=%3E100&color=GREEN&style=for-the-badge"/>
   <img src="http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=RED&style=for-the-badge"/>
   <img src="http://img.shields.io/static/v1?label=STATUS&message=CONCLUIDO&color=GREEN&style=for-the-badge"/>
</p>

### Tópicos 

:small_blue_diamond: [Descrição do projeto](#descrição-do-projeto)

:small_blue_diamond: [Funcionalidades Faseadas](#funcionalidades-faseadas)

:small_blue_diamond: [Layout do Projeto](#layout)

🔹[Jornada do Cliente](#Jornada_Cliente)

🔹[Tabelas IUC](#Tabelas_IUC)

🔹[Parcelamento](#Parcelamento)

:small_blue_diamond: [Pré-requisitos](#pré-requisitos)


... 

## Descrição do projeto 

<p align="justify">
  Projeto surgiu como uma solução webbased de organização financeira através de uma plataforma que permite ao usuário o pagamento do IUC de viaturas, de motas à aviões, parcelando antecipadamente o pagamento       para evitar que assim seja necessário o pagamento de caumo por atraso no pagamento, pelo fato da plataforma ficar responsável pelo seu pagamento. A plataforma permite o parcelamento em ate 12 vezes do valor do IUC de acordo com o prazo de pagamento do mesmo, com a cobrança de uma taxa de administração.
</p>

O que é o IUC?
</p>
O IUC é um imposto anual que incide sobre a propriedade de um veículo (e não sobre a circulação), pago até a matrícula ser cancelada, cujos valores são actualizados por norma todos os anos em Janeiro.</p>
No caso dos automóveis, é o imposto que substitui o antigo "selo do carro" ou "selo automóvel" e não deve ser confundido com o ISV, que é um imposto pago apenas quando o veículo é matriculado pela primeira vez em Portugal.
</p>

## Funcionalidades-Faseadas 

</p>
:heavy_check_mark: Fase 1 - Reconstrução
</p>
- Arquitetura da Solução
- Cálculo dos valores do IUC no ano
- Reconstrução do Backoffice atual
</p>
:heavy_check_mark: Aprimoramento Tecnológico
</p>
- Integração base de dados matrículas

- Integração bancária para autorizações de pagamento

- Integração consultas matrículas

- Integração com CRM
</p>

## Layout

</p>
💻 Layout Interface cálculo
O layout a ser seguido atualmente se baseia no site https://www.moneybox.pt

</p>
💻 Layout Interface Backoffice
O layout atual se baseará em nos conteúdos dos formulários e tabelas:
- Dados formulários:
    - Cadastro Clientes
    - Cadastro veículos
    - Relatório Financeiro
          - Vendas Mês
          - Categorias
- Tabelas:
    - [Tabelas_IUC](#Tabelas_IUC)
</p>

## Jornada_Cliente

**Direcionamento Site -» Área Cliente**
<img src="Fluxo Cadastro.png" alt="Jornada do Cliente">

**Direcionamento Site -» Área Cliente**
<img src="Fluxo Area Cliente.png" alt="Fluxo Área Cliente">

## Pré-requisitos

:warning: [Node](https://nodejs.org/en/download/)

Mínimo possíveis

## Tabelas_IUC
</p>
A primeira forma de cálculo, com base no combustível, cilindrada e ano da matrícula, por escalões, aplica-se aos veículos matriculados pela primeira vez em Portugal ou num país da UE/EEE até 30 de Junho de 2007. Tecnicamente, segundo o Código do IUC, estes veículos estão enquadrados na categoria A.</p>
A segunda forma de cálculo, com base no combustível, ano da matrícula, cilindrada e emissões de CO2, por escalões, aplica-se aos veículos matriculados em Portugal, na UE ou no EEE a partir de 1 de Julho de 2007, e aos veículos cuja matrícula portuguesa seja a partir de 1 de Julho de 2007 mas cuja primeira matrícula foi num país fora da UE + EEE. Estes veículos pertencem à categoria B do Código do IUC.
</p>
Primeira matrícula PT/UE/EEE de 1981 a Junho-07

|Cilindrada (cm3)|Matrícula de 96 a Junho-07|Matrícula de 90 a 95|Matrícula de 81 a 89|
| :--------: | :--------: | :--------: | :--------: |
|Até 1.000|19,90€|12,20€|Isento|
|1.001 a 1.300|39,95€|22,45€|12,55€|
|1.301 a 1.750|62,40€|34,87€|17,49€|
|1.751 a 2.600|158,31€|83,49€|36,09€|
|2.601 a 3.500|287,49€|156,54|79,72€|
|Mais de 3.500|512,23€|263,11€|120,90€|

Gasóleo com primeira matrícula PT/UE/EEE de 1981 a Junho de 2007
|Cilindrada (cm3)|Matrícula de 96 a Junho-07|Matrícula de 90 a 95|Matrícula de 81 a 89|
| :--------: | :--------: | :--------: | :--------: |
|Até 1.500|22,48€|14,18€|10,19€|
|1.501 a 2.000|45,13€|25,37€|14,18€|
|2.001 a 3.000|70,50€|39,40€|19,76€|
|Mais de 3.000|178,86€|94,33€|40,77€|

Eléctricos com primeira matrícula PT/UE/EEE de 1981 a Junho de 2007
|Voltagem total|Matrícula de 96 a Junho-07|Matrícula de 90 a 95|Matrícula de 1981 a 1989|
| :--------: | :--------: | :--------: | :--------: |
|Até 100|19,90€|12,55€|Isento|
|Mais de 100|39,95€|22,45€|12,55€|

````Veículos com primeira matrícula a partir de 1 de Julho de 2007 (inclusive) e importados usados de fora da UE/EEE a partir de 1 de Julho de 2007````

**Passo 1**: a tabela da cilindrada é aplicada de forma igual a automóveis a gasolina e a gasóleo (ou qualquer outro combustível). Veja em qual dos quatro escalões se insere o veículo.

À partir de Julho-07
|Cilindrada (cm3)|Taxa|
| :--------: | :--------: |
|Até 1.250|31,77€|
|1.251 a 1.750|63,74€|
|1.751 a 2.500|127,35€|
|Mais de 2.500|435,84€|

**Passo 2**: à taxa da cilindrada deve agora somar a taxa das emissões de CO2, mais uma vez, o valor é o mesmo para gasolina e gasóleo. Nos veículos com primeira matrícula PT/UE/EEE a partir de 2017 terá que somar o valor das duas colunas, da taxa e da taxa adicional. Em 2020 a tabela foi dividida em escalões diferentes consoante o método de homologação das emissões de CO2: NEDC ou WLTP.

Relembro: todos os automóveis novos vendidos entre 2018 e 2019 poderão ser NEDC ou WLTP, foi um período de transição onde as duas normas conviveram - para saber com certeza se um automóvel é NEDC ou WLTP tem que consultar a documentação do carro (DUA, COC, manual, etc.).

De forma geral, podendo haver excepções:

automóveis novos vendidos até 2017 são NEDC
automóveis novos vendidos em 2018 e 2019 podem ser NEDC ou WLTP
automóveis novos vendidos em 2018 são maioritariamente NEDC
automóveis novos vendidos em 2019 são maioritariamente WLTP
qualquer automóvel novo vendido a partir de 2020 é WLTP

|Emissões CO2 (g/km) NEDC|Emissões CO2 (g/km) WLTP|Taxa|Taxa adicional|
| :--------: | :--------: | :--------: | :--------: |
|Até 120|Até 140|65,15€|0€|
|121 a 180|141 a 205|97,63€|0€|
|181 a 250|206 a 260|212,04€|31,77€|
|Mais de 250|Mais de 260|363,25€|63,74€|

**Passo 3**: Deve agora multiplicar o resultado da soma da taxa da cilindrada com a das emissões de CO2 pelo número (coeficiente) que aparece na seguinte tabela.
Este coeficiente é um agravamento para veículos mais recentes, ou seja, carros mais recentes pagam mais IUC.

|Ano da primeira matrícula PT/UE/EEE|	Coeficiente|
| :--------: | :--------: |
|2007|1,00|
|2008|1,05|
|2009|1,10|
|2010 e seguintes|1,15|


**Passo 4** *(gasóleo apenas)*: criou-se uma taxa adicional aquando da intervenção da troika mas que ainda está em vigor, a cobrar em todos os veículos ligeiros de passageiros a gasóleo com primeira matrícula PT/UE/EEE a partir de 1 de Julho de 2007 (inclusive).
Supostamente, é uma taxa temporária, ou seja, deixará de existir no futuro porém, ainda existe em 2024.

Tabela IUC taxa gasóleo aplicável no ano 2024
Primeira matrícula PT/UE/EEE a partir de Julho de 2007
e
Origem fora PT/UE/EEE com matrícula portuguesa a partir de Julho de 2007
impostosobreveiculos.info
Gasóleo
|Cilindrada (cm3)|Taxa Adicional|
| :--------: | :--------: |
|Até 1.250|5,02€|
|1.251 a 1.750|10,07€|
|1.751 a 2.500|20,12€|
|Mais de 2.500|68,85€|

**Veículos comerciais de transporte particular com peso bruto inferior a 12t**
Esta é a tabela de IUC para 2024 dos veículos de transporte particular com peso bruto inferior a 12t (categoria C). Esta tabela é independente do ano da matrícula.

|Peso Bruto (kg)|	Taxa
| :--------: | :--------: |
|Até 2.500|35,15€
|2.501 a 3.500|58,21€
|3.501 a 7.500|139,47€
|7.501 a 11.999|226,24€

**Motociclos, ciclomotores, triciclos e quadriciclos**

|Cilindrada (cm3)|Matrícula de 97 a 24|Matrícula de 92 a 96
| :--------: | :--------: | :--------: |
|Até 119|Isento|Isento
|120 a 250|Isento|Isento
|251 a 350|Isento|Isento
|351 a 500|21,18€|12,53€
|501 a 750|63,62€|37,47€
|Mais de 750|138,15€|67,76€

## Parcelamento
1x custo fixo de €12 de comissão

2x custo fixo de €14 de comissão

4x custo fixo de €16 de comissão

12x custo fixo de €18 de comissão

## Tarefas em aberto

Se for o caso, liste tarefas/funcionalidades que ainda precisam ser implementadas na sua aplicação

:memo: Tarefa 1 

:memo: Tarefa 2 

:memo: Tarefa 3 
