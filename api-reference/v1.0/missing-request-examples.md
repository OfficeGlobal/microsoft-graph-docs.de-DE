---
title: Definieren von /me als Singleton
description: Hierbei handelt es sich um Dinge, die ich hatte in der Dokumentation, um sicherzustellen, dass den Abzugsverteilung(en)-Scanner hinzu
localization_priority: Normal
ms.openlocfilehash: da71bfcb25efbebdf4e6a111f23d8d16e3aca342
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842896"
---
# <a name="helpers-examples-that-arent-included-in-the-docs"></a>Hilfsprogramme (Beispiele, die nicht in den Dokumenten enthalten sind)

Dies sind Dinge, die ich in den Dokumenten hinzufügen musste, damit das Markdown-Scannertool die Graph-Dokumente ordnungsgemäß verarbeiten kann.


## <a name="define-the-me-as-singleton"></a>Definieren von /me als Singleton

<!-- {"blockType": "request", "name": "get_current_user" } -->
```http
GET https://graph.microsoft.com/v1.0/me
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-drives-as-an-queryable-entityset"></a>Definieren von Laufwerken als abfragbares Entityset
<!-- {"blockType": "request", "name": "get_drive_from_id" } -->
```http
GET https://graph.microsoft.com/v1.0/drives/{drive-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.drive", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-users-as-an-queryable-entityset"></a>Definieren von Benutzern als abfragbares Entityset

<!-- {"blockType": "request", "name": "get_users" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{user-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
