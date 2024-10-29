# 4-TAREA-1INT46-PUCP-

# Diccionario de Datos de COVID-19 en Perú

Este repositorio contiene información detallada sobre los registros de fallecidos y casos positivos de COVID-19 en Perú, extraídos de la plataforma de datos abiertos del Ministerio de Salud (MINSA).

## 1. Descripción de los Datos

### Fallecidos por COVID-19 - [Ministerio de Salud - MINSA]

**Categoría:** COVID-19, Salud  
**Descripción:**  
El dataset contiene el registro diario de muertes confirmadas por COVID-19 en Perú. Cada registro representa a una persona fallecida, caracterizada por variables como sexo, edad, y ubicación geográfica (hasta nivel de distrito). Desde el 06 de mayo de 2021, se incluyó el código de ubicación geográfica UBIGEO. A partir del 31 de mayo de 2021, se amplió la definición de fallecidos para incluir aquellos que cumplen con al menos uno de los siguientes siete criterios:

1. **Criterio virológico:** Fallecimiento en los 60 días posteriores a una prueba molecular (PCR) o antigénica positiva para SARS-CoV-2.
2. **Criterio serológico:** Fallecimiento en los 60 días posteriores a una prueba serológica positiva para SARS-CoV-2.
3. **Criterio radiológico:** Fallecimiento con imagen radiológica compatible con neumonía COVID-19.
4. **Criterio nexo epidemiológico:** Fallecimiento con nexo epidemiológico a un caso confirmado.
5. **Criterio investigación epidemiológica:** Verificación del fallecimiento por la Red Nacional de Epidemiología (RENACE).
6. **Criterio clínico:** Cuadro clínico compatible con COVID-19.
7. **Criterio SINADEF:** Diagnóstico de COVID-19 en el certificado de defunción (CIE-10: U071, U072, B342, B972 o términos asociados).

Para más información, consulta la [Resolución Ministerial N° 095-2021-PCM](https://cdn.www.gob.pe/uploads/document/file/1920118/Informe%20final%20del%20grupo%20de%20trabajo%20te%CC%81cnico%20con%20cifra%20de%20fallecidos%20por%20la%20COVID-19.pdf.pdf).

**Fuente:** Centro Nacional de Epidemiología, Prevención y Control de Enfermedades – MINSA.  
**Frecuencia de Actualización:** Diaria  
**Fecha de corte:** 28/10/2024

---

### Casos Positivos por COVID-19 - [Ministerio de Salud - MINSA]

**Categoría:** COVID-19, Salud  
**Descripción:**  
Este dataset contiene el registro diario de casos positivos de COVID-19 confirmados mediante cualquier tipo de prueba y que presentan síntomas. Cada registro corresponde a una persona caracterizada por sexo, edad, y ubicación geográfica hasta nivel de distrito.

Consulta la [Directiva Sanitaria para la Vigilancia Epidemiológica del Coronavirus en Perú](https://www.gob.pe/institucion/minsa/normas-legales/1322786-905-2020-minsa) para conocer los lineamientos de identificación de casos. Desde el 02 de junio de 2020, los casos confirmados por pruebas rápidas no incluyen los realizados en IPRESS privadas que tamizan trabajadores de empresas para la reactivación económica.

**Fuente:** Instituto Nacional de Salud y Centro Nacional de Epidemiología, Prevención y Control de Enfermedades – MINSA.  
**Frecuencia de Actualización:** Diaria  
**Fecha de corte:** 28/10/2024

## 2. Diccionario de Variables

### Variables para Fallecidos por COVID-19

| Variable               | Descripción                                                                                       |
|------------------------|---------------------------------------------------------------------------------------------------|
| `FECHA_CORTE`          | Fecha de corte de información                                                                     |
| `UUID`                 | ID de la persona fallecida por COVID-19                                                           |
| `FECHA_FALLECIMIENTO`  | Fecha del fallecimiento atribuido a COVID-19                                                      |
| `EDAD_DECLARADA`       | Edad de la persona fallecida por COVID-19                                                         |
| `SEXO`                 | Sexo de la persona fallecida por COVID-19                                                         |
| `CLASIFICACION_DEF`    | Criterio de confirmación de defunción por COVID-19                                                |
| `UBIGEO`               | Código de ubicación geográfica (Departamento, provincia, distrito)                                |
| `DEPARTAMENTO`         | Departamento de residencia de la persona fallecida                                                |
| `PROVINCIA`            | Provincia de residencia de la persona fallecida                                                   |
| `DISTRITO`             | Distrito de residencia de la persona fallecida                                                    |

### Variables para Casos Positivos por COVID-19

| Variable               | Descripción                                                                                       |
|------------------------|---------------------------------------------------------------------------------------------------|
| `FECHA_CORTE`          | Fecha de corte de información                                                                     |
| `UUID`                 | ID de la persona como caso positivo confirmado de COVID-19                                        |
| `UBIGEO`               | Código de ubicación geográfica (Departamento, provincia, distrito)                                |
| `DEPARTAMENTO`         | Departamento de residencia de la persona confirmada como caso positivo                            |
| `PROVINCIA`            | Provincia de residencia de la persona confirmada como caso positivo                               |
| `DISTRITO`             | Distrito de residencia de la persona confirmada como caso positivo                                |
| `METODODX`             | Método de diagnóstico de laboratorio de COVID-19                                                  |
| `EDAD`                 | Edad de la persona confirmada como caso positivo                                                  |
| `SEXO`                 | Sexo de la persona confirmada como caso positivo                                                  |
| `FECHA_RESULTADO`      | Fecha del resultado de la prueba de COVID-19                                                      |

## 3. Actualización de Datos

La información se actualiza diariamente, y la fecha de corte de los datos incluidos en este repositorio es el **28/10/2024**.

---

**Nota:** Este diccionario de datos se basa en las definiciones y directrices publicadas por el MINSA y el Instituto Nacional de Salud de Perú.


