# Planilha de Planejamento de Investimentos em FIIs

## Sobre o projeto

Esta planilha foi criada para ajudar no planejamento de investimentos em Fundos de Investimento Imobiliário (FIIs), permitindo simular o crescimento do patrimônio ao longo do tempo, estimar possíveis rendimentos mensais e organizar a distribuição dos aportes entre diferentes tipos de fundos.

O objetivo é tornar o planejamento financeiro mais simples e visual, permitindo ajustar os valores de acordo com a realidade e os objetivos de cada investidor.

## Funcionalidades

### 1. Configurações

Nesta seção, ficam algumas informações utilizadas como base para os cálculos da planilha.

- **Salário:** permite informar a renda mensal utilizada como referência para o planejamento.
- **Rendimento da carteira:** define a taxa mensal estimada de rendimento utilizada para calcular os possíveis dividendos.
- **Sugestão de investimento:** calcula automaticamente 30% do salário informado, servindo como referência de quanto poderia ser destinado aos investimentos.

### 2. Simulação de investimento mensal

Esta seção permite calcular quanto o patrimônio pode crescer com aportes mensais ao longo de um período determinado.

- **Quanto investir por mês?** valor que será aplicado mensalmente.
- **Por quantos anos investir?** período durante o qual os aportes serão realizados.
- **Taxa de rendimento mensal:** percentual de rentabilidade mensal utilizado na simulação.
- **Patrimônio acumulado:** estima o valor acumulado ao final do período, considerando os aportes mensais e a taxa informada.
- **Dividendos mensais:** estima quanto o patrimônio acumulado poderia gerar mensalmente, utilizando o percentual de rendimento definido nas configurações.

Os campos calculados são atualizados automaticamente quando os valores utilizados nas fórmulas são alterados.

### 3. Cenários de investimento

Esta seção permite comparar diferentes períodos de investimento: 2, 5, 10, 20 e 30 anos.

Para cada período, a planilha apresenta:

- **Patrimônio estimado:** valor que poderá ser acumulado com os aportes mensais e a rentabilidade informada.
- **Dividendos estimados:** possível rendimento mensal calculado com base no percentual definido para a carteira.

Essa comparação ajuda a visualizar como o tempo e a regularidade dos aportes podem influenciar o crescimento do patrimônio.

### 4. Distribuição dos investimentos por perfil

Nesta seção, é possível selecionar um perfil de investimento e informar o valor que será investido mensalmente.

A planilha utiliza o perfil escolhido para sugerir uma distribuição percentual entre seis categorias de fundos imobiliários:

- **Papel:** fundos que investem principalmente em títulos e recebíveis imobiliários.
- **Tijolo:** fundos que investem em imóveis físicos, como galpões logísticos, escritórios e shoppings.
- **Híbridos:** fundos que combinam diferentes estratégias e tipos de ativos imobiliários.
- **FOFs:** fundos que investem em cotas de outros fundos imobiliários.
- **Desenvolvimento:** fundos ligados a projetos de construção e desenvolvimento imobiliário.
- **Hotelaria:** fundos com investimentos relacionados a hotéis e empreendimentos de hospedagem.

Para cada categoria, a planilha apresenta o percentual sugerido e o valor correspondente em reais, calculado com base no aporte mensal informado.

O total dos valores distribuídos também é calculado automaticamente.

### 5. Base de parâmetros

A segunda aba da planilha contém a tabela de referência utilizada na distribuição dos investimentos.

Ela reúne os perfis disponíveis e os percentuais associados a cada categoria de FII. Esses valores são consultados automaticamente pela planilha principal de acordo com o perfil selecionado.

Os perfis disponíveis são:

- **Conservador**
- **Moderado**
- **Agressivo**

Essa estrutura permite alterar os percentuais de referência e adaptar as sugestões de distribuição, desde que os dados e as fórmulas sejam mantidos corretamente.

## Como utilizar

1. Abra a planilha no Microsoft Excel ou em um programa compatível.
2. Informe o salário e ajuste as premissas de rendimento nas configurações.
3. Defina o valor do aporte mensal, o prazo de investimento e a taxa de rendimento desejada.
4. Consulte os cenários para comparar os resultados estimados em diferentes períodos.
5. Escolha um perfil de investimento e informe o valor mensal que deseja distribuir entre as categorias de FIIs.
6. Consulte os percentuais sugeridos e os valores calculados para cada categoria.

Os resultados dependem dos valores informados e das fórmulas existentes na planilha.

## Observações importantes

Esta planilha é uma ferramenta de simulação e organização financeira. Os valores apresentados são estimativas matemáticas, não garantias de rentabilidade ou de recebimento de dividendos.

As simulações consideram taxas constantes e aportes regulares, sem representar todas as condições reais do mercado. Na prática, os rendimentos dos FIIs podem variar, e o patrimônio pode sofrer oscilações.

Os perfis e percentuais de distribuição são parâmetros editáveis da planilha, não recomendações personalizadas de investimento. Antes de investir, é importante avaliar os riscos, os custos e as características de cada fundo.

## Fórmulas e lógica de funcionamento

A planilha utiliza funções do Excel para automatizar cálculos, consultar parâmetros e simular o crescimento dos investimentos. Duas funções importantes nesse processo são `PROCV` e `VF`.

### PROCV — Busca de informações

A função `PROCV` procura uma informação em uma tabela e retorna um valor relacionado a ela.

Nesta planilha, ela permite consultar os parâmetros associados ao perfil de investimento selecionado, recuperando os percentuais definidos para cada categoria de FII.

Por exemplo, ao selecionar o perfil **Moderado**, a fórmula pode buscar na aba de parâmetros os percentuais correspondentes e utilizá-los para calcular como o aporte mensal será distribuído entre as categorias de fundos imobiliários.

Isso evita a necessidade de preencher os percentuais manualmente em cada campo e facilita a manutenção das informações.

### VF — Valor Futuro

A função `VF` calcula o valor futuro de um investimento considerando uma taxa de juros, um número de períodos e pagamentos periódicos.

Na planilha, ela é utilizada para simular quanto o patrimônio pode acumular ao longo do tempo a partir de aportes mensais e de uma taxa de rendimento definida.

Por exemplo, é possível informar quanto será investido por mês, durante quantos anos os aportes serão realizados e qual será a taxa mensal estimada. Com esses dados, a função calcula o valor futuro projetado para o investimento.

Essa função permite comparar diferentes prazos e valores de aporte, ajudando a visualizar como a regularidade dos investimentos e o tempo podem influenciar o patrimônio acumulado.

É importante lembrar que o resultado é uma simulação matemática baseada em uma taxa constante. Na prática, os rendimentos dos fundos imobiliários variam e não são garantidos.

### Por que utilizar essas funções?

- **Automatização:** os cálculos são atualizados quando os valores de entrada são alterados.
- **Consistência:** os parâmetros são consultados em uma tabela centralizada.
- **Facilidade de manutenção:** é possível ajustar os percentuais de referência sem precisar modificar manualmente todos os campos relacionados.
- **Simulação financeira:** a função `VF` permite estimar o patrimônio futuro a partir de aportes periódicos e de uma taxa de rendimento definida.

Em conjunto, essas funções ajudam a tornar a planilha mais prática, organizada e fácil de utilizar.

## Tecnologias utilizadas

- Microsoft Excel
- Fórmulas financeiras e referências entre abas
- Tabelas de parâmetros para distribuição percentual

## Objetivo do projeto

Desenvolver uma ferramenta prática para apoiar o planejamento de investimentos, facilitar a visualização de cenários futuros e demonstrar como o Excel pode ser utilizado na organização financeira pessoal.

---

**Desenvolvido por Construx Empreendimentos.**

