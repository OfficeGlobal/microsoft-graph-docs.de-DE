---
title: Gruppenbesitzer hinzufügen
description: Fügt einen Benutzer zu den Besitzern der Gruppe hinzu. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: c7153a00b9a06055ff26186183ac8b987c6901bf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936214"
---
# <a name="add-group-owner"></a><span data-ttu-id="b29f4-104">Gruppenbesitzer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="b29f4-104">Add group owner</span></span>

> <span data-ttu-id="b29f4-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b29f4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b29f4-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b29f4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b29f4-p103">Fügt einen Benutzer zu den Besitzern der Gruppe hinzu. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können.</span><span class="sxs-lookup"><span data-stu-id="b29f4-p103">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="b29f4-109">**Wichtig:** Wenn Sie die Gruppenbesitzer aktualisieren und Sie ein Team für die Gruppe erstellt, kann es bis zu 2 Stunden für den Besitzer für die Synchronisierung mit Microsoft-Teams, dauern.</span><span class="sxs-lookup"><span data-stu-id="b29f4-109">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="b29f4-110">Darüber hinaus muss den Besitzer eines Teams ändern – beispielsweise durch Erstellen eines Plans Planner - können der Besitzer auch als eine Gruppe/Teammitglieder hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b29f4-110">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b29f4-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b29f4-111">Permissions</span></span>
<span data-ttu-id="b29f4-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b29f4-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b29f4-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b29f4-114">Permission type</span></span>      | <span data-ttu-id="b29f4-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b29f4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b29f4-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b29f4-116">Delegated (work or school account)</span></span> | <span data-ttu-id="b29f4-117">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b29f4-117">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b29f4-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b29f4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b29f4-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b29f4-119">Not supported.</span></span>    |
|<span data-ttu-id="b29f4-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b29f4-120">Application</span></span> | <span data-ttu-id="b29f4-121">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b29f4-121">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b29f4-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b29f4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b29f4-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b29f4-123">Request headers</span></span>
| <span data-ttu-id="b29f4-124">Name</span><span class="sxs-lookup"><span data-stu-id="b29f4-124">Name</span></span>       | <span data-ttu-id="b29f4-125">Typ</span><span class="sxs-lookup"><span data-stu-id="b29f4-125">Type</span></span> | <span data-ttu-id="b29f4-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b29f4-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b29f4-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b29f4-127">Authorization</span></span>  | <span data-ttu-id="b29f4-128">string</span><span class="sxs-lookup"><span data-stu-id="b29f4-128">string</span></span>  | <span data-ttu-id="b29f4-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b29f4-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b29f4-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b29f4-131">Request body</span></span>
<span data-ttu-id="b29f4-132">Geben Sie im Anforderungstext eine JSON-Darstellung eines [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b29f4-132">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="b29f4-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b29f4-133">Response</span></span>
<span data-ttu-id="b29f4-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b29f4-p107">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b29f4-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b29f4-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b29f4-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b29f4-137">Request</span></span>
<span data-ttu-id="b29f4-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b29f4-138">The following is an example of the request.</span></span>
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
<span data-ttu-id="b29f4-139">Geben Sie im Anforderungstext eine JSON-Darstellung eines [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b29f4-139">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="b29f4-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="b29f4-140">Response</span></span>
<span data-ttu-id="b29f4-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b29f4-141">The following is an example of the response.</span></span>
><span data-ttu-id="b29f4-142">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="b29f4-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b29f4-143">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b29f4-143">All the properties will be returned from an actual call.</span></span>
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
