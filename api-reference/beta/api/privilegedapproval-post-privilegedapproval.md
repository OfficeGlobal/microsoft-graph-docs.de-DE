---
title: Erstellen von privilegedApproval
description: Verwenden Sie diese API, um eine neue PrivilegedApproval erstellen.
ms.openlocfilehash: 549f4e37ae60cf81d73163c1badd35247113119b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064607"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="48424-103">Erstellen von privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="48424-103">Create privilegedApproval</span></span>

> <span data-ttu-id="48424-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="48424-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48424-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="48424-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48424-106">Verwenden Sie diese API, um eine neue PrivilegedApproval erstellen.</span><span class="sxs-lookup"><span data-stu-id="48424-106">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="48424-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="48424-107">Permissions</span></span>
<span data-ttu-id="48424-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48424-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="48424-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48424-110">Permission type</span></span>      | <span data-ttu-id="48424-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48424-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48424-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48424-112">Delegated (work or school account)</span></span> | <span data-ttu-id="48424-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48424-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="48424-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48424-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48424-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48424-115">Not supported.</span></span>    |
|<span data-ttu-id="48424-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48424-116">Application</span></span> | <span data-ttu-id="48424-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48424-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48424-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48424-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="48424-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48424-119">Request headers</span></span>
| <span data-ttu-id="48424-120">Name</span><span class="sxs-lookup"><span data-stu-id="48424-120">Name</span></span>       | <span data-ttu-id="48424-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48424-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="48424-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="48424-122">Authorization</span></span>  | <span data-ttu-id="48424-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="48424-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48424-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48424-125">Request body</span></span>
<span data-ttu-id="48424-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [PrivilegedApproval](../resources/privilegedapproval.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="48424-126">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="48424-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="48424-127">Response</span></span>

<span data-ttu-id="48424-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [PrivilegedApproval](../resources/privilegedapproval.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="48424-128">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="48424-129">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="48424-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="48424-130">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="48424-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="48424-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48424-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48424-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48424-132">Request</span></span>
<span data-ttu-id="48424-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="48424-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_privilegedapproval_from_privilegedapproval"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedApproval
Content-type: application/json
Content-length: 180

{
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
<span data-ttu-id="48424-134">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [PrivilegedApproval](../resources/privilegedapproval.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="48424-134">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="48424-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="48424-135">Response</span></span>
<span data-ttu-id="48424-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48424-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 200

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
