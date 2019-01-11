---
title: List secureScores
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 6bf0a1e1964c93043bad4a81ab812786627ea737
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831815"
---
# <a name="list-securescores"></a><span data-ttu-id="44a81-104">List secureScores</span><span class="sxs-lookup"><span data-stu-id="44a81-104">List secureScores</span></span>

 > <span data-ttu-id="44a81-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="44a81-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44a81-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="44a81-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44a81-107">Rufen Sie die Eigenschaften und die Beziehungen eines [SecureScores](../resources/securescores.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="44a81-107">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="44a81-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="44a81-108">Permissions</span></span>

<span data-ttu-id="44a81-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44a81-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44a81-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="44a81-111">Permission type</span></span>      | <span data-ttu-id="44a81-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="44a81-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44a81-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="44a81-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="44a81-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="44a81-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="44a81-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="44a81-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="44a81-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44a81-116">Not supported.</span></span>  |
|<span data-ttu-id="44a81-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="44a81-117">Application</span></span> | <span data-ttu-id="44a81-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="44a81-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44a81-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="44a81-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="44a81-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="44a81-120">Request headers</span></span>

| <span data-ttu-id="44a81-121">Name</span><span class="sxs-lookup"><span data-stu-id="44a81-121">Name</span></span>      |<span data-ttu-id="44a81-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44a81-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="44a81-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44a81-123">Authorization</span></span>  | <span data-ttu-id="44a81-p104">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="44a81-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44a81-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="44a81-126">Request body</span></span>

<span data-ttu-id="44a81-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="44a81-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44a81-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="44a81-128">Response</span></span>

<span data-ttu-id="44a81-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **SecureScores** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="44a81-129">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44a81-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="44a81-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="44a81-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44a81-131">Request</span></span>

<span data-ttu-id="44a81-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44a81-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="44a81-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="44a81-133">Response</span></span>

<span data-ttu-id="44a81-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="44a81-134">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScores"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "value": [
        {
            "activeUserCount": "activeUserCount.value",
            "createdDateTime": "createdDateTime.value",
            "currentScore": "currentScore.value",
            "enabledServices": "enabledServices.value",
            "licensedUserCount": "licensedUserCount.value",
            "maxScore": "maxScore.value",
            "id": "id.value",
            "azureTenantId": "azureTenantId.value",
            "averageComparativeScores": [
                {
                    "basis": "AllTenants",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value"
                },
                {
                    "basis": "TotalSeats",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value",
                    "seatSizeRangeUpperValue": "seatSizeRangeUpperValue.value",
                    "categoryValue": "categoryValue.value",
                    "seatSizeRangeLowerValue": "seatSizeRangeLowerValue.value"
                },
                {
                    "basis": "IndustryTypes",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value",
                    "categoryValue": "categoryValue.value"
                }
            ],
            "controlScores": [
                {
                    "controlCategory": "controlCategory.value",
                    "controlName": "controlName.value",
                    "description": "description.value",
                    "score": "score.value",
                    "total": "total.value",
                    "count": "count.value"
                }
            ]
        }
    ]            
}

```


<!-- {
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
