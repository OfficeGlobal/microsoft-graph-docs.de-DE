# <a name="onenote-resource-type"></a>onenote-Ressourcentyp

Der Einstiegspunkt für OneNote-Ressourcen.

Alle Aufrufe des OneNote-Diensts über die Microsoft Graph-API verwenden diese Dienststamm-URL:

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

Der Speicherort können Benutzernotizbücher in Office 365 oder im OneDrive-Consumerdienst sowie Gruppennotizbüchern in Office 365 sein. Auf der SharePoint-Website gehostete Notizbücher werden derzeit nicht unterstützt. 

**Benutzernotizbücher** Verwenden Sie einen der folgenden URLs, um auf persönliche Notizbücher im OneDrive-Consumerdienst oder in OneDrive for Business zuzugreifen:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

**Gruppennotizbücher** Verwenden Sie die folgende Dienststamm-URL, um auf Notizbücher zuzugreifen, die im Besitz einer Gruppe sind:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

Die folgenden Berechtigungsbereiche bieten verschiedene Zugriffsstufen auf OneNote-Notizbücher. Das Auswählen von Berechtigungsbereichen ist sowohl vom Speicherort der gewünschten Notizbücher als auch von der Funktionalität Ihrer App abhängig. 

**Bereiche für persönliche Notizbücher im OneDrive-Consumerdienst oder in OneDrive for Business, die im Besitz des aktuellen Benutzers sind**

| Bereich | Berechtigung im Azure-Portal | Beschreibung |
|:-------|:------|:------|
| Notes.Create | Erstellen von OneNote-Notizbüchern von Benutzern | Die Titel Ihrer OneNote-Notizbücher und -Abschnitte können angezeigt werden; es werden neue Notizbücher, Abschnitte und Seiten erstellt. |
| Notes.Read | Lesezugriff auf OneNote-Notizbücher von Benutzern | Ihre OneNote-Notizbücher können gelesen werden. |
| Notes.ReadWrite | Lese- und Schreibzugriff auf OneNote-Notizbücher von Benutzern | Ihre OneNote-Notizbücher können gelesen, freigegeben und geändert werden. |

**Bereiche für persönliche Notizbücher, die von anderen Benutzern freigegeben werden, und Gruppennotizbücher, auf die der aktuelle Benutzer zugreifen kann**

| Bereich | Berechtigung im Azure-Portal | Beschreibung |
|:-------|:------|:------|
| Notes.Read.All | Lesezugriff auf alle OneNote-Notizbücher, auf die der Benutzer Zugriff hat | Alle OneNote-Notizbücher, auf die der angemeldete Benutzer Zugriff hat, können gelesen werden. |
| Notes.ReadWrite.All | Lese- und Schreibzugriff auf alle OneNote-Notizbücher, auf die der Benutzer Zugriff hat | Alle OneNote-Notizbücher, auf die der angemeldete Benutzer Zugriff hat, können gelesen, freigegeben und geändert werden. |

**Hinweis:** Das Zugreifen auf SharePoint-Website-Notizbücher über die Graph-API wird derzeit nicht unterstützt.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "notebooks",
    "pages",
    "resources",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.onenote"
}-->

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|Notizbücher|[Notebook](notebook.md)-Sammlung|Die Sammlung von OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind. Schreibgeschützt. Lässt Nullwerte zu.|
|Vorgänge|[Operation](onenoteoperation.md)-Sammlung |Der Status von OneNote-Vorgängen. Das Abrufen einer operations-Sammlung wird nicht unterstützt, Sie können aber den Status von lange dauernden Vorgängen abrufen, wenn der `Operation-Location`-Header in der Antwort zurückgegeben wird. Schreibgeschützt. Lässt Nullwerte zu.|
|Seiten|[Page](page.md)-Sammlung|Die Seiten in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.|
|Ressourcen|[Ressourcensammlung](resource.md) |Das Bild und andere Dateiressourcen in OneNote-Seiten. Das Abrufen einer Ressourcensammlung wird nicht unterstützt, Sie können aber [den binären Inhalt einer bestimmten Ressource abrufen](resource.md). Schreibgeschützt. Lässt Nullwerte zu.|
|sectionGroups|[SectionGroup](sectiongroup.md)-Sammlung|Die Abschnittsgruppen in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.|
|Abschnitte|[Section](section.md)-Sammlung|Die Abschnitte in allen OneNote-Notizbüchern, die im Besitz des Benutzers oder der Gruppe sind.  Schreibgeschützt. Lässt Nullwerte zu.|


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Notizbuch erstellen](../api/onenote_post_notebooks.md) |[Notizbuch](notebook.md)| Dient zum Erstellen eines Notizbuchs durch Veröffentlichung in der notebooks-Sammlung.|
|[Notizbücher auflisten](../api/onenote_list_notebooks.md) |[Notebook](notebook.md)-Sammlung| Dient zum Abrufen einer Sammlung von Notizbüchern.|
|[Seite erstellen](../api/onenote_post_pages.md) |[Seite](page.md)| Dient zum Erstellen einer Seite durch Veröffentlichung in der pages-Sammlung.|
|[Seiten auflisten](../api/onenote_list_pages.md) |[Page](page.md)-Sammlung| Dient zum Abrufen einer Sammlung von Seiten.|
|[Abschnittsgruppen auflisten](../api/onenote_list_sectiongroups.md) |[SectionGroup](sectiongroup.md)-Sammlung| Dient zum Abrufen einer Sammlung von Abschnittsgruppen.|
|[Abschnitte auflisten](../api/onenote_list_sections.md) |[Section](section.md)-Sammlung| Dient zum Abrufen einer Sammlung von Abschnitten.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
