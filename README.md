import random

# Genera un número aleatorio entre 1 y 10
numero = random.randint(1, 10)

# Comprueba si el número es mayor que 5 e imprime un mensaje en consecuencia
if numero > 5:
    print(f"El número {numero} es mayor que 5")
else:
    print(f"El número {numero} es menor o igual a 5")

# Comprueba si 5 es mayor que 4 y luego imprime True o False
print(True if 5 > 4 else False)

# Comprueba si 5 es mayor que 7 y luego imprime el resultado
print(5 > 7)

# Define una variable booleana "recibido" y luego imprime su negación
recibido = False
print(not recibido)

# Define una variable de cadena "nombre" y realiza varias operaciones con ella
nombre = "Gael"
print(nombre)
print(type(nombre))
print(nombre.capitalize())
print(nombre.upper())

# Muestra varias variables con formato en una cadena
num = 10
pi = 3.14
es_estudiante = True
print(f"{num} - {pi} - {es_estudiante} - {nombre}")

# Realiza operaciones aritméticas e imprime los resultados
print(5 + 4)  # Suma
print(5 - 4)  # Resta
print(5 * 4)  # Multiplicación
print(5 / 4)  # División
print(5 // 4)  # División Entera
print(5 % 4)  # Módulo
print(5 ** 4)  # Exponenciación

# Realiza operaciones lógicas e imprime los resultados
print(True and False)
print(True or False)
print(not False)

# Compara dos números y muestra un mensaje si se cumple la condición
n1 = 30
n2 = 20
if n1 > n2:
    print(f"{n1} > {n2}")

# Cambia el valor de n1 y compara nuevamente
n1 = 10
if n1 > n2:
    print(f"{n1} > {n2}")
else:
    print(f"{n1} < {n2}")

# Comprueba la edad y muestra un mensaje según la condición
edad = 18
if edad > 18:
    print("Adulto")
elif edad == 18:
    print("Recién cumplió 18")
else:
    print("Menor")

# Define funciones para realizar operaciones matemáticas
def suma(a, b):
    return a + b

def resta(a, b):
    return a - b

def multiplicacion(a, b):
    return a * b

def division(a, b):
    return a / b

# Crea una lista de funciones y realiza operaciones con ellas
operaciones = [suma, resta, multiplicacion, division]
print(operaciones[0](5, 4))
print(operaciones[1](5, 4))
print(operaciones[2](5, 4))
print(operaciones[3](5, 4))

# Define una lista con varios tipos de datos y realiza diversas operaciones con ella
mi_lista = [1, 2, 3, 4, 5, True, 4.5, "Gael", [1, 2, 3]]
print(mi_lista[8])
print(mi_lista)
print(mi_lista[:])
print(mi_lista[0:1])
print(mi_lista[0:])
print(mi_lista[-3:-1])

# Define una función sin contenido y la llama
def suma(a, b):
    pass

print(suma(3, 4))

# Define una función que devuelve una lista de resultados y realiza operaciones con ella
def operaciones(a, b):
    return [a + b, a - b, a * b, a / b]

respuestas = operaciones(5, 4)
print(respuestas)
w, x, y, z = operaciones(5, 4)
print(w)

resultado_suma, _, _, _ = operaciones(5, 4)
print(resultado_suma)

# Define una tupla de funciones y realiza operaciones con ella
operaciones_tupla = (suma, resta, multiplicacion, division)
print(operaciones_tupla[1](5, 4))

# Define una tupla de valores
mi_tupla = (1, 2, 3, 4, 5, True, 4.5, "Oliver", [1, 2, 3])

# Modifica la lista original agregando un valor
mi_lista.append(10)
print(mi_lista)

# Concatena una tupla adicional a la tupla existente
mi_tupla += (10, 11, 12)
print(mi_tupla)

# Imprime el primer elemento de la tupla
print(mi_tupla[0])

# Define funciones con anotaciones de tipo
def suma(a: int, b: int) -> int:
    return a + b

def operacion(a: int, b: int) -> tuple:
    return (a + b, a - b)

# Llama a las funciones y muestra los resultados
(a, b) = operacion(5, 6)
a, b = operacion(6, 5)
print(a, b)

# Crea un rango de números y muestra sus valores
numeros = range(10)
print(numeros)
for i in numeros:
    print(i, end=" ")

# Crea un rango de números específico y muestra sus valores
numeros = range(5, 10)
for i in numeros:
    print(i, end=" ")

# Crea un rango de números pares y muestra sus valores
numeros_pares = range(2, 11, 2)
for par in numeros_pares:
    print(par, end=" ")

# Utiliza un bucle for para mostrar números pares en un rango
for item in range(2, 11, 2):
    print(item, end=" ")

# Convierte un rango en una lista
numeros = range(5, 10)
numeros = list(numeros)
print(numeros)

# Define una lista de números y realiza operaciones con ella
mi_lista = [3, 6, 7, 40, 34, 67, 89]
print(max(mi_lista))
print(min(mi_lista))
print(sum(mi_lista))

# Ordena la lista de números de forma ascendente y descendente
mi_lista.sort()
print(mi_lista)
mi_lista.sort(reverse=True)
print(mi_lista)

# Define un conjunto (set) y muestra su contenido
mi_set = {1, 2, 3, 3, 3, 3, 3}
print(mi_set)

# Convierte una lista en un conjunto para eliminar duplicados
data = [15, 14, 13, 12, 11, 10, 1, 2, 3, 4, 5, 6, 7, 8, 9, 1, 2, 1, 2, 1, 2, 1, 2]
conjunto_unico = set(data)
print(conjunto_unico)

# Define otro conjunto y realiza una unión con el conjunto original
data2 = {1, 56, 57, 58}
conjunto_fusionado = mi_set.union(data2)
print(conjunto_fusionado)

# Define un diccionario y muestra sus valores mediante claves
mi_diccionario = {"clave": "valor"}
print(mi_diccionario["clave"])
print(mi_diccionario.keys())
print(mi_diccionario.values())

# Define un diccionario de días de la semana y muestra sus elementos
dias_de_la_semana = {
    "Lunes": "1",
    "Martes": "2",
    "Miércoles": "3",
    "Jueves": "4",
    "Viernes": "5",
    "Sábado": "6",
    "Domingo": "7"
}

# Muestra elementos del conjunto y diccionario
for elemento in mi_set:
    print(elemento, end=" ")

for clave in dias_de_la_semana.keys():
    print(clave)

for valor in dias_de_la_semana.values():
    print(valor)

for clave, valor in dias_de_la_semana.items():
    print(clave, valor)

# Imprime el diccionario de días de la semana
print(dias_de_la_semana)



