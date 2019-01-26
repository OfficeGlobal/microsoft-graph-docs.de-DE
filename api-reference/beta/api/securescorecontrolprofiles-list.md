---
title: List secureScoreControlProfiles
description: Rufen Sie die Eigenschaften und die Beziehungen eines SecureScoreControlProfiles-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: 6177af7da65d268af7c089aee3772109fb182959
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571093"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="13a0b-103">List secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="13a0b-103">List secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13a0b-104">Rufen Sie die Eigenschaften und die Beziehungen eines [SecureScoreControlProfiles](../resources/securescorecontrolprofiles.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="13a0b-104">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="13a0b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="13a0b-105">Permissions</span></span>

<span data-ttu-id="13a0b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13a0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13a0b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="13a0b-108">Permission type</span></span>      | <span data-ttu-id="13a0b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="13a0b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13a0b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="13a0b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="13a0b-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="13a0b-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="13a0b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="13a0b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="13a0b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13a0b-113">Not supported.</span></span>  |
|<span data-ttu-id="13a0b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="13a0b-114">Application</span></span> | <span data-ttu-id="13a0b-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="13a0b-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13a0b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13a0b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="13a0b-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="13a0b-117">Request headers</span></span>

| <span data-ttu-id="13a0b-118">Name</span><span class="sxs-lookup"><span data-stu-id="13a0b-118">Name</span></span>      |<span data-ttu-id="13a0b-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13a0b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="13a0b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="13a0b-120">Authorization</span></span>  | <span data-ttu-id="13a0b-p102">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="13a0b-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="13a0b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="13a0b-123">Request body</span></span>

<span data-ttu-id="13a0b-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="13a0b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13a0b-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="13a0b-125">Response</span></span>

<span data-ttu-id="13a0b-126">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **SecureScoreControlProfiles** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="13a0b-126">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfiles** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13a0b-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="13a0b-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="13a0b-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="13a0b-128">Request</span></span>

<span data-ttu-id="13a0b-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="13a0b-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="13a0b-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="13a0b-130">Response</span></span>

<span data-ttu-id="13a0b-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="13a0b-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "actionType": "actionType.value",
            "actionUrl": "actionUrl.value",
            "controlCategory": "controlCategory.value",
            "title": "title.value",
            "deprecated": "deprecated.value",
            "implementationCost": "implementationCost.value",
            "lastModifiedDateTime": "lastModifiedDateTime.value",
            "maxScore": "maxScore.value",
            "rank": "rank.value",
            "remediation": "remediation.value",
            "remediationImpact": "remediationImpact.value",
            "service": "service.value",
            "threats": [
                "threats.value"
            ],
            "tier": "tier.value",
            "userImpact": "userImpact.value",
            "id": "id.value",
            "azureTenantId": "azureTenantId.value",
            "controlStateUpdates": [
                {
                    "assignedTo": "assignedTo.value",
                    "comment": "comment.value",
                    "state": "state.value",
                    "updatedBy": "updatedBy.value",
                    "updatedDateTime": "updatedDateTime.value"
                }
            ],
            "vendorInformation": {
                "provider": "SecureScore",
                "providerVersion": null,
                "subProvider": null,
                "vendor": "Microsoft"
            }
         }
     ]
}
```


<!--
{
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescorecontrolprofiles-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
