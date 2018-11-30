---
title: Abrufen von governanceRoleSetting
description: Abrufen der Eigenschaften und Beziehungen zwischen einer GovernanceRoleSetting.
ms.openlocfilehash: 2b0a54fc31ec18816e32bfa2377ddcc0974ac09d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063048"
---
# <a name="get-governancerolesetting"></a><span data-ttu-id="5ab36-103">Abrufen von governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="5ab36-103">Get governanceRoleSetting</span></span>


> <span data-ttu-id="5ab36-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5ab36-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ab36-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5ab36-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5ab36-106">Abrufen der Eigenschaften und Beziehungen zwischen einer [GovernanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="5ab36-106">Retrieve the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5ab36-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5ab36-107">Permissions</span></span>
<span data-ttu-id="5ab36-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ab36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ab36-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5ab36-110">Permission type</span></span>      | <span data-ttu-id="5ab36-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5ab36-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ab36-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5ab36-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5ab36-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="5ab36-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="5ab36-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5ab36-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ab36-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5ab36-115">Not supported.</span></span>    |
|<span data-ttu-id="5ab36-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5ab36-116">Application</span></span> | <span data-ttu-id="5ab36-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="5ab36-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="5ab36-118">Neben den Berechtigungsbereich benötigt diese API den Requestor mindestens eine rollenzuweisung für die Ressource verfügen, die die [GovernanceRoleSetting](../resources/governancerolesetting.md) gehört.</span><span class="sxs-lookup"><span data-stu-id="5ab36-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleSetting](../resources/governancerolesetting.md) belongs to.</span></span>
## <a name="http-request"></a><span data-ttu-id="5ab36-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ab36-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5ab36-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5ab36-120">Optional query parameters</span></span>
<span data-ttu-id="5ab36-121">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5ab36-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ab36-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5ab36-122">Request headers</span></span>
| <span data-ttu-id="5ab36-123">Name</span><span class="sxs-lookup"><span data-stu-id="5ab36-123">Name</span></span>      |<span data-ttu-id="5ab36-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5ab36-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5ab36-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ab36-125">Authorization</span></span>  | <span data-ttu-id="5ab36-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5ab36-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ab36-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5ab36-127">Request body</span></span>
<span data-ttu-id="5ab36-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5ab36-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5ab36-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ab36-129">Response</span></span>
<span data-ttu-id="5ab36-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [GovernanceRoleSetting](../resources/governancerolesetting.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5ab36-130">If successful, this method returns a `200 OK` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5ab36-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5ab36-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ab36-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ab36-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9
```
##### <a name="response"></a><span data-ttu-id="5ab36-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ab36-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 370

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleSettings/$entity",
    "id": "80dc5d6f-8d89-47b3-953f-01dc909ed3f9",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "5b8bea96-e9f6-4c63-a8e9-fb092c79f0a1",
    "isDefault": false,
    "lastUpdatedDateTime": "2018-03-26T21:21:43.113Z",
    "lastUpdatedBy": "Vishal Seri",
    "adminEligibleSettings": [
        {
            "ruleIdentifier": "ExpirationRule",
            "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
        }
    ],
    "adminMemberSettings": [
        {
            "ruleIdentifier": "ExpirationRule",
            "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":43200}"
        },
        {
            "ruleIdentifier": "MfaRule",
            "setting": "{\"mfaRequired\":false}"
        },
        {
            "ruleIdentifier": "JustificationRule",
            "setting": "{\"required\":true}"
        }
    ],
    "userEligibleSettings": [],
    "userMemberSettings": [
        {
            "ruleIdentifier": "ExpirationRule",
            "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":480}"
        },
        {
            "ruleIdentifier": "MfaRule",
            "setting": "{\"mfaRequired\":false}"
        },
        {
            "ruleIdentifier": "JustificationRule",
            "setting": "{\"required\":true}"
        },
        {
            "ruleIdentifier": "ApprovalRule",
            "setting": "{\"Enabled\":true,\"Approvers\":[{\"Id\":\"20083cf1-b8d8-43be-9d37-96adfb09e619\",\"Type\":\"User\",\"DisplayName\":\"Vishal Seri\",\"Email\":\"viseri@fimdev.net\"},{\"Id\":\"d158e1b0-5080-4088-a1e7-9ca54f39eb53\",\"Type\":\"User\",\"DisplayName\":\"viseri\",\"Email\":\"viseri@microsoft.com\"}],\"BusinessFlowId\":\"8df9e93a-6ba9-4453-af43-07cb95435032\"}"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
