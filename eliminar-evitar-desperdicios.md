# Como evitar e eliminar Desperdícios em um projeto de automação?

Bom, quando possuímos um cenário onde a empresa opta por ter um projeto de automação, a primeira coisa que pensa é em quantos Especialistas ou Engenheiros em automação serão necessários para esse projeto e acabamos por ter vários QAs no time e mais um monte de "Messias" em automação que não vão conseguir resolver o problema, vai causar um turnover na equipe, seja por insatisfação (porque o QA manual não vai conseguir ir pra esse projeto, e o automatizador vai uma hora ou outra ter que ajudar na demanda manual). Dado esse cenário, sugiro que tragam uma pessoa com skill de automação de testes e quando esse profissional chegar, temos algumas coisas que podemos fazer para agilizar o processo e o primeiro deles é identificar os fatores que geram desperdício, então segue algumas ações que devemos fazer para iniciar um projeto desses:

## Reunir os QAs + Gestor + Dev para uma retrospectiva

Quando sabemos da existência desse projeto, uma ação interessante é reunir todos os QAs, porque todos vão ter participação (veremos isso) e o ideal é que o stakeholder, com pelo menos alguma pessoa que possa ser o porta voz do time de dev (tech lead é uma boa) possa participar, porque será nessa reunião que as expectativas **DEVEM** ser colocadas a mesa para que as ações que iremos tomar possam ser de conhecimento de todos. Primeira expectativa, deixar claro o objetivo se ter testes automatizados, assim como deixar claro que todos que vão participar não são especialistas em automação de testes e que uma hora ou outa, a equipe de desenvolvimento vai ser "parada" para remover algum impedimento técnico com relação a linguagem em questão. 
Nessa retrospectiva, vamos alinhar alguns pontos:

1. _**Fazer uma triagem do que pode estar errado**_

Pontuar as causas que levaram a não automatizar os testes ou alguns dos testes do início até agora.

Fazer isso em um modelo de retrospectiva ajuda para que o time inteiro possa saber onde estão os problemas que levaram a decisão de não automatizar, e podemos ver que as vezes são processos burocráticos na própria empresa que dificultou essa cultura de testes ser melhor. Coloque todos os itens escritos em post its para que possamos discutí-los e encontrar formas de melhorar nosso fluxo de trabalho.

2. _**Eliminar processos que não agregam valor**_

Eu já trabalhei em equipes de qualidade onde cada QA estava em um time de desenvolvimento e mesmo assim insistia em fazer uma reunião diária, que levava mais de 20 minutos porque tinham muitos QAs falando, a grande maioria dispersa e se em uma daily estamos dispersos ou não entendemos o propósito da reunião ou ela não agrega valor para mim, e no meu caso, ela não agregava valor, pois eu tinha uma daily de 15 a 20 minutos no time (que fazia todo o sentido) e depois uma daily com o time de QA, e nessa brincadeira se vai quase 1 hora do meu dia de 8 horas úteis.

Outro exemplo é quando você é chamado para uma reunião que não faz sentido algum, como por exemplo, reunião para marcar reunião (isso é uma história real).

O que quero dizer é que todo processo que seja burocrático, que demanda tempo do profissional e que não agrega valor, **DEVE** ser eliminado para que o projeto da automação venha a fazer sentido e possa agregar valor para a empresa.

## Reunir apenas os QAs e alguém da área de produtos para um bate papo (Timebox de 45 minutos pelo menos)

O objetivo desse bate papo é para saber quais cenários seriam desperdícios de se automatizar ou que não teriam valor algum (acreditem, existem cenários que não vale a pena automatizar). E também no modelo de retrospectiva, um modelo interessante para a reunião fluir é deixar o quadro no padrão happiness canvas e pedir para cada um colocar na sua percepção quais cenários seriam de maior valor, de um valor médio e de pequeno valor:

```ruby
|         =)         |        =(            |
| Cadastro de usr    |  Fluxos de Login     |
| Pagamento          |  Reativação de usr   |
```

Coloquei exemplos bem toscos ta, mas pensa no seguinte, temos um produto a anos, funcionando, com seus bugs é verdade, mas quantas vezes se queixaram que não conseguiam logar, ou com qual frequência reativamos clientes?? Diferente de Cadastro e Pagamento, que se parar de funcionar, nós como empresa perdemos dinheiro.

Mapear e deixar de lado por enquanto.

## Bugs vindos de produção devemos parar e automatizar

Essa é uma forma de eliminar desperdício, pois dado que não tivemos condição de prever que esse bug iria acontecer antes de entrar em produção, devemos agora garantir que nunca mais irá ocorrer e isso quer dizer que devemos simular o problema e automatizar.

## Mudança de mindset

Ter uma mudança de mindset muitas vezes não é fácil, mas dia após dia, gerando valor as coisas vão acontecendo, então sugiro que após as dicas acima serem feitas, um próximo passo será trabalhar com [antecipação de problemas.](https://github.com/thiagomarquessp/lean-em-projetos-automacao/blob/master/antecipar-problemas.md)

[Home](https://github.com/thiagomarquessp/lean-em-projetos-automacao/blob/master/README.md)
