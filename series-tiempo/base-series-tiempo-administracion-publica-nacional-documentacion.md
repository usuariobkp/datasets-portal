# Base de Series de Tiempo de la Administración Pública Nacional

Base de series de tiempo de distintas fuentes primarias y secundarias de la Administración Pública Nacional, compilada por el Ministerio de Modernización. Estas series son normalizadas por organismos de la APN de acuerdo a los estandares propuestos por Modernización.

## Recursos del dataset

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Base de Series de Tiempo: valores y metadatos (CSV)](#base-de-series-de-tiempo-valores-y-metadatos-csv)
- [Base de Series de Tiempo: metadatos enriquecidos de las series (CSV)](#base-de-series-de-tiempo-metadatos-enriquecidos-de-las-series-csv)
- [Base de Series de Tiempo: valores (CSV)](#base-de-series-de-tiempo-valores-csv)
- [Base de Series de Tiempo: fuentes (CSV)](#base-de-series-de-tiempo-fuentes-csv)
- [Base de Series de Tiempo: valores y metadatos (XLSX)](#base-de-series-de-tiempo-valores-y-metadatos-xlsx)
- [Base de Series de Tiempo: metadatos enriquecidos de las series (XLSX)](#base-de-series-de-tiempo-metadatos-enriquecidos-de-las-series-xlsx)
- [Base de Series de Tiempo: valores (XLSX)](#base-de-series-de-tiempo-valores-xlsx)
- [Base de Series de Tiempo: fuentes (XLSX)](#base-de-series-de-tiempo-fuentes-xlsx)
- [Base de Series de Tiempo: valores y metadatos (DTA)](#base-de-series-de-tiempo-valores-y-metadatos-dta)
- [Base de Series de Tiempo: metadatos enriquecidos de las series (DTA)](#base-de-series-de-tiempo-metadatos-enriquecidos-de-las-series-dta)
- [Base de Series de Tiempo: valores (DTA)](#base-de-series-de-tiempo-valores-dta)
- [Base de Series de Tiempo: fuentes (DTA)](#base-de-series-de-tiempo-fuentes-dta)
- [Base de Series de Tiempo: valores y metadatos (DB)](#base-de-series-de-tiempo-valores-y-metadatos-db)
- [Base de Series de Tiempo: metadatos enriquecidos de las series (DB)](#base-de-series-de-tiempo-metadatos-enriquecidos-de-las-series-db)
- [Base de Series de Tiempo: valores (DB)](#base-de-series-de-tiempo-valores-db)
- [Base de Series de Tiempo: fuentes (DB)](#base-de-series-de-tiempo-fuentes-db)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

### Base de Series de Tiempo: valores y metadatos (CSV)

Valores y metadatos básicos de las series (CSV). Contiene todos los pares (fecha, valor) que componen cada una de las series de la base, enriquecidos con sus metadatos básicos.

#### Campos del recurso

- **catalog_id** (string): Identificador del catálogo al que pertenece la serie. Un catálogo es la unidad de documentación de activos de datos de un nodo.
- **dataset_id** (string): Identificador del dataset al que pertenece la serie. Es único dentro del catálogo al que pertenece el dataset.
- **distribution_id** (string): Identificador de la distribución a la que pertenece la serie. Es único dentro del catálogo al que pertenece la distribución.
- **serie_id** (string): Identificador de la serie. Es único dentro de toda base de series de tiempo.
- **indice_tiempo** (date): Fecha de la observación en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **indice_tiempo_frecuencia** (string): Frecuencia de las observaciones de la serie en formato ISO 8601 para intervalos repetidos (Ej.: "R/P3M" significa "cada 3 meses" y marca que una serie es trimestral).
- **valor** (number): Valor numérico de la observación de una serie para una fecha determinada.
- **serie_titulo** (string): Nombre normalizado corto de la serie compatible con su uso seguro en distintas aplicaciones. Tiene 60 caracteres como máximo y está compuesto por letras minúsculas de la "a" a la "z" sin caracteres especiales (sin tildes y sin la "ñ"), números y guiones bajos "_".
- **serie_unidades** (string): Unidades en las que están expresados los valores de la serie (Ej.: "Millones de pesos de 1993").
- **serie_descripcion** (string): Descripción completa de la información que contiene la serie.
- **distribution_titulo** (string): Título de la distribución a la que pertenece la serie.
- **distribution_descripcion** (string): Descripción completa de la información que contiene la distribución a la que pertenece la serie.
- **dataset_responsable** (string): Responsable de la publicación del dataset.
- **dataset_fuente** (string): Fuente primaria de los datos contenidos en el dataset al que pertenece la serie.
- **dataset_titulo** (string): Título del dataset al que pertenece la serie.
- **dataset_descripcion** (string): Descripción completa de la información que contiene el dataset al que pertenece la serie.

### Base de Series de Tiempo: metadatos enriquecidos de las series (CSV)

Listado de las series de tiempo disponibles en la base (CSV). Contiene los metadatos básicos de la series enriquecidos con indicadores descriptivos actualizados al día de la fecha.

#### Campos del recurso

- **catalog_id** (string): Identificador del catálogo al que pertenece la serie. Un catálogo es la unidad de documentación de activos de datos de un nodo.
- **dataset_id** (string): Identificador del dataset al que pertenece la serie. Es único dentro del catálogo al que pertenece el dataset.
- **distribution_id** (string): Identificador de la distribución a la que pertenece la serie. Es único dentro del catálogo al que pertenece la distribución.
- **serie_id** (string): Identificador de la serie. Es único dentro de toda base de series de tiempo.
- **indice_tiempo_frecuencia** (string): Frecuencia de las observaciones de la serie en formato ISO 8601 para intervalos repetidos (Ej.: "R/P3M" significa "cada 3 meses" y marca que una serie es trimestral).
- **serie_titulo** (string): Nombre normalizado corto de la serie compatible con su uso seguro en distintas aplicaciones. Tiene 60 caracteres como máximo y está compuesto por letras minúsculas de la "a" a la "z" sin caracteres especiales (sin tildes y sin la "ñ"), números y guiones bajos "_".
- **serie_unidades** (string): Unidades en las que están expresados los valores de la serie (Ej.: "Millones de pesos de 1993").
- **serie_descripcion** (string): Descripción completa de la información que contiene la serie.
- **distribution_titulo** (string): Título de la distribución a la que pertenece la serie.
- **distribution_descripcion** (string): Descripción completa de la información que contiene la distribución a la que pertenece la serie.
- **dataset_responsable** (string): Responsable de la publicación del dataset.
- **dataset_fuente** (string): Fuente primaria de los datos contenidos en el dataset al que pertenece la serie.
- **dataset_titulo** (string): Título del dataset al que pertenece la serie.
- **dataset_descripcion** (string): Descripción completa de la información que contiene el dataset al que pertenece la serie.
- **serie_indice_inicio** (date): Fecha de la primera observación de la serie en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **serie_indice_final** (date): Fecha de la última observación de la serie en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **serie_valores_cant** (number): Cantidad de observaciones contenidas en la serie.
- **serie_dias_no_cubiertos** (number): Días transcurridos desde el final del último período de tiempo para el que la serie tiene observaciones hasta la última fecha de actualización de la base de series de tiempo. Es una medida del período de tiempo más reciente no cubierto por las observaciones de la serie.
- **serie_actualizada** (boolean): Indicación estimativa de que el último valor de la serie está relativamente actualizado con respecto a la última fecha de actualización de la base.

Se considera que una serie está desactualizada cuando su último valor pertenece a una fecha 14 días anterior (serie diaria), 3 meses anterior (serie mensual) o 2 períodos anterior (para el resto de las frecuencias posibles).
- **serie_valor_ultimo** (number): Última observación disponible de la serie.
- **serie_valor_anterior** (number): Anteúltima observación disponible de la serie.
- **serie_var_pct_anterior** (number): Variación porcentual de la última observación disponible de la serie respecto de la anteúltima observación (la inmediatamente anterior).

### Base de Series de Tiempo: valores (CSV)

Valores de las series (CSV). Contiene todos los pares (fecha, valor) que componen cada una de las series de la base.

#### Campos del recurso

- **catalog_id** (string): Identificador del catálogo al que pertenece la serie. Un catálogo es la unidad de documentación de activos de datos de un nodo.
- **dataset_id** (string): Identificador del dataset al que pertenece la serie. Es único dentro del catálogo al que pertenece el dataset.
- **distribution_id** (string): Identificador de la distribución a la que pertenece la serie. Es único dentro del catálogo al que pertenece la distribución.
- **serie_id** (string): Identificador de la serie. Es único dentro de toda base de series de tiempo.
- **indice_tiempo** (string): Fecha de la observación en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **valor** (number): Valor numérico de la observación de una serie para una fecha determinada.

### Base de Series de Tiempo: fuentes (CSV)

Fuentes primarias de las series (CSV). Contiene la cantidad de series y valores presentes en la base de cada una de las fuentes primarias compiladas.

#### Campos del recurso

- **dataset_fuente** (string): Fuente primaria de los datos contenidos en el dataset al que pertenece una serie.
- **series_cant** (number): Cantidad de series de la fuente primaria presentes en la base.
- **valores_cant** (number): Cantidad de observaciones de la fuente primaria presentes en la base.
- **fecha_primer_valor** (date): Fecha de la primera observación de la fuente primaria en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **fecha_ultimo_valor** (date): Fecha de la última observación de la fuente primaria en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).

### Base de Series de Tiempo: valores y metadatos (XLSX)

Valores y metadatos básicos de las series (XLSX). Contiene todos los pares (fecha, valor) que componen cada una de las series de la base, enriquecidos con sus metadatos básicos.

#### Campos del recurso

- **catalog_id** (string): Identificador del catálogo al que pertenece la serie. Un catálogo es la unidad de documentación de activos de datos de un nodo.
- **dataset_id** (string): Identificador del dataset al que pertenece la serie. Es único dentro del catálogo al que pertenece el dataset.
- **distribution_id** (string): Identificador de la distribución a la que pertenece la serie. Es único dentro del catálogo al que pertenece la distribución.
- **serie_id** (string): Identificador de la serie. Es único dentro de toda base de series de tiempo.
- **indice_tiempo** (date): Fecha de la observación en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **indice_tiempo_frecuencia** (string): Frecuencia de las observaciones de la serie en formato ISO 8601 para intervalos repetidos (Ej.: "R/P3M" significa "cada 3 meses" y marca que una serie es trimestral).
- **valor** (number): Valor numérico de la observación de una serie para una fecha determinada.
- **serie_titulo** (string): Nombre normalizado corto de la serie compatible con su uso seguro en distintas aplicaciones. Tiene 60 caracteres como máximo y está compuesto por letras minúsculas de la "a" a la "z" sin caracteres especiales (sin tildes y sin la "ñ"), números y guiones bajos "_".
- **serie_unidades** (string): Unidades en las que están expresados los valores de la serie (Ej.: "Millones de pesos de 1993").
- **serie_descripcion** (string): Descripción completa de la información que contiene la serie.
- **distribution_titulo** (string): Título de la distribución a la que pertenece la serie.
- **distribution_descripcion** (string): Descripción completa de la información que contiene la distribución a la que pertenece la serie.
- **dataset_responsable** (string): Responsable de la publicación del dataset.
- **dataset_fuente** (string): Fuente primaria de los datos contenidos en el dataset al que pertenece la serie.
- **dataset_titulo** (string): Título del dataset al que pertenece la serie.
- **dataset_descripcion** (string): Descripción completa de la información que contiene el dataset al que pertenece la serie.

### Base de Series de Tiempo: metadatos enriquecidos de las series (XLSX)

Listado de las series de tiempo disponibles en la base (XLSX). Contiene los metadatos básicos de la series enriquecidos con indicadores descriptivos actualizados al día de la fecha.

#### Campos del recurso

- **catalog_id** (string): Identificador del catálogo al que pertenece la serie. Un catálogo es la unidad de documentación de activos de datos de un nodo.
- **dataset_id** (string): Identificador del dataset al que pertenece la serie. Es único dentro del catálogo al que pertenece el dataset.
- **distribution_id** (string): Identificador de la distribución a la que pertenece la serie. Es único dentro del catálogo al que pertenece la distribución.
- **serie_id** (string): Identificador de la serie. Es único dentro de toda base de series de tiempo.
- **indice_tiempo_frecuencia** (string): Frecuencia de las observaciones de la serie en formato ISO 8601 para intervalos repetidos (Ej.: "R/P3M" significa "cada 3 meses" y marca que una serie es trimestral).
- **serie_titulo** (string): Nombre normalizado corto de la serie compatible con su uso seguro en distintas aplicaciones. Tiene 60 caracteres como máximo y está compuesto por letras minúsculas de la "a" a la "z" sin caracteres especiales (sin tildes y sin la "ñ"), números y guiones bajos "_".
- **serie_unidades** (string): Unidades en las que están expresados los valores de la serie (Ej.: "Millones de pesos de 1993").
- **serie_descripcion** (string): Descripción completa de la información que contiene la serie.
- **distribution_titulo** (string): Título de la distribución a la que pertenece la serie.
- **distribution_descripcion** (string): Descripción completa de la información que contiene la distribución a la que pertenece la serie.
- **dataset_responsable** (string): Responsable de la publicación del dataset.
- **dataset_fuente** (string): Fuente primaria de los datos contenidos en el dataset al que pertenece la serie.
- **dataset_titulo** (string): Título del dataset al que pertenece la serie.
- **dataset_descripcion** (string): Descripción completa de la información que contiene el dataset al que pertenece la serie.
- **serie_indice_inicio** (date): Fecha de la primera observación de la serie en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **serie_indice_final** (date): Fecha de la última observación de la serie en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **serie_valores_cant** (number): Cantidad de observaciones contenidas en la serie.
- **serie_dias_no_cubiertos** (number): Días transcurridos desde el final del último período de tiempo para el que la serie tiene observaciones hasta la última fecha de actualización de la base de series de tiempo. Es una medida del período de tiempo más reciente no cubierto por las observaciones de la serie.
- **serie_actualizada** (boolean): Indicación estimativa de que el último valor de la serie está relativamente actualizado con respecto a la última fecha de actualización de la base.

Se considera que una serie está desactualizada cuando su último valor pertenece a una fecha 14 días anterior (serie diaria), 3 meses anterior (serie mensual) o 2 períodos anterior (para el resto de las frecuencias posibles).
- **serie_valor_ultimo** (number): Última observación disponible de la serie.
- **serie_valor_anterior** (number): Anteúltima observación disponible de la serie.
- **serie_var_pct_anterior** (number): Variación porcentual de la última observación disponible de la serie respecto de la anteúltima observación (la inmediatamente anterior).

### Base de Series de Tiempo: valores (XLSX)

Valores de las series (XLSX). Contiene todos los pares (fecha, valor) que componen cada una de las series de la base.

#### Campos del recurso

- **catalog_id** (string): Identificador del catálogo al que pertenece la serie. Un catálogo es la unidad de documentación de activos de datos de un nodo.
- **dataset_id** (string): Identificador del dataset al que pertenece la serie. Es único dentro del catálogo al que pertenece el dataset.
- **distribution_id** (string): Identificador de la distribución a la que pertenece la serie. Es único dentro del catálogo al que pertenece la distribución.
- **serie_id** (string): Identificador de la serie. Es único dentro de toda base de series de tiempo.
- **indice_tiempo** (string): Fecha de la observación en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **valor** (number): Valor numérico de la observación de una serie para una fecha determinada.

### Base de Series de Tiempo: fuentes (XLSX)

Fuentes primarias de las series (XLSX). Contiene la cantidad de series y valores presentes en la base de cada una de las fuentes primarias compiladas.

#### Campos del recurso

- **dataset_fuente** (string): Fuente primaria de los datos contenidos en el dataset al que pertenece una serie.
- **series_cant** (number): Cantidad de series de la fuente primaria presentes en la base.
- **valores_cant** (number): Cantidad de observaciones de la fuente primaria presentes en la base.
- **fecha_primer_valor** (date): Fecha de la primera observación de la fuente primaria en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **fecha_ultimo_valor** (date): Fecha de la última observación de la fuente primaria en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).

### Base de Series de Tiempo: valores y metadatos (DTA)

Valores y metadatos básicos de las series (DTA). Contiene todos los pares (fecha, valor) que componen cada una de las series de la base, enriquecidos con sus metadatos básicos.

#### Campos del recurso

- **catalog_id** (string): Identificador del catálogo al que pertenece la serie. Un catálogo es la unidad de documentación de activos de datos de un nodo.
- **dataset_id** (string): Identificador del dataset al que pertenece la serie. Es único dentro del catálogo al que pertenece el dataset.
- **distribution_id** (string): Identificador de la distribución a la que pertenece la serie. Es único dentro del catálogo al que pertenece la distribución.
- **serie_id** (string): Identificador de la serie. Es único dentro de toda base de series de tiempo.
- **indice_tiempo** (date): Fecha de la observación en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **indice_tiempo_frecuencia** (string): Frecuencia de las observaciones de la serie en formato ISO 8601 para intervalos repetidos (Ej.: "R/P3M" significa "cada 3 meses" y marca que una serie es trimestral).
- **valor** (number): Valor numérico de la observación de una serie para una fecha determinada.
- **serie_titulo** (string): Nombre normalizado corto de la serie compatible con su uso seguro en distintas aplicaciones. Tiene 60 caracteres como máximo y está compuesto por letras minúsculas de la "a" a la "z" sin caracteres especiales (sin tildes y sin la "ñ"), números y guiones bajos "_".
- **serie_unidades** (string): Unidades en las que están expresados los valores de la serie (Ej.: "Millones de pesos de 1993").
- **serie_descripcion** (string): Descripción completa de la información que contiene la serie.
- **distribution_titulo** (string): Título de la distribución a la que pertenece la serie.
- **dataset_responsable** (string): Responsable de la publicación del dataset.
- **dataset_fuente** (string): Fuente primaria de los datos contenidos en el dataset al que pertenece la serie.
- **dataset_titulo** (string): Título del dataset al que pertenece la serie.

### Base de Series de Tiempo: metadatos enriquecidos de las series (DTA)

Listado de las series de tiempo disponibles en la base (DTA). Contiene los metadatos básicos de la series enriquecidos con indicadores descriptivos actualizados al día de la fecha.

#### Campos del recurso

- **catalog_id** (string): Identificador del catálogo al que pertenece la serie. Un catálogo es la unidad de documentación de activos de datos de un nodo.
- **dataset_id** (string): Identificador del dataset al que pertenece la serie. Es único dentro del catálogo al que pertenece el dataset.
- **distribution_id** (string): Identificador de la distribución a la que pertenece la serie. Es único dentro del catálogo al que pertenece la distribución.
- **serie_id** (string): Identificador de la serie. Es único dentro de toda base de series de tiempo.
- **indice_tiempo_frecuencia** (string): Frecuencia de las observaciones de la serie en formato ISO 8601 para intervalos repetidos (Ej.: "R/P3M" significa "cada 3 meses" y marca que una serie es trimestral).
- **serie_titulo** (string): Nombre normalizado corto de la serie compatible con su uso seguro en distintas aplicaciones. Tiene 60 caracteres como máximo y está compuesto por letras minúsculas de la "a" a la "z" sin caracteres especiales (sin tildes y sin la "ñ"), números y guiones bajos "_".
- **serie_unidades** (string): Unidades en las que están expresados los valores de la serie (Ej.: "Millones de pesos de 1993").
- **serie_descripcion** (string): Descripción completa de la información que contiene la serie.
- **distribution_titulo** (string): Título de la distribución a la que pertenece la serie.
- **distribution_descripcion** (string): Descripción completa de la información que contiene la distribución a la que pertenece la serie.
- **dataset_responsable** (string): Responsable de la publicación del dataset.
- **dataset_fuente** (string): Fuente primaria de los datos contenidos en el dataset al que pertenece la serie.
- **dataset_titulo** (string): Título del dataset al que pertenece la serie.
- **dataset_descripcion** (string): Descripción completa de la información que contiene el dataset al que pertenece la serie.
- **serie_indice_inicio** (date): Fecha de la primera observación de la serie en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **serie_indice_final** (date): Fecha de la última observación de la serie en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **serie_valores_cant** (number): Cantidad de observaciones contenidas en la serie.
- **serie_dias_no_cubiertos** (number): Días transcurridos desde el final del último período de tiempo para el que la serie tiene observaciones hasta la última fecha de actualización de la base de series de tiempo. Es una medida del período de tiempo más reciente no cubierto por las observaciones de la serie.
- **serie_actualizada** (boolean): Indicación estimativa de que el último valor de la serie está relativamente actualizado con respecto a la última fecha de actualización de la base.

Se considera que una serie está desactualizada cuando su último valor pertenece a una fecha 14 días anterior (serie diaria), 3 meses anterior (serie mensual) o 2 períodos anterior (para el resto de las frecuencias posibles).
- **serie_valor_ultimo** (number): Última observación disponible de la serie.
- **serie_valor_anterior** (number): Anteúltima observación disponible de la serie.
- **serie_var_pct_anterior** (number): Variación porcentual de la última observación disponible de la serie respecto de la anteúltima observación (la inmediatamente anterior).

### Base de Series de Tiempo: valores (DTA)

Valores de las series (DTA). Contiene todos los pares (fecha, valor) que componen cada una de las series de la base.

#### Campos del recurso

- **catalog_id** (string): Identificador del catálogo al que pertenece la serie. Un catálogo es la unidad de documentación de activos de datos de un nodo.
- **dataset_id** (string): Identificador del dataset al que pertenece la serie. Es único dentro del catálogo al que pertenece el dataset.
- **distribution_id** (string): Identificador de la distribución a la que pertenece la serie. Es único dentro del catálogo al que pertenece la distribución.
- **serie_id** (string): Identificador de la serie. Es único dentro de toda base de series de tiempo.
- **indice_tiempo** (string): Fecha de la observación en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **valor** (number): Valor numérico de la observación de una serie para una fecha determinada.

### Base de Series de Tiempo: fuentes (DTA)

Fuentes primarias de las series (DTA). Contiene la cantidad de series y valores presentes en la base de cada una de las fuentes primarias compiladas.

#### Campos del recurso

- **dataset_fuente** (string): Fuente primaria de los datos contenidos en el dataset al que pertenece una serie.
- **series_cant** (number): Cantidad de series de la fuente primaria presentes en la base.
- **valores_cant** (number): Cantidad de observaciones de la fuente primaria presentes en la base.
- **fecha_primer_valor** (date): Fecha de la primera observación de la fuente primaria en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **fecha_ultimo_valor** (date): Fecha de la última observación de la fuente primaria en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).

### Base de Series de Tiempo: valores y metadatos (DB)

Valores y metadatos básicos de las series (DB). Contiene todos los pares (fecha, valor) que componen cada una de las series de la base, enriquecidos con sus metadatos básicos.

#### Campos del recurso

- **catalog_id** (string): Identificador del catálogo al que pertenece la serie. Un catálogo es la unidad de documentación de activos de datos de un nodo.
- **dataset_id** (string): Identificador del dataset al que pertenece la serie. Es único dentro del catálogo al que pertenece el dataset.
- **distribution_id** (string): Identificador de la distribución a la que pertenece la serie. Es único dentro del catálogo al que pertenece la distribución.
- **serie_id** (string): Identificador de la serie. Es único dentro de toda base de series de tiempo.
- **indice_tiempo** (date): Fecha de la observación en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **indice_tiempo_frecuencia** (string): Frecuencia de las observaciones de la serie en formato ISO 8601 para intervalos repetidos (Ej.: "R/P3M" significa "cada 3 meses" y marca que una serie es trimestral).
- **valor** (number): Valor numérico de la observación de una serie para una fecha determinada.
- **serie_titulo** (string): Nombre normalizado corto de la serie compatible con su uso seguro en distintas aplicaciones. Tiene 60 caracteres como máximo y está compuesto por letras minúsculas de la "a" a la "z" sin caracteres especiales (sin tildes y sin la "ñ"), números y guiones bajos "_".
- **serie_unidades** (string): Unidades en las que están expresados los valores de la serie (Ej.: "Millones de pesos de 1993").
- **serie_descripcion** (string): Descripción completa de la información que contiene la serie.
- **distribution_titulo** (string): Título de la distribución a la que pertenece la serie.
- **distribution_descripcion** (string): Descripción completa de la información que contiene la distribución a la que pertenece la serie.
- **dataset_responsable** (string): Responsable de la publicación del dataset.
- **dataset_fuente** (string): Fuente primaria de los datos contenidos en el dataset al que pertenece la serie.
- **dataset_titulo** (string): Título del dataset al que pertenece la serie.
- **dataset_descripcion** (string): Descripción completa de la información que contiene el dataset al que pertenece la serie.

### Base de Series de Tiempo: metadatos enriquecidos de las series (DB)

Listado de las series de tiempo disponibles en la base (DB). Contiene los metadatos básicos de la series enriquecidos con indicadores descriptivos actualizados al día de la fecha.

#### Campos del recurso

- **catalog_id** (string): Identificador del catálogo al que pertenece la serie. Un catálogo es la unidad de documentación de activos de datos de un nodo.
- **dataset_id** (string): Identificador del dataset al que pertenece la serie. Es único dentro del catálogo al que pertenece el dataset.
- **distribution_id** (string): Identificador de la distribución a la que pertenece la serie. Es único dentro del catálogo al que pertenece la distribución.
- **serie_id** (string): Identificador de la serie. Es único dentro de toda base de series de tiempo.
- **indice_tiempo_frecuencia** (string): Frecuencia de las observaciones de la serie en formato ISO 8601 para intervalos repetidos (Ej.: "R/P3M" significa "cada 3 meses" y marca que una serie es trimestral).
- **serie_titulo** (string): Nombre normalizado corto de la serie compatible con su uso seguro en distintas aplicaciones. Tiene 60 caracteres como máximo y está compuesto por letras minúsculas de la "a" a la "z" sin caracteres especiales (sin tildes y sin la "ñ"), números y guiones bajos "_".
- **serie_unidades** (string): Unidades en las que están expresados los valores de la serie (Ej.: "Millones de pesos de 1993").
- **serie_descripcion** (string): Descripción completa de la información que contiene la serie.
- **distribution_titulo** (string): Título de la distribución a la que pertenece la serie.
- **distribution_descripcion** (string): Descripción completa de la información que contiene la distribución a la que pertenece la serie.
- **dataset_responsable** (string): Responsable de la publicación del dataset.
- **dataset_fuente** (string): Fuente primaria de los datos contenidos en el dataset al que pertenece la serie.
- **dataset_titulo** (string): Título del dataset al que pertenece la serie.
- **dataset_descripcion** (string): Descripción completa de la información que contiene el dataset al que pertenece la serie.
- **serie_indice_inicio** (date): Fecha de la primera observación de la serie en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **serie_indice_final** (date): Fecha de la última observación de la serie en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **serie_valores_cant** (number): Cantidad de observaciones contenidas en la serie.
- **serie_dias_no_cubiertos** (number): Días transcurridos desde el final del último período de tiempo para el que la serie tiene observaciones hasta la última fecha de actualización de la base de series de tiempo. Es una medida del período de tiempo más reciente no cubierto por las observaciones de la serie.
- **serie_actualizada** (boolean): Indicación estimativa de que el último valor de la serie está relativamente actualizado con respecto a la última fecha de actualización de la base.

Se considera que una serie está desactualizada cuando su último valor pertenece a una fecha 14 días anterior (serie diaria), 3 meses anterior (serie mensual) o 2 períodos anterior (para el resto de las frecuencias posibles).
- **serie_valor_ultimo** (number): Última observación disponible de la serie.
- **serie_valor_anterior** (number): Anteúltima observación disponible de la serie.
- **serie_var_pct_anterior** (number): Variación porcentual de la última observación disponible de la serie respecto de la anteúltima observación (la inmediatamente anterior).

### Base de Series de Tiempo: valores (DB)

Valores de las series (DB). Contiene todos los pares (fecha, valor) que componen cada una de las series de la base.

#### Campos del recurso

- **catalog_id** (string): Identificador del catálogo al que pertenece la serie. Un catálogo es la unidad de documentación de activos de datos de un nodo.
- **dataset_id** (string): Identificador del dataset al que pertenece la serie. Es único dentro del catálogo al que pertenece el dataset.
- **distribution_id** (string): Identificador de la distribución a la que pertenece la serie. Es único dentro del catálogo al que pertenece la distribución.
- **serie_id** (string): Identificador de la serie. Es único dentro de toda base de series de tiempo.
- **indice_tiempo** (string): Fecha de la observación en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **valor** (number): Valor numérico de la observación de una serie para una fecha determinada.

### Base de Series de Tiempo: fuentes (DB)

Fuentes primarias de las series (DB). Contiene la cantidad de series y valores presentes en la base de cada una de las fuentes primarias compiladas.

#### Campos del recurso

- **dataset_fuente** (string): Fuente primaria de los datos contenidos en el dataset al que pertenece una serie.
- **series_cant** (number): Cantidad de series de la fuente primaria presentes en la base.
- **valores_cant** (number): Cantidad de observaciones de la fuente primaria presentes en la base.
- **fecha_primer_valor** (date): Fecha de la primera observación de la fuente primaria en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
- **fecha_ultimo_valor** (date): Fecha de la última observación de la fuente primaria en formato ISO 8601 sin horas, minutos ni segundos (YYYY-MM-DD). La fecha siempre indica el primer día del período al que hace referencia la observación (Ej.: "2017-04-01" hace referencia al segundo trimestre de 2017).
