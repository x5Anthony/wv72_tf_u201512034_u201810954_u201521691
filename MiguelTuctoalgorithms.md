# MiguelAlgorithm

Topic | Desc
-|-
Autor | Miguel Tucto
Técnica principal | Fuerza Bruta

Decidi utilizar este algortimo ya que es capaz de encontrar la solución a cualquier problema por complicado que sea. Es decir, prueba
todas las posibles combinaciones, recorre todos los caminos hasta dar con la situación que es igual que la solución.

~~
def bfmax(a):
  m = a[0]
  for i in range(1, len(a)):
    if a[i] > m:
      m = a[i]
  return m
~~

__Análisis Asintótico:__ O(n)
