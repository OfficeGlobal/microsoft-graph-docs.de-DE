---
title: Mitgliedergruppen prüfen
description: Überprüfen Sie die Mitgliedschaft in einer angegebenen Liste von Gruppen und gibt aus dieser Liste dieser Gruppen
ms.openlocfilehash: b7baccd19b9d5a84ecbca4d75bca053eb51bc3f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058028"
---
# <a name="check-member-groups"></a><span data-ttu-id="b85aa-103">Mitgliedergruppen prüfen</span><span class="sxs-lookup"><span data-stu-id="b85aa-103">Check member groups</span></span>

> <span data-ttu-id="b85aa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b85aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b85aa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b85aa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b85aa-106">Überprüfen Sie für die Mitgliedschaft in einer angegebenen Liste von Gruppen und gibt aus der Liste diese Gruppen, die dem angegebenen Benutzer, Gruppe, Dienstprinzipal oder Verzeichnisobjekt Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="b85aa-106">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, service principal or directory object is a member.</span></span> <span data-ttu-id="b85aa-107">Diese Funktion ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="b85aa-107">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b85aa-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b85aa-108">Permissions</span></span>
<span data-ttu-id="b85aa-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b85aa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b85aa-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b85aa-111">Permission type</span></span>      | <span data-ttu-id="b85aa-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b85aa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b85aa-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b85aa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b85aa-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b85aa-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="b85aa-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b85aa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b85aa-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b85aa-116">Not supported.</span></span>    |
|<span data-ttu-id="b85aa-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b85aa-117">Application</span></span> | <span data-ttu-id="b85aa-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b85aa-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b85aa-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b85aa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servciePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="b85aa-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b85aa-120">Request headers</span></span>
| <span data-ttu-id="b85aa-121">Name</span><span class="sxs-lookup"><span data-stu-id="b85aa-121">Name</span></span>       | <span data-ttu-id="b85aa-122">Typ</span><span class="sxs-lookup"><span data-stu-id="b85aa-122">Type</span></span> | <span data-ttu-id="b85aa-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b85aa-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b85aa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b85aa-124">Authorization</span></span>  | <span data-ttu-id="b85aa-125">string</span><span class="sxs-lookup"><span data-stu-id="b85aa-125">string</span></span>  | <span data-ttu-id="b85aa-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b85aa-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b85aa-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b85aa-128">Content-Type</span></span>  | <span data-ttu-id="b85aa-129">application/json</span><span class="sxs-lookup"><span data-stu-id="b85aa-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b85aa-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b85aa-130">Request body</span></span>
<span data-ttu-id="b85aa-131">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="b85aa-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b85aa-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="b85aa-132">Parameter</span></span>    | <span data-ttu-id="b85aa-133">Typ</span><span class="sxs-lookup"><span data-stu-id="b85aa-133">Type</span></span>   |<span data-ttu-id="b85aa-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b85aa-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b85aa-135">groupIds</span><span class="sxs-lookup"><span data-stu-id="b85aa-135">groupIds</span></span>|<span data-ttu-id="b85aa-136">String</span><span class="sxs-lookup"><span data-stu-id="b85aa-136">String</span></span>|<span data-ttu-id="b85aa-p105">Eine Sammlung mit den Objekt-IDs der Gruppen, in denen die Mitgliedschaft überprüft werden soll. Bis zu 20 Gruppen können angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="b85aa-p105">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="b85aa-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="b85aa-139">Response</span></span>

<span data-ttu-id="b85aa-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b85aa-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b85aa-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b85aa-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b85aa-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b85aa-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="b85aa-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="b85aa-143">Response</span></span>
<span data-ttu-id="b85aa-p106">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b85aa-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
