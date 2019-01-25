---
title: 'PrivilegedRole: SelfDeactivate'
description: Deaktivieren Sie die Rolle, die an den Requestor zugewiesen ist.
localization_priority: Normal
ms.openlocfilehash: 7175af64e7e36087bd048cd6e160393e2bf6377e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528690"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="3a67e-103">PrivilegedRole: SelfDeactivate</span><span class="sxs-lookup"><span data-stu-id="3a67e-103">privilegedRole: selfDeactivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a67e-104">Deaktivieren Sie die Rolle, die an den Requestor zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="3a67e-104">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a67e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3a67e-105">Permissions</span></span>
<span data-ttu-id="3a67e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a67e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3a67e-108">Der Requestor kann nur aufgerufen ```selfDeactivate``` für die Rolle, die ihm zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="3a67e-108">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="3a67e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3a67e-109">Permission type</span></span>      | <span data-ttu-id="3a67e-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3a67e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a67e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3a67e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3a67e-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a67e-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3a67e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3a67e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a67e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a67e-114">Not supported.</span></span>    |
|<span data-ttu-id="3a67e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3a67e-115">Application</span></span> | <span data-ttu-id="3a67e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a67e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a67e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a67e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="3a67e-118">Beachten Sie, dass ``<id>`` ist die Id der Ziel-Rolle.</span><span class="sxs-lookup"><span data-stu-id="3a67e-118">Note that ``<id>`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3a67e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3a67e-119">Request headers</span></span>
| <span data-ttu-id="3a67e-120">Name</span><span class="sxs-lookup"><span data-stu-id="3a67e-120">Name</span></span>       | <span data-ttu-id="3a67e-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a67e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3a67e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a67e-122">Authorization</span></span>  | <span data-ttu-id="3a67e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3a67e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a67e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3a67e-125">Request body</span></span>
<span data-ttu-id="3a67e-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3a67e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a67e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a67e-127">Response</span></span>

<span data-ttu-id="3a67e-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekt Code und [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3a67e-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="3a67e-129">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="3a67e-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="3a67e-130">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="3a67e-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="3a67e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3a67e-131">Example</span></span>
<span data-ttu-id="3a67e-132">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="3a67e-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3a67e-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a67e-133">Request</span></span>
<span data-ttu-id="3a67e-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3a67e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```

##### <a name="response"></a><span data-ttu-id="3a67e-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a67e-135">Response</span></span>
<span data-ttu-id="3a67e-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a67e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole: selfDeactivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-selfdeactivate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
