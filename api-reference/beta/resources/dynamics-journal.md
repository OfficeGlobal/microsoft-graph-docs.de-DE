---
title: Journal-Ressourcentyp
description: Ein Journal in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: bef5008bbacb1729f48758b228e55a3f6adc2af0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365472"
---
# <a name="journal-resource-type"></a>Journal-Ressourcentyp
Stellt ein Journal in Dynamics 365 Business Central dar.

## <a name="methods"></a>Methoden

| Methode                                            |Rückgabetyp|Beschreibung    |
|:--------------------------------------------------|:----------|:--------------|
|[Journal abrufen](../api/dynamics-journal-get.md)      |Journal    |Ruft ein Journal ab.   |
|[Post Journal](../api/dynamics-create-journal.md)  |Journal    |Erstellt ein Journal.|
|[Patch-Journal](../api/dynamics-journal-update.md) |Journal    |Aktualisiert ein Journal.|
|[Journal löschen](../api/dynamics-journal-delete.md)|Keine       |Löscht ein Journal.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft           | Typ                  |Beschreibung                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|id                  |GUID                   |Die eindeutige ID des Journals. Nicht bearbeitbar.           |
|code                |Zeichenfolge, maximale Größe 10| Der Code des Journals.                             |
|displayName         |Zeichenfolge, maximale Größe 50| Der Anzeigename des Journals.                     |
|lastModifiedDateTime|DateTime               |Die letzte DateTime, die das Journal geändert wurde. Schreibgeschützt.|

## <a name="bound-actions"></a>Gebundene Aktionen
Der Ressourcentyp Journal bietet eine gebundene Aktion `post` , die den entsprechenden allgemeinen Journal Batch bereitstellt.

Die Buchung des Fibu Buch.-Blatts wird im folgenden Beispiel veranschaulicht:  
`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.

Die Antwort hat keinen Inhalt; der Antwortcode lautet 204.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

