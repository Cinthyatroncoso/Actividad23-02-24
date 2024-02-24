
clean = pd.read_csv("clean.csv")
print(clean)
print(clean.head(5))

while True:
    print("Menú:")
    print("1. Mostrar estadísticas")
    print("2. Filtrar registros")
    print("3. Máximo")
    print("4. Mínimo")
    print("5. Salir")

    opcion = input("Ingrese el número de la opción deseada: ")

    if opcion == '1':
        for columna in ['kilometer', 'age']:
            print(f"Estadísticas de {kilometer}:")
            print(f"Promedio: {clean[age].prom()}")
            print(f"Máximo: {clean[age].max()}")
            print(f"Mínimo: {clean[kilometer].min()}\n")
    
    elif opcion == '2':
        print("kilometer' es mayor que 50000:")
        print(clean[clean['kilometer'] > 50000])

    elif opcion == '3':
        print("Mostraremos el Máximo:")
        print(clean.max())

    elif opcion == '4':
        print("Mostraremos el Mínimo:")
        print(clean.min())

    elif opcion == '5':
        print("salir")
