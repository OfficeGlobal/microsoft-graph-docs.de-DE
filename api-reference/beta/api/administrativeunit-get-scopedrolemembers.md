---
title: Abrufen einer scopedRoleMember
description: Rufen Sie eine bestimmte ScopedRoleMembership Ressource ab.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bf707c4bca33302286ab686cf74d9faba63fac7a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971704"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="06be6-103">Abrufen einer scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="06be6-103">Get a scopedRoleMember</span></span>

> <span data-ttu-id="06be6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="06be6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06be6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="06be6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06be6-106">Rufen Sie eine bestimmte [ScopedRoleMembership](../resources/scopedrolemembership.md) Ressource ab.</span><span class="sxs-lookup"><span data-stu-id="06be6-106">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="06be6-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="06be6-107">Permissions</span></span>
<span data-ttu-id="06be6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06be6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="06be6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06be6-110">Permission type</span></span>      | <span data-ttu-id="06be6-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06be6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06be6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06be6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="06be6-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="06be6-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="06be6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06be6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06be6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06be6-115">Not supported.</span></span>    |
|<span data-ttu-id="06be6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06be6-116">Application</span></span> | <span data-ttu-id="06be6-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06be6-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06be6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06be6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="06be6-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="06be6-119">Optional query parameters</span></span>
<span data-ttu-id="06be6-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="06be6-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06be6-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06be6-121">Request headers</span></span>
| <span data-ttu-id="06be6-122">Name</span><span class="sxs-lookup"><span data-stu-id="06be6-122">Name</span></span>      |<span data-ttu-id="06be6-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06be6-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="06be6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="06be6-124">Authorization</span></span>  | <span data-ttu-id="06be6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="06be6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06be6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06be6-127">Request body</span></span>
<span data-ttu-id="06be6-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="06be6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06be6-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="06be6-129">Response</span></span>

<span data-ttu-id="06be6-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und das angeforderte [ScopedRoleMembership](../resources/scopedrolemembership.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="06be6-130">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="06be6-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06be6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06be6-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06be6-132">Request</span></span>
<span data-ttu-id="06be6-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06be6-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="06be6-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="06be6-134">Response</span></span>
<span data-ttu-id="06be6-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06be6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "id": "id-value",
  "roleId": "roleId-value",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleMemberInfo": {
      "id": "id-value",
      "displayName": "displayName-value",
      "userPrincipalName": "userPrincipalName-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List scopedRoleMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
