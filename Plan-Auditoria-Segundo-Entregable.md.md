

Plan de auditoría: del riesgo priorizado al plan
Asignatura: ET0114 – Auditoría de Sistemas Docente: Juan Duque

## Integrantes:

## - Dahiana Alejandra Alvarez Vinasco

Matriz de riesgos vigente (anexo):
Taller-Sesion7-Matriz-Riesgos.md



- Contexto y riesgo seleccionado
Caso. Clínica Aburrá Salud es una IPS de mediana complejidad en Medellín, con consulta
externa, urgencias básicas y laboratorio. Usa un sistema de historias clínicas electrónicas
(HCE) en un servidor propio. La preocupación central es proteger la confidencialidad de los
datos de salud de los pacientes y la disponibilidad de la HCE durante la atención. Los marcos
elegidos fueron ISO/IEC 27001 e ITIL; para este riesgo se usa principalmente ISO/IEC 27001.

Riesgo seleccionado: R-01 de la matriz.

## Elemento Detalle
Activo o proceso Altas y bajas de cuentas de la HCE
Amenaza Un médico o auxiliar retirado intenta ingresar
con su cuenta
Vulnerabilidad La baja de cuentas es manual y no se verifica
contra los retiros de Talento Humano
## (supuesto)
Consecuencia posible Un exempleado podría consultar historias
clínicas porque su cuenta sigue activa,
exponiendo datos de salud de pacientes
Probabilidad / Impacto / Nivel 4 / 5 / 20 (justificación en la matriz)
Control actual No verificado. Se solicitaría el listado de
cuentas activas frente a la nómina vigente

## Elemento Detalle
Control propuesto Desactivar la cuenta el día del retiro como
paso del paz y salvo y revisar cada mes las
cuentas sin contrato vigente

Por qué vale la pena auditarlo. Además de tener el puntaje más alto, el control es revisable
con evidencia objetiva: se puede contrastar el listado de cuentas contra el de retiros. La HCE
contiene datos sensibles de salud, de modo que una cuenta activa indebidamente tiene
consecuencias legales y reputacionales.
- Objetivo de auditoría
Objetivo principal: Determinar si las cuentas de usuarios de la HCE se desactivan conforme al
procedimiento vigente cuando termina el vínculo laboral o contractual del usuario, durante el
periodo definido.
- Alcance funcional
## Aspecto Definición
Proceso o función Desactivación de cuentas de la HCE al
terminar el vínculo del usuario
Sistema o componente Módulo de administración de usuarios de la
HCE y su registro de cuentas
Población Cuentas de usuarios que dejaron de tener
vínculo con la clínica durante el periodo
Periodo propuesto 1 de enero al 30 de septiembre de 2026, por
ser un periodo reciente que abarca varios
retiros. Es una propuesta del equipo
Áreas o responsables Talento Humano (retiros y paz y salvo) y
Sistemas (administración de cuentas)

Inclusiones: cuentas de personal asistencial y administrativo con acceso a la HCE.
## Exclusiones:

- Cuentas de otros sistemas (agenda, facturación). Se excluyen para concentrar el plan
en el riesgo seleccionado. Limita la conclusión: no permite concluir sobre esos
sistemas.

- Calidad de contraseñas y autenticación. Se excluye por ser otro control. No limita el
objetivo.
- Criterios de evaluación
Control Condición esperada Fuente Estado
Baja de cuentas al
retiro
La cuenta se
desactiva en el plazo
definido por el
procedimiento al
terminar el vínculo
## Procedimiento
interno de gestión de
accesos
Por confirmar:
solicitar la política y
el plazo vigentes
Revisión periódica de
cuentas
Existe revisión
periódica de cuentas
activas con registro
## Procedimiento
interno y buenas
prácticas de ISO/IEC
27001 en gestión de
accesos
Por confirmar:
verificar el control
específico en la
versión vigente de la
norma
Protección de datos
de salud
Solo accede a la
historia clínica
personal autorizado
Ley 1581 de 2012 y
Resolución 1995 de
## 1999
Por confirmar los
artículos aplicables

Aplican al caso porque la HCE contiene datos sensibles y la clínica está sujeta a normas
colombianas de protección de datos e historia clínica. No se atribuyen plazos ni porcentajes a
ningún marco: el plazo concreto será el de la política interna, una vez la clínica la entregue.
- Programa de trabajo
Procedimiento 1. Comprender el diseño del control
## Elemento Detalle
Control Baja de cuentas al retiro, a cargo de
Sistemas tras aviso de Talento Humano
Criterio Procedimiento vigente de baja de cuentas
(por confirmar)
Procedimiento 1) Solicitar el procedimiento y confirmar su
vigencia. 2) Entrevistar a Talento Humano y a
Sistemas sobre quién avisa, cómo y cuándo.

## Elemento Detalle
3) Documentar el flujo y quién responde por
cada paso
Población o muestra No aplica (revisión de diseño)
Evidencia esperada Procedimiento aprobado, formato de paz y
salvo, descripción del flujo, política de
accesos
Posibles excepciones No existe procedimiento. No define plazo. No
asigna responsable
Procedimiento 2. Verificar la operación del control
## Elemento Detalle
Control Desactivación efectiva de las cuentas de
quienes se retiraron
Criterio Cuenta desactivada dentro del plazo definido
en el procedimiento (por confirmar)
Procedimiento 1) Obtener de Talento Humano el listado de
retiros del periodo. 2) Obtener de Sistemas el
listado de cuentas de la HCE con su estado y
fecha de desactivación. 3) Cruzar ambos
listados. 4) Para cada retirado, comparar la
fecha de retiro con la de desactivación. 5)
Registrar excepciones
Población o muestra Todos los retirados del periodo. Si la
población es muy grande, muestra aleatoria
cuyo tamaño se definirá al conocer la
población real
Evidencia esperada Listado de retiros (Talento Humano),
exportación de cuentas con estado y fechas
(Sistemas), formatos de paz y salvo
Posibles excepciones Cuenta activa de una persona retirada.
Desactivación posterior al plazo. Retiro sin
paz y salvo

Procedimiento 3. Verificar si hubo uso de cuentas tras el retiro
## Elemento Detalle
Control Registro de accesos de la HCE (control
detectivo)
Criterio No debe haber accesos de cuentas después
de la fecha de retiro
Procedimiento Para las cuentas con excepción en el
procedimiento 2, solicitar el registro de
accesos y buscar ingresos posteriores a la
fecha de retiro
Población o muestra Cuentas con excepción del procedimiento 2
Evidencia esperada Registro de accesos de la HCE del periodo
Posibles excepciones Existen accesos posteriores al retiro. El
registro de accesos no existe o no es
confiable

Las entrevistas del procedimiento 1 se corroboran con los listados y registros de los
procedimientos 2 y 3.
Tabla de trazabilidad
ID del riesgo Control a
evaluar
Criterio y
fuente
## Procedimien
to
Población o
muestra
## Evidencia
esperada
R-01 Baja de
cuentas al
retiro
## (diseño)
## Procedimient
o interno de
accesos (por
confirmar)
## Procedimient
o 1
No aplica Procedimient
o, paz y
salvo, política
de accesos
## R-01 Desactivació
n efectiva de
cuentas
Plazo del
procedimient
o interno (por
confirmar)
## Procedimient
o 2
Retirados del
periodo (o
muestra
aleatoria)
Listado de
retiros,
exportación
de cuentas

ID del riesgo Control a
evaluar
Criterio y
fuente
## Procedimien
to
Población o
muestra
## Evidencia
esperada
R-01 Registro de
accesos
## (detectivo)
No debe
haber
accesos tras
el retiro
## Procedimient
o 3
Cuentas con
excepción
Registro de
accesos de la
## HCE
- Responsables, cronograma, supuestos y limitaciones
## Responsables (equipo)
## Responsable Tarea
[Integrante 1] Procedimiento 1 y solicitud de información
[Integrante 2] Procedimientos 2 y 3 y documentación de
excepciones
Todos Revisión final y exposición
Cronograma propuesto
## Semana Fase Actividad
1 Preparación Definir criterios y plan de
solicitud de información
2 Solicitud de información Pedir procedimiento, listados
y registros
3 Revisión Ejecutar los procedimientos
1, 2 y 3
4 Cierre Consolidar excepciones y
preparar el informe

Dependencias de la organización: que Talento Humano y Sistemas entreguen los listados y
el registro de accesos. Recursos: acceso de solo lectura a los listados y al registro de accesos
de la HCE. Qué se podría hacer realmente: el diseño del plan, la matriz y los criterios.
Quedaría como planificación por falta de acceso: todos los procedimientos de verificación,
porque requieren datos de la organización.

Hechos, supuestos, información por solicitar y propuestas
## Tipo Contenido
Hecho comprobado Ninguno sobre la clínica, por ser un caso
hipotético. Las normas citadas (Ley 1581 de
2012 y Resolución 1995 de 1999) existen,
pero sus artículos se deben confirmar
Supuesto La baja de cuentas es manual y no se
concilia con Talento Humano. Hay un solo
servidor y un solo funcionario de sistemas
Información por solicitar Procedimiento de gestión de accesos, listado
de retiros, exportación de cuentas, registro
de accesos, paz y salvo
Propuesta del equipo Objetivo, alcance, periodo, procedimientos y
tabla de trazabilidad

Limitaciones. No se ejecutó ninguna revisión. Este documento no contiene hallazgos,
porcentajes de cumplimiento ni conclusiones sobre la eficacia del control. La evidencia
indicada es la que se solicitaría, no evidencia obtenida.
## 7. Fuentes
- Matriz de riesgos del equipo:
Taller-Sesion7-Matriz-Riesgos.md
## .
- ISO/IEC 27001 (controles de gestión de accesos; versión vigente por confirmar).
- Ley 1581 de 2012 (protección de datos personales, Colombia).
- Resolución 1995 de 1999 (historia clínica, Colombia).
- Taller y guía del curso ET0114.