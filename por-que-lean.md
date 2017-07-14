# Por que aplicar Lean?

O Lean possui diversas filosofias, mas vou listar aqui o que de fato eu considero pontos fundamentais para aplicar principalmente na nossa área de testes:

1. Evitar e Elinimar desperdícios;
2. Antecipar os problemas (esse complementa o de cima);
3. Melhora contínua;
4. Aprendizado contínuo;
5. Respeitar as pessoas.

Fazem quase 12 anos que trabalho com testes e qualidade de Software e ainda escuto QAs falando que o objetivo de um QA ou Tester é encontrar bugs e o problema de pensar assim é ir de encontro com as seguintes desculpas: "Os testes de regressão tomam meu tempo todo", "Eu não tenho tempo para automatizar os testes!", "A empresa que eu trabalho não da oportunidade de automação.", "Não tenho tempo para estudar automação.", "Vou estudar automação em casa e não tenho onde aplicar.", etc. E perceba que tudo está em, volta da desculpa do tempo.

# Conta de padaria baseado em testes no fim

```ruby
|Equipe                     | Valor/mês | Features/mês |
|10 pessoas (PO, Devs e QA) | R$40K     | 2            |
```
Conta bem besta ta ...

Considerando esse cenário, estamos dizendo que cada feature desenvolvida tem o valor de R$20K e por isso entregamos 2 features por mês ou uma feature por sprint.

Agora imagina se volta uma feature que acabamos de desenvolver com bug crítico de produção. Então esse bug será corrigido, mas digamos que na tal fase de testes encontramos outros e outros e vai e volta e levam duas semanas também para ser entregue um bug que esteve em produção. Vamos olhar os valores:

```ruby
| Valor da Feature | Valor do Bug                                                        |
| R$20K/mês        | R$0 quando não tem bug                                              |
| R$20K/mês        | R$20K quando volta de produção e levamos duas semanas para entregar |
```

Estamos dizendo que nesse caso, uma feature que hoje vale R$20K está valendo R$40K porque teve um bug e levamos mais duas semanas pra corrigir certo?

**ERRADO**

As duas semanas que levamos corrigindo o bug eram pra ser utilizadas para desenvolver mais uma feature que custa R$20K e vamos atrasar por conta do bug, mas a empresa vai sempre pagar os funcionários em dia, ou seja, aquela feature que custou R$20K e teve bug não custou R$40K, ela custou R$60K.

"Ahhh, mas eu não quero saber desses números."

Ok, e vou falar que nem seus gestores sabem desses números, MAS, aos poucos as empresas estão mais ligadas com o fator custo/produtividade e uma hora essa conta vai aparecer, e vão ver que se gasta muito dinheiro com bug encontrado em produção e vão demitir muita gente e aí vira o caos.

# E agora, podemos reverter esse quadro?

Sim, apenas quando colocamos na nossa cabeça que nosso papel é evitar que os bugs possam chegar em produção e passamos a estar mais próximos da área de produtos e desenvolvedores, todo esse marasmo de ter que testar no final do sprint, ou na etapa de testes acaba porque conseguimos prever que algo possa dar errado bem antes de dar errado, e com isso os devs conseguem desenvolver esse fluxo antes de ir pra produção, e por ai vai, ou seja, features com mais qualidade em produção em menos tempo, e com a maturidade e a confiança, porque ter que testar no fim, sendo que você sabe que o desenvolvedor fez a feature de acordo com o que a área de produto queria juntamente com os cenários que tu encontrou? Dado que esteja maduro, sobra-se o tão sonhado tempo para estudar e aplicar automação.

Algumas empresas tem a mania de eleger um "projeto de automação de testes", o que é natural, apesar de não concordar com a idéia, mas, sabendo que é assim, e aqui onde estou não é diferente, resolvi aplicar alguns conceitos de Lean (esses citados acima) para que pudesse também gerar o máximo de valor em menos tempo e vem dando resultados bem animadores.

Vamos ver tópico a tópico:

Primeiro vamos ver o que eu mais gosto, de [evitar e eliminar desperdícios](WIP)
