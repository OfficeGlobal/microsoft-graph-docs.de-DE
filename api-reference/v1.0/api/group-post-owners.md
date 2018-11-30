---
title: Gruppenbesitzer hinzufügen
description: Fügt einen Benutzer zu den Besitzern der Gruppe hinzu. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können.
ms.openlocfilehash: 8c879430c78cb1d06150bade842addcb4ba0af38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017916"
---
# <a name="add-group-owner"></a><span data-ttu-id="39c4e-104">Gruppenbesitzer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="39c4e-104">Add group owner</span></span>
<span data-ttu-id="39c4e-p102">Fügt einen Benutzer zu den Besitzern der Gruppe hinzu. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können.</span><span class="sxs-lookup"><span data-stu-id="39c4e-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="39c4e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="39c4e-107">Permissions</span></span>
<span data-ttu-id="39c4e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39c4e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39c4e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="39c4e-110">Permission type</span></span>      | <span data-ttu-id="39c4e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="39c4e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39c4e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="39c4e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="39c4e-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="39c4e-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="39c4e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="39c4e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39c4e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39c4e-115">Not supported.</span></span>    |
|<span data-ttu-id="39c4e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="39c4e-116">Application</span></span> | <span data-ttu-id="39c4e-117">Group.ReadWrite.All und User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39c4e-117">Group.ReadWrite.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39c4e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="39c4e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="39c4e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="39c4e-119">Request headers</span></span>
| <span data-ttu-id="39c4e-120">Name</span><span class="sxs-lookup"><span data-stu-id="39c4e-120">Name</span></span>       | <span data-ttu-id="39c4e-121">Typ</span><span class="sxs-lookup"><span data-stu-id="39c4e-121">Type</span></span> | <span data-ttu-id="39c4e-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39c4e-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="39c4e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="39c4e-123">Authorization</span></span>  | <span data-ttu-id="39c4e-124">string</span><span class="sxs-lookup"><span data-stu-id="39c4e-124">string</span></span>  | <span data-ttu-id="39c4e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="39c4e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39c4e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="39c4e-127">Request body</span></span>
<span data-ttu-id="39c4e-128">Geben Sie im Anforderungstext eine JSON-Darstellung eines [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="39c4e-128">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="39c4e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="39c4e-129">Response</span></span>
<span data-ttu-id="39c4e-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39c4e-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39c4e-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="39c4e-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="39c4e-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39c4e-133">Request</span></span>
<span data-ttu-id="39c4e-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="39c4e-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="39c4e-135">Geben Sie im Anforderungstext eine JSON-Darstellung eines [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="39c4e-135">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="39c4e-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="39c4e-136">Response</span></span>
<span data-ttu-id="39c4e-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="39c4e-137">The following is an example of the response.</span></span>
><span data-ttu-id="39c4e-138">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="39c4e-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="39c4e-139">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="39c4e-139">All the properties will be returned from an actual call.</span></span>
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
