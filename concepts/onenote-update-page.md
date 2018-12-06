---
title: Aktualisieren der Inhalte von OneNote-Seiten
description: " Enterprise-Notizbücher in Office 365"
ms.openlocfilehash: 746520c5071dba0cf11d2fde02daa502522c56f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092227"
---
# <a name="update-onenote-page-content"></a>Aktualisieren der Inhalte von OneNote-Seiten

**Gilt für** Heimanwender-Notizbücher in OneDrive | Unternehmensnotizbücher in Office 365


Sollen die Inhalte einer OneNote-Seite aktualisiert werden, senden Sie eine PATCH-Anforderung an den Endpunkt *content* der Seite:

`PATCH ../notes/pages/{id}/content`</p>

Im Anforderungstext senden Sie ein JSON-Änderungsobjekt. Wenn die Anforderung erfolgreich ist, gibt Microsoft Graph den HTTP-Statuscode 204 zurück.


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a>Zusammensetzen des Anforderungs-URI

Beginnen Sie bei der Zusammensetzung des Anforderungs-URI mit der Stamm-URL des Diensts:

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

Fügen Sie dann den Endpunkt *content* der Seite an:

- **Abrufen des HTML-Codes der Seite und aller definierten Werte des Typs *data-id***<br/><br/>`../pages/{id}/content`   

- **Abrufen des HTML-Codes der Seite, aller definierten Werte des Typs *data-id* und aller generierten Werte des Typs *id***<br/><br/>`../pages/{page-id}/content?includeIDs=true` 

Die Werte des Typs **data-id** und des Typs **id** dienen als Bezeichner für die Elemente mit dem Attribut **target**, also die Elemente, die aktualisiert werden sollen.

 
Der vollständige Anforderungs-URI sieht so aus:<br/><br/>`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


Weitere Informationen zur Stamm-URL des Service finden Sie unter [diesem Link](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).


<a name="message-body"></a>

## <a name="construct-the-message-body"></a>Erstellen des Anforderungstexts

Der HTML-Code einer OneNote-Seite enthält Text, Bilder und andere Inhalte, die in Strukturen wie Elementen des Typs **div**, **img** oder **ol** organisiert sind. Sollen die Inhalte einer OneNote-Seite aktualisiert werden, fügen Sie der Seite HTML-Elemente hinzu oder ersetzen vorhandene HTML-Elemente.

Ihre Änderungen werden als Array von JSON-Änderungsobjekten im Anforderungstext gesendet. Jedes Objekt definiert das Zielelement, neue HTML-Inhalte und die auf die Inhalte anzuwendende Aktion.

Das folgende Array definiert zwei Änderungen. Bei der ersten wird ein Bild über einem Absatz als gleichgeordnetes Element eingefügt, bei der zweiten wird ein Element an eine Liste als letztes untergeordnetes Element angefügt.

```json
[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="Image above the target paragraph" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the end of the list</li>'
  }
]
```

Weitere Beispiele finden Sie [hier](#example-requests).


### <a name="attributes-for-json-change-objects"></a>Attribute für JSON-Änderungsobjekte

JSON-Objekte für PATCH-Anforderungen werden mithilfe der Attribute **target**, **action**, **position** und **content** definiert.

#### <a name="target"></a>target

Das zu aktualisierende Element. Der Wert muss einer der folgenden Bezeichner sein:

| Bezeichner | Beschreibung |  
|------|------|  
| #{data-id} | <p>Diese ID wird bei der [Erstellung einer Seite](onenote-create-page.md) oder der [Aktualisierung einer Seite](onenote-update-page.md) optional den Elementen im Eingabe-HTML-Code zugewiesen. Setzen Sie vor den Wert als Präfix das Symbol #.</p><p> Beispiel:<br/>`'target':'#intro'` legt das Element `<div data-id="intro" ...>` als Ziel fest.</p> |  
| id | <p>Hierbei handelt es sich um die von Microsoft Graph [generierte ID](#generated-ids). Sie ist für die meisten Ersetzungsvorgänge erforderlich. Setzen Sie hier kein Symbol # als Präfix.</p><p> Beispiel:<br/>`'target':'div:{33f8a2...}{37}'` legt das Element `<div id="div:{33f8a2...}{37}" ...>` als Ziel fest.</p><p>Verwechseln Sie IDs dieses Typs nicht mit den Werten des Typs **id** im [Eingabe-HTML-Code](onenote-input-output-html.md). Alle im Eingabe-HTML-Code gesendeten Werte des Typs **id** werden verworfen.</p> |  
| body | Das Schlüsselwort, dass als Ziel das erste „div“-Element auf der Seite festlegt. Setzen Sie hier kein Symbol # als Präfix. |  
| title | Das Schlüsselwort, das als Ziel den Seitentitel festlegt. Setzen Sie hier kein Symbol # als Präfix. |  
 
#### <a name="action"></a>Aktion

Die für das Zielelement auszuführende Aktion. Siehe [Unterstützte Aktionen für Elemente](#supported-elements-and-actions).

| Aktion | Beschreibung |  
|------|------|  
| append | <p>Fügt den angegebenen Inhalt als erstes oder letztes untergeordnetes Element zum Ziel hinzu, je nach dem im Attribut **position** festgelegten Wert.</p><p>Kann nur auf Elemente des Typs **body**, **div**, **ol** oder **ul** angewendet werden.</p> |  
| insert | Fügt den angegebenen Inhalt als gleichgeordnetes Element vor oder nach dem Ziel hinzu, je nach dem im Attribut **position** festgelegten Wert. |  
| prepend | <p>Fügt den angegebenen Inhalt als erstes untergeordnetes Element zum Ziel hinzu. Kurzbefehl als Ersatz für **append** + **before**.</p><p>Kann nur auf Elemente des Typs **body**, **div**, **ol** oder **ul** angewendet werden.</p> |  
| replace | <p>Ersetzt das Ziel durch den angegebenen Inhalt.</p><p>Für die meisten Aktionen des Typs **replace** muss das Ziel in Form der [generierten ID](#generated-ids) angegeben werden. (Ausnahme: Elemente des Typs **img** oder **object** innerhalb eines „div“-Elements. Sie können auch per **data-id** angegeben werden.)</p> |  
 
#### <a name="position"></a>position

Die Position, an der der angegebene Inhalt hinzugefügt werden soll, relativ zum Zielelement. Wenn der Wert weggelassen wird, gilt der Standardwert **after**.

| Position | Beschreibung |  
|------|------|  
| after (Standard) |<p>Mit **append**: das letzte untergeordnete Element des Zielelements</p><p>Mit **insert**: das nachfolgende gleichgeordnete Element des Zielelements</p> |
| before | <p>Mit **append**: das erste untergeordnete Element des Zielelements</p><p>Mit **insert**: das vorhergehende gleichgeordnete Element des Zielelements</p> |

#### <a name="content"></a>content

Eine Zeichenfolge aus wohlgeformtem HTML-Code, die der Seite hinzugefügt werden soll, sowie alle Bild- oder Dateibinärdaten. Wenn der Inhalt Binärdaten enthält, muss die Anforderung unter Verwendung des Inhaltstyps `multipart/form-data` in einem Teil „Commands“ gesendet werden (siehe [Beispiel](#multipart-request-with-binary-content)). 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a>Generierte IDs
Microsoft Graph generiert Werte des Typs **id** für alle Seitenelemente, die aktualisiert werden können. Abrufen können Sie die generierten IDs über den Abfragezeichenfolgenausdruck `includeIDs=true` in der GET-Anforderung:

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> **Hinweis:** Die API verwirft alle Werte des Typs **id**, die im [Eingabe-HTML-Code](onenote-input-output-html.md) von Anforderungen des Typs „create-page“ oder „update-page“ angegeben sind.

Das folgende Beispiel zeigt generierte IDs für einen Absatz und ein Bild im [Ausgabe-HTML-Code](onenote-input-output-html.md) einer Seite.

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

Generierte **id**-Werte ändern sich nach dem Aktualisieren einer Seite möglicherweise, Sie sollten daher die aktuellen Werte abrufen, bevor Sie eine PATCH-Anforderung erstellen, die diese verwendet.
 
Angeben können Sie Zielelemente in Form eines Werts des Typs **data-id** oder eines Werts des Typs **id**. Dabei gilt:

- Bei Aktionen des Typs **append** oder des Typs **insert** können Sie beide ID-Typen als Zielwert verwenden.
- Bei Aktionen des Typs **replace** müssen Sie für alle Elemente die generierte ID verwenden. Ausgenommen hiervon sind lediglich der Seitentitel sowie Bilder und Objekte innerhalb von „div“-Elementen. 
    - Ersetzen eines Titels: Verwenden Sie das Schlüsselwort **title**. 
    - Ersetzen von Bildern und Objekten in einem „div“-Element: Verwenden Sie entweder **data-id** oder **id**.

Im folgenden Beispiel wird das Ziel in Form eines Werts des Typs **id** angegeben. Setzen Sie vor generierten IDs niemals das Präfix #.

```json
[
   {
    'target':'p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}',
    'action':'insert',
    'position':'before',
    'content':'<p>This paragraph goes above the target paragraph.</p>'
  }
]
```

<a name="support-matrix"></a>

## <a name="supported-elements-and-actions"></a>Unterstützte Elemente und Aktionen

Viele Elemente auf einer Seite lassen sich aktualisieren, doch unterstützt jeder Elementtyp nur bestimmte Aktionen. In der folgenden Tabelle sind die unterstützten Zielelemente aufgeführt sowie die Aktualisierungsaktionen, die sie unterstützen.

| Element | Ersetzen | Untergeordnetes Element anfügen | Gleichgeordnetes Element einfügen |  
|------|:------:|:------:|:------:|  
| body<br /> (Ziel: erstes „div“-Element auf der Seite) | Nein | **Ja** | Nein |  
| div<br /> ([absolut positioniert](onenote-abs-pos.md)) | Nein | **Ja** | Nein |  
| div<br /> (in einem anderen „div“-Element) | **Ja**<br/>(nur per „id“) | **Ja** | **Ja** |   
| img, object<br /> (in einem anderen „div“-Element) | **Ja** | Nein | **Ja** |   
| ol, ul | **Ja**<br/>(nur per „id“) | **Ja** | **Ja** |   
| table | **Ja**<br/>(nur per „id“) | Nein | **Ja** |   
| p, li, h1-h6 | **Ja**<br/>(nur per „id“) | Nein | **Ja** |   
| title | **Ja** | Nein | Nein |  
 
<br/>

Die folgenden Elemente unterstützen keinerlei Aktualisierungsaktionen:

- img ([absolut positioniert](onenote-abs-pos.md))
- object ([absolut positioniert](onenote-abs-pos.md))
- tr, td
- meta
- head
- span
- a
- „style“-Tags


<a name="examples"></a>

## <a name="example-requests"></a>Beispielanforderungen

Eine Aktualisierungsanforderung enthält eine oder mehrere Änderungen, jeweils dargestellt als JSON-Änderungsobjekt. Diese Objekte können unterschiedliche Ziele auf der Seite sowie unterschiedliche Aktionen und Inhalte für diese Ziele definieren.

Die folgenden Beispiele zeigen JSON-Objekte, die in PATCH-Anforderungen verwendet werden, sowie vollständige PATCH-Anforderungen:

- [Anfügen von untergeordneten Elementen](#append-child-elements)
- [Einfügen von gleichgeordneten Elementen](#insert-sibling-elements)
- [Ersetzen von Elementen](#replace-elements)
- [Vollständige PATCH-Anforderungen](#complete-patch-request-examples)


<a name="append-examples"></a>

### <a name="append-child-elements"></a>Anfügen von untergeordneten Elementen

Die **append**-Aktion fügt ein untergeordnetes Element zu einem **body**-, **div**- (innerhalb eines div-Elements), **ol**- oder **ul**-Element hinzu. Das **position**-Attribut bestimmt, ob das untergeordnete Element vor oder nach dem Tag angefügt wird. Die Standardposition ist **after**.

#### <a name="append-to-a-div"></a>Anfügen an ein „div“-Element

Das folgende Beispiel fügt dem Element **div1** zwei untergeordnete Knoten hinzu. Als erstes untergeordnetes Element wird ein Bild hinzugefügt, als letztes untergeordnetes Element ein Absatz. 

```json
[
 {
    'target':'#div1',
    'action':'append',
    'position':'before',
    'content':'<img data-id="first-child" src="image-url-or-part-name" />'
  },
  {
    'target':'#div1',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph appended to the div</p>'
  }
]
```
 

#### <a name="append-to-the-body-element"></a>Anfügen an das *body*-Element

Sie können **body** als schnellen Weg verwenden, um ein untergeordnetes Element im ersten „div“-Element auf der Seite anzufügen.

Im folgenden Beispiel werden dem ersten „div“-Element auf der Seite zwei Absätze hinzugefügt, einer als erstes untergeordnetes Element und einer als letztes untergeordnetes Element. Setzen Sie vor ein Ziel des Typs **body** niemals das Präfix #. In diesem Beispiel verwenden wir die Aktion **prepend** als Kurzversion von **append** + **before**.

```json
[
  {
    'target':'body',
    'action':'prepend',
    'content':'<p data-id="first-child">New paragraph as first child in the first div</p>'
  },
  {
    'target':'body',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph as last child in the first div</p>'
  }
]
```
 

#### <a name="append-to-a-list"></a>Anfügen an eine Liste

Im folgenden Beispiel wird ein Listenelement als letztes untergeordnetes Element zur Zielliste hinzugefügt. Die **list-style-type**-Eigenschaft ist definiert, da das Element einen nicht standardmäßigen Listenstil verwendet.

```json
[
  {
    'target':'#circle-ul',
    'action':'append',
    'content':'<li style="list-style-type:circle">Item at the end of the list</li>'
  }
]
```
 

<a name="insert-examples"></a>

### <a name="insert-sibling-elements"></a>Einfügen von gleichgeordneten Elementen

Die Aktion **insert** fügt dem Zielelement ein gleichgeordnetes Element hinzu. Das Attribut **position** legt fest, ob das gleichgeordnete Element vor oder nach dem Ziel eingefügt wird. Die Standardposition ist **after**. In diesem Abschnitt finden Sie alle [Elemente, die **insert** unterstützen](#supported-elements-and-actions).

#### <a name="insert-siblings"></a>Einfügen von gleichgeordneten Elementen

Im folgenden Beispiel werden zwei gleichgeordnete Knoten zu der Seite hinzugefügt. Über dem **para1**-Element wird ein Bild und über dem **para2**-Element wird ein Absatz hinzugefügt.

```json
[
  {
     'target':'#para1',
     'action':'insert',
     'position':'before',
     'content':'<img src="image-url-or-part-name" alt="Image inserted above the target" />'
  },
  {
    'target':'#para2',
     'action':'insert',
     'content':'<p data-id="next-sibling">Paragraph inserted below the target</p>'
  }
]
```
 

<a name="replace-examples"></a>

### <a name="replace-elements"></a>Ersetzen von Elementen

Sie können entweder den Wert **data-id** oder den generierten Wert **id** als Zielwert nutzen, wenn Sie Elemente des Typs **img** oder **object** in einem „div“-Element ersetzen möchten. Verwenden Sie das Schlüsselwort **title**, wenn der Seitentitel ersetzt werden soll. Bei allen anderen [Elementen, die **replace** unterstützen](#supported-elements-and-actions), müssen Sie die generierte ID verwenden.

#### <a name="replace-an-image"></a>Ersetzen eines Bilds

Im folgenden Beispiel wird ein Bild durch ein „div“-Element ersetzt. Als Zielwert wird der Wert **data-id** des Bilds verwendet. 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a>Aktualisieren einer Tabelle 

In diesem Beispiel wird gezeigt, wie eine Tabelle mithilfe ihrer generierten ID aktualisiert wird. Das Ersetzen von **tr**- und **td**-Elementen wird nicht unterstützt, Sie können jedoch die gesamte Tabelle ersetzen.

```json
[
  {
    'target':'table:{de3e0977-94e4-4bb0-8fee-0379eaf47486}{11}',
    'action':'replace',
    'content':'<table data-id="football">
      <tr><td><p><b>Brazil</b></p></td><td><p>Germany</p></td></tr>
      <tr><td><p>France</p></td><td><p><b>Italy</b></p></td></tr>
      <tr><td><p>Netherlands</p></td><td><p><b>Spain</b></p></td></tr>
      <tr><td><p>Argentina</p></td><td><p><b>Germany</b></p></td></tr></table>'
  }
]
```
 

#### <a name="change-the-title"></a>Ändern des Titels 

Dieses Beispiel demonstriert, wie Sie den Titel einer Seite ändern. Verwenden Sie zum Ändern des Titels als Zielwert das Schlüsselwort **title**. Setzen Sie vor ein Ziel des Typs „title“ niemals das Präfix #.

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a>Aktualisieren eines Aufgabenelements

Im folgenden Beispiel wird die Aktion „replace“ verwendet, um das Kontrollkästchen eines Aufgabenelements auf „Abgeschlossen“ zu setzen.

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

Weitere Informationen zum Verwenden des Attributs **data-tag** finden Sie im Artikel zum Thema [Verwenden von Notiztags](onenote-note-tags.md).


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a>Beispiele für vollständige PATCH-Anforderungen

Die folgenden Beispiele zeigen vollständige PATCH-Anforderungen.

#### <a name="request-with-text-content-only"></a>Anforderung ausschließlich mit Textinhalten

Das folgende Beispiel zeigt eine PATCH-Anforderung, die den Inhaltstyp **application/json** verwendet. Dieses Format können Sie verwenden, wenn Ihr Inhalt keine Binärdaten enthält.

```json
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url" alt="New image from a URL" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]
```
 
<a name="multipart"></a>

#### <a name="multipart-request-with-binary-content"></a>Mehrteilige Anforderung mit Binärinhalten 

Das folgende Beispiel zeigt eine mehrteilige PATCH-Anforderung, die Binärdaten enthält. Mehrteilige Anforderungen müssen einen Teil „Commands“ enthalten, in dem der Inhaltstyp **application/json** angegeben ist und der das Array von JSON-Änderungsobjekten enthält. Andere Datenteile dürfen Binärdaten enthalten. Die Namen von Teilen sind in der Regel Zeichenfolgen, an die die aktuelle Zeit in Millisekunden oder eine zufällige GUID angefügt ist.

```json
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: multipart/form-data; boundary=PartBoundary123
Authorization: Bearer {token}

--PartBoundary123
Content-Disposition: form-data; name="Commands"
Content-Type: application/json

[
  {
    'target':'img:{2998967e-69b3-413f-a221-c1a3b5cbe0fc}{42}',
    'action':'replace',
    'content':'<img src="name:image-part-name" alt="New binary image" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]

--PartBoundary123
Content-Disposition: form-data; name="image-part-name"
Content-Type: image/png

... binary image data ...

--PartBoundary123--
```

<a name="request-response-info"></a>

## <a name="request-and-response-information-for-patch-requests"></a>Anforderungs- and Antwortinformationen in PATCH-Anforderungen

| Daten in der Anforderung | Beschreibung |  
|------|------|  
| Protokoll | Alle Anforderungen verwenden das SSL/TLS HTTPS-Protokoll. |  
| Header „Authorization“ | <p>`Bearer {token}`, wobei `{token}` ein gültiges OAuth 2.0-Zugriffstoken für Ihre registrierte App ist.</p><p>Wenn dies fehlt oder ungültig ist, schlägt die Anforderung mit dem Statuscode 401 fehl. Siehe [Authentifizierung und Berechtigungen](permissions-reference.md).</p> |  
| Header „Content-Type“ | <p>`application/json` für das Array von JSON-Änderungsobjekten, unabhängig davon, ob es direkt im Anforderungstext gesendet wird oder im Pflichtteil „Commands“ einer [mehrteiligen Anforderung](#multipart-request-with-binary-content).</p><p>Mehrteilige Anfragen sind erforderlich, wenn Binärdaten gesendet werden sollen. Sie verwenden den Inhaltstyp `multipart/form-data; boundary=part-boundary`, wobei `{part-boundary}` eine Zeichenfolge ist, die den Beginn und das Ende jedes Datenteils signalisiert.</p> |  

<br/> 

| Antwortdaten | Beschreibung |  
|------|------|  
| Erfolgscode | 204 HTTP-Statuscode. Für eine PATCH-Anforderung werden keine JSON-Daten zurückgegeben. |  
| Fehler | Informationen zu OneNote-Fehlern, die Microsoft Graph zurückgeben kann, finden Sie unter [Fehlercodes für OneNote-APIs in Microsoft Graph](onenote-error-codes.md). |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a>Zusammensetzen der Stamm-URL des Microsoft Graph-Diensts

Die Stamm-URL des OneNote-Diensts verwendet das folgende Format für alle Aufrufe der OneNote-API:

`https://graph.microsoft.com/{version}/me/onenote/`

Das Segment `version` in der URL ist die Version von Microsoft Graph, die verwendet werden soll. Setzen Sie `v1.0` für stabilen Produktionscode. Setzen Sie `beta`, wenn Sie ein Feature testen möchten, das sich noch in der Entwicklung befindet. Features und Funktionen in der Betaphase werden möglicherweise noch geändert und sollten daher nicht in Produktionscode verwendet werden.

Setzen Sie `me` für OneNote-Inhalte, auf die der aktuelle Benutzer zugreifen kann (eigene und freigegebene Inhalte). Setzen Sie `users/{id}` für OneNote-Inhalte, die der (in der URL) angegebene Benutzer für den aktuellen Benutzer freigegeben hat. Verwenden Sie dazu die [Azure AD-Graph-API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog).


> **Hinweis:** Benutzer-IDs können Sie über eine GET-Anforderung an `https://graph.microsoft.com/v1.0/users` abrufen.



<a name="permissions"></a>

## <a name="permissions"></a>Berechtigungen

Zum Aktualisieren von OneNote-Seiten müssen Sie die entsprechenden Berechtigungen anfordern. Wählen Sie die niedrigste Berechtigungsstufe, die erforderlich ist, damit Ihre App korrekt funktioniert.

- Notes.ReadWrite
- Notes.ReadWrite.All

Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie unter [OneNote-Berechtigungsbereiche](permissions-reference.md).
   

<a name="see-also"></a>

## <a name="see-also"></a>Siehe auch

- [Hinzufügen von Bildern und Dateien](onenote-images-files.md)
- [Integrieren mit OneNote](integrate-with-onenote.md)
- [OneNote-Entwicklerblog](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Fragen zur OneNote-Entwicklung auf Stack Overflow](https://go.microsoft.com/fwlink/?LinkID=390182)
- [OneNote GitHub-Repos](https://go.microsoft.com/fwlink/?LinkID=390178)  
