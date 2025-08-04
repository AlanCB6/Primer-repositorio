# if - else
La estructura if-else permite ejecutar diferentes bloques de código dependiendo de si una condición se cumple o no.

###Sintaxis

if (condición) {
    // Código si la condición es verdadera
} else {
    // Código si la condición es falsa
}
C++
Ejemplo: Verificar si un número es positivo o negativo

#include <iostream>
using namespace std;

int main() {
    int numero;
    cout << "Ingrese un número: ";
    cin >> numero;

    if (numero > 0) {
        cout << "El número es positivo." << endl;
    } else if (numero < 0) {
        cout << "El número es negativo." << endl;
    } else {
        cout << "El número es cero." << endl;
    }

    return 0;
}
C++
Explicación:
Si el número ingresado es mayor que 0, se imprime "El número es positivo".
Si el número es menor que 0, se imprime "El número es negativo".
Si no se cumplen las dos condiciones anteriores, significa que el número es 0.
# switch - case
La estructura switch-case permite evaluar múltiples casos en función del valor de una variable.

###Sintaxis

switch (variable) {
    case valor1:
        // Código si variable == valor1
        break;
    case valor2:
        // Código si variable == valor2
        break;
    default:
        // Código si no coincide ningún caso
}
C++
Ejemplo: Menú de opciones

#include <iostream>
using namespace std;

int main() {
    int opcion;
    
    cout << "Seleccione una opción:\n";
    cout << "1. Saludar\n";
    cout << "2. Decir adiós\n";
    cout << "3. Salir\n";
    cout << "Ingrese su opción: ";
    cin >> opcion;

    switch (opcion) {
        case 1:
            cout << "¡Hola! ¿Cómo estás?" << endl;
            break;
        case 2:
            cout << "Adiós, que tengas un buen día." << endl;
            break;
        case 3:
            cout << "Saliendo del programa..." << endl;
            break;
        default:
            cout << "Opción no válida." << endl;
    }

    return 0;
}
C++
Explicación:
Si el usuario ingresa 1, imprime "¡Hola!".
Si ingresa 2, imprime "Adiós".
Si ingresa 3, imprime "Saliendo del programa...".
Si el usuario ingresa otro número, se ejecuta default y muestra "Opción no válida".
🏆 Ejercicios Prácticos
Pon a prueba lo aprendido con estos ejercicios:

✅ Ejercicio 1: Verificar si un número es par o impar con if-else

#include <iostream>
using namespace std;

int main() {
    int num;
    cout << "Ingrese un número: ";
    cin >> num;

    if (num % 2 == 0) {
        cout << "El número es par." << endl;
    } else {
        cout << "El número es impar." << endl;
    }

    return 0;
}
C++
✅ Ejercicio 2: Convertir un número de día de la semana a texto con switch-case

#include <iostream>
using namespace std;

int main() {
    int dia;
    cout << "Ingrese un número de día (1-7): ";
    cin >> dia;

    switch (dia) {
        case 1: cout << "Lunes" << endl; break;
        case 2: cout << "Martes" << endl; break;
        case 3: cout << "Miércoles" << endl; break;
        case 4: cout << "Jueves" << endl; break;
        case 5: cout << "Viernes" << endl; break;
        case 6: cout << "Sábado" << endl; break;
        case 7: cout << "Domingo" << endl; break;
        default: cout << "Número no válido." << endl;
    }

    return 0;
}
C++
# Conclusión
1 item if-else permite tomar decisiones en el código.
2 item switch-case es útil cuando hay múltiples opciones fijas