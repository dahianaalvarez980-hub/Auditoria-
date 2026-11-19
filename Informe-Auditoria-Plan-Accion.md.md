

Informe de auditoría y plan de acción
## 1. Identificación
Asignatura: ET0114 – Auditoría de Sistemas · Taller final
## Docente: Juan Duque
## Integrantes:
## Dahiana Alejandra Alvarez Vinasco

Caso: Clínica Aburrá Salud, IPS de mediana complejidad en Medellín
## Fecha: 19/11/2026
Nota sobre el caso: EJERCICIO SIMULADO. La organización (Clínica Aburrá Salud)
es hipotética. La política, los registros, la muestra y los resultados de este informe son
ficticios, creados para demostrar cómo se aplicaría la prueba. No describen el
cumplimiento ni el incumplimiento de ninguna organización real.
- Resumen ejecutivo
Se retoma el riesgo R-01 de la matriz (cuentas de la historia clínica electrónica, HCE, que
siguen activas tras el retiro del usuario) y el control de baja de cuentas definido en el plan de
auditoría. Se ejecutó una prueba simulada sobre una muestra ficticia de 12 retiros del periodo.
De los 12, 9 cumplieron el criterio ficticio y se identificaron 3 excepciones: 2 bajas tardías y 1
cuenta sin desactivar. En el registro de accesos simulado no aparecen ingresos posteriores al
retiro. Se propone un plan de acción con dos acciones. Todo lo anterior es simulado y no
permite concluir nada sobre una organización real.
- Objetivo y alcance
Objetivo. Determinar si las cuentas de la HCE se desactivan conforme al criterio establecido
cuando termina el vínculo del usuario.

## Aspecto Definición
Proceso Desactivación de cuentas de la HCE al
terminar el vínculo
Sistema Módulo de administración de usuarios de la
## HCE
Periodo 1 de enero al 30 de septiembre de 2026

## Aspecto Definición
Población Cuentas de usuarios retirados en el periodo.
Tamaño real desconocido
Inclusiones Personal asistencial y administrativo con
acceso a la HCE
Exclusiones Agenda y facturación. Limita la conclusión
solo a la HCE

Frente al plan de auditoría anterior no hubo cambios de alcance. Se agregó el criterio ficticio y
la ejecución simulada.
- Criterios y metodología
Criterio (ficticio, para el ejercicio): la cuenta debe desactivarse a más tardar un día hábil
después de la fecha de retiro. Fuente: política simulada de gestión de accesos de la clínica. Es
un criterio inventado para este ejercicio, no una política real ni un plazo de ISO/IEC 27001.

Marco de referencia: ISO/IEC 27001, usado como referencia general para la gestión de
accesos. No se le atribuye ningún plazo específico.

Población y muestra. Como la población real es desconocida, se construyó un conjunto ficticio
de 12 retiros del periodo y se revisaron los 12 (examen total de la muestra simulada).

## Procedimiento.

- Se tomó el listado simulado de retiros (Talento Humano) y la exportación simulada de
cuentas (Sistemas).
- Se cruzaron por identificador de cuenta.
- Se comparó la fecha de retiro con la de desactivación frente al criterio.
- En las excepciones, se revisó el registro de accesos simulado en busca de ingresos
posteriores al retiro.

Evidencia examinada: listado de retiros, exportación de cuentas con fechas de desactivación
y registro de accesos.

- Resultados y hallazgos
Papel de trabajo
ID cuenta Rol Fecha de
retiro
Fecha de
desactivació
n
## Retraso
## (días
hábiles)
## Resultado
CTA-01 Médico 06-feb-2026 06-feb-2026 0 Conforme
CTA-02 Enfermería 27-feb-2026 27-feb-2026 0 Conforme
CTA-03 Auxiliar 13-mar-2026 13-mar-2026 0 Conforme
CTA-04 Administrativ
o
## 31-mar-2026 01-abr-2026 1 Conforme
CTA-05 Médico 17-abr-2026 17-abr-2026 0 Conforme
CTA-06 Laboratorio 08-may-2026 14-may-2026 4 Excepción
CTA-07 Enfermería 29-may-2026 29-may-2026 0 Conforme
CTA-08 Auxiliar 12-jun-2026 12-jun-2026 0 Conforme
CTA-09 Administrativ
o
## 30-jun-2026 01-jul-2026 1 Conforme
CTA-10 Médico 24-jul-2026 04-ago-2026 7 Excepción
CTA-11 Enfermería 14-ago-2026 Sin
desactivar
n/a Excepción
CTA-12 Auxiliar 11-sep-2026 11-sep-2026 0 Conforme

Resumen: 12 revisadas, 9 conformes, 3 excepciones. Registro de accesos: no hay ingresos
posteriores al retiro en las 3 cuentas con excepción. Los datos son ficticios y no se pueden
extrapolar a ninguna población real.
H-01. Baja tardía de cuentas
- Criterio: desactivar la cuenta a más tardar un día hábil después del retiro (política
ficticia del ejercicio).

- Condición: 2 de las 12 cuentas revisadas (CTA-06 y CTA-10) se desactivaron 4 y 7
días hábiles después del retiro, según la exportación simulada.
- Causa: pendiente de confirmar.
- Efecto o riesgo: posible: durante ese lapso la cuenta pudo estar disponible para un
acceso no autorizado. Observado: el registro de accesos no muestra ingresos
posteriores. La prueba no demuestra que alguien las haya usado.
- Recomendación: revisar el flujo de aviso de retiro entre Talento Humano y Sistemas y
fijar un plazo con seguimiento.
H-02. Cuenta sin desactivar tras el retiro
- Criterio: igual que H-01.
- Condición: la cuenta CTA-11 aparece sin desactivar en la exportación simulada, con
retiro registrado el 14 de agosto de 2026.
- Causa: pendiente de confirmar.
- Efecto o riesgo: posible: acceso no autorizado a historias clínicas con una cuenta
vigente de una persona retirada. Observado: sin ingresos posteriores en el registro.
- Recomendación: desactivar la cuenta de inmediato y establecer una revisión mensual
de cuentas activas frente a los retiros.
- Conclusión y limitaciones
Con la muestra simulada, el control de baja de cuentas mostró excepciones (3 de 12) frente al
criterio ficticio. Esto demuestra cómo se aplicaría la prueba, pero no demuestra cumplimiento
ni incumplimiento de una organización real.

## Limitaciones.

- Datos, política y criterio son ficticios.
- Población real desconocida. Una muestra limitada no permite generalizar.
- Las causas no se comprobaron.
- Solo se revisó la HCE, no la agenda ni la facturación.
- No se probó el registro de accesos en profundidad, por ser simulado.
- Plan de acción
ID del
hallazgo
## Acción
propuesta
## Responsabl
e propuesto
Prioridad y
justificación
## Plazo
propuesto
Evidencia de
cierre
H-01 Revisar el
flujo de aviso
de retiro
## Responsable
de gestión de
accesos y
Alta: la baja
tardía deja la
cuenta
30 días,
sujeto a
acuerdo
## Procedimient
o actualizado
y resultado

ID del
hallazgo
## Acción
propuesta
## Responsabl
e propuesto
Prioridad y
justificación
## Plazo
propuesto
Evidencia de
cierre
entre Talento
Humano y
Sistemas e
incluir la baja
de la cuenta
como paso
obligatorio
del paz y
salvo, con
plazo
definido
## Talento
## Humano
disponible
tras el retiro
de una
prueba
posterior del
control
H-02 Desactivar la
cuenta
pendiente y
revisar cada
mes las
cuentas
activas frente
al listado de
retiros
## Responsable
de gestión de
accesos
Alta: una
cuenta
vigente de
una persona
retirada
expone datos
de salud
## Inmediato
para la
cuenta, 30
días para la
revisión
mensual
Registro de
desactivación
y acta de la
primera
revisión
mensual

Las acciones son propuestas: no se presentan como aprobadas ni implementadas.
- Referencias y anexos
- Matriz de riesgos:
Taller-Sesion7-Matriz-Riesgos.md
## (fila R-01).
- Plan de auditoría:
Plan-Auditoria-Segundo-Entregable.md
## .
- Papel de trabajo: sección 5 de este informe (datos simulados).
- ISO/IEC 27001 (referencia general sobre gestión de accesos).
- Taller y guía del curso ET0114.