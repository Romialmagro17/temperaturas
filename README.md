# temperaturas
def calcular_temperatura_promedio(temperaturas):
    """
    Calcula la temperatura promedio de múltiples ciudades durante varias semanas.

    Parámetros:
    temperaturas (dict): Un diccionario donde la clave es el nombre de la ciudad y el valor es una lista con las temperaturas semanales.

    Ejemplo de formato de entrada:
    {
        "Guayaquil": [30, 32, 31, 29],
        "Quito": [18, 20, 19, 17],
        "Cuenca": [15, 14, 16, 13]
    }
    """
    for ciudad, temps in temperaturas.items():
        promedio = sum(temps) / len(temps)
        print(f"La temperatura promedio en {ciudad} es: {promedio:.2f}°C")

# Ejemplo de uso
temperaturas = {
    "Guayaquil": [30, 32, 31, 29],
    "Quito": [18, 20, 19, 17],
    "Cuenca": [15, 14, 16, 13]
}

calcular_temperatura_promedio(temperaturas)
