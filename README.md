# CreaTuCuento - Creador de Cuentos Infantiles Terapeuticos

## Descripcion

**CreaTuCuento** es una aplicacion web interactiva monolitica (archivo HTML unico) disenada para la creacion de cuentos infantiles con fines terapeuticos. La herramienta transforma perfiles psicologicos detallados en historias magicas personalizadas, aplicando principios de biblioterapia, narrativa terapeutica y reestructuracion cognitiva.

Este archivo HTML autonomo no requiere servidor, compilacion ni dependencias externas (salvo una conexion a CDN para la generacion de PDF). Funciona completamente en el navegador del usuario.

---

## Caracteristicas Principales

| Modulo | Descripcion |
|--------|-------------|
| **Formulario de Perfil** | 9 secciones colapsables para capturar datos del estudiante, personaje principal, secundarios, antecedentes, actitud, talentos, interaccion social y condiciones |
| **24 Metaforas Terapeuticas** | Cada condicion psicologica se transforma en metafora magica (animal, objeto o espectro) con descripciones narrativas detalladas |
| **5 Estados de Transformacion** | Humano, Animal, Objeto Inerte, Objeto Bidimensional y Espectro - cada uno con simbolismo terapeutico propio |
| **Personajes Secundarios (1-3)** | Configuracion de apoyo con 10 tipos de roles terapeuticos distintos |
| **Diagrama de Flujo Narrativo** | 5 pasos interactivos que estructuran el arco dramatico terapeutico |
| **Guion Tecnico** | 5 escenas con duracion, tono y elementos clave |
| **5 Cuentos Sugeridos** | Historias predefinidas por valor educativo (empatia, perseverancia, solidaridad, coraje, honestidad) |
| **Generador de Cuento** | Motor de narrativa que integra todo el perfil en una historia coherente |
| **Reporte PDF** | Generacion profesional de informe completo con html2pdf.js |
| **Arco Narrativo** | Grafico SVG integrado en el reporte mostrando la intensidad emocional |

---

## Requisitos

- Navegador web moderno (Chrome, Firefox, Edge, Safari)
- Conexion a internet (unicamente para el CDN de html2pdf.js y la carga inicial)
- JavaScript habilitado

---

## Como Usar

### 1. Abrir el archivo

Simplemente abre el archivo `index.html` (o `CreaTuCuento_Completo.html`) en cualquier navegador web. No necesitas servidor web ni instalacion adicional.

```bash
# Opcion A: Doble clic en el archivo
# Opcion B: Desde terminal
open index.html

# Opcion C: Con servidor local (opcional)
python3 -m http.server 8000
# Luego visitar http://localhost:8000
```

### 2. Completar el formulario

Sigue las secciones del acordeon en orden:

| Seccion | Contenido |
|---------|-----------|
| **0. Datos del Estudiante** | Nombre, apellidos y fecha de desarrollo |
| **1. Personaje Principal** | Nombre, edad, genero, descripcion fisica y de personalidad |
| **2. Personajes Secundarios** | Hasta 3 personajes con nombre, relacion y tipo de apoyo |
| **3. Antecedentes** | Contexto familiar, escolar y medico |
| **4. Actitud** | Comportamiento en casa, escuela y con companeros |
| **5. Talentos** | Habilidades, intereses y estilo de aprendizaje |
| **6. Social** | Habilidades sociales, comunicacion y regulacion emocional |
| **7. Condiciones** | Seleccion de condiciones con metaforas magicas (pasa el mouse sobre las i para ver) |
| **8. Configuracion** | Edad objetivo, genero, duracion, tono, valores y objetivo terapeutico |

### 3. Seleccionar transformacion

En la seccion "Transformacion del Personaje", elige uno de los 5 estados disponibles haciendo clic en la tarjeta correspondiente:

- Humano (predeterminado)
- Animal
- Objeto Inerte
- Objeto Bidimensional
- Espectro

### 4. Generar el cuento

Haz clic en el boton **"Generar Cuento Magico"**. El sistema procesara toda la informacion y generara una historia personalizada.

### 5. Generar el reporte PDF

Una vez generado el cuento, ve a la seccion "Reporte Completo en PDF" y haz clic en **"Generar Reporte PDF"**. El documento incluira:

- Portada profesional
- Datos del estudiante y personaje
- Tablas de antecedentes y evaluacion
- Metaforas seleccionadas con descripciones
- Cuento terapeutico generado
- Guion tecnico narrativo
- Arco narrativo grafico (SVG)
- Notas para el terapeuta
- Espacios para firmas

---

## Estructura del Archivo

El archivo es monolitico y contiene tres componentes integrados:

```
CreaTuCuento_Completo.html
|
|-- <style>        CSS completo (variables, grid, flexbox, animaciones, responsive)
|-- <body>         Estructura HTML (navegacion, hero, formulario, secciones, pie)
|-- <script>       JavaScript vanilla (motor de metaforas, generador, PDF)
```

**Tamano**: ~106 KB (sin compresion)

---

## Dependencias Externas

| Dependencia | Uso | CDN |
|-------------|-----|-----|
| html2pdf.js | Generacion de PDF del reporte | cdnjs.cloudflare.com |

---

## Sistema de Metaforas

La herramienta incluye 24 condiciones con metaforas magicas organizadas en tres categorias:

- **Metafora Animal**: Transformacion en criatura con caracteristicas especiales
- **Metafora Objeto**: Conversion en artefacto magico con conciencia
- **Metafora Espectro**: Forma eterea con poderes unicos

Condiciones disponibles: TDAH, TEA, Ansiedad, Depresion Infantil, TND, Ansiedad por Separacion, Mutismo Selectivo, TEPT Infantil, Bipolaridad Infantil, Tics, Trastorno de Aprendizaje, Trastorno de Alimentacion, Enuresis/Encopresis, Trastornos del Sueno, Incumplimiento Terapeutico, Duelo Infantil, Secuelas de Abuso, Proceso de Adopcion, Divorcio Parental, Fobias, Baja Autoestima, Agresividad, Dificultades Sociales, Ritualidades Obsesivas.

---

## Tipos de Apoyo (Personajes Secundarios)

1. Apoyo Emocional - Escucha y consuela
2. Apoyo Motivacional - Anima a seguir adelante
3. Apoyo Inteligente - Ayuda a resolver problemas
4. Apoyo Protector - Cuida y defiende
5. Apoyo Comico - Alivia tension con humor
6. Apoyo de Sabiduria - Comparte consejos
7. Apoyo de Fuerza - Proporciona coraje
8. Apoyo Creativo - Inspira ideas nuevas
9. Apoyo de Lealtad - Permanece siempre
10. Apoyo Practico - Ayuda con recursos

---

## Diagrama de Flujo Narrativo

La estructura narrativa sigue 5 pasos fundamentales:

1. **Presentacion del Mundo** - Contexto y conexion emocional
2. **Llamado a la Aventura** - Conflicto y duda normalizada
3. **Transformacion y Pruebas** - Metaforas magicas activas
4. **Crisis y Eleccion** - Punto maximo, decision valiente
5. **Resolucion** - Triunfo emocional, mensaje terapeutico

---

## Valores Educativos Disponibles

Empatia, Responsabilidad, Solidaridad, Tolerancia, Respeto, Honestidad, Perseverancia, Creatividad, Coraje, Amistad, Humildad, Generosidad (seleccion de hasta 3).

---

## Consideraciones Eticas

Esta herramienta es un complemento para profesionales de la salud mental y la educacion. No sustituye evaluacion clinica ni tratamiento psicologico profesional. En casos que involucren abuso, automutilacion o ideacion suicida, derive inmediatamente a servicios especializados.

---

## Licencia y Uso

Herramienta educativa para formacion en psicologia infantil, biblioterapia y narrativa terapeutica. Uso academico y profesional.
