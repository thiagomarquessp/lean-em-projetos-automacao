# Melhora contínua no nosso projeto de automação de testes

Um dos pilares do Lean é justamente o conceito de melhora contínua e eu gosto muito desse tema, porque eu não gosto com o fator "vou contratar um Messias para o time". Eu acredito que um time cheio de estrelas é prejudicial a saúde e um câncer nos times, porque gera expectativa, gera ciúmes, e cá entre nós, controlar o ego dessas "celebridades" é algo extremamente difícil. O ideal é ter um time o mais diversificado possível, e voltando pro nosso projeto, ter uma pessoa mais SR com skill de automação do que uma corporação de Espscialistas é o melhor dos mundos.

# Faça -> Aprenda com os erros -> Melhore

"É errando que se aprende". Nunca uma frase foi tão clara e tão explicativa desde quando eu começei a trabalhar com testes, e faz todo o sentido. E na automação não é diferente, nos testes não são diferentes, porque a todo momento estamos errando, se estamos escrevendo scripts de testes, estamos errando, e com isso, aprendemos e temos a capacidade de melhorar para o futuro. E esse ciclo será eterno e saudável, quando temos times com diversos níveis de senioridade, porque errando vamos amadurecendo, aprendendo, estudando melhores práticas, etc.

Partindo do princípio que sempre estaremos aprendendo, não pense em fazer da forma mais linda do mundo um cenário automatizado. O que eu tenho aplicado no meu dia a dia é a cada 7 dias de código, 1 dia é dedicado para pagar os débitos técnicos gerados e a cada débito técnico pago, eu aprendo uma nova maneira de fazer as mesmas coisas e o melhor, deixar meu código com menos linhas e mais performático e escalável.

Atualmente estou com um estagiário muito inteligente que está estudando automação e linguagem ruby e javascript e ele terminou o primeiro ciclo de 7 dias, ou seja, no 8 dia vai pagar os débitos técnicos, e juntos vamos fazer **pair** para que possamos aprender juntos as melhores práticas.

# Usar um sistema puxado de tarefas

Dado que o projeto exista, fatalmente histórias ou cards são criados para que seja então estimado, o melhor método que eu trabalhei para projetos desse tipo foi com [Kanban](https://pt.wikipedia.org/wiki/Kanban).

Uma dica de ouro pessoal e que muitos times pecam é com relação a ficar voltando tarefas no quadro, e isso é extremamente prejudicial a saúde de qualquer time, porque gera muita disciplina e o fator "Ah, to com dificuldade, não vou atrapalhar ninguém, eu vou voltar essa tarefa e depois eu pego outra".

Para que esse tipo de hábito não ocorra, crie um quadro de tarefas com as colunas básicas:

```ruby
| TO DO                   | DOING                     | DONE                    |
| Card a ser automatizado |                           |                         |
| Card //     //       // |                           |                         |
|                         | Card a ser automatizado   |                         |
|                         |                           | Card //     //       // |
```
Existem duas possibilidades para se trabalhar de forma efetiva com Kanban em um time com pelo menos 4 pessoas ou mais:

1. Cada pessoa pega uma tarefa na coluna **TO DO** e vai com ela até o final, vamos imaginar esse cenário então com 4 pessoas no time de QAs fazendo automação:

```ruby
| TO DO                   | DOING                        | DONE                    |
|                         | Card a ser automatizado (P1) |                         |
|                         | Card a ser automatizado (P2) |                         |
|                         | Card a ser automatizado (P3) |                         |
|                         | Card a ser automatizado (P4) |                         |
```
Podemos imaginar "Olha como são produtivos, cada um com uma feature sendo automatizada.". Realmente é lindo de se ver quando temos muitas tarefas em **DOING** chegando próximas de ir para **DONE**, agora imagine que os 4 estão com impedimentos em suas tarefas (o que é normal de acontecer), vamos deslocar uma ou mais pessoas para remover o impedimento, porém as features que estavam com essas pessoas por algum momento vão ficar "orfãs", causando assim uma demora na entrega, nas métricas, etc.

Quando tem esse cenário dos impedimentos vem o péssimo hábito como falamos um pouco acima, de pegar e voltar a tarefa, porque não queremos deixar que outras pessoas "percam seu tempo ajudando a remover o impedimento".

Essa maneira 1 é a que eu menos gosto de trabalhar, porque em algum momento aquela velocidade vai cair drasticamente por conta dos impedimentos, mas é uma forma.

2. **Pair** por feature a ser automatizada

Essa é a maneira que eu vi que realmente funciona, não apenas para um projeto de automação, mas para qualquer time e forma de trabalho, porque com o pair é muito mais fácil de solucionar problemas, porque enquanto um pilota o outro vai ajudando, promovendo conhecimento, aprendizado e vem a frase "Duas cabeças pensam melhor que uma", e com isso a possibilidade de ter impedimentos reduz, e fatalmente a feature vai pra **DONE** com muito mais qualidade e o quadro vai ficar dessa forma:

```ruby
| TO DO                   | DOING                             | DONE                    |
|                         | Card a ser automatizado (P1 e P2) |                         |
| Card a ser automatizado |                                   |                         |
|                         | Card a ser automatizado (P3 e P4) |                         |
| Card a ser automatizado |                                   |                         |
```
Dica: Quando a feature com a dupla chegar em **DONE** não assuma outra antes de garantir que a primeira tarefa que está com a outra dupla chegue em produção o mais rápido, e com isso, pergunte como podem ajudar, se estão com algum impedimento e se não tem como ajudar, ai sim, assumir outra tarefa e recomeçar o plano.

# Planejar

Todo card deve ser planejado, e isso requer um tempo da dupla (recomendo fazer planejamento sempre em dois pelo menos). A escrita genérica pode ser feita pra que eu consiga saber de maneira abstrata o que deve ser automatizado, mas antes de sair se aventurando no código, senta com o coleguinha para planejar essa tarefa, analisar se realmente é algo "automatizável", por onde começar, quais cenários atacar para essa feature chegar a **DONE** com sucesso e realmente ir quebrando as tasks, é um bom exercício.

# Pair Auto coleguinha

Pair programming é muito formal rssr e no nosso caso, como estamos fazendo automação, quis chamar assim!

Fazer pair não só pra programar os testes, mas para qualquer coisa é muito bom porque simplesmente:

1. Gera conhecimento contínuo;
Porque ambos enxergam o desenvolvimento de uma forma, e essa forma abre a cabeça das pessoas.

2. Gera aprendizado contínuo;
No pair é o momento onde você, pelo menos comigo é assim, é onde eu mais aprendo, porque enquanto eu estou desenvolvendo eu pergunto para o pair se o que eu estou realizando é uma boa prática, o que ele acha, o que ele pensa, e nesse momento passamos um pouco de experiência, então eu pude absorver bastante coisa técnica realizando pair.

3. Ajuda a eliminar e não gerar desperdício
Enquanto estamos desenvolvendo os testes sozinhos, somos tomados por muitos sentimentos, desde a ansiedade, passando pela raiva, pelo comodismo até a raiva do próprio código e nesse momento a tendência é que façamos um código ruim ou com más práticas e que na hora de abrir um **PR**, ele vai ser rejeitado, e vamos ter que voltar e repensar e escrever o código de uma maneira mais elegante. Esse vai e volta é o desperdício, e realizando pair isso não ocorre porque na primeira má prática podemos conversar com o pair se essa é a forma mais elegante, e se estivermos com os sentimentos ruins que nos levam a fazer isso, deixamos o pair pilotar, que ele encontra a melhor maneira, explica, e todos aprendem, e quando o PR for aberto, será facilmente aprovado pelos outros QAS.

4. Melhora contínua
Sim, em pair sabemos que a cada vez que pilotamos podemos melhorar.

# Refatorar e pagar os débitos

Pensem que sempre podemos melhorar, e com certeza, entregamos automações com muitos débitos (seja na estrutura do projeto ou mesmo no código), quem nunca deixou um monte de sleeps no código?

Mas isso não é o problema. O problema é não pagar. E pagar débitos técnicos deve ser um hábito e esse hábito quem deve definir é o time.

No meu caso, a cada 7 dias de código, 1 é dedicado para pagar todos os débitos técnicos gerados nesse período. E só pego uma nova feature depois que eu certifico que paguei os débitos. Em pair vai mais rápido pode ter certeza.
