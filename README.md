# Practica Semana 9 - Pruebas unitarias: Ecuacion cuadratica

Resolvedor de ecuaciones de segundo grado (ax^2 + bx + c = 0) con pruebas unitarias en `unittest`.

## Archivos
- `ecuacion.py`: funcion `resolver_ecuacion(a, b, c)` que devuelve un diccionario con `tipo` y `soluciones`.
- `test_ecuacion.py`: 6 pruebas base + 5 pruebas del reto (11 en total).

## Como ejecutar
python -m unittest test_ecuacion -v

## Casos cubiertos
| Prueba | Caso |
|---|---|
| test_dos_soluciones_reales | D > 0 |
| test_una_solucion | D = 0 (raiz doble) |
| test_sin_solucion_real | D < 0 |
| test_ecuacion_lineal | a = 0 |
| test_coeficientes_invalidos | a = 0 y b = 0 → ValueError |
| test_multiples_casos_con_subTest | Varios casos con subTest |
| test_coeficientes_grandes | Coeficientes de 1 000 000 |
| test_precision_decimal | Raiz de 2 con places=10 |
| test_x_cuadrado_igual_cero | x^2 = 0 → x = 0 |
| test_a_negativo | a = -1 |
| test_todos_cero | (0, 0, 0) → ValueError |

## Observacion
En la guia, `test_una_solucion` comparaba la lista `[1.0]` con `1.0` y fallaba. Se corrigio usando `res["soluciones"][0]`.

## Equipo
- Lider de proyecto: Ruth estefani huaman mamani
- Desarrollador principal: Eduardo Puma Ccorimanya
- Revisor de codigo: Junior
- Documentador: Eduardo Puma Ccorimanya
