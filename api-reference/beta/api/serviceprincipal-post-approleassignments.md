---
title: Erstellen von appRoleAssignment
description: Verwenden Sie diese API, um eine neue AppRoleAssignment erstellen.
localization_priority: Normal
ms.openlocfilehash: 33bf7a577b01b2f23132a2b761bd80f24e8268c7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574340"
---
# <a name="create-approleassignment"></a><span data-ttu-id="ae2ed-103">Erstellen von appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ae2ed-103">Create appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae2ed-104">Verwenden Sie diese API, um eine neue AppRoleAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="ae2ed-104">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae2ed-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ae2ed-105">Permissions</span></span>
<span data-ttu-id="ae2ed-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae2ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae2ed-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae2ed-108">Permission type</span></span>      | <span data-ttu-id="ae2ed-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae2ed-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae2ed-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae2ed-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae2ed-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae2ed-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae2ed-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae2ed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae2ed-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae2ed-113">Not supported.</span></span>    |
|<span data-ttu-id="ae2ed-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae2ed-114">Application</span></span> | <span data-ttu-id="ae2ed-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae2ed-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae2ed-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae2ed-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="ae2ed-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae2ed-117">Request headers</span></span>
| <span data-ttu-id="ae2ed-118">Name</span><span class="sxs-lookup"><span data-stu-id="ae2ed-118">Name</span></span>       | <span data-ttu-id="ae2ed-119">Typ</span><span class="sxs-lookup"><span data-stu-id="ae2ed-119">Type</span></span> | <span data-ttu-id="ae2ed-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae2ed-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ae2ed-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae2ed-121">Authorization</span></span>  | <span data-ttu-id="ae2ed-122">string</span><span class="sxs-lookup"><span data-stu-id="ae2ed-122">string</span></span>  | <span data-ttu-id="ae2ed-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae2ed-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae2ed-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae2ed-125">Request body</span></span>
<span data-ttu-id="ae2ed-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [AppRoleAssignment](../resources/approleassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae2ed-126">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ae2ed-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae2ed-127">Response</span></span>

<span data-ttu-id="ae2ed-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [AppRoleAssignment](../resources/approleassignment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ae2ed-128">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae2ed-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae2ed-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae2ed-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae2ed-130">Request</span></span>
<span data-ttu-id="ae2ed-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae2ed-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
<span data-ttu-id="ae2ed-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [AppRoleAssignment](../resources/approleassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae2ed-132">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ae2ed-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae2ed-133">Response</span></span>
<span data-ttu-id="ae2ed-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae2ed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-post-approleassignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
