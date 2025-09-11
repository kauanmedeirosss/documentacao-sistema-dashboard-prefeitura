# Um pequeno guia para entender o Diagramas de Classes

## Classes
### Classes comuns
<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/3dd2a03a-bfc0-4f22-9e2a-4b2891efaa21" />

* O que temos em cada um dos 3 blocos da classe:
  - 1° -> Nome da classe (Em negrito)
  - 2° -> Atributos. Estrutura:
    * " - nomeAtributo : tipoAtributo "
  - 3° -> Métodos. Estrutura:
    * " + nomeMetodo(argumento : tipoArgumento) : tipoRetorno "

### Enum
<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/1ac047e9-5139-4478-9378-9b7d33149fd3" />

* Estrutura dos enums:
  - 1° -> Especificação do esteorótipo 
  - 1° -> Nome
  - 2° -> Atributos
  - 3° -> Métodos
  - 4° -> Constantes

### Enum enriquecido ou Enum orientado a objetos
<img width="200" height="300" alt="image" src="https://github.com/user-attachments/assets/2a70959a-3596-4be7-a9a0-0a03dfc92239" />

* Estrutura acima foi gerada pelo ChatGPT para exemplificar como ficaria um Enum cujas constantes possuem atributos.

## Níveis de visibilidade
São usados em atributos e métodos.
* '+ público' - visível em qualquer classe
* '# protegido' - qualquer descendente pode usar
* '- privado' - visível somente dentro da classe

## Relacionamentos
<img width="200" height="300" alt="image" src="https://github.com/user-attachments/assets/0f12fab0-ddd1-4eff-b9d4-eb0702d708b7" />

* Associação
  - "uma “conhece” ou “usa” a outra como atributo"
  - se tiver seta, fica do lado do todo
    * Com seta → unidirecional (só uma classe conhece a outra).
    * Sem seta → bidirecional (ambas se conhecem).
* Herança (Generalização)
  - "Uma classe é um tipo especializado de outra"
  - linha contínua com seta aberta para o pai (superclasse), linha mais grossa/negrita que as demais
* Dependência
  - "Um relacionamento fraco, temporário, geralmente porque uma classe usa a outra como parâmetro ou variável local"
  - linha tracejada com seta aberta aponta para o elemento do qual depende
* Agregação
  - "uma solicitação PODE ter vários feedbacks"
  - losango branco do lado do todo
* Composição
  - "um dashboard pode ter várias notificações, mas uma notificação NÃO EXISTE SEM o dashboard"
  - losango preto no lado do todo

### As setas
* Losango + linha simples = agregação/composição sem direção explícita → indica só a relação "todo–parte".
* Losango + seta = agregação/composição com direção → indica que o lado do losango conhece a parte, mas a parte não necessariamente conhece o todo.
  - Ou seja, não existe referencia do todo na classe da parte

## Exemplo de Modelo relacional 
<img width="800" height="550" alt="image" src="https://github.com/user-attachments/assets/633e0e01-bcea-4ab3-ae29-5c8bca92a022" />
