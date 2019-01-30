---
title: List secureScores
description: Rufen Sie die Eigenschaften und die Beziehungen eines SecureScores-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: e574c3e52eb60f29dac89e2795b04666c7a1f02b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642961"
---
# <a name="list-securescores"></a><span data-ttu-id="e6e02-103">List secureScores</span><span class="sxs-lookup"><span data-stu-id="e6e02-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6e02-104">Rufen Sie die Eigenschaften und die Beziehungen eines [SecureScores](../resources/securescores.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="e6e02-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6e02-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e6e02-105">Permissions</span></span>

<span data-ttu-id="e6e02-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6e02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6e02-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e6e02-108">Permission type</span></span>      | <span data-ttu-id="e6e02-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e6e02-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6e02-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e6e02-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e6e02-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="e6e02-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="e6e02-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e6e02-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e6e02-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e6e02-113">Not supported.</span></span>  |
|<span data-ttu-id="e6e02-114">Application</span><span class="sxs-lookup"><span data-stu-id="e6e02-114">Application</span></span> | <span data-ttu-id="e6e02-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="e6e02-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6e02-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6e02-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="e6e02-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e6e02-117">Request headers</span></span>

| <span data-ttu-id="e6e02-118">Name</span><span class="sxs-lookup"><span data-stu-id="e6e02-118">Name</span></span>      |<span data-ttu-id="e6e02-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6e02-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e6e02-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e6e02-120">Authorization</span></span>  | <span data-ttu-id="e6e02-p102">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e6e02-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6e02-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e6e02-123">Request body</span></span>

<span data-ttu-id="e6e02-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e6e02-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6e02-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6e02-125">Response</span></span>

<span data-ttu-id="e6e02-126">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **SecureScores** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e6e02-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6e02-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e6e02-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6e02-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6e02-128">Request</span></span>

<span data-ttu-id="e6e02-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e6e02-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="e6e02-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6e02-130">Response</span></span>

<span data-ttu-id="e6e02-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e6e02-131">The following is an example of the response.</span></span>
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


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
