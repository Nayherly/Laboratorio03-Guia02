# Evidencia SonarCloud — Laboratorio 02

## Datos del proyecto
| Campo        | Valor                          |
|--------------|--------------------------------|
| Proyecto     | [Evidencia Sonar Cloud]        |
| URL          | [https://sonarcloud.io/project/overview?id=Nayherly_Laboratorio03-Guia02] |
| Fecha        | 09/05/2026                     |

---

## Dashboard principal
![Dashboard SonarCloud](https://raw.githubusercontent.com/Nayherly/Laboratorio03-Guia02/QANayherly/QA/image-1.png)

**Quality Gate Status: ✅ PASSED — All conditions passed**

El análisis automático de SonarCloud arrojó los siguientes resultados:


## Quality Gate


| Métrica          | Resultado         | Descripción                                      |
|------------------|-------------------|--------------------------------------------------|
| Quality Gate     | PASSED            | Todas las condiciones de calidad fueron superadas |
| Open Issues      | 4                 | Existen 4 issues abiertos en el código           |
| Duplications     | 0.0%              | No se detectó código duplicado                   |
| Coverage         | Sin datos         | No se configuraron pruebas unitarias aún         |
| Security Rating  | A                 | Calificación máxima en seguridad                 |
| Security Issues  | 0                 | No se encontraron vulnerabilidades de seguridad  |


## Interpretación de resultados

- **Quality Gate PASSED:** el código cumple con los umbrales mínimos de calidad
  establecidos por SonarCloud.
- **4 Open Issues:** SonarCloud detectó 4 problemas abiertos, relacionados
  principalmente con malas prácticas de código (code smells) como el uso de
  `var` y comparaciones no estrictas.
- **Security Rating A:** no se encontraron vulnerabilidades de seguridad,
  lo cual indica que el código no expone datos ni tiene riesgos críticos.
- **0% Duplicación:** el código no tiene bloques repetidos, lo que favorece
  la mantenibilidad.
- **Sin cobertura:** no existe aún una suite de pruebas unitarias (.test.js),
  por lo que SonarCloud no puede medir la cobertura del código.