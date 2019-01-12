---
title: Mitgliedergruppen prüfen
description: Überprüfen Sie die Mitgliedschaft in einer angegebenen Liste von Gruppen und gibt aus dieser Liste dieser Gruppen
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99ebf38b8f230233b50fa642f7503302afd02b33
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941786"
---
# <a name="check-member-groups"></a><span data-ttu-id="30b46-103">Mitgliedergruppen prüfen</span><span class="sxs-lookup"><span data-stu-id="30b46-103">Check member groups</span></span>

<span data-ttu-id="30b46-p101">Dient zum Überprüfen der Mitgliedschaft in einer angegebenen Liste von Gruppen und gibt aus dieser Liste die Gruppen zurück, in denen das angegebene Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Diese Funktion ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="30b46-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="30b46-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="30b46-106">Permissions</span></span>
<span data-ttu-id="30b46-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30b46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30b46-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="30b46-109">Permission type</span></span>      | <span data-ttu-id="30b46-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="30b46-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30b46-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="30b46-111">Delegated (work or school account)</span></span> | <span data-ttu-id="30b46-112">User.Read.All und Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="30b46-112">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="30b46-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="30b46-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30b46-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30b46-114">Not supported.</span></span>    |
|<span data-ttu-id="30b46-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="30b46-115">Application</span></span> | <span data-ttu-id="30b46-116">User.Read.All und Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="30b46-116">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="30b46-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="30b46-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="30b46-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="30b46-118">Request headers</span></span>
| <span data-ttu-id="30b46-119">Name</span><span class="sxs-lookup"><span data-stu-id="30b46-119">Name</span></span>       | <span data-ttu-id="30b46-120">Typ</span><span class="sxs-lookup"><span data-stu-id="30b46-120">Type</span></span> | <span data-ttu-id="30b46-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30b46-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="30b46-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="30b46-122">Authorization</span></span>  | <span data-ttu-id="30b46-123">string</span><span class="sxs-lookup"><span data-stu-id="30b46-123">string</span></span>  | <span data-ttu-id="30b46-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="30b46-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="30b46-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="30b46-126">Content-Type</span></span>  | <span data-ttu-id="30b46-127">string</span><span class="sxs-lookup"><span data-stu-id="30b46-127">string</span></span> | <span data-ttu-id="30b46-128">application/json</span><span class="sxs-lookup"><span data-stu-id="30b46-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="30b46-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="30b46-129">Request body</span></span>
<span data-ttu-id="30b46-130">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="30b46-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="30b46-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="30b46-131">Parameter</span></span>    | <span data-ttu-id="30b46-132">Typ</span><span class="sxs-lookup"><span data-stu-id="30b46-132">Type</span></span>   |<span data-ttu-id="30b46-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30b46-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30b46-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="30b46-134">groupIds</span></span>|<span data-ttu-id="30b46-135">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="30b46-135">String collection</span></span>|<span data-ttu-id="30b46-p104">Eine Sammlung mit den Objekt-IDs der Gruppen, in denen die Mitgliedschaft überprüft werden soll. Bis zu 20 Gruppen können angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="30b46-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="30b46-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="30b46-138">Response</span></span>

<span data-ttu-id="30b46-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="30b46-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30b46-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="30b46-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="30b46-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="30b46-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{id}/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64b130f4eb9e75525e",
        "4fe90ae065a-478b9400e0a0e1cbd540"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="30b46-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="30b46-142">Response</span></span>
<span data-ttu-id="30b46-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="30b46-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
