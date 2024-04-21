
### Ejercicio Nro.1

Genere un programa que encuentre todos los numeros divisibles por 7 pero que no sean multiplos de 5, comprendidos entre 2000 y 3200 (ambos incluidos). Los numeros obtenidos deben imprimirse en una secuencia separada por comas en una sola linea.
Considere la posibilidad de utilizar el metodo range(#inicio, #fin)

Respuesta:
```python
l=[]
for i in range(2000, 3201):
    if (i%7==0) and (i%5!=0):
        l.append(str(i))

print(','.join(l))
```

### Ejercicio Nro.2

Escriba un programa que pueda calcular el factorial de un numero dado. Los resultados deben imprimirse en una secuencia separada por comas en una sola linea. Supongamos que el programa recibe la siguiente entrada: 8 Entonces, la salida debe ser: 40320.
En caso de que se suministren datos de entrada a la pregunta, debe suponerse que se trata de una entrada de consola.

Respuesta:
```python
def fact(x):
    if x == 0:
        return 1
    return x * fact(x - 1)

x=int(input())
print(fact(x))
```

### Ejercicio Nro.3

Con un numero integral n dado, escriba un programa para generar un diccionario que contenga (i, i*i) tal que sea un numero integral entre 1 y n (ambos incluidos). y luego el programa debe imprimir el diccionario. Suponga que se suministra la siguiente entrada al programa: 8 Entonces, la salida deberia ser: {1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64}
En caso de que se suministren datos de entrada a la pregunta, debe asumirse que se trata de una entrada de consola. Considere el uso de dict()

Respuesta:
```python
n=int(input())
d=dict()
for i in range(1,n+1):
    d[i]=i*i

print(d)
```

### Ejercicio Nro.4

Pregunta: Escribe un programa que acepte por consola una secuencia de numeros separados por comas y genere una lista y una tupla que contenga cada numero. Supongamos que el programa recibe la siguiente entrada: 34,67,55,33,12,98 Entonces, la salida deberia ser: ['34', '67', '55', '33', '12', '98'] ('34', '67', '55', '33', '12', '98')
El metodo tuple() puede convertir una lista en una tupla

Respuesta:
```python
values=input()
l=values.split(",")
t=tuple(l)
print(l)
print(t)
```

---- Gracias por leer ----