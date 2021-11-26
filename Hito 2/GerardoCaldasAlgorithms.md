# Algoritmo 3

Topic | Desc
-|-
Autor | Gerardo Caldas
Técnica principal | Backtracking

El backtracking, o más conocido como el metodo de retroceso o vuelta atrás), es una técnica general de resolución de problemas,
aplicable en problemas de optimización, juegos y otros tipos. 

~~~
void permutaciones(int n){
int[] perm = new int[n];
boolean[] libres = new boolean[n];

for(int i=0; i<n; i++)
libres[i] = true;

perms(n, 0, perm, libres);
}

void imprimir(int[] v){
for(int i=0; i<v.length; i++)
System.out.print(v[i]+" ");

System.out.println();
}

~~~

Análisis Asintótico: O(n)
