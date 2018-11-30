---
title: Gruppenbesitzer hinzufügen
description: Fügt einen Benutzer zu den Besitzern der Gruppe hinzu. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können.
ms.openlocfilehash: e65db3a57f6a50afb95b432a53b1821065e5867a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058947"
---
# <a name="add-group-owner"></a><span data-ttu-id="228c4-104">Gruppenbesitzer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="228c4-104">Add group owner</span></span>

> <span data-ttu-id="228c4-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="228c4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="228c4-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="228c4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="228c4-p103">Fügt einen Benutzer zu den Besitzern der Gruppe hinzu. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können.</span><span class="sxs-lookup"><span data-stu-id="228c4-p103">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="228c4-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="228c4-109">Permissions</span></span>
<span data-ttu-id="228c4-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="228c4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="228c4-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="228c4-112">Permission type</span></span>      | <span data-ttu-id="228c4-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="228c4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="228c4-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="228c4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="228c4-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="228c4-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="228c4-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="228c4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="228c4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="228c4-117">Not supported.</span></span>    |
|<span data-ttu-id="228c4-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="228c4-118">Application</span></span> | <span data-ttu-id="228c4-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="228c4-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="228c4-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="228c4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="228c4-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="228c4-121">Request headers</span></span>
| <span data-ttu-id="228c4-122">Name</span><span class="sxs-lookup"><span data-stu-id="228c4-122">Name</span></span>       | <span data-ttu-id="228c4-123">Typ</span><span class="sxs-lookup"><span data-stu-id="228c4-123">Type</span></span> | <span data-ttu-id="228c4-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="228c4-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="228c4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="228c4-125">Authorization</span></span>  | <span data-ttu-id="228c4-126">string</span><span class="sxs-lookup"><span data-stu-id="228c4-126">string</span></span>  | <span data-ttu-id="228c4-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="228c4-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="228c4-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="228c4-129">Request body</span></span>
<span data-ttu-id="228c4-130">Geben Sie im Anforderungstext eine JSON-Darstellung eines [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="228c4-130">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="228c4-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="228c4-131">Response</span></span>
<span data-ttu-id="228c4-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="228c4-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="228c4-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="228c4-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="228c4-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="228c4-135">Request</span></span>
<span data-ttu-id="228c4-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="228c4-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```
<span data-ttu-id="228c4-137">Geben Sie im Anforderungstext eine JSON-Darstellung eines [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="228c4-137">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="228c4-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="228c4-138">Response</span></span>
<span data-ttu-id="228c4-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="228c4-139">The following is an example of the response.</span></span>
><span data-ttu-id="228c4-140">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="228c4-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="228c4-141">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="228c4-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
