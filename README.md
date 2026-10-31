# Asignaci-n-de-Porcentaje-de-Evaluaci-n-
Es un programa que considera asignar un porcentaje a la evaluación si cumple dos condiciones participación en evento escolar y es del turno vespertino

Algoritmo AsignarPorcentajeEvaluacion
    // 1. Declaración de variables
    Definir participo_evento Como Logico
    Definir turno Como Cadena
    Definir porcentaje Como Entero

    // 2. Entrada de datos
    Escribir "¿El alumno participó en el evento escolar? (Verdadero / Falso):"
    Leer participo_evento

    Escribir "Ingrese el turno del alumno (matutino / vespertino):"
    Leer turno

    // 3. Evaluación de condiciones (Operador lógico Y / AND)
    // Ambas condiciones deben cumplirse estrictamente para obtener el 30%
    Si (participo_evento == Verdadero) Y (Minusculas(turno) == "vespertino") Entonces
        porcentaje <- 30
    Sino
        porcentaje <- 10
    FinSi

    // 4. Salida de resultados
    Escribir "El porcentaje de evaluación asignado es: ", porcentaje, "%"
FinAlgoritmo
