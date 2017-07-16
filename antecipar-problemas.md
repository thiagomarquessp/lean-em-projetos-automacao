# Antecipando problemas e não mais "achando problemas"

Nossa vida começa agora, com a nossa mudança de mindset, e temos que colocar na nossa cabeça que **QA deve antecipar e prevenir problemas e não achar bugs** e outro detalhe, ficar feliz com bug encontrado é **NOJENTO**, eu tenho pena de quem comemora que encontrou bug, eu mesmo fico puto pra caramba, porque é algo que eu poderia prever, falar lá atrás na fase de planejamento ou antes ainda (como vamos ver) que esse erro poderia ocorrer, e bug em produção então, acaba meu dia, porque fatalmente vem a famosa pergunta "Por que não pegamos isso nos testes?". Então vamos deixar claro que nosso trabalho não é medido por Bugs encontrados, e se a empresa que tu trabalha tem esse pensamento, sugiro que abra o linkedin e busque um novo lugar pra trabalhar. Precisamos promover qualidade em todas as etapas do processo de desenvolvimento e para que isso seja possível, algumas mudanças no nosso dia a dia vão ser necessárias, e são elas:

## Ser mais atuante no processo de desenvolvimento

Se o cenário é de trabalhar em times de processo ágil de desenvolvimento de software, temos que identificar como podemos promover qualidade em todas as etapas. Eu vou usar o exemplo do Scrum que é um framework bem comum e utilizado em muitas empresas. A melhor forma de promover a qualidade é estando antes do início das cerimônias. Isso mesmo, devemos começar no momento em que o Product Manager ou Product Owner vai escrever uma história de usuário, e nesse momento, estarmos juntos com ele para entender o contexto daquela nova feature, conversar sobre ela, levantar junto com ele critérios de aceitação.

Usar Gherkin é uma boa idéia para esse momento, caso o PO ou PM não esteja familiarizado com a linguagem, não o force, porque esse é um momento em que devemos **Aprender a Aprender** e então segue o padrão dele para criar os seus critérios de maneira igual, depois utilize o Gherkin para transformar seus critérios de aceite e os dele nesse modelo, porque dessa forma promovemos o que o Lean chama de _**Aprendizado Contínuo**_.

Após escrever as histórias junto com o PO, podemos:

1. Apresentar junto com o PO ou PM em um Grooming Session;
2. Apresentar no Planning*.

Particularmente usar a segunda opção pode gerar desperdício de tempo, porque passamos muito tempo no planning, com o time tirando dúvidas de negócio com o PO ou PM, depois tu apresentando os cenários encontrados que poderão quebrar, deixando a cerimônia chata, diferente de uma reunião de grooming, onde o PO apresenta a lista de itens para o próximo sprint, da a visão do negócio, e com isso, temos tempo para tirar dúvidas relacionadas ao negócio, assim como os devs podem encontrar cenários que não encontramos junto com o PO ou PM, deixando o planning apenas para apresentar a priorização e pontuação das histórias.

3. Durante a fase de desenvolvimento, criar os testes de forma automatizada de cada feature mesmo sabendo que os testes não vão passar, mas sabemos que quando o time terminar uma história, devemos apenas fazer o refactory, colocando o css correto dos elementos no código, executar o teste automatizado, e partir para produção.

4. Todo cenário automatizado deve ser criado um PR para os DEVs, assim como devemos olhar os PRs dos devs também. Tudo que for automatizado deverá ser apresentado para o PO ou PM para que ele possa enxergar valor, assim como, por mais que no início o PM ou PO venha a realizar o teste final (review), mostre que a execução dos testes na etapa de desenvolvimento faz mais sentido, deixando de lado o review (que também pode ser considerado desperdício) para que o PO não passe a ser o gargalo e possamos entregar mais rápido para produção.

# E agora, entendi, mas o que tem a ver com meu projeto de automação??

É simples, nosso projeto não vai começar com os testes legados e sim com todas as novas features pelo simples fato que se começarmos pelo legado, nosso projeto vai ser legado, porque nunca vamos chegar a alinhar com o produto e desenvolvimento de novas features, sempre vamos correr atrás do rabo. Assim como vamos tomar uma atitude de não mais realizar testes de regressão de forma manual em cada iteração. Veremos [aqui](https://github.com/thiagomarquessp/lean-em-projetos-automacao/blob/master/nao-automatizar-o-legado.md) porque devemos tomar essa atitude de não automatizar o legado primeiro. 
