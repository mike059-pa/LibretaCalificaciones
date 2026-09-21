# Actividad #3 - Libro de Calificaciones

**Fecha:** 07/09/2026

## Contenido del Repositorio

Este repositorio contiene el desarrollo de la **Actividad #3** de la materia **HPA III**, realizada utilizando el lenguaje de programación **C#**.

La actividad consiste en desarrollar un sistema de **Libro de Calificaciones**, aplicando conceptos de programación orientada a objetos, clases, constructores, propiedades, métodos, estructuras repetitivas y estructuras condicionales.

El programa contiene dos clases para realizar el cálculo del promedio de las calificaciones:

1. **LibroCalificaciones:** permite ingresar exactamente 10 calificaciones y calcular el promedio de la clase.
2. **LibroCalificaciones1:** permite ingresar una cantidad variable de calificaciones utilizando `-1` como valor centinela para finalizar el ingreso.

La clase `PruebaLibroCalificaciones` contiene el método `Main`, desde donde se crean los objetos de ambas clases y se ejecutan sus respectivos métodos.

---

## Tecnologías Utilizadas

* **Lenguaje:** C#
* **Framework:** .NET
* **IDE:** Visual Studio
* **Tipo de aplicación:** Aplicación de consola
* **Programación orientada a objetos:** Clases, objetos, constructores, propiedades y métodos
* **Estructuras de control:** `while` e `if/else`
* **Entrada de datos:** `Console.ReadLine()`
* **Conversión de datos:** `Convert.ToInt32()`

---

## Capturas de Pantalla y Problemas

### 1. Clase LibroCalificaciones

La clase `LibroCalificaciones` representa un libro de calificaciones asociado a un curso.

La clase contiene una propiedad llamada `NombreCurso`, un constructor para inicializar el nombre del curso y los métodos `MostrarMensaje()` y `DeterminarPromedioClase()`.

El método `DeterminarPromedioClase()` solicita al usuario **10 calificaciones**, acumula sus valores y posteriormente calcula el promedio de la clase.

#### Ejecución del programa

<img width="1401" height="647" alt="image" src="https://github.com/user-attachments/assets/a24c5127-6d46-4131-870a-52680aed0c0c" />


#### Resultado del promedio

<img width="602" height="392" alt="image" src="https://github.com/user-attachments/assets/0923d648-76c3-400d-8244-19ef4b5ebf78" />


---

### 2. Clase LibroCalificaciones1

La clase `LibroCalificaciones1` implementa una segunda forma de calcular el promedio de una clase.

A diferencia de la primera implementación, este método utiliza un **valor centinela (****`-1`****)** para indicar que el usuario desea finalizar el ingreso de calificaciones.

El método `DeterminaPromedioClase1()` utiliza un ciclo `while` para recibir las calificaciones, acumularlas y contar la cantidad de valores introducidos.

Al finalizar, se verifica mediante una estructura `if/else` si se ingresaron calificaciones antes de calcular el promedio.

#### Ingreso de calificaciones

<img width="542" height="190" alt="image" src="https://github.com/user-attachments/assets/bbc15454-dc89-4335-b2e4-617b728488c2" />


#### Resultado del promedio

<img width="646" height="70" alt="image" src="https://github.com/user-attachments/assets/6909f20c-265a-4913-9ca4-59ec6a84b18c" />


#### Caso sin calificaciones

<img width="522" height="65" alt="image" src="https://github.com/user-attachments/assets/592ae2b9-c7b5-4735-8c22-39102fb20e92" />


---

### 3. Clase PruebaLibroCalificaciones

La clase `PruebaLibroCalificaciones` contiene el método principal `Main()` del programa.

Desde este método se crean dos objetos:

```csharp
LibroCalificaciones miLibroCalificaciones =
    new LibroCalificaciones(
        "CS101 Introducción a la programación en C#");

LibroCalificaciones1 miLibroCalificaciones1 =
    new LibroCalificaciones1(
        "CS102 Indroduccion a Java");
```

Posteriormente, se invocan los métodos correspondientes para mostrar el mensaje de bienvenida y calcular el promedio de cada curso.

#### Ejecución completa

<img width="902" height="507" alt="image" src="https://github.com/user-attachments/assets/cca1087f-7940-4cf6-a7c6-87362a56fcdb" />


---

## Conceptos Aplicados

Durante el desarrollo de esta actividad se aplicaron los siguientes conceptos:

### Clases y objetos

Se crearon las clases `LibroCalificaciones`, `LibroCalificaciones1` y `PruebaLibroCalificaciones`.

También se crearon objetos de las clases `LibroCalificaciones` y `LibroCalificaciones1` desde el método `Main()`.

### Constructores

Los constructores permiten inicializar el nombre del curso al momento de crear cada objeto.

### Propiedades

Se utilizó la propiedad `NombreCurso` para obtener y modificar el nombre del curso mediante los métodos `get` y `set`.

### Métodos

Se implementaron métodos para mostrar mensajes y realizar el cálculo de los promedios:

```text
MostrarMensaje()
DeterminarPromedioClase()
DeterminaPromedioClase1()
```

### Estructura repetitiva `while`

La clase `LibroCalificaciones1` utiliza un ciclo `while` para continuar solicitando calificaciones hasta que el usuario introduzca `-1`.

### Estructuras condicionales

Se utiliza `if/else` para verificar si se introdujeron calificaciones antes de calcular el promedio.

### Valor centinela

El valor `-1` se utiliza como indicador para finalizar el ingreso de calificaciones en la clase `LibroCalificaciones1`.

---

## Estructura de Carpetas o Directorios

La estructura del repositorio puede organizarse de la siguiente manera:

```text
Actividad-3/
│
├── Actividad__3/
│   ├── Program.cs
│   ├── LibroCalificaciones.cs
│   ├── LibroCalificaciones1.cs
│   └── ...
│
│
│
└── README.md
```

>

---

## Instrucciones de Ejecución / Uso

### 1. Clonar el repositorio

Clonar el repositorio desde GitHub:

```bash
git clone [URL_DEL_REPOSITORIO]
```

### 2. Abrir el proyecto

Abrir el archivo de solución `.sln` utilizando **Visual Studio**.

### 3. Ejecutar el programa

Ejecutar la aplicación utilizando el botón **Iniciar** de Visual Studio o presionando:

```text
F5
```

### 4. Ingresar las calificaciones

Para el primer libro de calificaciones:

* Introducir las **10 calificaciones** solicitadas.
* El programa mostrará el total de calificaciones y el promedio.

Para el segundo libro de calificaciones:

* Introducir las calificaciones que se deseen.
* Introducir `-1` para finalizar.
* El programa mostrará el total y el promedio de las calificaciones introducidas.

---

## Autor y Contexto

**Nombre:** Michael Hunt
**Materia:** HPA III
**Institución:** Universidad Tecnológica de Panamá (UTP)
**Actividad:** Actividad #3 - Libro de Calificaciones
**Fecha de Realización:** 07/09/2026

---

## Conclusión

Esta actividad permitió aplicar conceptos fundamentales de programación en **C#**, especialmente el uso de clases, objetos, constructores, propiedades y métodos.

También se practicó el uso de estructuras repetitivas y condicionales para procesar las calificaciones y calcular el promedio de una clase mediante dos métodos diferentes: utilizando una cantidad fija de 10 calificaciones y utilizando un valor centinela para determinar cuándo finalizar el ingreso de datos.

