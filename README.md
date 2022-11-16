# Design-Pattern

Padrões de Projeto 

 

  Padrão MVC  

É um padrão de arquitetura de software responsável por contribuir na otimização da velocidade entre as requisições feitas pelo comando dos usuários.   

Foi criado em 1979 por Trygve Reenskaugh um cientista da computação norueguês, que escreveu esse padrão para o projeto de software Graphic User interface,  é dividido em três componentes essenciais: Model, Controller e View.   

Model ou Modelo  

Essa classe também é conhecida como Business Object Model (objeto modelo de negócio). Sua responsabilidade é gerenciar e controlar a forma como os dados se comportam por meio das funções, lógica e regras de negócios estabelecidas, como por exemplo acesso a uma api que retornará um Json.   
 
 

Ele é o detentor dos dados que recebe as informações do Controller, válida se ela está correta ou não e envia a resposta mais adequada. 

Controller ou Controlador: 

A camada de controle é responsável por intermediar as requisições enviadas pelo View com as respostas fornecidas pelo Model, processando os dados que o usuário informou e repassando para outras camadas.  
Numa analogia bem simplista, o controller  operaria como o ‘’maestro de uma orquestra’’  que permite a comunicação entre o detentor dos dados e a pessoa com vários questionamentos no MVC.  

View ou Visão 

Essa camada é responsável por apresentar as informações de forma visual ao usuário. Em seu desenvolvimento devem ser aplicados apenas recursos ligados a aparência como mensagens, botões ou telas.  

Seguindo nosso processo de comparação o View está na linha de frente da comunicação com usuário e é responsável transmitir questionamentos ao controller e entregar as respostas obtidas ao usuário. É a parte da interface que se comunica, disponibilizando e capturando todas as informação do usuário. 

Router ou rotas 

Ele é responsável por criar as rotas que vão ligar os endereços dos requests dos controllers para as respectivas views. 

Como os componentes interagem? 

Tudo começa com a interação do usuário na camada View. A partir daí o controlador pega essa informações e envia para o Model que fica responsável por avaliar aqueles dados e transmitir uma resposta.  

O controlador recebe essas respostas e envia uma notificação de validação daquela informação para a camada visão, fazendo com a mesma apresente o resultado de maneira gráfica e visual. 

Todo esse processo leva em consideração as regras de negócio aplicadas na construção de todo projeto. 

Por que usar MVC? 

Segurança: O controller funciona como uma espécie de filtro capaz de impedir que 		qualquer dado incorreto chegue até a camada modelo. 

Organização: Esse método de programação permite que um novo desenvolvedor tenha muito mais facilidade em entender o que foi construído, assim como os erros se tornam mais fácil de serem encontrados e corrigidos. 

Eficiência: Como a arquitetura de software é dividida em 3 componentes , sua aplicação fica muito mais leve, permitindo que vários desenvolvedores trabalhem no projeto de forma independente. 

Tempo: Com a dinâmica facilitada pela colaboração entre os profissionais de desenvolvimento, o projeto pode ser concluído com muito mais rapidez, tornando o projeto escalável.   

Transformação: As mudanças que forem necessárias também são mais fluidas, já que não será essencial trabalhar nas regras de negócio e correção de bugs. 

Além disso, fornece ao software estabilidade no processo de comunicação entre 	seus elementos de maneira dinâmica para que a experiência do usuário não seja 	prejudicada.  

 

Desvantagens na utilização do MVC: 

Complexidade inicial do entendimento do conceito da divisão de camadas, e o tempo para planejamento  

Uma dúvida muito recorrente na programação é se no processo de desenvolvimento pode ter apenas esses 3 componentes ou se é possível acrescentar mais alguns. A resposta é sim para a possibilidade de inserir uma camada extra. Essa sequência de códigos pode ser alterada conforme a necessidade do projeto.  

Mas um código com muitas camadas se torna muito confuso e por isso, o ideal é manter o padrão original. A seguir vamos explicar os conceitos e aplicações dos componentes que acompanham essa arquitetura de software. 

Como implementar um projeto MVC? 

Essa arquitetura de software pode ser utilizada no programação web, mobile ou desktop e ela pode ser implementada através de diversos frameworks como o Spring MVC ou Play Framework, Laravel, Aspnetmvc,Django,Angular e Rails. 
