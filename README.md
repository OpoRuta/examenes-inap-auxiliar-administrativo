# Exámenes INAP — Auxiliar Administrativo del Estado (C2)

Preguntas oficiales de los exámenes del INAP para el Cuerpo General Auxiliar de la Administración del Estado, en formato JSON estructurado.

Los exámenes del INAP son **dominio público**. Este repositorio los ofrece en formato legible por máquina para facilitar su uso por investigadores, desarrolladores y opositores.

## Convocatorias disponibles

| Convocatoria | Preguntas | Archivos | Fuente |
|---|---|---|---|
| **2024** | 80 (modelo A + B) | [`examenes/2024/`](examenes/2024/) | INAP — Convocatoria Auxiliar AGE 2024 |
| **2022** | 100 | [`examenes/2022/`](examenes/2022/) | INAP — Convocatoria Auxiliar AGE 2022 |
| **2019** | 60 | [`examenes/2019/`](examenes/2019/) | INAP — Convocatoria Auxiliar AGE 2019 |
| **2018** | 51 (modelo A + B) | [`examenes/2018/`](examenes/2018/) | INAP — Convocatoria Auxiliar AGE 2018 |

**Total: ~290 preguntas oficiales** de 4 convocatorias.

## Formato JSON

Cada archivo sigue esta estructura:

```json
{
  "convocatoria": "2024",
  "anno": 2024,
  "turno": "libre",
  "modelo": "A",
  "total_preguntas": 40,
  "preguntas": [
    {
      "numero": 1,
      "enunciado": "¿Cuál de los siguientes sistemas numéricos...?",
      "opciones": [
        "Hexadecimal",
        "Binario",
        "Decimal",
        "Octal"
      ],
      "correcta": 3
    }
  ]
}
```

| Campo | Tipo | Descripción |
|---|---|---|
| `convocatoria` | string | Año de la convocatoria |
| `anno` | number | Año numérico |
| `turno` | string | Siempre "libre" |
| `modelo` | string \| null | "A", "B" o null si modelo único |
| `total_preguntas` | number | Número de preguntas en el archivo |
| `preguntas[].numero` | number | Número de pregunta (1-indexed) |
| `preguntas[].enunciado` | string | Texto de la pregunta |
| `preguntas[].opciones` | string[] | 4 opciones de respuesta |
| `preguntas[].correcta` | number | Índice de la respuesta correcta (0-indexed) |

## Sobre el examen

- **Oposición:** Cuerpo General Auxiliar de la Administración del Estado (Subgrupo C2)
- **Convocatoria vigente:** 1.700 plazas de acceso libre (BOE 22/12/2025, RD 651/2025)
- **Formato:** Ejercicio único, 100 preguntas puntuables + 10 de reserva, 90 minutos
- **Penalización:** -1/3 del valor de un acierto por respuesta incorrecta
- **Temario:** 28 temas — 16 de Organización Pública (Bloque I) + 12 de Ofimática (Bloque II)

## Análisis de frecuencia

¿Quieres saber qué artículos de la legislación pregunta el INAP con más frecuencia? Hemos analizado las 4 convocatorias y publicado los resultados:

**[Análisis de frecuencia de artículos INAP (2018-2024)](https://oporuta.es/blog/analisis-frecuencia-articulos-inap-auxiliar-administrativo)** — Los 15 artículos más preguntados, desglose por ley, y patrones del tribunal.

## Practicar con estos exámenes

Puedes practicar estos exámenes de forma interactiva (con cronómetro, penalización real y explicaciones de cada error) en **[OpoRuta](https://oporuta.es/examenes-oficiales)** — plataforma de preparación para Auxiliar Administrativo con IA y verificación determinista de citas legales.

- [Simulacro INAP 2024](https://oporuta.es/examenes-oficiales/inap-2024)
- [Simulacro INAP 2022](https://oporuta.es/examenes-oficiales/inap-2022)
- [Simulacro INAP 2019](https://oporuta.es/examenes-oficiales/inap-2019)
- [Simulacro INAP 2018](https://oporuta.es/examenes-oficiales/inap-2018)

## Licencia

Los exámenes del INAP son documentos públicos de la Administración General del Estado.

Este repositorio y su estructuración en JSON están bajo [MIT License](LICENSE).

---

Mantenido por [OpoRuta](https://oporuta.es) — Prepara tu oposición con IA verificada.
