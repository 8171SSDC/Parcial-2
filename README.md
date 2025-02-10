# Parcial-2
##Desarrollar un programa que determine si en una lista no existen elementos repetidos 
lista1 = [4,5,6,7,8,9,10,11,12,13]

def no_repetir (lista1):
    return len(lista1) == len(set(lista1))
print( no_repetir (lista1))
        

##Desarrollar un programa que determine si en una lista se encuentra una cadena de caracteres con dos o mas vocales. Si la cadena existe debe imprimirla y si no existe debe imprimir "no existe"
lista2 = ["ugh", "abe", "yxz"]

def encontrar_vocales (lista2) : 
    vocales = "aeiouAEIOU"
    for cadena in lista2 :
        contador = sum(1 for c in cadena if c in vocales)
        if contador >= 2:
            return cadena
    return "No existe"
print(encontrar_vocales (lista2))
#Desarrollar un programa que dados dos listas determine que elementos tiene la primera lista que no tenga la segunda lista
lista3 = [1,2,3,4,5,6,7]
lista4 = [1,3,5,7,9]
for i in lista3:
    if i not in lista4:
        print(i)
#Desarrollar un lagoritmo que calcule el promedio de un arreglo de reales
def promedio_del_arreglo(A):
    if len(A) == 0:
        return 0 
    suma = sum(A)  / len(A)  
    return promedio

A = [1.5, 2.7, 3.1, 4.9, 5.6]
promedio = promedio_del_arreglo(A)
print("El promedio del arreglo es:", promedio)
#desarrollar un algoritmo que determine la mediana de un arreglo de enteros. La mediana es el número que queda en la mitad del arreglo despues de ser ordenado
def calcular_mediana(arreglo):
    arreglo_ordenado = sorted(arreglo)
    n = len(arreglo_ordenado)
    
    
    if n % 2 != 0:
        return arreglo_ordenado[n // 2]
    else:
       
        medio1 = arreglo_ordenado[n // 2 - 1]
        medio2 = arreglo_ordenado[n // 2]
        return (medio1 + medio2) / 2


arreglo = [1, 3, 4, 2, 5]
mediana = calcular_mediana(arreglo)
print("La mediana del arreglo es:", mediana)
