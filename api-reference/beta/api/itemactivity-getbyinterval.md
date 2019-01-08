---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Rufen Sie Element-Aktivität Stats ab, indem Sie Intervall
ms.openlocfilehash: 3b3c7139678715a11365f2551c318dcf66e68e7a
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748192"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="e5078-102">Rufen Sie Element-Aktivität Stats ab, indem Sie Intervall</span><span class="sxs-lookup"><span data-stu-id="e5078-102">Get item activity stats by interval</span></span>

> <span data-ttu-id="e5078-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e5078-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5078-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e5078-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5078-105">Rufen Sie [ItemActivityStats][] für die Aktivitäten, die stattgefunden unter diese Ressource innerhalb des angegebenen Zeitintervalls.</span><span class="sxs-lookup"><span data-stu-id="e5078-105">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="e5078-106">**Hinweis:** Die Ressource **ItemAnalytics** ist noch nicht in allen [nationalen Bereitstellungen](/graph/deployments)verfügbar.</span><span class="sxs-lookup"><span data-stu-id="e5078-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="e5078-107">Analytics Aggregate möglicherweise nicht für alle Aktivitätstypen von zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="e5078-107">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="e5078-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e5078-109">Permissions</span></span>

<span data-ttu-id="e5078-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5078-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5078-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e5078-112">Permission type</span></span>                        | <span data-ttu-id="e5078-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e5078-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="e5078-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e5078-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5078-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5078-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="e5078-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e5078-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5078-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e5078-117">Not supported.</span></span>
|<span data-ttu-id="e5078-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e5078-118">Application</span></span>                            | <span data-ttu-id="e5078-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5078-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="e5078-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5078-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="e5078-121">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="e5078-121">Function parameters</span></span>

| <span data-ttu-id="e5078-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="e5078-122">Parameter</span></span>      | <span data-ttu-id="e5078-123">Typ</span><span class="sxs-lookup"><span data-stu-id="e5078-123">Type</span></span>               | <span data-ttu-id="e5078-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5078-124">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="e5078-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e5078-125">startDateTime</span></span>  | <span data-ttu-id="e5078-126">Zeichenfolge (Zeitstempel)</span><span class="sxs-lookup"><span data-stu-id="e5078-126">string (timestamp)</span></span> | <span data-ttu-id="e5078-127">Die Anfangszeit über die aggregierte Aktivitäten.</span><span class="sxs-lookup"><span data-stu-id="e5078-127">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="e5078-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e5078-128">endDateTime</span></span>    | <span data-ttu-id="e5078-129">Zeichenfolge (Zeitstempel)</span><span class="sxs-lookup"><span data-stu-id="e5078-129">string (timestamp)</span></span> | <span data-ttu-id="e5078-130">Die Endzeit über die aggregierte Aktivitäten.</span><span class="sxs-lookup"><span data-stu-id="e5078-130">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="e5078-131">Intervall</span><span class="sxs-lookup"><span data-stu-id="e5078-131">interval</span></span>       | <span data-ttu-id="e5078-132">string</span><span class="sxs-lookup"><span data-stu-id="e5078-132">string</span></span>             | <span data-ttu-id="e5078-133">Das Intervall Aggregation.</span><span class="sxs-lookup"><span data-stu-id="e5078-133">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="e5078-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e5078-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e5078-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5078-135">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a><span data-ttu-id="e5078-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5078-136">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivityStat)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "startDateTime": "2017-01-01T00:00:00.000Z",
            "endDateTime": "2017-01-02T00:00:00.000Z",
            "delete": {
                "actionCount": 1,
                "actorCount": 1
            },
            "access": {
                "actionCount": 5,
                "actorCount": 3
            }
        },
        {
            "startDateTime": "2017-01-02T00:00:00.000Z",
            "endDateTime": "2017-01-03T00:00:00.000Z",
            "edit": {
                "actionCount": 3,
                "actorCount": 1
            },
            "access": {
                "actionCount": 7,
                "actorCount": 6
            }
        }
    ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get activities by interval"
} -->
