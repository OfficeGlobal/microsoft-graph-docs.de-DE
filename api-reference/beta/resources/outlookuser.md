---
title: outlookUser-Ressourcentyp
description: Stellt die für einen Benutzer verfügbaren Outlook-Dienste dar.
author: angelgolfer-ms
ms.openlocfilehash: 51926b84b2e8ed19225369eda774408ae6031b58
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319971"
---
# <a name="outlookuser-resource-type"></a>outlookUser-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die für einen Benutzer verfügbaren Outlook-Dienste dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Kategorie erstellen](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) |Erstellen eines **outlookCategory**-Objekts in der Masterliste von Kategorien.|
|[Kategorien auflisten](../api/outlookuser-list-mastercategories.md) | [outlookCategory](outlookcategory.md)-Sammlung |Ruft alle Kategorien ab, die für den Benutzer definiert wurden.|
|[Erstellen von outlookTaskFolder](../api/outlookuser-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| Erstellen Sie einen Aufgabenordner in der Standardgruppe Aufgabe (`My Tasks`) für das Postfach des Benutzers.|
|[Liste taskFolders](../api/outlookuser-list-taskfolders.md) |[OutlookTaskFolder](outlooktaskfolder.md) -Auflistung| Rufen Sie alle Outlook Aufgabenordner im Postfach des Benutzers.|
|[Erstellen von outlookTaskGroup](../api/outlookuser-post-taskgroups.md) |[outlookTaskGroup](outlooktaskgroup.md)| Erstellen eines Outlook-"Task Group" im Postfach des Benutzers an.|
|[Liste taskGroups](../api/outlookuser-list-taskgroups.md) |[OutlookTaskGroup](outlooktaskgroup.md) -Auflistung| Rufen Sie die Outlook-Vorgangsgruppen im Postfach des Benutzers.|
|[Erstellen von outlookTask](../api/outlookuser-post-tasks.md) |[outlookTask](outlooktask.md)| Erstellen Sie eine Outlook-Aufgabe in der Standardgruppe Aufgabe (`My Tasks`) und Aufgabe Standardordner (`Tasks`) in das Postfach des Benutzers.|
|[Aufgaben auflisten](../api/outlookuser-list-tasks.md) |[OutlookTask](outlooktask.md) -Auflistung| Rufen Sie die Outlook-Aufgaben in das Postfach des Benutzers.|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md) | [localeInfo](localeinfo.md)-Sammlung | Abrufen der Liste von Gebietsschemas und Sprachen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert. |
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md) | [timeZoneInformation](timezoneinformation.md)-Sammlung | Abrufen der Liste von Zeitzonen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert. |


## <a name="properties"></a>Eigenschaften
Keine

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|masterCategories|[outlookCategory](../resources/outlookcategory.md)-Sammlung| Eine Liste von Kategorien, die für den Benutzer definiert sind. | 
|taskFolders|[OutlookTaskFolder](outlooktaskfolder.md) -Auflistung| Outlook-Aufgabe-Ordner des Benutzers. Schreibgeschützt. Lässt Nullwerte zu.|
|taskGroups|[OutlookTaskGroup](outlooktaskgroup.md) -Auflistung| Der Benutzer Outlook Vorgangsgruppen. Schreibgeschützt. Lässt Nullwerte zu.|
|tasks|[OutlookTask](outlooktask.md) -Auflistung| Outlook-Aufgaben des Benutzers. Schreibgeschützt. Lässt Nullwerte zu.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->