# Informe de Revisión Estática — Laboratorio 02
## IS-489 Pruebas y Aseguramiento de Calidad de Software

## Presentación

| Campo           | Valor                              |
|-----------------|------------------------------------|
| Integrante 1    | Vila Cayo Nayherly Dianeth                 |
| Fecha           | 09/05/2026                         |
| Módulo revisado | src/products.js                    |
| URL SonarCloud  | [https://sonarcloud.io/project/overview?id=Nayherly_Laboratorio03-Guia02]  |
|Repositorio      |[https://github.com/Nayherly/Laboratorio03-Guia02]|


## Resumen del trabajo realizado

### Rama QANayherly
- Se ejecutó ESLint sobre `src/products.js`
- Se identificaron **4 errors y 4 warnings**
- Se documentaron los hallazgos en `QA/resultado-qa.md`
- Se analizó el proyecto con SonarCloud — **Quality Gate: PASSED**
- Se documentó la evidencia en `QA/SonarCloud.md`

### Rama dev
- Se corrigieron todos los errores identificados en QA
- Se verificó con ESLint — **0 errors, 0 warnings** ✅
- Se agregó documentación JSDoc a todas las funciones
- Se corrigieron precios inválidos (null, undefined, negativos)
- Se corrigió comparación `==` por `===`
- Se reemplazó `var` por `const/let`

## Errores encontrados y corregidos

| # | Línea | Tipo    | Descripción                          | Estado    |
|---|-------|---------|--------------------------------------|-----------|
| 1 | 14    | error   | Comparación == en lugar de ===       | Corregido |
| 2 | 3,11,12,25 | warning | Uso de var en lugar de const/let | Corregido |
| 3 | 13,22,29 | error | console no definido en globals      | Corregido |
| 4 | 2-5   | error   | Precios null, undefined y negativos  | Corregido |
| 5 | 25    | error   | calculateDiscount sin validación     | Corregido |


## Informe monográfico (Word)

El informe completo en formato Word está disponible en Google Drive:
 [Ver informe monográfico completo](https://docs.google.com/document/d/1qWLgMJPVzyDIxqsLy4niHUI0GQeRRKRfsZeYK0nJA6w/edit?usp=sharing)

## Conclusión

ESLint detectó automáticamente los errores de sintaxis y estilo antes del commit.
La revisión manual con checklist permitió detectar errores de lógica de negocio
que ESLint no puede ver. SonarCloud complementó el análisis con métricas de
calidad a nivel de proyecto. Las tres herramientas juntas garantizan la calidad
del código antes del merge a main.