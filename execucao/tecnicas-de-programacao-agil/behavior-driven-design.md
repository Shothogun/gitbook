# Behavior Driven Design

Behavior-Driven Design \(Design voltado para comportamento\) é uma forma de desenvolvimento de projetos que consiste em estabelecer as funcionalidades de um projeto antes de se definir como implementa-las. Isso deve ser feito por meio da constante interação com o cliente e garante que o projeto que está sendo desenvolvido realmente é aquele que o cliente deseja.

## Recursos para interação com o cliente

A grande premissa por trás do behavior-driven design é melhorar a forma como a equipe de desenvolvimento se comunica com o cliente. Para auxiliar a interação com o cliente, o BDD utiliza vários recursos, os quais tem em comum o foco apenas na funcionalidade presente no projeto, omitindo-se os detalhes técnicos relativos à implementação dessas funcionalidades, os quais ficariam inteiramente a cargo da equipe de desenvolvedores. Esse princípio permite que um cliente sem nenhum conhecimento técnico esteja ativamente direcionando o desenvolvimento do projeto, e não apenas avaliando o estado do projeto de tempos em tempos. Além disso, esses recursos garantem que a equipe de desenvolvimento não terá que gastar tempo para gerar exemplos de funcionalidades e de telas que não estarão presentes no projeto final apenas para deduzir a vontade do cliente.

Os recursos oferecidos pelo behavior-driven design estão detalhados abaixo.

### Histórias de usuário

Histórias de usuário são uma forma simples de se extrair os detalhes de uma feature com base na descrição de uso do programa fornecida pelo cliente. Cada história de usuário deve conter informações básicas como o nome, a descrição, o público alvo e a finalidade de uma feature \(esse formato de histórias de usuário é conhecido como formato Connextra\) e deve ser escrita em uma linguagem simples e compreensível, sem a utilização de termos técnicos.

A utilização de histórias de usuário proporciona alguns benefícios no desenvolvimento do projeto. Primeiramente, as histórias de usuário permitem que o cliente possua um maior engajamento no desenvolvimento do programa ao descrever as features desejadas e ao orientar os desenvolvedores acerca de quais features devem ter maior prioridade. Além disso, as histórias de usuário permitem que os desenvolvedores tenham uma forma simples e fácil de visualizar e organizar todas as features contidas no projeto \(para isso, as histórias de usuário são escritas ou em cards do Trello ou em folhas de post-it\). Por fim, a dinâmica de desenvolvimento fornecida pelas histórias de usuário é compatível com várias ideias da programação ágil, de forma que os dois podem ser utilizados em conjunto no desenvolvimento de projetos.

### Sistema de pontuação de features

O sistema de pontuação de features é uma forma de aferir a dificuldade de implementação das features existentes para um projeto. Cada feature deve ser classificada com um número da sequência de Fibonacci \(1, 2, 3, 5, 8, 13, ...\), que expressa o trabalho necessário para se implementar a funcionalidade, os testes e a documentação por trás dessa feature. Features com uma dificuldade maior ou igual a 5 são chamadas de _épicos_ e devem ser divididas em sub-features mais fáceis.

Para definir a dificuldade de uma feature, os desenvolvedores do projeto se reunem e, após ouvirem uma breve descrição da feature, votam acerca da dificuldade que deve ser atribuída a essa feature. Caso exista um grande consenso em torno de um nível de dificuldade, este nível é atribuído à feature. Do contrário, os desenvolvedores devem conversar entre si acerca dos detalhes presentes na feature com o intuito de se chegar a um consenso.

### Esboços Lo-Fi

Esboços Lo-Fi são uma forma de apresentar ao cliente a ideia por trás de uma view do website sem a utilizado de código \(o qual consome recursos e tempo para ser escrito\). Assim, ao invés de se preparar vislumbrantes previews com recursos HTML e CSS, os desenvolvedores do projeto apresentam esboços simples e rápidos das views de uma feature, feitos ou à mão ou com algum programa de computador, ao cliente. Por meio desses esboços, o cliente pode visualizar o layout das páginas de uma feature, enteder quais botões de cada página conduzem a quais views e sugerir mudanças aos desenvolvedores. Apenas quando o cliente e os desenvolvedores concordarem no formato dos layouts a serem utilizados é que os desenvolvedores iniciam o trabalho com HTML e CSS.

## Vantagens

* Facilita a comunicação com o cliente do projeto.
* Diminiu a quantidade de retrabalho devido a especificações erradas.
* Auxilia a divisão e a administração do trabalho a ser feito.
* Evita problemas de integração de front-end e back-end.

## Desvantagens

* Requer comunicação constante com o cliente do projeto.
* Estruturado especificamente para desenvolvedores full-stack.

## BDD em Ruby on Rails

O behavior-driven design em Ruby on Rails é feito por meio das gems _cucumber-rails_ e _capybara_. A gem _cucumber-rails_ permite que as histórias de usuário de um projeto sejam armazenadas e descritas em arquivos com a extensão _feature_. A gem _capybara_ permite que a descrição das histórias de usuário seja transformada em testes de aceitação e de integração para o projeto por meio de arquivos ruby para a definição dos passos de uma história de usuário.

Opcionalmente, a gem _gemaina_ pode ser utilizada para gerar arquivos .feature e seus respectivos arquivos de definição de passos a partir de um comando do rails. Estes arquivos podem ser gerados tanto em inglês como em português brasileiro.

## Disciplinas do curso que abordam esse conteúdo

* Métodos de programação \(3º Semestre\)
* Engenharia de software \(6º Semestre\)

