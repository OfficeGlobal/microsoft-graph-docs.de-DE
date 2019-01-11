---
title: 'PrivilegedRole: SelfDeactivate'
description: Deaktivieren Sie die Rolle, die an den Requestor zugewiesen ist.
localization_priority: Normal
ms.openlocfilehash: 5d3d23acd63609ad6f2b4b53db1be328c03aba1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868789"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="6024d-103">PrivilegedRole: SelfDeactivate</span><span class="sxs-lookup"><span data-stu-id="6024d-103">privilegedRole: selfDeactivate</span></span>

> <span data-ttu-id="6024d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6024d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6024d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6024d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6024d-106">Deaktivieren Sie die Rolle, die an den Requestor zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="6024d-106">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="6024d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6024d-107">Permissions</span></span>
<span data-ttu-id="6024d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6024d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6024d-110">Der Requestor kann nur aufgerufen ```selfDeactivate``` für die Rolle, die ihm zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="6024d-110">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="6024d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6024d-111">Permission type</span></span>      | <span data-ttu-id="6024d-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6024d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6024d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6024d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6024d-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6024d-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6024d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6024d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6024d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6024d-116">Not supported.</span></span>    |
|<span data-ttu-id="6024d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6024d-117">Application</span></span> | <span data-ttu-id="6024d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6024d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6024d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6024d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="6024d-120">Beachten Sie, dass ``<id>`` ist die Id der Ziel-Rolle.</span><span class="sxs-lookup"><span data-stu-id="6024d-120">Note that ``<id>`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6024d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6024d-121">Request headers</span></span>
| <span data-ttu-id="6024d-122">Name</span><span class="sxs-lookup"><span data-stu-id="6024d-122">Name</span></span>       | <span data-ttu-id="6024d-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6024d-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6024d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6024d-124">Authorization</span></span>  | <span data-ttu-id="6024d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6024d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6024d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6024d-127">Request body</span></span>
<span data-ttu-id="6024d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6024d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6024d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6024d-129">Response</span></span>

<span data-ttu-id="6024d-130">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekt Code und [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6024d-130">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="6024d-131">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="6024d-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="6024d-132">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="6024d-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="6024d-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6024d-133">Example</span></span>
<span data-ttu-id="6024d-134">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="6024d-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6024d-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6024d-135">Request</span></span>
<span data-ttu-id="6024d-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6024d-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```

##### <a name="response"></a><span data-ttu-id="6024d-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="6024d-137">Response</span></span>
<span data-ttu-id="6024d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6024d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRole: selfDeactivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
