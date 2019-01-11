---
title: Mitgliedergruppen abrufen
description: Gibt alle Gruppen zurück, in denen das angegebene Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Diese Funktion ist transitiv.
localization_priority: Normal
ms.openlocfilehash: b3556140aa0113c403f80d95e0a258be03f27125
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814651"
---
# <a name="get-member-groups"></a><span data-ttu-id="2a4dc-104">Mitgliedergruppen abrufen</span><span class="sxs-lookup"><span data-stu-id="2a4dc-104">Get member groups</span></span>

<span data-ttu-id="2a4dc-p102">Gibt alle Gruppen zurück, in denen das angegebene Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Diese Funktion ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="2a4dc-p102">Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a4dc-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2a4dc-107">Permissions</span></span>
<span data-ttu-id="2a4dc-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a4dc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a4dc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2a4dc-110">Permission type</span></span>      | <span data-ttu-id="2a4dc-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2a4dc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a4dc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2a4dc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2a4dc-113">User.Read.All und Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a4dc-113">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="2a4dc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2a4dc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a4dc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a4dc-115">Not supported.</span></span>    |
|<span data-ttu-id="2a4dc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2a4dc-116">Application</span></span> | <span data-ttu-id="2a4dc-117">User.Read.All und Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a4dc-117">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a4dc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a4dc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="2a4dc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a4dc-119">Request headers</span></span>
| <span data-ttu-id="2a4dc-120">Name</span><span class="sxs-lookup"><span data-stu-id="2a4dc-120">Name</span></span>       | <span data-ttu-id="2a4dc-121">Typ</span><span class="sxs-lookup"><span data-stu-id="2a4dc-121">Type</span></span> | <span data-ttu-id="2a4dc-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a4dc-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2a4dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a4dc-123">Authorization</span></span>  | <span data-ttu-id="2a4dc-124">string</span><span class="sxs-lookup"><span data-stu-id="2a4dc-124">string</span></span>  | <span data-ttu-id="2a4dc-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2a4dc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2a4dc-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a4dc-127">Content-Type</span></span>   | <span data-ttu-id="2a4dc-128">string</span><span class="sxs-lookup"><span data-stu-id="2a4dc-128">string</span></span>  | <span data-ttu-id="2a4dc-129">application/json</span><span class="sxs-lookup"><span data-stu-id="2a4dc-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2a4dc-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a4dc-130">Request body</span></span>
<span data-ttu-id="2a4dc-131">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="2a4dc-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2a4dc-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="2a4dc-132">Parameter</span></span>    | <span data-ttu-id="2a4dc-133">Typ</span><span class="sxs-lookup"><span data-stu-id="2a4dc-133">Type</span></span>   |<span data-ttu-id="2a4dc-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a4dc-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a4dc-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="2a4dc-135">securityEnabledOnly</span></span>|<span data-ttu-id="2a4dc-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a4dc-136">Boolean</span></span>| <span data-ttu-id="2a4dc-p105">**true** gibt an, dass nur Sicherheitsgruppen, in denen die Person Mitglied ist, zurückgegeben werden sollen; **falsch** gibt an, dass alle Gruppen und Verzeichnisrollen, in denen die Person ein Mitglied ist, zurückgegeben werden sollen. **Hinweis**: Die Funktion kann nur für einen Benutzer aufgerufen werden, wenn der Parameter **true** lautet.</span><span class="sxs-lookup"><span data-stu-id="2a4dc-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="2a4dc-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a4dc-139">Response</span></span>

<span data-ttu-id="2a4dc-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a4dc-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a4dc-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a4dc-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2a4dc-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a4dc-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="2a4dc-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a4dc-143">Response</span></span>
<span data-ttu-id="2a4dc-p106">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a4dc-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
