---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
ms.openlocfilehash: e7df636f9c406a499baa5ef3be1748273920cac4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885477"
---
# <a name="itempreviewinfo-resource-type"></a>Ressourcentyp itemPreviewInfo

Die Ressource **ItemPreviewInfo** enthält Informationen dazu, wie eine Vorschau einer [DriveItem](driveitem.md)einbetten.

## <a name="json-representation"></a>JSON-Darstellung

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a>Eigenschaften

| Name           | Typ   | Beschreibung
|:---------------|:-------|:---------------------------------------------------
| getUrl         | string | URL für das Einbetten von mit HTTP-GET (Iframes usw.) geeignet
| postUrl        | string | URL für das Einbetten von mithilfe von HTTP POST geeignet (bilden, JS, usw..)
| postParameters | string | POST-Parameter einschließen, wenn PostUrl verwenden

GetUrl, PostUrl oder beide möglicherweise abhängig vom aktuellen Status der Unterstützung für den angegebenen Optionen zurückgegeben.

PostParameters ist eine Zeichenfolge, die als formatiert `application/x-www-form-urlencoded`, und wenn Ausführen von POST an den PostUrl Content-Type entsprechend festgelegt werden sollen. Beispiel:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Die Formate der URLs und Parametern sollten nicht transparent berücksichtigt werden.
