# catanzarolucas-UTN-TUPaD-P1
Estrucruras secuenciales

#---------------------- estacion_año.py------------------------------------

# este programa determina la estacion del año basandose en el hemisferio, mes dia
hemisferio = input("¿en que hemisferio se encuentra? (N/S): ").upper()
mes = input("¿que (mes del año es? ")).lower
dia = int(input("¿que dia es?: "))

if hemisferio == "N":
    if (mes == "diciembre" and dia >= 21) or (mes == "enero") or (mes == "febrero") or (mes == "marzo" and dia <= 20):
        print("Invierno")
    elif (mes == "marzo" and dia >= 21) or (mes == "abril") or (mes == "mayo") or (mes == "junio" and dia <= 20):
        print("Primavera")
    elif (mes == "junio" and dia >= 21) or (mes == "julio") or (mes == "agosto") or (mes == "septiembre" and dia <= 20):
        print("Verano")
    else:
        print("Otoño")
elif hemisferio == "S":
    if (mes == "diciembre" and dia >= 21) or (mes == "enero") or (mes == "febrero") or (mes == "marzo" and dia <= 20):
        print("Verano")
    elif (mes == "marzo" and dia >= 21) or (mes == "abril") or (mes == "mayo") or (mes == "junio" and dia <= 20):
        print("Otoño")
    elif (mes == "junio" and dia >= 21) or (mes == "julio") or (mes == "agosto") or (mes == "septiembre" and dia <= 20):
        print("Invierno")
    else:
        print("Primavera")
else:
    print("Hemisferio no válido. Por favor, ingrese 'N' o 'S'.")


#---------------------longitud_contraseña.py-----------------------------


# este programa verifica longitud de una contraseña entre 8 y 14 caracteres
contraseña = input("por favor ingrese una contraseña: ")
if len(contraseña) >= 8 and len(contraseña) <= 14:
    print("ha ingresado una contraseña correcta.")
else:
    print("por favor, una contraseña de entre 8 y 14 caracteres. ")



#---------------------------mayor_edad.py---------------------------------


# este programa solicita la edad del usuario verifica si es mayor de 18 años
edad = int(input("por favor, ingresa tu edad: "))
if edad > 18:
    print("es mayor de edad. ")


#------------------------------numero_par.py--------------------------------


#este programa utiliza el operardor modulo(%) verifica si es numero par
numero = int(input("por favor, ingresar un numero: "))
if numero % 2 == 0:
    print("ingreso un numero par")
else:
    print("ingrese un numero par")




#-----------------------------sesgo_estadistico.py-----------------------


# este programa utiliza la libreria statistics para calcular el seego de lista numeros
import random
from statistics import mode, median, mean
numeros_aleatorios = [random.randint(1, 100) for i in range(50)]
moda = mode(numeros_aleatorios)
mediana = median(numeros_aleatorios)
media = mean(numeros_aleatorios)
if media > mediana and mediana > moda:
    print("sesgo positivo o a la derecha ")
elif media < mediana and mediana < moda:
    print("seego negativo a la izquierda ")
else:
    print("sin sesgo ")




#------------------------string_termina_vocal.py-------------------------



# este programa verifica si un string termina en vocal y añade signo de exclamacion
frase = input("por favor, ingrese un frase o palabra: ")
vocales = "a", "e", "i", "o", "u"
if frase.lower().endswith(vocales):
    print(frase + "!")
else:
    print(frase)






#---------------------escala_richter.py-----------------------------------






# Este programa clasifica la magnitud de un terremoto en escala de Richter
magnitud = float(input("por favor, ingrese magnitud del terremoto: "))
if magnitud < 3:
    print("muy leve (imperceptible) ")
elif magnitud >= 3 and magnitud < 4:
    print("leve (ligeramente perceptible) ")
elif magnitud >= 4 and magnitud < 5:
    print("moderado (sentido por personas, no causa daños)")
elif magnitud >= 5 and magnitud < 6:
    print("fuerte (causa daños en estructuras debiles) ")
elif magnitud >= 6 and magnitud < 7:
    print("muy fuerte(causa daños significativos )")
else: 
    print("extremo (causa daños a gran escala) ")





#---------------------------conversor_nombre.py----------------------------



# conversor de nombre a mayuscula, minusculas o con la primer letra en mayuscula segun la opcion elegida 
nombre = input("por favor, ingrese su nombre: ")
opcion = input("elija una opcion (1, 2 o 3): ")
if opcion == "1":
    print(nombre.upper())
elif opcion == "2": 
    print(nombre.lower())
elif opcion == "3":
    print(nombre.title())
else:
    print("opcion no valida")




#------------------------categoria_edad.py---------------------------------



#este programa clasifica al usuario en una categoria sun la edad
edad = int(input("ingresa tu edad. "))
if edad < 12:
    print("niño/a. ")
elif edad >= 12 and edad < 18:
    print("adolescente. ")
elif edad >= 18 and edad < 30:
    print("adulto/a joven. ")
else:
    print("adulto/a. ")








#----------------------aprobado_desaprobado.py------------------------------




# este programa pide una nota y determina si el estudiante aprobo o desaprobo
nota = float(input("por favor, ingresa tu nota: "))
if nota >= 6:
    print("aprobado")
else:
    print("desaprobado")
    



    







