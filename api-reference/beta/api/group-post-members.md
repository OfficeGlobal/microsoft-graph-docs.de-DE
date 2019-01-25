---
title: Mitglied hinzufügen
description: Verwenden Sie diese API, um ein Mitglied einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die **member**-Navigationseigenschaft hinzuzufügen.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: ac21262858137074ed92978f0ab6530052fcc2de
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515678"
---
# <a name="add-member"></a><span data-ttu-id="b6798-103">Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="b6798-103">Add member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6798-104">Verwenden Sie diese API, um ein Mitglied einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die **member**-Navigationseigenschaft hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="b6798-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="b6798-105">Sie können Benutzer oder andere Gruppen hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="b6798-105">You can add users or other groups.</span></span> <span data-ttu-id="b6798-106">Wichtig: Sie können nur Benutzer zu Office 365-Gruppen hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="b6798-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6798-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b6798-107">Permissions</span></span>
<span data-ttu-id="b6798-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6798-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6798-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b6798-110">Permission type</span></span>      | <span data-ttu-id="b6798-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b6798-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6798-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b6798-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b6798-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b6798-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b6798-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b6798-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6798-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6798-115">Not supported.</span></span>    |
|<span data-ttu-id="b6798-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b6798-116">Application</span></span> | <span data-ttu-id="b6798-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6798-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6798-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6798-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b6798-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b6798-119">Request headers</span></span>
| <span data-ttu-id="b6798-120">Name</span><span class="sxs-lookup"><span data-stu-id="b6798-120">Name</span></span>       | <span data-ttu-id="b6798-121">Typ</span><span class="sxs-lookup"><span data-stu-id="b6798-121">Type</span></span> | <span data-ttu-id="b6798-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6798-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b6798-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6798-123">Authorization</span></span>  | <span data-ttu-id="b6798-124">string</span><span class="sxs-lookup"><span data-stu-id="b6798-124">string</span></span>  | <span data-ttu-id="b6798-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b6798-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6798-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b6798-127">Request body</span></span>
<span data-ttu-id="b6798-128">Geben Sie im Anforderungstext eine JSON-Darstellung eines [directoryObject](../resources/directoryobject.md)- oder [user](../resources/user.md)- oder [group](../resources/group.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b6798-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="b6798-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6798-129">Response</span></span>
<span data-ttu-id="b6798-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b6798-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6798-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b6798-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b6798-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6798-133">Request</span></span>
<span data-ttu-id="b6798-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b6798-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
<span data-ttu-id="b6798-135">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der die `id` des Objekts [DirectoryObject](../resources/directoryobject.md), [Benutzer](../resources/user.md)oder [Gruppe](../resources/group.md) hinzufügen möchten.</span><span class="sxs-lookup"><span data-stu-id="b6798-135">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="b6798-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6798-136">Response</span></span>
<span data-ttu-id="b6798-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b6798-137">The following is an example of the response.</span></span>
><span data-ttu-id="b6798-138">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="b6798-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b6798-139">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b6798-139">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
