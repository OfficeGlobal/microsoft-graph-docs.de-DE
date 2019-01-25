---
title: Gruppenbesitzer hinzufügen
description: Fügt einen Benutzer zu den Besitzern der Gruppe hinzu. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 049c860be95e2f4f4b83848d8d8be6b3dd0ed9c5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517169"
---
# <a name="add-group-owner"></a><span data-ttu-id="c902f-104">Gruppenbesitzer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="c902f-104">Add group owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c902f-p102">Fügt einen Benutzer zu den Besitzern der Gruppe hinzu. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können.</span><span class="sxs-lookup"><span data-stu-id="c902f-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="c902f-107">**Wichtig:** Wenn Sie die Gruppenbesitzer aktualisieren und Sie ein Team für die Gruppe erstellt, kann es bis zu 2 Stunden für den Besitzer für die Synchronisierung mit Microsoft-Teams, dauern.</span><span class="sxs-lookup"><span data-stu-id="c902f-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="c902f-108">Darüber hinaus muss den Besitzer eines Teams ändern – beispielsweise durch Erstellen eines Plans Planner - können der Besitzer auch als eine Gruppe/Teammitglieder hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c902f-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c902f-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c902f-109">Permissions</span></span>
<span data-ttu-id="c902f-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c902f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c902f-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c902f-112">Permission type</span></span>      | <span data-ttu-id="c902f-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c902f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c902f-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c902f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c902f-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c902f-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c902f-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c902f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c902f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c902f-117">Not supported.</span></span>    |
|<span data-ttu-id="c902f-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c902f-118">Application</span></span> | <span data-ttu-id="c902f-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c902f-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c902f-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c902f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="c902f-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c902f-121">Request headers</span></span>
| <span data-ttu-id="c902f-122">Name</span><span class="sxs-lookup"><span data-stu-id="c902f-122">Name</span></span>       | <span data-ttu-id="c902f-123">Typ</span><span class="sxs-lookup"><span data-stu-id="c902f-123">Type</span></span> | <span data-ttu-id="c902f-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c902f-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c902f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c902f-125">Authorization</span></span>  | <span data-ttu-id="c902f-126">string</span><span class="sxs-lookup"><span data-stu-id="c902f-126">string</span></span>  | <span data-ttu-id="c902f-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c902f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c902f-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c902f-129">Request body</span></span>
<span data-ttu-id="c902f-130">Geben Sie im Anforderungstext eine JSON-Darstellung eines [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c902f-130">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="c902f-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c902f-131">Response</span></span>
<span data-ttu-id="c902f-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c902f-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c902f-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c902f-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c902f-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c902f-135">Request</span></span>
<span data-ttu-id="c902f-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c902f-136">The following is an example of the request.</span></span>
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
<span data-ttu-id="c902f-137">Geben Sie im Anforderungstext eine JSON-Darstellung eines [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c902f-137">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="c902f-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="c902f-138">Response</span></span>
<span data-ttu-id="c902f-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c902f-139">The following is an example of the response.</span></span>
><span data-ttu-id="c902f-140">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="c902f-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c902f-141">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="c902f-141">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-owners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
