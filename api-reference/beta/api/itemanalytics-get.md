---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Abrufen von analytics
ms.openlocfilehash: 57f009e0d2a07a5bf8c9a0f3b3617083bc279545
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062399"
---
# <a name="get-analytics"></a><span data-ttu-id="c1780-102">Abrufen von analytics</span><span class="sxs-lookup"><span data-stu-id="c1780-102">Get analytics</span></span>

> <span data-ttu-id="c1780-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c1780-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1780-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1780-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c1780-105">Rufen Sie [ItemAnalytics][] über die Ansichten, die unter diese Ressource durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="c1780-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="c1780-106">Die **ItemAnalytics** Ressource ist eine bequeme Möglichkeit zum Abrufen der Aktivität Statistik für `allTime` und die `lastSevenDays`.</span><span class="sxs-lookup"><span data-stu-id="c1780-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="c1780-107">Verwenden Sie für einen benutzerdefinierten Zeitbereich oder Intervall [GetActivitiesByInterval][] API.</span><span class="sxs-lookup"><span data-stu-id="c1780-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="c1780-108">**Hinweis:** Die Ressource **ItemAnalytics** ist noch nicht in allen [nationalen Bereitstellungen](/graph/deployments)verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c1780-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="c1780-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c1780-111">Permissions</span></span>

<span data-ttu-id="c1780-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1780-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1780-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1780-114">Permission type</span></span>                        | <span data-ttu-id="c1780-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1780-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="c1780-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1780-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1780-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1780-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="c1780-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1780-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1780-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1780-119">Not supported.</span></span>
|<span data-ttu-id="c1780-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1780-120">Application</span></span>                            | <span data-ttu-id="c1780-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1780-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c1780-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1780-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="c1780-123">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1780-123">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c1780-124">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1780-124">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

#### <a name="response"></a><span data-ttu-id="c1780-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1780-125">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics"
} -->
