---
tags: [Implementatie details]
---

# Front-end

**Ready-to-go**: 
Zie de Ready-to-go pagina voor de beschikbaarheid van de api-calls. Toont beschikbaarheid in de backend en documentatiestatus. Graag mogelijke toevoegingen/wijzigingen in de backend discord zetten.

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
Gebruik het try it element (te zien op een api-call pagina) om een request te sturen naar de testserver.

**Query**:
GET data.

**Body**
POST data. In JSON formaat, gebruik daarom het `Raw` type.

**Code generation**:
Gebruik het `Code Generation` tabblad voor het genereren van kant-en-klare jQuery/XMLHttpRequest code. 
