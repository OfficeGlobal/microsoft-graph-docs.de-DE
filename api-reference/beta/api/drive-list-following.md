---
author: chackman
ms.author: chackman
title: Gefolgt Listenelemente
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: df38a11a09f4ec86eb029f236030cc4565e5d939
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523309"
---
# <a name="list-followed-items"></a><span data-ttu-id="0641d-102">Gefolgt Listenelemente</span><span class="sxs-lookup"><span data-stu-id="0641d-102">List followed items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0641d-103">Liste der [Elemente](../resources/driveitem.md) , die vom Benutzer angemeldet besucht wurden.</span><span class="sxs-lookup"><span data-stu-id="0641d-103">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="0641d-104">Diese Auflistung enthält Elemente, die sich in dem Laufwerk des Benutzers sowie Elemente, die von anderen Laufwerken zugreifen kann.</span><span class="sxs-lookup"><span data-stu-id="0641d-104">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="0641d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0641d-105">Permissions</span></span>

<span data-ttu-id="0641d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0641d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0641d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0641d-108">Permission type</span></span>      | <span data-ttu-id="0641d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0641d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0641d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0641d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0641d-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0641d-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0641d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0641d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0641d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0641d-113">Not supported.</span></span>    |
|<span data-ttu-id="0641d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0641d-114">Application</span></span> | <span data-ttu-id="0641d-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0641d-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0641d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0641d-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a><span data-ttu-id="0641d-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="0641d-117">Response</span></span>

<span data-ttu-id="0641d-118">Diese Methode gibt eine Auflistung von [DriveItem](../resources/driveitem.md) Ressourcen für Elemente, die der Besitzer des Laufwerks folgt.</span><span class="sxs-lookup"><span data-stu-id="0641d-118">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="0641d-119">Wenn keine Elemente gefunden wurden, wird eine leere Auflistung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0641d-119">If no items were found, an empty collection is returned.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
