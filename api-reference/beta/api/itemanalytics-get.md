---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Analysen abrufen
localization_priority: Normal
ms.openlocfilehash: d1f6b255747cffe7fdccb5d098e73a56151b6245
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516259"
---
# <a name="get-analytics"></a><span data-ttu-id="5ac73-102">Analysen abrufen</span><span class="sxs-lookup"><span data-stu-id="5ac73-102">Get analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ac73-103">Rufen Sie [ItemAnalytics][] über die Ansichten, die unter diese Ressource durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="5ac73-103">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="5ac73-104">Die **ItemAnalytics** Ressource ist eine bequeme Möglichkeit zum Abrufen der Aktivität Statistik für `allTime` und die `lastSevenDays`.</span><span class="sxs-lookup"><span data-stu-id="5ac73-104">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="5ac73-105">Verwenden Sie für einen benutzerdefinierten Zeitbereich oder Intervall [GetActivitiesByInterval][] API.</span><span class="sxs-lookup"><span data-stu-id="5ac73-105">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="5ac73-106">**Hinweis:** Die Ressource **ItemAnalytics** ist noch nicht in allen [nationalen Bereitstellungen](/graph/deployments)verfügbar.</span><span class="sxs-lookup"><span data-stu-id="5ac73-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="5ac73-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5ac73-109">Permissions</span></span>

<span data-ttu-id="5ac73-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ac73-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ac73-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5ac73-112">Permission type</span></span>                        | <span data-ttu-id="5ac73-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5ac73-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="5ac73-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5ac73-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ac73-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ac73-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="5ac73-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5ac73-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ac73-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5ac73-117">Not supported.</span></span>
|<span data-ttu-id="5ac73-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5ac73-118">Application</span></span>                            | <span data-ttu-id="5ac73-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ac73-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="5ac73-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ac73-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="5ac73-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5ac73-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5ac73-122">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ac73-122">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

#### <a name="response"></a><span data-ttu-id="5ac73-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ac73-123">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "allTime": {
        "access": {
            "actionCount": 123,
            "actorCount": 89
        }
    },
    "lastSevenDays": {
        "access": {
            "actionCount": 52,
            "actorCount": 41
        }
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": [
    "Error: /api-reference/beta/api/itemanalytics-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
