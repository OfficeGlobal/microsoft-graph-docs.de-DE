# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a>Abrufen von OneNote-Inhalten und -Strukturen mit Microsoft Graph

*__Gilt für:__ Privatanwender-Notizbücher auf OneDrive | Enterprise-Notizbücher auf Office 365*

Um OneNote-Inhalte und -Strukturen abzurufen, senden Sie eine GET-Anforderung an den Zielendpunkt. Beispiel:

`GET ../onenote/pages/{id}`</p>

Wenn die Anforderung erfolgreich ist, gibt Microsoft Graph den HTTP-Statuscode 200 und die Entitäten bzw. Inhalte zurück, die Sie angefordert haben. OneNote-Entitäten werden als JSON-Objekte zurückgegeben, die der Spezifikation der OData-Version 4.0 entsprechen.

Mithilfe von Abfragezeichenfolgenoptionen können Sie Ihre Abfragen filtern und die Leistung verbessern.


<a name="request-uri"></a>
## <a name="construct-the-request-uri"></a>Erstellen des Anforderungs-URI

Um den Anforderungs-URI zu erstellen, beginnen Sie mit der Stamm-URL des Diensts:

`https://graph.microsoft.com/v1.0/me/onenote`

Fügen Sie dann den Endpunkt der Ressource an, die Sie abrufen möchten. ([Ressourcenpfade](#resource-paths-for-get-requests) werden im nächsten Abschnitt gezeigt.)


Ihr vollständiger Anforderungs-URI gleicht einem der folgenden Beispiele:
- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`</p>
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`</p>
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`</p>

> **Hinweis:** Hier erfahren Sie mehr über die [Stamm-URL des Diensts](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).

<a name="resource-paths"></a>
## <a name="resource-paths-for-get-requests"></a>Ressourcenpfade für GET-Anforderungen

Verwenden Sie die folgenden Ressourcenpfade, um Seiten, Abschnitte, Abschnittsgruppen, Notizbücher und Bild- oder Dateiressourcen abzurufen.

[Page-Sammlung](#page-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Page-Entität](#page-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Seitenvorschau](#page-preview)&nbsp;&nbsp;|&nbsp;&nbsp;[HTML-Inhalt einer Seite](#page-html-content)&nbsp;&nbsp;|&nbsp;&nbsp;[Section-Sammlung](#section-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Section-Entität](#section-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[SectionGroup-Sammlung](#sectiongroup-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[SectionGroup-Entität](#sectiongroup-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Notebook-Sammlung](#notebook-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Notebook-Entität](#notebook-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Bild oder andere Dateiressource](#image-or-other-file-resource)

<a name="get-pages"></a>
### <a name="page-collection"></a>Page-Sammlung

Abrufen von Seiten (Metadaten) aus allen Notizbüchern

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

Abrufen von Seiten (Metadaten) aus einem bestimmten Abschnitt

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

 
Die `search`-Abfragezeichenfolgenoption ist nur für Heimanwender-Notizbücher verfügbar.

Die Standardsortierreihenfolge für Seiten ist `lastModifiedTime desc`.

Die Standardabfrage erweitert den übergeordneten Abschnitt und wählt die Eigenschaften `id`, `name` und `self` des Abschnitts aus.

Standardmäßig werden nur die ersten 20 Einträge für *GET pages*-Anforderungen zurückgegeben. Anforderungen, die keine **top**-Abfragezeichenfolgenoption enthalten, geben einen **@odata.nextLink**-Link in der Antwort zurück, mit dem Sie die nächsten 20 Einträge abrufen können.

Verwenden Sie für die Sammlung der Seiten in einem Abschnitt **pagelevel**, um die Einzugsebene von Seiten und ihre Reihenfolge innerhalb des Abschnitts zurückzugeben. 

**Beispiel:**  `GET ../sections/{section-id}/pages?pagelevel=true`.

- - -

<a name="get-page"></a> 
### <a name="page-entity"></a>Page-Entität

Abrufen der Metadaten für eine bestimmte Seite. 

`../pages/{page-id}[?select,expand,pagelevel]` 


Seiten können die Eigenschaften **parentNotebook** und **parentSection** erweitern.

Die Standardabfrage erweitert den übergeordneten Abschnitt und wählt die Eigenschaften `id`, `name` und `self` des Abschnitts aus.

Verwenden Sie **pagelevel**, um die Einzugsebene der Seite und ihre Reihenfolge im übergeordneten Abschnitt zurückzugeben. Beispiel: `GET ../pages/{page-id}?pagelevel=true`.

- - -

<a name="get-page-preview"></a> 
### <a name="page-preview"></a>Seitenvorschau

Abrufen von Text- und Bild-Vorschauinhalt für eine Seite

`../pages/{page-id}/preview`


Die JSON-Antwort enthält den Vorschauinhalt, anhand dessen Benutzer feststellen können, was sich auf der Seite befindet.

```json
{
  "@odata.context":"https://www.onenote.com/api/v1.0/$metadata#Microsoft.OneNote.Api.PagePreview",
  "previewText":"text-snippet",
  "links":{
    "previewImageUrl":{
      "href":"https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png"
    }
  }
}
```

Die **previewText**-Eigenschaft enthält einen Textausschnitt von der Seite. Microsoft Graph gibt vollständige Ausdrücke im Umfang von maximal 300 Zeichen zurück. 

Wenn die Seite über ein Bild verfügt, das zum Erstellen einer Vorschau der Benutzeroberfläche verwendet werden kann, enthält die **href**-Eigenschaft im **previewImageUrl**-Objekt einen Link zu einer öffentlichen, vorab authentifizierten [Bildressource](#image-or-other-file-resource). Sie können diesen Link in HTML-Code verwenden.

**Beispiel: ** `<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`. Andernfalls gibt **href** NULL zurück.

- - -

<a name="get-page-content"></a> 
### <a name="page-html-content"></a>HTML-Inhalt einer Seite

Abrufen des HTML-Codes einer Seite `../pages/{page-id}/content[?includeIDs,preAuthenticated]`

(*Weitere Informationen zu [zurückgegebenen HTML-Inhalten](onenote_input_output_html.md)*) 

 
Verwenden Sie die Abfragezeichenfolgenoption **includeIDs=true**, um die zum [Aktualisieren der Seite](onenote_update_page.md) generierten IDs abzurufen.

Verwenden Sie die Abfragezeichenfolgenoption **preAuthenticated=true** zum Abrufen von öffentlichen URLs zu den [Bildressourcen](#image-or-other-file-resource), die sich auf der Seite befinden. Die öffentlichen URLs sind eine Stunde lang gültig. 

- - -

<a name="get-sections"></a>
### <a name="section-collection"></a>Section-Sammlung

Abrufen aller Abschnitte aus allen Notizbüchern im Besitz des Benutzers, einschließlich der Abschnitte in geschachtelten Abschnittsgruppen `../sections[?filter,orderby,select,top,skip,expand,count]` 

Abrufen aller Abschnitte, die sich direkt unter einer bestimmten Abschnittsgruppe befinden

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

Abrufen aller Abschnitte, die sich direkt unter einem bestimmten Notizbuch befinden `../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

 
Abschnitte können die Eigenschaften **parentNotebook** und **parentSectionGroup** erweitern.

Die Standardsortierreihenfolge für Abschnitte ist `name asc`.

Die Standardabfrage erweitert das übergeordnete Notizbuch und die übergeordnete Abschnittsgruppe und wählt deren Eigenschaften `id`, `name` und `self` aus.

- - -

<a name="get-section"></a>
### <a name="section-entity"></a>Section-Entität

Abrufen eines bestimmten Abschnitts

`../sections/{section-id}[?select,expand]` 

 
Abschnitte können die Eigenschaften **parentNotebook** und **parentSectionGroup** erweitern.

Die Standardabfrage erweitert das übergeordnete Notizbuch und die übergeordnete Abschnittsgruppe und wählt deren Eigenschaften `id`, `name` und `self` aus.

- - -

<a name="get-section-groups"></a>
### <a name="sectiongroup-collection"></a>SectionGroup-Sammlung

Abrufen aller Abschnittsgruppen aus allen Notizbüchern im Besitz des Benutzers, einschließlich geschachtelter Abschnittsgruppen

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

Abrufen aller Abschnittsgruppen, die sich direkt unter einem bestimmten Notizbuch befinden 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

Abschnittsgruppen können die Eigenschaften **sections**, **sectionGroups**, **parentNotebook** und **parentSectionGroup** erweitern.

Die Standardsortierreihenfolge für Abschnittsgruppen ist `name asc`.

Die Standardabfrage erweitert das übergeordnete Notizbuch und die übergeordnete Abschnittsgruppe und wählt deren Eigenschaften `id`, `name` und `self` aus.

- - -

<a name="get-section-group"></a>
### <a name="sectiongroup-entity"></a>SectionGroup-Entität

Abrufen einer bestimmten Abschnittsgruppe

`../sectionGroups/{sectiongroup-id}[?select,expand]` 


Abschnittsgruppen können die Eigenschaften **sections**, **sectionGroups**, **parentNotebook** und **parentSectionGroup** erweitern.

Die Standardabfrage erweitert das übergeordnete Notizbuch und die übergeordnete Abschnittsgruppe und wählt deren Eigenschaften `id`, `name` und `self` aus.

- - -

<a name="get-notebooks"></a>
### <a name="notebook-collection"></a>Notebook-Sammlung

Abrufen aller Notizbücher, deren Eigentümer der Benutzer ist 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

 
Notizbücher können die Eigenschaften **sections** und **sectionGroups** erweitern.

Die Standardsortierreihenfolge für Notizbücher ist `name asc`. 

- - -

<a name="get-notebook"></a>
### <a name="notebook-entity"></a>Notebook-Entität

Abrufen eines bestimmten Notizbuchs `../notebooks/{notebook-id}[?select,expand]` 


Notizbücher können die Eigenschaften **sections** und **sectionGroups** erweitern.

- - -

<a name="get-resource"></a>
### <a name="image-or-other-file-resource"></a>Bild- oder andere Dateiressource

Abrufen der Binärdaten einer bestimmten Ressource 

`../resources/{resource-id}/$value` 


Sie finden den Ressourcen-URI der Datei im [Ausgabe-HTML-Code](onenote_input_output_html.md) der Seite.

Beispielsweise enthält ein **img**-Tag Endpunkte für das Originalbild im **data-fullres-src**-Attribut und das optimierte Bild im **src**-Attribut. 

**Beispiel:**

```
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

Und ein **object**-Tag enthält den Endpunkt für die Dateiressource im **data**-Attribut. 

**Beispiel:**

```
<object
    data="http://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

Um öffentliche, vorab authentifizierte URLs für die Bildressourcen auf einer Seite zu erhalten, fügen Sie **preAuthenticated=true** in die Abfragezeichenfolge ein, wenn Sie [die Seiteninhalte abrufen](#page-html-content) (**Beispiel:**  `GET ../pages/{page-id}/content?preAuthenticated=true`). Die öffentlichen URLs, die im [Ausgabe-HTML-Code](onenote_input_output_html.md#output-html-examples-for-images) zurückgegeben werden, sind eine Stunde lang gültig. Ohne dieses Flag können Bilder nicht direkt in einem Browser gerendert werden, da sie wie die restlichen Seiteninhalte privat sind und eine Autorisierung erforderlich ist, um sie abzurufen. 

> **Hinweis:** Das Abrufen einer Sammlung von Ressourcen wird nicht unterstützt. 

Beim Abrufen einer Dateiressource müssen Sie keinen **Accept**-Inhaltstyp in der Anforderung angeben.

Weitere Informationen zu GET-Anforderungen finden Sie unter: 
- [GET Pages](../api-reference/v1.0/api/page_get.md)
- [GET Sections](../api-reference/v1.0/api/section_get.md)
- [GET SectionGroups](../api-reference/v1.0/api/sectiongroup_get.md)
- [GET Notebooks](../api-reference/v1.0/api/notebook_get.md) 

in der Microsoft Graph-API-REST-Referenz.


<a name="example"></a>
## <a name="example-get-requests"></a>Beispiele für GET-Anforderungen
Sie können Abfragen für OneNote-Entitäten stellen und Seiteninhalte durchsuchen, um genau die gesuchten Informationen zu erhalten. Die folgenden Beispiele zeigen einige Verwendungsmöglichkeiten für [unterstützte Abfragezeichenfolgenoptionen](#supported-odata-query-string-options) in GET-Anforderungen für Microsoft Graph. 

**Zur Erinnerung:**

- Alle GET-Anforderungen beginnen mit der [Stamm-URL des Diensts](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).

  **Beispiele:** 
  - `https://www.onenote.com/api/v1.0/me/notes`
  - `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`

- Leerzeichen in der URL-Abfragezeichenfolge müssen mit %20 codiert sein.

Beispiel: `filter=title%20eq%20'biology'`

- Bei Eigenschaftennamen und OData-Zeichenfolgenvergleichen wird die Groß-/Kleinschreibung beachtet. Wir empfehlen die Verwendung der OData-Funktion **tolower** für Zeichenfolgenvergleiche.

   Beispiel: `filter=tolower(name) eq 'spring'`
 

**search & filter**  

Abrufen aller Seiten, die den Begriff *recipe* enthalten und von einer bestimmten App erstellt wurden.  (`search` ist nur für Heimanwender-Notizbücher verfügbar)

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
**search & select**  

Abrufen des Titels, der OneNote-Clientlinks und des **contentUrl**-Links für alle Seiten, die den Begriff *golgi app* enthalten.  (`search` ist nur für Heimanwender-Notizbücher verfügbar)

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
**expand**  

Abrufen aller Notizbücher und Erweitern ihrer Abschnitte und Abschnittsgruppen.  

```
[GET] ../notebooks?expand=sections,sectionGroups
```
 
Abrufen einer bestimmten Abschnittsgruppe und Erweitern ihrer Abschnitte und Abschnittsgruppen:  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

Abrufen einer Seite und Erweitern Ihres übergeordneten Abschnitts und übergeordneten Notizbuchs.

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

**expand** (mehrere Ebenen)  

Abrufen aller Notizbücher und Erweitern ihrer Abschnitte und Abschnittsgruppen sowie aller Abschnitte in jeder Abschnittsgruppe.  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
>Das Erweitern übergeordneter Elemente von untergeordneten Entitäten oder das Erweitern von untergeordneten Elementen von übergeordneten Entitäten erstellt einen Zirkelbezug und wird nicht unterstützt.

 
**expand & select** (mehrere Ebenen)  

Abrufen des Namens und des **self**-Links für eine bestimmte Abschnittsgruppe sowie des Namens und **self**-Links für alle enthaltenen Abschnitte.  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```
 
Abrufen des Namens und des **self**-Links für alle Abschnitte sowie des Namens und der Erstellungszeit des übergeordneten Notizbuchs jedes Abschnitts.  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```
 
Abrufen des Titels und der ID für alle Seiten sowie Abrufen des Namens des übergeordneten Abschnitts und des übergeordneten Notizbuchs.

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

**expand & levels** (mehrere Ebenen)  

Abrufen aller Notizbücher, Abschnitte und Abschnittsgruppen.  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
**filter**  

Abrufen aller Abschnitte, die im Oktober 2014 erstellt wurden.

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

Abrufen der Seiten, die von einer bestimmten App seit dem 1. Januar 2015 erstellt wurden.

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

**filter & expand**  

Abrufen aller Seiten in einem bestimmten Notizbuch. Die API gibt standardmäßig 20 Seiten zurück.

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

Abrufen des Namens und des **pagesUrl**-Links für alle Abschnitte aus dem Notizbuch *School*. In OData-Zeichenfolgenvergleichen wird die Groß-/Kleinschreibung beachtet. Verwenden Sie daher am besten die **tolower**-Funktion.

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

**filter & select & orderby**   

Abrufen des Namens und des **pagesUrl**-Links für alle Abschnitte, die den Ausdruck *spring* im Abschnittsnamen enthalten. Sortieren der Abschnitte nach dem Datum der letzten Änderung.

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
**orderby**  

Abrufen der ersten 20 Seiten, sortiert nach der **createdByAppId**-Eigenschaft und dann nach der letzten Erstellungszeit. Die API gibt standardmäßig 20 Seiten zurück.

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

**search & filter & top**  

Abrufen der fünf neuesten Seiten, die seit dem 1. Januar 2015 erstellt wurden und die den Ausdruck *cell division* enthalten. Die API gibt standardmäßig 20 und maximal 100 Einträge zurück. Die Standardsortierreihenfolge für Seiten ist `lastModifiedTime desc`. (`search` ist nur für Heimanwender-Notizbücher verfügbar)

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

**search & filter & top & skip**  

Abrufen der nächsten fünf Seiten im Resultset. (`search` ist nur für Heimanwender-Notizbücher verfügbar)

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

Und der nächsten fünf. (`search` ist nur für Heimanwender-Notizbücher verfügbar)

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> **Hinweis:** Wenn **search** und **filter** auf dieselbe Anforderung angewendet werden, enthält das Ergebnis nur die Entitäten, die beide Kriterien erfüllen.
 
**select**  

Abrufen von Name, Erstellungszeit und **self**-Link für alle Abschnitte in den Notizbüchern des Benutzers.

```
[GET] ../sections?select=name,createdTime,self
```

Abrufen des Titels, der Erstellungszeit und der OneNote-Clientlinks für eine bestimmte Seite.

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

**select & expand & filter** (mehrere Ebenen)  

Abrufen von Name und **pagesUrl**-Link für alle Abschnitte im Standardnotizbuch des Benutzers.

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

**top & select & orderby**  

Abrufen des Titels und des **self**-Links für die ersten 50 Seiten, alphabetisch sortiert nach Titel. Die API gibt standardmäßig 20 und maximal 100 Einträge zurück. Die Standardsortierreihenfolge für Seiten ist `lastModifiedTime desc`.

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

**skip & top & select & orderby**  

Abrufen der Seiten 51 bis 100. Die API gibt standardmäßig 20 und maximal 100 Einträge zurück.

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> **Hinweis:** GET-Anforderungen für Seiten, die die Standardanzahl von Einträgen abrufen (d. h., sie enthalten keinen **top**-Ausdruck) geben einen **@odata.nextLink**-Link in der Antwort zurück, mit dem Sie die nächsten 20 Einträge abrufen können.
 

<a name="query-options"></a>
## <a name="supported-odata-query-string-options"></a>Unterstützte Optionen für OData-Abfragezeichenfolgen

Beim Senden von GET-Anforderungen an Microsoft Graph können Sie die Abfrage mit Optionen für OData-Abfragezeichenfolgen anpassen und so genau die gewünschten Informationen erhalten. Sie können auch eine Leistungssteigerung erzielen, indem die Anzahl der Aufrufe an den Dienst und die Größe der Antwortnutzlast reduziert wird.

> **Hinweis:** Zur besseren Lesbarkeit wird in den Beispielen in diesem Artikel nicht die erforderliche Prozentcodierung %20 für Leerzeichen in der URL-Abfragezeichenfolge verwendet: `filter=isDefault%20eq%20true`
 
| Abfrageoption | Beispiel und Beschreibung |  
|------|------|  
| count | <p>`count=true`</p><p>Die Anzahl der Entitäten in der Sammlung. Der Wert wird in der Antwort in der **@odata.count**-Eigenschaft zurückgegeben.</p> |  
| expand | <p>`expand=sections,sectionGroups`</p><p>Die Navigationseigenschaften, die inline in der Antwort zurückgegeben werden sollen. Die folgenden Eigenschaften werden für **expand**-Ausdrücke unterstützt:<br /> – Seiten: **parentNotebook**, **parentSection**<br /> – Abschnitte: **parentNotebook**, **parentSectionGroup**<br /> – Abschnittsgruppen: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**<br /> – Notizbücher: **sections**, **sectionGroups**</p><p>Standardmäßig erweitern GET-Anforderungen für Seiten **parentSection** und wählen die Eigenschaften **id**, **name** und **self** des Abschnitts aus. Standardmäßig erweitern GET-Anforderungen für Abschnitte und Abschnittsgruppen **parentNotebook** und **parentSectionGroup** und wählen die Eigenschaften **id**, **name** und **self** der übergeordneten Elemente aus. </p><p>Kann für eine einzelne Entität oder eine Sammlung verwendet werden. Trennen Sie mehrere Eigenschaften durch Kommas. Bei Eigenschaftennamen wird die Groß-/Kleinschreibung beachtet.</p> |   
| filter | <p>`filter=isDefault eq true`</p><p>Ein boolescher Ausdruck, der angibt, ob ein Eintrag in das Resultset aufgenommen werden soll. Unterstützt die folgenden OData-Operatoren und -Funktionen:<br /> – Vergleichsoperatoren: **eq**, **ne**, **gt**, **ge**, **lt**, **le**<br /> – Logische Operatoren: **and**, **or**, **not**<br /> – Zeichenfolgenfunktionen: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</p><p>Bei [Eigenschaften](#onenote-entity-properties)namen und OData-Zeichenfolgenvergleichen wird die Groß-/Kleinschreibung beachtet. Wir empfehlen die Verwendung der OData-Funktion **tolower** für Zeichenfolgenvergleiche. Beispiel: `filter=tolower(name) eq 'spring'`</p> |  
| orderby | <p>`orderby=title,createdTime desc`</p><p>Die [Eigenschaften](#onenote-entity-properties), nach denen sortiert werden soll, mit einer optionalen Sortierreihenfolge **asc** (Standard) oder **desc**. Sie können nach jeder beliebigen Eigenschaft der Entität in der angeforderten Sammlung sortieren.</p><p>Die Standardsortierreihenfolge für Notizbücher, Abschnittsgruppen und Abschnitte ist `name asc` und für Seiten `lastModifiedTime desc` (zuletzt geänderte Seite zuerst).</p><p>Trennen Sie mehrere Eigenschaften durch Kommas, und führen Sie sie in der Reihenfolge auf, in der sie angewendet werden sollen. Bei Eigenschaftennamen wird die Groß-/Kleinschreibung beachtet.</p> |  
| search | <p>`search=cell div`</p><p>Nur für Heimanwender-Notizbücher verfügbar.</p><p>Der zu suchende Begriff oder Ausdruck im Seitentitel, Seitentext, Alternativtext für Bilder und OCR-Text für Bilder. Standardmäßig werden die Ergebnisse von Suchabfragen nach Relevanz sortiert zurückgegeben.</p><p>OneNote verwendet die Bing-Volltextsuche, um die Suche nach Wortgruppen, Wortstammerkennung, Toleranz gegen Rechtschreibfehler, Relevanz und Bewertung, Worttrennung, mehrere Sprachen und andere Volltext-Suchfunktionen zu unterstützen. In Suchzeichenfolgen wird die Groß-/Kleinschreibung nicht beachtet.</p><p>Gilt nur für Seiten in Notizbüchern im Besitz des Benutzers (nicht in für den Benutzer freigegebenen). Indizierter Inhalt ist privat und nur für den Besitzer zugänglich. Kennwortgeschützte Seiten werden nicht indiziert. Gilt nur für den `pages`-Endpunkt.</p> |  
| select | <p>`select=id,title`</p><p>Die [Eigenschaften](#onenote-entity-properties), die zurückgegeben werden sollen. Kann für eine einzelne Entität oder eine Sammlung verwendet werden. Trennen Sie mehrere Eigenschaften durch Kommas. Bei Eigenschaftennamen wird die Groß-/Kleinschreibung beachtet.</p> |  
| skip | <p>`skip=10`</p><p>Die Anzahl der Einträge, die im Resultset übersprungen werden sollen. In der Regel für die Seitenverwaltung der Ergebnisse verwendet.</p> |  
| Nach oben | <p>`top=50`</p><p>Die Anzahl der zurückzugebenden Einträge im Resultset, maximal 100. Der Standardwert ist 20.</p> |  

Microsoft Graph bietet außerdem die `pagelevel`-Zeichenfolgenoption, mit der Sie die Ebene und die Reihenfolge der Seiten innerhalb des übergeordneten Abschnitts abrufen können. Gilt nur für Abfragen für Seiten in einem bestimmten Abschnitt oder für Abfragen für eine bestimmte Seite. 

**Beispiel:** 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a>Unterstützte OData-Operatoren und -Funktionen

Microsoft Graph unterstützt die folgenden OData-Operatoren und Funktionen in **filter**-Ausdrücken. Beachten Sie bei der Verwendung von OData-Ausdrücken Folgendes:  
- Leerzeichen in der URL-Abfagezeichenfolge müssen durch die Codierung `%20` ersetzt werden.

   **Beispiel:** `filter=isDefault%20eq%20true`
- Bei Eigenschaftennamen und OData-Zeichenfolgenvergleichen wird die Groß-/Kleinschreibung beachtet. Wir empfehlen die Verwendung der OData-Funktion **tolower** für Zeichenfolgenvergleiche.
   
   **Beispiel:** `filter=tolower(name) eq 'spring'`

| Vergleichsoperator | Beispiel |  
|------|------|  
| eq<br />(gleich) | `createdByAppId eq '{app-id}'` |  
| ne<br />(nicht gleich) | `userRole ne 'Owner'` |  
| gt<br />(größer als) | `createdTime gt 2014-02-23` |  
| ge<br />(größer als oder gleich) | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| lt<br />(kleiner als) | `createdTime lt 2014-02-23` |  
| le<br />(kleiner als oder gleich) | `lastModifiedTime le 2014-02-23` |  
 
| Logischer Operator | Beispiel |  
|------|------|  
| und | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| oder | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| not | `not contains(tolower(title),'school')` |  
 
| String-Funktion | Beispiel |  
|------|------|   
| contains | `contains(tolower(title),'spring')` |  
| endswith | `endswith(tolower(title),'spring')` |  
| startswith | `startswith(tolower(title),'spring')` |  
| length | `length(title) eq 19` |  
| indexof | `indexof(tolower(title),'spring') eq 1` |  
| substring | `substring(tolower(title),1) eq 'spring'` |  
| tolower | `tolower(title) eq 'spring'` |  
| toupper | `toupper(title) eq 'SPRING'` |  
| trim | `trim(tolower(title)) eq 'spring'` |  
| concat | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>
## <a name="onenote-entity-properties"></a>OneNote-Entitätseigenschaften

Die Abfrageausdrücke **filter**, **select**, **expand** und **orderby** können Eigenschaften von OneNote-Entitäten enthalten. 

**Beispiel:**

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

Bei Eigenschaftennamen in Abfrageausdrücken wird die Groß-/Kleinschreibung beachtet.

Die Liste der Eigenschaften und Eigenschaftentypen finden Sie unter:

- [GET Pages](../api-reference/v1.0/api/page_get.md)
- [GET Sections](../api-reference/v1.0/api/section_get.md)
- [GET SectionGroups](../api-reference/v1.0/api/sectiongroup_get.md)
- [GET Notebooks](../api-reference/v1.0/api/notebook_get.md) 

in der Microsoft Graph-API-REST-Referenz.

Die Abfragezeichenfolgenoption **expand** kann mit folgenden Navigationseigenschaften verwendet werden:

- Seiten: **parentNotebook**, **parentSection**
- Abschnitte: **parentNotebook**, **parentSectionGroup**
- Abschnittsgruppen: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**
- Notizbücher: **sections**, **sectionGroups**


<a name="request-response-info"></a>
## <a name="request-and-response-information-for-get-requests"></a>Anforderungs- and Antwortinformationen für *GET*-Anforderungen

| Anforderungsdaten | Beschreibung |  
|------|------|  
| Protokoll | Alle Anforderungen verwenden das SSL/TLS HTTPS-Protokoll. |  
| Header „Authorization“ | <p>`Bearer {token}`, wobei *{token}* ein gültiges OAuth 2.0-Zugriffstoken für Ihre registrierte App ist.</p><p>Wenn dies fehlt oder ungültig ist, schlägt die Anforderung mit dem Statuscode 401 fehl. Siehe [Authentifizierung und Berechtigungen](permissions_reference.md).</p> |  
| Header „Accept“ | <p>- `application/json` für OneNote-Entitäten und -Entitätenmengen</p><p>- `text/html` für Seiteninhalt</p> | 

| Antwortdaten | Beschreibung |  
|------|------|  
| Erfolgscode | HTTP-Statuscode 200. |  
| Antworttext | Eine OData-Darstellung der Entität oder der Entitätenmenge im JSON-Format, der HTML-Code der Seite oder Binärdaten der Dateiressource.  |  
| Fehler | Wenn die Anforderung nicht erfüllt wird, gibt die API [Fehler](onenote_error_codes.md) im **@api.diagnostics**-Objekt im Antworttext zurück. |  
| Header „X-CorrelationId“ | Ein globaler Bezeichner (GUID), über den die Anforderung eindeutig identifiziert wird. Sie können diesen Wert zusammen mit dem Wert des Date-Headers verwenden, um zusammen mit dem Microsoft Support Probleme zu behandeln. |  


<a name="root-url"></a>
### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a>Erstellen der Stamm-URL des Microsoft Graph-Notizendiensts

Die Stamm-URL des Microsoft Graph-Notizendienses verwendet das folgende Format für alle Aufrufe von Microsoft Graph-Notizen. `https://graph.microsoft.com/{version}/me/onenote/`  Das `version`-Segment in der URL stellt die Version von Microsoft Graph dar, die Sie verwenden möchten. Verwenden Sie `v1.0` für stabilen Produktionscode. Verwenden Sie `beta`, um ein Feature zu testen, das sich in der Entwicklung befindet. Features und Funktionen in der Betaversion ändern sich möglicherweise, sodass Sie es nicht in Ihrem Produktionscode verwenden sollten. Verwenden Sie `me` für OneNote-Inhalt, auf den der aktuelle Benutzer zugreifen kann (eigene und freigegebene Inhalte). Verwenden Sie `users/{id}` für OneNote-Inhalte, die der (in der URL) angegebene Benutzer für den aktuellen Benutzer freigegeben hat. Verwenden Sie [Microsoft Graph](https://graph.microsoft.com/v1.0/users), um Benutzer-IDs abzurufen. 


<a name="permissions"></a>
## <a name="permissions-for-get-requests"></a>Berechtigungen für GET-Anforderungen

Um OneNote-Inhalte oder -Strukturen abzurufen, müssen Sie entsprechende Berechtigungen anfordern. 

Die folgenden Bereiche lassen GET-Anforderungen für Microsoft Graph zu. Wählen Sie die niedrigste Berechtigungsstufe, die Ihre App zur Erledigung ihrer Aufgaben benötigt.

Wählen Sie zwischen: 
- Notes.Read
- Notes.ReadWrite
- Notes.ReadWrite.All


Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie in der [Microsoft Graph-Berechtigungsreferenz](permissions_reference.md).

<a name="see-also"></a>
## <a name="additional-resources"></a>Weitere Ressourcen

- [Eingabe- und Ausgabe-HTML für OneNote-Seiten](onenote_input_output_html.md)
- [Integrieren in OneNote](integrate_with_onenote.md)
- [OneNote-Entwicklerblog](http://go.microsoft.com/fwlink/?LinkID=390183)
- [Fragen zur OneNote-Entwicklung auf Stack Overflow](http://go.microsoft.com/fwlink/?LinkID=390182)
- [OneNote GitHub-Repos](http://go.microsoft.com/fwlink/?LinkID=390178)  
