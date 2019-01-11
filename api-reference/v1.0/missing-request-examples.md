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
# <a name="helpers-examples-that-arent-included-in-the-docs"></a><span data-ttu-id="0529b-103">Hilfsprogramme (Beispiele, die nicht in den Dokumenten enthalten sind)</span><span class="sxs-lookup"><span data-stu-id="0529b-103">Helpers (examples that aren't included in the docs)</span></span>

<span data-ttu-id="0529b-104">Dies sind Dinge, die ich in den Dokumenten hinzufügen musste, damit das Markdown-Scannertool die Graph-Dokumente ordnungsgemäß verarbeiten kann.</span><span class="sxs-lookup"><span data-stu-id="0529b-104">These are things I had to add in the docs to make sure the Markdown-Scanner tool was able to properly handle the Graph docs.</span></span>


## <a name="define-the-me-as-singleton"></a><span data-ttu-id="0529b-105">Definieren von /me als Singleton</span><span class="sxs-lookup"><span data-stu-id="0529b-105">Define the /me as singleton</span></span>

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


## <a name="define-drives-as-an-queryable-entityset"></a><span data-ttu-id="0529b-106">Definieren von Laufwerken als abfragbares Entityset</span><span class="sxs-lookup"><span data-stu-id="0529b-106">Define drives as an queryable entityset</span></span>
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


## <a name="define-users-as-an-queryable-entityset"></a><span data-ttu-id="0529b-107">Definieren von Benutzern als abfragbares Entityset</span><span class="sxs-lookup"><span data-stu-id="0529b-107">define users as an queryable entityset</span></span>

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
