---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo - OneDrive-API
ms.openlocfilehash: 3fa9d10ae3aade7be96e81168b34df84698da1c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059802"
---
# <a name="itempreviewinfo-resource-type"></a>Ressourcentyp ItemPreviewInfo

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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