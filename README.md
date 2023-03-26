Juegos-de-los-Pancakes-aplicando-busqueda-en-profundidad

Juego de los pancakes (pancake sorting) aplicando busqueda en amplitud o tambien BFS en ingles.

Hecho por Marcos Zacarias, ITC-TM, Universidad Autonoma de Baja California Sur

Pequeña explicacion de las funciones:

--"void voltear(string& pancakes, int k)"
Esta función recibe una cadena de caracteres, en este caso, los pancakes, y un entero k, y voltea los primeros k caracteres de la cadena. Se utiliza para simular la acción de voltear un número determinado de pancakes en una pila.

--"bool esta_ordenada(string pancakes)"
Esta función recibe una cadena de caracteres pancakes y devuelve true si la cadena está ordenada de forma ascendente, es decir, si cada caracter es mayor o igual al caracter que le precede en la cadena. Se llama para verificar si el parametro que recibe esta ordenado.

--"vector<string> generar_sucesores(string pancakes)"
Esta función recibe una cadena de caracteres pancakes y devuelve un vector de cadenas de caracteres, son las posibles opciones de voltear distintos numeros de pancakes del arreglo. Se usa para generas sucesores de la cadena actual que recibe y los agrega a la cola de busqueda.
  
--"string generar_caracteres_aleatorios(int n)"
Esta función recibe un entero n y devuelve una cadena de caracteres de longitud n, se usa para generar caracteres aleatorios, asi ahorrando estar pidiendo al usuario que se ingrese caracter por caracter.

--"void bfs(string pancakes)"
Esta es la función principal de búsqueda por amplitud. Recibe una cadena de caracteres pancakes, los cuales son los desordenados. La función utiliza una cola y un conjunto de visitados para llevar a cabo la búsqueda por amplitud. En cada iteración, se saca el primer elemento de la cola y se generan sus sucesores, que se agregan a la cola si no han sido visitados previamente. La función termina cuando se encuentra los pancakes ordenados.

--"int main()"
 Esta es la función principal del programa. Solicita al usuario el número de caracteres de la pila de pancakes, genera una configuración aleatoria de pancakes utilizando la función generar_caracteres_aleatorios y llama a la función bfs para llevar a cabo la búsqueda por amplitud.
