---
title: List secureScoreControlProfiles
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: cd13e4349119202f5f9e026973f3a90ee99f1019
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884553"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="13385-104">List secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="13385-104">List secureScoreControlProfiles</span></span>

 > <span data-ttu-id="13385-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="13385-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13385-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13385-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13385-107">Rufen Sie die Eigenschaften und die Beziehungen eines [SecureScoreControlProfiles](../resources/securescorecontrolprofiles.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="13385-107">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="13385-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="13385-108">Permissions</span></span>

<span data-ttu-id="13385-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13385-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13385-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="13385-111">Permission type</span></span>      | <span data-ttu-id="13385-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="13385-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13385-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="13385-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="13385-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="13385-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="13385-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="13385-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="13385-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13385-116">Not supported.</span></span>  |
|<span data-ttu-id="13385-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="13385-117">Application</span></span> | <span data-ttu-id="13385-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="13385-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13385-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13385-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="13385-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="13385-120">Request headers</span></span>

| <span data-ttu-id="13385-121">Name</span><span class="sxs-lookup"><span data-stu-id="13385-121">Name</span></span>      |<span data-ttu-id="13385-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13385-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="13385-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="13385-123">Authorization</span></span>  | <span data-ttu-id="13385-p104">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="13385-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="13385-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="13385-126">Request body</span></span>

<span data-ttu-id="13385-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="13385-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13385-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="13385-128">Response</span></span>

<span data-ttu-id="13385-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **SecureScoreControlProfiles** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="13385-129">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfiles** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13385-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="13385-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="13385-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="13385-131">Request</span></span>

<span data-ttu-id="13385-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="13385-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="13385-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="13385-133">Response</span></span>

<span data-ttu-id="13385-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="13385-134">The following is an example of the response.</span></span>
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


<!-- {
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
