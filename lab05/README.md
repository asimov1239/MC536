# Aluno
* `216111`: `Gabriel Bonfim Silva de Moraes`

## Tarefa de Cypher sobre Marcadores e Taxonomia

## Tarefa 1

### Resolução

~~~cypher
MATCH p=()-[r:Pertence]->({id:"Serviços"}) 
RETURN p LIMIT 25
~~~

## Tarefa 2


### Resolução


~~~cypher
MATCH x=()-[r:Superior]->({id:"Serviços"}) 
MATCH y=()-[p:Pertence]->({id:"Serviços"}) 
MATCH z=()-[q:Pertence]-> () - [t:Superior]->({id:"Serviços"}) 
RETURN x, y, z LIMIT 25
~~~
