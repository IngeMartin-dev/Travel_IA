# Lógica del Proyecto - Travel AI

## Descripción

Este documento explica la lógica del proyecto desarrollado en Scratch, detallando cada bloque utilizado, la sección a la que pertenece y su función dentro del programa.

---

# Flujo General

```text
Inicio
   │
   ▼
El usuario escribe un país
   │
   ▼
El programa compara la respuesta
   │
   ├── Si es "Colombia"
   │        │
   │        ▼
   │   Muestra la lista de destinos
   │
   └── Si no
            │
            ▼
     Informa que el país no está disponible
```

---

# Bloque 1 - Inicio del programa

## Sección

**Eventos (amarillo)**

## Bloque

```scratch
al presionar bandera verde
```

## Función

Este bloque inicia la ejecución del programa cuando el usuario presiona la bandera verde.

### Evidencia

```md
![Bloque Inicio](../public/Sin%20título.jpg)
```

---

# Bloque 2 - Solicitar información

## Sección

**Sensores (celeste)**

## Bloque

```scratch
preguntar [¿Qué país deseas visitar?] y esperar
```

## Función

Solicita al usuario escribir el nombre del país que desea consultar y espera su respuesta.

### Evidencia

```md
![Bloque Preguntar](../img/bloque_preguntar.png)
```

---

# Bloque 3 - Comparación

## Sección

**Control (naranja)**

## Bloque

```scratch
si <> entonces
```

## Función

Permite ejecutar una acción únicamente cuando se cumple una condición.

### Evidencia

```md
![Bloque Si](../img/bloque_si.png)
```

---

# Bloque 4 - Condición

## Sección

**Operadores (verde)**

## Bloque

```scratch
(respuesta) = (Colombia)
```

## Función

Compara el texto escrito por el usuario con la palabra **Colombia**.

Si ambos textos son iguales, el resultado es verdadero.

### Evidencia

```md
![Bloque Operador](../img/bloque_operador.png)
```

---

# Bloque 5 - Respuesta del usuario

## Sección

**Sensores (celeste)**

## Bloque

```scratch
respuesta
```

## Función

Obtiene el texto que escribió el usuario después de la pregunta.

### Evidencia

```md
![Bloque Respuesta](../img/bloque_respuesta.png)
```

---

# Bloque 6 - Mostrar información

## Sección

**Apariencia (morado)**

## Bloque

```scratch
decir [🇨🇴 Colombia]
```

## Función

Informa al usuario que el país fue encontrado.

### Evidencia

```md
![Bloque Decir](../img/bloque_decir.png)
```

---

# Bloque 7 - Mostrar destinos

## Sección

**Apariencia (morado)**

## Bloque

```scratch
decir [1. Bogotá

2. Medellín

3. Cartagena

4. Santa Marta

5. Cali]
```

## Función

Muestra la lista de ciudades recomendadas para visitar en Colombia.

### Evidencia

```md
![Bloque Lista](../img/bloque_lista.png)
```

---

# Lógica Completa

```text
Bandera Verde
      │
      ▼
Preguntar país
      │
      ▼
Guardar respuesta
      │
      ▼
¿Respuesta = Colombia?
      │
 ┌────┴─────┐
 │          │
Sí          No
 │          │
 ▼          ▼
Mostrar    Mostrar
lista      "País no disponible"
```

---

# Resultado Esperado

Si el usuario escribe:

```text
Colombia
```

El programa responderá:

```text
🇨🇴 Colombia

1. Bogotá
2. Medellín
3. Cartagena
4. Santa Marta
5. Cali
```

Si escribe cualquier otro país, el programa mostrará un mensaje indicando que la información aún no está disponible.
