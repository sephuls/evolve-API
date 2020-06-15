---
tags: [Implementatie details]
---

# Front-end
**Rollen**: leerlingen, TA's, Docenten OC, administrator.
Er is momenteel geen manier om d.m.v. de API een TA, docent of OC-lid te definieren. Mogelijk gaat dat gedaan worden met (bijvoorbeeld) `/user/{user_id}/promote` waarbij een user met eenzelfde of hoger authenticatie niveau deze user kan 'promoveren'.

**URL's**: Volgens de http en Django standaard moet een url eindigen met een slash: `/user/?param=...` ipv `/user?param=...`. Als je dit niet doet zal de api een error returnen. En als je denkt "mijn browser kan dat wel gewoon", dan wil ik je graag uitnodigen het eens te proberen, alle browsers gooien er namelijk gewoon een shash achter.

**HTTP methodes**: de `PUT` en `DELETE` methodes zijn geschrapt en omgezet naar `POST` methodes omdat de circusartiesten bij Django daar niet (goed) mee om kunnen gaan.

**Aanpassingen**: Graag mogelijke toevoegingen/wijzigingen in de backend discord zetten.

### Algemene pagina's

**Ready-to-go**: 
Zie de "Ready-to-go" pagina voor de beschikbaarheid van de api-calls. Toont beschikbaarheid in de backend en documentatiestatus. Graag mogelijke toevoegingen/wijzigingen in de backend discord zetten.

**Error codes**:
Zie de "Error codes" pagina voor info over alle huidige error codes.


### Docs tab

**Path Parameters**: 
Data die in de url wordt meegegeven, zoals: user_id, issue_id en (course) code.

**Query Parameters**:
GET data. `access_token` moet standaard in de GET parameters staan als authenticatie nodig is. Uit de `access_token` wordt de user en user-rol in de backed opgehaald.

**Header Parameters**:
Header data. `Content-Type: application/json` verwacht als POST data aanwezig.

**Body**:
POST data. Wordt verwacht in JSON formaat.

**Responses**:
Alle mogelijke responses en errors. In JSON formaat.

### Try-it tab
Gebruik het try it element (te zien op een api-call pagina) om een request te sturen. Klik op de eerste url-deel om van server (lokaal, test) te switchen.

~~WARNING: stoplight kan niet overweg met error responses (http code /= 200), dus deze kunnen alleen gesimuleerd worden in de browser of met iets als Postman.~~
Error responses werken wel nu.

**Query**:
GET data.

**Body**
POST data. In JSON formaat, gebruik daarom het `Raw` type.

**Code generation**:
Gebruik het `Code Generation` tabblad voor het genereren van kant-en-klare jQuery/XMLHttpRequest code. 

