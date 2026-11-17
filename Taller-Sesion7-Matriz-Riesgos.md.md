

Matriz inicial de riesgos
Asignatura: ET0114 – Auditoría de Sistemas · Sesión 7 Docente: Juan Duque

## Integrantes:

## - Dahiana Alejandra Alvarez Vinasco
Caso y contexto actualizado
Clínica Aburrá Salud (organización hipotética) es una IPS de mediana complejidad en Medellín,
con unos 120 empleados y consulta externa, urgencias básicas y laboratorio. Maneja historias
clínicas electrónicas (HCE), agenda de citas y facturación en un servidor propio. Esta entrega
analiza el proceso de administración de cuentas de usuarios de la HCE y los sistemas que
dependen de él. La preocupación principal es proteger la confidencialidad de los datos de salud
de los pacientes y la disponibilidad de la HCE durante la atención.

Marcos (hipotéticos, definidos para este caso): primero ISO/IEC 27001, para proteger la
confidencialidad de las historias clínicas, y después ITIL, para la disponibilidad del servicio de
agenda y HCE. Evidencia que se solicitaría: ISO/IEC 27001: política de control de accesos y
listado de cuentas activas de la HCE. ITIL: registro de incidentes de caída del servicio y acta de
pruebas de restauración.
## Supuestos
- La clínica tiene un solo servidor local para HCE, agenda y facturación.
- Las cuentas de la HCE se crean y retiran por solicitud de Talento Humano al área de
sistemas, de forma manual.
- Los roles de la HCE están definidos, pero no se han recertificado desde su creación.
- Hay copias de seguridad diarias en un disco externo conectado al mismo servidor.
- Hay un solo funcionario de sistemas, sin respaldo.
- Se aplican las normas colombianas de protección de datos (Ley 1581 de 2012) y de
historia clínica (Resolución 1995 de 1999).
- Probabilidad e impacto se estiman con estos supuestos y no con datos internos. "Se
solicitaría" indica la evidencia que se pediría al auditar, no un hallazgo.

Activos y procesos analizados
Activo o proceso Tipo
Historias clínicas electrónicas (HCE) Información
Proceso de altas y bajas de cuentas de la
## HCE
## Proceso
Servidor de HCE, agenda y facturación Infraestructura
Agenda de citas Aplicación
Copias de seguridad de la HCE Proceso / infraestructura
## Escala
## Valor Probabilidad Impacto
1 Raro Consecuencia menor y fácil
de corregir
2 Poco probable Afecta una operación limitada
3 Posible Afecta un proceso relevante
o varios usuarios
4 Probable Interrumpe un servicio
importante o expone
información sensible
5 Muy probable Puede afectar gravemente la
operación, datos críticos o
cumplimiento

Nivel = Probabilidad × Impacto. Las filas están ordenadas de mayor a menor nivel.

Matriz de riesgos
ID Activ
o o
proce
so
## Amen
aza
## Vulne
rabili
dad
## Riesg
o
## Prob. Impa
cto
## Nivel Contr
ol
actua
l o
evide
ncia
## Contr
ol
propu
esto
## Justif
icació
n
## R-01 Altas
y
bajas
de
cuent
as de
la
## HCE
## Un
médic
o o
auxilia
r
retirad
o
intent
a
ingres
ar con
su
cuent
a
## La
baja
de
cuent
as es
manu
al y
no se
verific
a
contra
los
retiros
de
## Talent
o
## Huma
no
## (supu
esto)
## Un
exem
plead
o
podría
consu
ltar
histori
as
clínica
s
porqu
e su
cuent
a
sigue
activa
tras el
retiro,
expon
iendo
datos
de
salud
de
pacie
ntes
## 4 5 20 Se
solicit
aría el
listad
o de
cuent
as
activa
s
frente
a la
nómin
a
vigent
e
## Preve
ntivo:
desac
tivar
la
cuent
a el
día
del
retiro
como
paso
obliga
torio
del
paz y
salvo.
## Detec
tivo:
revisa
r cada
mes
las
cuent
as
activa
s sin
contra
to
vigent
e
## Proba
bilida
d 4: la
baja
depen
de de
un
aviso
manu
al y la
rotaci
ón en
salud
es
frecue
nte.
## Impac
to 5:
datos
sensi
bles
de
salud
con
implic
acion
es
legale
s

ID Activ
o o
proce
so
## Amen
aza
## Vulne
rabili
dad
## Riesg
o
## Prob. Impa
cto
## Nivel Contr
ol
actua
l o
evide
ncia
## Contr
ol
propu
esto
## Justif
icació
n
## R-02 Histori
as
clínica
s
## (HCE)
## Perso
nal
admin
istrati
vo o
asiste
ncial
que
consu
lta
histori
as sin
neces
idad
de
atenci
ón
## Roles
con
permi
sos
ampli
os,
sin
recerti
ficació
n
desde
su
creaci
ón
## (supu
esto)
## Un
funcio
nario
sin
relaci
ón
con el
pacie
nte
podría
consu
ltar su
histori
a y
divulg
ar
inform
ación,
con
pérdid
a de
confid
enciali
dad
## 4 4 16 Se
solicit
aría la
matriz
de
roles
y la
fecha
de la
última
revisi
ón
## Preve
ntivo:
limitar
la
consu
lta a
pacie
ntes
asign
ados
y
recerti
ficar
roles
cada
seis
mese
s.
## Detec
tivo:
revisa
r cada
mes
el
registr
o de
consu
ltas
de
histori
as
## Proba
bilida
d 4:
much
os
usuari
os
con
acces
o
ampli
o.
## Impac
to 4:
expon
e
inform
ación
sensi
ble de
pacie
ntes
## R-03 Servid
or de
## HCE,
## Rans
omwa
re
## Los
equip
os de
## Un
funcio
nario
## 3 5 15 Se
solicit
aría el
## Preve
ntivo:
capac
## Proba
bilida
d 3: el

ID Activ
o o
proce
so
## Amen
aza
## Vulne
rabili
dad
## Riesg
o
## Prob. Impa
cto
## Nivel Contr
ol
actua
l o
evide
ncia
## Contr
ol
propu
esto
## Justif
icació
n
agend
a y
factur
ación
entreg
ado
por
correo
de
phishi
ng
atenci
ón
comp
arten
el
correo
con la
red
del
servid
or y
los
usuari
os no
recibe
n
capac
itació
n
periód
ica
## (supu
esto)
podría
abrir
un
correo
malici
oso y
el
ranso
mwar
e
cifrarí
a la
## HCE,
impidi
endo
atend
er
pacie
ntes y
factur
ar
plan
de
capac
itació
n y el
registr
o de
actual
izacio
nes
del
servid
or
itació
n
seme
stral
con
simul
acros
de
phishi
ng y
separ
ación
de la
red
del
servid
or.
## Detec
tivo:
antivir
us
con
alerta
s
revisa
das
por el
respo
nsabl
e de
siste
mas
sector
salud
es
objeti
vo
frecue
nte.
## Impac
to 5:
puede
deten
er la
atenci
ón
## R-04 Copia
s de
## Rans
omwa
## El
respal
## Tras
un
## 3 4 12 Se
solicit
## Preve
ntivo:
## Proba
bilida

ID Activ
o o
proce
so
## Amen
aza
## Vulne
rabili
dad
## Riesg
o
## Prob. Impa
cto
## Nivel Contr
ol
actua
l o
evide
ncia
## Contr
ol
propu
esto
## Justif
icació
n
seguri
dad
de la
## HCE
re o
falla
del
servid
or que
afecta
tambi
én el
disco
de
respal
do
do
está
conec
tado
al
mism
o
servid
or y
no se
prueb
a su
restau
ración
## (supu
esto)
ataqu
e o
falla,
las
copia
s
podría
n
queda
r
cifrad
as o
dañad
as, y
la
clínica
perde
ría
días
de
histori
as
clínica
s
aría el
acta
de la
última
prueb
a de
restau
ración
copia
adicio
nal
desco
necta
da o
fuera
de la
sede.
## Corre
ctivo:
prueb
a de
restau
ración
trimes
tral
con
acta y
medic
ión
del
tiemp
o de
recup
eració
n
d 3:
ataqu
e o
falla
posibl
e y
respal
do no
aislad
o.
## Impac
to 4:
pérdid
a de
inform
ación
crítica
## R-05 Agen
da de
citas
## Falla
del
servid
or o
ausen
cia
del
## Depe
ndenc
ia de
una
sola
perso
na y
## Una
falla
durant
e la
ausen
cia
del
## 3 3 9 Se
solicit
aría el
proce
dimie
nto de
contin
## Corre
ctivo:
docu
menta
r el
proce
dimie
## Proba
bilida
d 3: la
falla
es
posibl
e y no

ID Activ
o o
proce
so
## Amen
aza
## Vulne
rabili
dad
## Riesg
o
## Prob. Impa
cto
## Nivel Contr
ol
actua
l o
evide
ncia
## Contr
ol
propu
esto
## Justif
icació
n
único
funcio
nario
de
siste
mas
sin
proce
dimie
nto
docu
menta
do de
contin
genci
a
## (supu
esto)
funcio
nario
podría
dejar
la
agend
a
fuera
de
servici
o
varias
horas,
con
citas
perdid
as y
queja
s de
pacie
ntes
genci
a y el
registr
o de
incide
ntes
nto de
contin
genci
a con
agend
a
manu
al de
respal
do y
desig
nar un
suple
nte
capac
itado
hay
suple
nte.
## Impac
to 3:
afecta
un
proce
so
releva
nte,
pero
con
altern
ativa
manu
al
Lista de verificación
Cada riesgo se relaciona con un activo o proceso específico
La amenaza y la vulnerabilidad son diferentes
El riesgo explica qué podría pasar y su consecuencia
El control propuesto reduce una vulnerabilidad concreta
Probabilidad e impacto tienen justificación