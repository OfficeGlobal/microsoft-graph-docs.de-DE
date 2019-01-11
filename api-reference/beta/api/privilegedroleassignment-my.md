---
title: 'PrivilegedRoleAssignment: Meine'
description: Rufen Sie das jeweilige privilegierten rollenzuweisungen.
localization_priority: Normal
ms.openlocfilehash: fca950413d2f0a50b6ea9e09b859d2ecf926261b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840257"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="ec740-103">PrivilegedRoleAssignment: Meine</span><span class="sxs-lookup"><span data-stu-id="ec740-103">privilegedRoleAssignment: my</span></span>

> <span data-ttu-id="ec740-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ec740-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec740-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ec740-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec740-106">Rufen Sie das jeweilige privilegierten rollenzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="ec740-106">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec740-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ec740-107">Permissions</span></span>
<span data-ttu-id="ec740-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec740-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec740-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ec740-110">Permission type</span></span>      | <span data-ttu-id="ec740-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ec740-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec740-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ec740-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ec740-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ec740-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ec740-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ec740-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec740-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec740-115">Not supported.</span></span>    |
|<span data-ttu-id="ec740-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ec740-116">Application</span></span> | <span data-ttu-id="ec740-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec740-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec740-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec740-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="ec740-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ec740-119">Request headers</span></span>
| <span data-ttu-id="ec740-120">Name</span><span class="sxs-lookup"><span data-stu-id="ec740-120">Name</span></span>       | <span data-ttu-id="ec740-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec740-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ec740-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec740-122">Authorization</span></span>  | <span data-ttu-id="ec740-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ec740-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec740-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ec740-125">Request body</span></span>
<span data-ttu-id="ec740-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ec740-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec740-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec740-127">Response</span></span>

<span data-ttu-id="ec740-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwort Code und [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) -Auflistungsobjekt in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ec740-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec740-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ec740-129">Example</span></span>
<span data-ttu-id="ec740-130">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="ec740-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ec740-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec740-131">Request</span></span>
<span data-ttu-id="ec740-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ec740-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```

##### <a name="response"></a><span data-ttu-id="ec740-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec740-133">Response</span></span>
<span data-ttu-id="ec740-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec740-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
