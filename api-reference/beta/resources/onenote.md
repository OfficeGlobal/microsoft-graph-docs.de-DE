---
title: onenote-Ressourcentyp
description: Der Einstiegspunkt für OneNote-Ressourcen.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 5ed063fb485acdbd029a977ffb6cd721bf7085c8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508727"
---
# <a name="onenote-resource-type"></a>onenote-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Der Einstiegspunkt für OneNote-Ressourcen.

Alle Aufrufe des OneNote-Diensts über die Microsoft Graph-API verwenden diese Dienststamm-URL:

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

Der Speicherort kann Benutzer Notizbücher auf Office 365 oder Consumer OneDrive, Gruppe Notebooks oder SharePoint-Website gehosteten Team Notizbücher auf Office 365 sein. 

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
**SharePoint-Websiten-Notizbücher** VerwendenSie die folgende Dienststamm-URL, um auf Notizbücher zuzugreifen, die einer SharePoint-Teamwebsite gehören:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a>Authorization

Informationen über die erforderlichen Berechtigungen zum Arbeiten mit OneNote-APIs finden Sie unter [Notizenberechtigungen](/graph/permissions-reference#notes-permissions).

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
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
|[Notizbuch erstellen](../api/onenote-post-notebooks.md) |[Notizbuch](notebook.md)| Dient zum Erstellen eines Notizbuchs durch Veröffentlichung in der notebooks-Sammlung.|
|[Notizbücher auflisten](../api/onenote-list-notebooks.md) |[Notebook](notebook.md)-Sammlung| Dient zum Abrufen einer Sammlung von Notizbüchern.|
|[Seite erstellen](../api/onenote-post-pages.md) |[Seite](page.md)| Dient zum Erstellen einer Seite durch Veröffentlichung in der pages-Sammlung.|
|[Seiten auflisten](../api/onenote-list-pages.md) |[Page](page.md)-Sammlung| Dient zum Abrufen einer Sammlung von Seiten.|
|[Abschnittsgruppen auflisten](../api/onenote-list-sectiongroups.md) |[SectionGroup](sectiongroup.md)-Sammlung| Dient zum Abrufen einer Sammlung von Abschnittsgruppen.|
|[Abschnitte auflisten](../api/onenote-list-sections.md) |[Section](section.md)-Sammlung| Dient zum Abrufen einer Sammlung von Abschnitten.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenote.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
