# Avaliação de Modelos: Preditivos & Descritivos

**INTRODUÇÃO**

_O que é Análise de Dados_?

A **análise de dados** é um processo de inspeção, limpeza, transformação e [modelagem de](https://pt.wikipedia.org/wiki/Modelagem_de_dados) [dados](https://pt.wikipedia.org/wiki/Dados) com o objetivo de descobrir informações úteis, informar conclusões e apoiar a tomada de decisões. A análise de dados tem múltiplas facetas e abordagens, abrangendo diversas técnicas sob uma variedade de nomes, e é usada em diferentes domínios dos negócios, ciências e ciências sociais. No mundo dos negócios de hoje, a análise de dados desempenha um papel tornando a tomada de decisões mais científicas e ajudando as empresas a operar com mais eficácia.

A [mineração de dados](https://pt.wikipedia.org/wiki/Minera%C3%A7%C3%A3o_de_dados) é uma técnica de análise de dados específica que se concentra na modelagem estatística e na descoberta de conhecimento para fins preditivos em vez de puramente descritivos, enquanto a [inteligência de negócios](https://pt.wikipedia.org/wiki/Intelig%C3%AAncia_empresarial) cobre análises de dados que dependem fortemente da agregação, com foco principalmente nas informações de negócios. Em aplicativos estatísticos, a análise de dados pode ser dividida em [estatística descritiva](https://pt.wikipedia.org/wiki/Estat%C3%ADstica_descritiva), [análise exploratória de dados](https://pt.wikipedia.org/wiki/An%C3%A1lise_explorat%C3%B3ria_de_dados) (AED) e [análise confirmatória de dados](https://pt.wikipedia.org/wiki/Testes_de_hip%C3%B3teses) (ACD). A AED se concentra em descobrir novas características nos dados, enquanto a ACD se concentra em confirmar ou refutar [hipóteses](https://pt.wikipedia.org/wiki/Hip%C3%B3tese) existentes. A análise preditiva se concentra na aplicação de modelos estatísticos para previsão ou classificação preditiva, enquanto a [análise de texto](https://pt.wikipedia.org/wiki/Minera%C3%A7%C3%A3o_de_texto) aplica técnicas estatísticas, linguísticas e estruturais para extrair e classificar informações de fontes textuais, um tipo de dados não estruturados. Todos os itens acima são variedades de análise de dados.

A integração de dados é um precursor da análise de dados, e a análise de dados está intimamente ligada à [visualização](https://pt.wikipedia.org/wiki/Visualiza%C3%A7%C3%A3o_de_dados) e disseminação de dados.

Fonte: [Análise de dados](https://pt.wikipedia.org/wiki/An%C3%A1lise_de_dados)

Na aplicação de **análise de dados**, comumente temos 4 tipos utilizados no mercado. São:

- Análise descritiva

  Como o nome diz, essa análise descreve os dados observados, de forma que eles “digam” o que aconteceu. Por vezes, é chamada de _"estatística descritiva"_, já que é comum utilizar métodos da estatística nesse tipo.

  Por exemplo, você pode descrever os acessos ao seu site de vendas, no intervalo de uma hora, pela [média](https://pt.wikipedia.org/wiki/M%C3%A9dia) de usuários que visitaram o site nesse mesmo intervalo de tempo. A média é um conceito emprestado da estatística, bastante útil para descrever dados.

  A análise descritiva é, portanto, o tipo de análise mais simples e rápida de executar, pois emprega apenas cálculos padronizados (que podem ser automatizados), como a média, [variância](https://pt.wikipedia.org/wiki/Vari%C3%A2ncia), entre outros, além de [gráficos](https://pt.wikipedia.org/wiki/Gr%C3%A1fico), [diagramas](https://pt.wikipedia.org/wiki/Diagrama) e etc.

  Essas visualizações, originadas da análise descritiva, são a principal matéria-prima dos dashboards de indicadores-chave de desempenho (em Inglês, Key Performance Indicator ou apenas [KPI](https://pt.wikipedia.org/wiki/Indicador-chave_de_desempenho)).
   <br><br>

- Análise diagnóstica

  Conhecidas as características dos dados, imediatamente vem a pergunta: qual a causa desses dados? A resposta a essa pergunta é justamente o objetivo da análise diagnóstica.

  Porém, realizar esse passo extra não é simples, pois ele se relaciona com a dinâmica subjacente aos dados, frequentemente não acessível. Por exemplo, o fato de você observar 1000 usuários, em média, acessando seu site no intervalo de uma hora, pode estar relacionado com a depreciação média do produto que você vende, com a quantidade de concorrentes, com seu programa de fidelidade, fenômenos sociais e etc.

  Para mensurar esses “possíveis” relacionamentos, precisamos novamente emprestar métodos da estatística, como os [testes de hipótese](https://pt.wikipedia.org/wiki/Testes_de_hip%C3%B3teses), além do [método científico](https://pt.wikipedia.org/wiki/M%C3%A9todo_cient%C3%ADfico). O [teste A/B](https://pt.wikipedia.org/wiki/Teste_A/B), por exemplo, é bastante conhecido: consiste em expor a dinâmica subjacente aos dados a cenários controlados.

  Por exemplo, você pode oferecer o programa de fidelidade para alguns usuários (cenário A), mas não para outros (cenário B), e comparar a média de acessos. Além de ser trabalhoso fazer isso, há situações que não podem ser controladas, como a quantidade de concorrentes e a depreciação média do produto.

  É nesse cenário que surge o bordão "~[correlação](https://pt.wikipedia.org/wiki/Correla%C3%A7%C3%A3o) não implica causalidade": correlação é uma característica dos dados (uma métrica de associação, por assim dizer). Mas ela não pode ser imediatamente associada a uma causa, sem uma análise diagnóstica adequada, que envolve a manipulação de cenários controlados.
   <br><br>

- Análise preditiva

  Se entendemos a dinâmica subjacente aos dados, possivelmente seremos também capazes de fazer previsões. E esse é o objetivo da análise preditiva.

  Para isso, precisamos abstrair do que aconteceu e pensar no que poderia acontecer, relacionando as causas e os efeitos (dados). Chamamos isso de "modelo" e ao processo de encontrá-lo, "modelagem".

  Suponha, por exemplo, que seus dados permitam a afirmação de que a quantidade média de visitantes do site, no período de uma hora, depende linearmente do custo de cada ponto do programa de fidelidade. A palavra-chave, nesse exemplo, é o termo "linearmente" (nesse caso, se diz que o modelo é linear).

  Ele indica que um acréscimo de, digamos 30% no custo de um ponto, implica decréscimo de 30% na quantidade média de visitantes, no mesmo intervalo de tempo.

  Perceba que essa afirmação não se refere mais ao conjunto de dados originais, mas sim a uma situação hipotética genérica. Assim, é essa qualidade que nos permite fazer previsões.

  Um exemplo bem conhecido de análise preditiva é aquela que os bancos fazem ao identificar riscos de investimento, quando o empréstimo efetivamente não foi feito, mas o modelo desenvolvido pelo banco é capaz de prever o resultado.

  Contudo, essa previsão nem sempre se concretiza. Grande parte do trabalho do analista de dados é justamente otimizar essa incerteza.
   <br><br>

- Análise prescritiva

  Agora que sabemos descrever os dados, entendemos o porquê de eles apresentarem essas características, criarmos uma representação abstrata deles, capaz de prever um cenário hipotético, podemos então pensar no processo inverso e introduzir objetivos a serem alcançados.

  Suponha que estejamos no final de uma campanha de marketing, na qual é preciso aumentar 15% a quantidade média de visitas no site. Como sabemos que essa quantidade se relaciona linearmente com o custo de um ponto de fidelidade, podemos optar por reduzir o custo em 15%. Isso é uma prescrição do que fazer, com base na modelagem e nos objetivos a serem atingidos.

  Outro exemplo, fora do mundo dos negócios, é o dos sistemas de controle da SpaceX, que analisam continuamente o movimento do foguete, para prescrever ações de seu motor. Este trabalho tem o objetivo de trazê-lo em segurança para o solo.

  Essa é a análise prescritiva e, como você já deduziu, é a etapa mais complexa, pois demanda conhecimento profundo sobre o sistema.
  
  
Para atividade prática, de **Avaliação de Modelos: Preditivos & Descritivos**, iremos utilizar o `Python` e o `R` no ambiente do _jupyter notebook_.
