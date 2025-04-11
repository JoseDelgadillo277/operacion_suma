- ## Logo de python
- ![Logo de pyhton](https://w7.pngwing.com/pngs/585/822/png-transparent-python-scalable-graphics-logo-javascript-creative-dimensional-code-angle-text-rectangle-thumbnail.png)

# Aplicación operación Suma
## Descripción
El script implementa la suma de dos números y realiza la validación de los operandos.
## Funcionalidad
- Suma dos operandos
- **Verifica** los operandos sean números (int o float)
- [Repositorio Github](https://github.com/JoseDelgadillo277/operacion_suma.git)

  ### Equipo de desarrollo
  | Apellidos y Nombres | Rol |
  | --------------- | -------------- |
  | 1 | Jefe de proyecto |
  | 2 | Analista |


## python suma.py
💻 Ejemplo Interactivo
Ingrese el primer número: 10
Ingrese el segundo número: 5.5
Resultado de la suma: 15.5
Si se ingresan datos inválidos:

cpp
Copiar
Editar
Ingrese el primer número: diez
Error: Ambos operandos deben ser de tipo int o float.
🧠 Código (suma.py)
python
Copiar
Editar
def sumar(a, b):
    if not isinstance(a, (int, float)) or not isinstance(b, (int, float)):
        raise ValueError("Ambos operandos deben ser de tipo int o float.")
    return a + b

if __name__ == "__main__":
    try:
        num1 = float(input("Ingrese el primer número: "))
        num2 = float(input("Ingrese el segundo número: "))
        resultado = sumar(num1, num2)
        print(f"Resultado de la suma: {resultado}")
    except ValueError as e:
        print(f"Error: {e}")
