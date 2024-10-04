# numerostriunfadores
#actividad3_numerostriunfadores
print("Paola Gutierrez Torres")
print(" ")
#solicita al usuario ingresar los numeros triunfadores
def main():
    numeros_triunfadores = []
    
    print("Introduce los números triunfadores de la lotería. Escribe 'fin' para terminar.")
    
    while True:
        entrada = input("Ingresa un número (o 'fin' para terminar): ")
        
        if entrada.lower() == 'fin':
            break
            
        try:
            numero = int(entrada)
            numeros_triunfadores.append(numero)
        except ValueError:
            print("Por favor, ingresa un número válido.")
    
    # Ordenar la lista de menor a mayor
    numeros_triunfadores.sort()
    
    # Mostrar la lista
    print("Números triunfadores de la lotería (de menor a mayor):")
    print(numeros_triunfadores)

if __name__ == "__main__":
    main()
