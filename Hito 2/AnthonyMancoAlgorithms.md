# Algoritmo 2

Topic | Desc
-|-
Autor | Anthony Manco
Técnica principal | Dijkstra

Decidimos utilizar este algoritmo, ya que determina el camino mas corto, dado un vertice origen, hacia el resto de los vertices en un grafo que tiene persos en cada arista.

Análisi asintotico: O(n^2)

*Pseudocódigo: Cola de prioridad
~~~  
DIJKSTRA (Grafo G, nodo_fuente s)       
       para u ∈ V[G] hacer
           distancia[u] = INFINITO
           padre[u] = NULL
           visto[u] = false
       distancia[s] = 0
       adicionar (cola, (s, distancia[s]))
       mientras que cola no es vacía hacer
           u = extraer_mínimo(cola)
           visto[u] = true
           para todos v ∈ adyacencia[u] hacer
               si no visto[v] y distancia[v] > distancia[u] + peso (u, v) hacer
                   distancia[v] = distancia[u] + peso (u, v)
                   padre[v] = u
                   adicionar(cola,(v, distancia[v]))
~~~
