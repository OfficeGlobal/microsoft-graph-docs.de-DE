---
author: chackman
ms.author: chackman
title: Gefolgt Listenelemente
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0489c14b943b6fa6eafb41932bb9bb906fea3351
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921479"
---
# <a name="list-followed-items"></a><span data-ttu-id="dab19-102">Gefolgt Listenelemente</span><span class="sxs-lookup"><span data-stu-id="dab19-102">List followed items</span></span>

> <span data-ttu-id="dab19-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dab19-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dab19-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dab19-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dab19-105">Liste der [Elemente](../resources/driveitem.md) , die vom Benutzer angemeldet besucht wurden.</span><span class="sxs-lookup"><span data-stu-id="dab19-105">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="dab19-106">Diese Auflistung enthält Elemente, die sich in dem Laufwerk des Benutzers sowie Elemente, die von anderen Laufwerken zugreifen kann.</span><span class="sxs-lookup"><span data-stu-id="dab19-106">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="dab19-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dab19-107">Permissions</span></span>

<span data-ttu-id="dab19-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dab19-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dab19-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dab19-110">Permission type</span></span>      | <span data-ttu-id="dab19-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dab19-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dab19-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dab19-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dab19-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dab19-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="dab19-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dab19-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dab19-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dab19-115">Not supported.</span></span>    |
|<span data-ttu-id="dab19-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dab19-116">Application</span></span> | <span data-ttu-id="dab19-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dab19-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dab19-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dab19-118">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a><span data-ttu-id="dab19-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="dab19-119">Response</span></span>

<span data-ttu-id="dab19-120">Diese Methode gibt eine Auflistung von [DriveItem](../resources/driveitem.md) Ressourcen für Elemente, die der Besitzer des Laufwerks folgt.</span><span class="sxs-lookup"><span data-stu-id="dab19-120">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="dab19-121">Wenn keine Elemente gefunden wurden, wird eine leere Auflistung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dab19-121">If no items were found, an empty collection is returned.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "name": "March Proposal.docx",
      "size": 19121,
      "lastModifiedDateTime": "2017-12-12T10:40:59Z"
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "size": 37810,
      "lastModifiedDateTime": "2016-10-18T10:40:59Z"
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items"
} -->
