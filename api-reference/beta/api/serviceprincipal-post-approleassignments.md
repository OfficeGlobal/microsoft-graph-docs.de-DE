---
title: Erstellen von appRoleAssignment
description: Verwenden Sie diese API, um eine neue AppRoleAssignment erstellen.
localization_priority: Normal
ms.openlocfilehash: ce498312f294ff11b97f12b136a6f48ebb4d3791
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886982"
---
# <a name="create-approleassignment"></a><span data-ttu-id="54c5f-103">Erstellen von appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="54c5f-103">Create appRoleAssignment</span></span>

> <span data-ttu-id="54c5f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="54c5f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54c5f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="54c5f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54c5f-106">Verwenden Sie diese API, um eine neue AppRoleAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="54c5f-106">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="54c5f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="54c5f-107">Permissions</span></span>
<span data-ttu-id="54c5f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54c5f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54c5f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="54c5f-110">Permission type</span></span>      | <span data-ttu-id="54c5f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="54c5f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54c5f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="54c5f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="54c5f-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="54c5f-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="54c5f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="54c5f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54c5f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54c5f-115">Not supported.</span></span>    |
|<span data-ttu-id="54c5f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="54c5f-116">Application</span></span> | <span data-ttu-id="54c5f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54c5f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="54c5f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="54c5f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="54c5f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="54c5f-119">Request headers</span></span>
| <span data-ttu-id="54c5f-120">Name</span><span class="sxs-lookup"><span data-stu-id="54c5f-120">Name</span></span>       | <span data-ttu-id="54c5f-121">Typ</span><span class="sxs-lookup"><span data-stu-id="54c5f-121">Type</span></span> | <span data-ttu-id="54c5f-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54c5f-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="54c5f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="54c5f-123">Authorization</span></span>  | <span data-ttu-id="54c5f-124">string</span><span class="sxs-lookup"><span data-stu-id="54c5f-124">string</span></span>  | <span data-ttu-id="54c5f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="54c5f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54c5f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="54c5f-127">Request body</span></span>
<span data-ttu-id="54c5f-128">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [AppRoleAssignment](../resources/approleassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="54c5f-128">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="54c5f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="54c5f-129">Response</span></span>

<span data-ttu-id="54c5f-130">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [AppRoleAssignment](../resources/approleassignment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="54c5f-130">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54c5f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="54c5f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54c5f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="54c5f-132">Request</span></span>
<span data-ttu-id="54c5f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="54c5f-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="54c5f-134">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [AppRoleAssignment](../resources/approleassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="54c5f-134">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="54c5f-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="54c5f-135">Response</span></span>
<span data-ttu-id="54c5f-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="54c5f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment"
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
<!-- {
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
