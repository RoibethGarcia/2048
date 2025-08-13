# 2048Pro - Juego de 2048 en C++

## 🎮 Descripción
2048Pro es una implementación completa del popular juego 2048 desarrollada en C++. El juego incluye un sistema de gestión de usuarios que permite a múltiples jugadores registrarse, jugar y competir por el puntaje más alto.

## ✨ Características Principales

### 👥 Sistema de Usuarios
- **Registro de usuarios**: Cada jugador puede crear un perfil con:
  - Alias (máximo 5 caracteres)
  - Nombre y apellido
  - Edad
  - Puntaje máximo personal
- **Gestión de perfiles**: Ver datos de usuarios registrados
- **Listado de jugadores**: Muestra todos los usuarios registrados

### 🎯 Mecánica del Juego
- **Tablero 4x4**: Matriz de números donde el objetivo es alcanzar el número 2048
- **Movimientos**: Utiliza las teclas WASD para mover las fichas:
  - **W**: Mover hacia arriba
  - **A**: Mover hacia la izquierda
  - **S**: Mover hacia abajo
  - **D**: Mover hacia la derecha
  - **E**: Salir del juego
- **Fusión de números**: Los números iguales se combinan al moverse en la misma dirección
- **Generación de nuevos números**: Después de cada movimiento válido, aparece un nuevo 2 o 4 en una posición aleatoria

### 🏆 Sistema de Puntuación
- **Puntaje máximo**: Se calcula basado en el número más alto alcanzado en el tablero
- **Victoria**: Alcanzar el número 2048
- **Derrota**: Cuando no hay más movimientos posibles

## 🚀 Funcionalidades del Programa

### Menú Principal
El programa presenta un menú interactivo con las siguientes opciones:

1. **R - Registrar**: Crear un nuevo perfil de usuario
2. **L - Listado**: Mostrar todos los usuarios registrados
3. **J - Jugar**: Iniciar una partida de 2048
4. **D - Datos**: Ver información detallada de un usuario específico
5. **E - Eliminar**: Eliminar un usuario (funcionalidad pendiente)
6. **S - Salir**: Terminar el programa

### Estructura del Código

#### Estructuras de Datos
```cpp
struct Usuario {
    int numero;           // Número de usuario
    char alias[5];        // Alias del jugador
    char nombre[20];      // Nombre del jugador
    char apellido[20];    // Apellido del jugador
    int edad;            // Edad del jugador
    int puntajeMax;      // Puntaje máximo alcanzado
};
```

#### Funciones Principales
- `registrar()`: Crea un nuevo usuario
- `lista()`: Muestra todos los usuarios registrados
- `datos()`: Muestra información detallada de un usuario
- `juego()`: Lógica principal del juego 2048
- `leer_linea()`: Función auxiliar para leer entrada de texto

## 🎮 Cómo Jugar

1. **Registrarse**: Selecciona 'R' y completa tus datos
2. **Iniciar partida**: Selecciona 'J' e ingresa tu alias
3. **Mover fichas**: Usa WASD para mover las fichas en el tablero
4. **Combinar números**: Mueve fichas iguales para que se fusionen
5. **Alcanzar 2048**: El objetivo es crear el número 2048
6. **Salir**: Presiona 'E' para terminar la partida

## 📋 Reglas del Juego

- **Movimiento**: Solo se pueden mover fichas hacia espacios vacíos o hacia fichas del mismo valor
- **Fusión**: Dos fichas del mismo valor se combinan en una sola al moverse juntas
- **Generación**: Después de cada movimiento, aparece una nueva ficha (2 o 4)
- **Victoria**: Crear una ficha con el valor 2048
- **Derrota**: Cuando no hay más movimientos posibles

## 🔧 Compilación y Ejecución

### Requisitos
- Compilador de C++ (gcc, clang, etc.)
- Sistema operativo compatible con C++

### Compilar
```bash
g++ -o 2048Pro 2048Pro.cpp
```

### Ejecutar
```bash
./2048Pro
```

## 📁 Estructura del Proyecto
```
2048Pro/
├── 2048Pro.cpp    # Código fuente principal
├── README.md      # Este archivo
└── .gitignore     # Archivos a ignorar por Git
```

## ⚠️ Limitaciones Actuales

- Máximo 10 usuarios registrados
- No hay persistencia de datos (se pierden al cerrar el programa)
- Función de eliminar usuarios no implementada
- No hay validación de alias duplicados
- Interfaz de texto simple

## 🔮 Mejoras Futuras Sugeridas

- [ ] Persistencia de datos en archivo
- [ ] Validación de alias duplicados
- [ ] Implementar función de eliminar usuarios
- [ ] Interfaz gráfica
- [ ] Sistema de rankings
- [ ] Diferentes niveles de dificultad
- [ ] Estadísticas de juego más detalladas
- [ ] Modo multijugador
- [ ] Tabla de puntuaciones global

## 👨‍💻 Autor
Programa desarrollado en C++ como proyecto educativo.

## 📄 Licencia
Este proyecto es de uso educativo y personal.

## 🤝 Contribuciones
Las contribuciones son bienvenidas. Por favor, abre un issue o un pull request para sugerir mejoras.

## 📞 Contacto
Para preguntas o sugerencias sobre este proyecto, puedes contactar al desarrollador.

---

**¡Disfruta jugando 2048Pro! 🎉**

