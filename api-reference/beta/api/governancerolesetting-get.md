---
title: Abrufen von governanceRoleSetting
description: Abrufen der Eigenschaften und Beziehungen zwischen einer GovernanceRoleSetting.
localization_priority: Normal
ms.openlocfilehash: 2c432c0f680acd2411d57ab6e4b4a7af21f3350a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511037"
---
# <a name="get-governancerolesetting"></a><span data-ttu-id="eff40-103">Abrufen von governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="eff40-103">Get governanceRoleSetting</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eff40-104">Abrufen der Eigenschaften und Beziehungen zwischen einer [GovernanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="eff40-104">Retrieve the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eff40-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="eff40-105">Permissions</span></span>
<span data-ttu-id="eff40-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eff40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eff40-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eff40-108">Permission type</span></span>      | <span data-ttu-id="eff40-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="eff40-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eff40-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eff40-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eff40-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="eff40-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="eff40-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eff40-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eff40-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eff40-113">Not supported.</span></span>    |
|<span data-ttu-id="eff40-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eff40-114">Application</span></span> | <span data-ttu-id="eff40-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="eff40-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="eff40-116">Neben den Berechtigungsbereich benötigt diese API den Requestor mindestens eine rollenzuweisung für die Ressource verfügen, die die [GovernanceRoleSetting](../resources/governancerolesetting.md) gehört.</span><span class="sxs-lookup"><span data-stu-id="eff40-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleSetting](../resources/governancerolesetting.md) belongs to.</span></span>
## <a name="http-request"></a><span data-ttu-id="eff40-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eff40-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eff40-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="eff40-118">Optional query parameters</span></span>
<span data-ttu-id="eff40-119">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="eff40-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eff40-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eff40-120">Request headers</span></span>
| <span data-ttu-id="eff40-121">Name</span><span class="sxs-lookup"><span data-stu-id="eff40-121">Name</span></span>      |<span data-ttu-id="eff40-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eff40-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eff40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eff40-123">Authorization</span></span>  | <span data-ttu-id="eff40-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="eff40-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="eff40-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eff40-125">Request body</span></span>
<span data-ttu-id="eff40-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="eff40-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="eff40-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="eff40-127">Response</span></span>
<span data-ttu-id="eff40-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [GovernanceRoleSetting](../resources/governancerolesetting.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="eff40-128">If successful, this method returns a `200 OK` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eff40-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eff40-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eff40-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eff40-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9
```
##### <a name="response"></a><span data-ttu-id="eff40-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="eff40-131">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governancerolesetting-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
