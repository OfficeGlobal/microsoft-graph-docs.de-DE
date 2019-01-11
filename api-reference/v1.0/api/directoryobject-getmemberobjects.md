---
title: Mitgliedsobjekte abrufen
description: " Gibt alle Gruppen und Verzeichnisrollen zurück, in denen ein Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Diese Funktion ist transitiv. "
localization_priority: Normal
ms.openlocfilehash: b7c4c09991d31141e12fb6cd900309f81e22f8e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815911"
---
# <a name="get-member-objects"></a><span data-ttu-id="02743-104">Mitgliedsobjekte abrufen</span><span class="sxs-lookup"><span data-stu-id="02743-104">Get member objects</span></span>

 <span data-ttu-id="02743-p102">Gibt alle Gruppen und Verzeichnisrollen zurück, in denen ein Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Diese Funktion ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="02743-p102">Returns all the groups and directory roles that a user, group, or directory object is a member of. This function is transitive.</span></span> 
 > <span data-ttu-id="02743-107">Hinweis: Nur Benutzer können Verzeichnisrollen angehören.</span><span class="sxs-lookup"><span data-stu-id="02743-107">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="02743-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="02743-108">Permissions</span></span>
<span data-ttu-id="02743-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02743-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02743-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="02743-111">Permission type</span></span>      | <span data-ttu-id="02743-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="02743-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02743-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="02743-113">Delegated (work or school account)</span></span> | <span data-ttu-id="02743-114">User.Read.All und Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="02743-114">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="02743-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="02743-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02743-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02743-116">Not supported.</span></span>    |
|<span data-ttu-id="02743-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="02743-117">Application</span></span> | <span data-ttu-id="02743-118">User.Read.All und Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="02743-118">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02743-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="02743-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="02743-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="02743-120">Request headers</span></span>
| <span data-ttu-id="02743-121">Name</span><span class="sxs-lookup"><span data-stu-id="02743-121">Name</span></span>       | <span data-ttu-id="02743-122">Typ</span><span class="sxs-lookup"><span data-stu-id="02743-122">Type</span></span> | <span data-ttu-id="02743-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02743-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="02743-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="02743-124">Authorization</span></span>  | <span data-ttu-id="02743-125">string</span><span class="sxs-lookup"><span data-stu-id="02743-125">string</span></span>  | <span data-ttu-id="02743-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="02743-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="02743-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02743-128">Content-Type</span></span>   | <span data-ttu-id="02743-129">string</span><span class="sxs-lookup"><span data-stu-id="02743-129">string</span></span>  | <span data-ttu-id="02743-130">application/json</span><span class="sxs-lookup"><span data-stu-id="02743-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="02743-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="02743-131">Request body</span></span>
<span data-ttu-id="02743-132">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="02743-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="02743-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="02743-133">Parameter</span></span>    | <span data-ttu-id="02743-134">Typ</span><span class="sxs-lookup"><span data-stu-id="02743-134">Type</span></span>   |<span data-ttu-id="02743-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02743-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02743-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="02743-136">securityEnabledOnly</span></span>|<span data-ttu-id="02743-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="02743-137">Boolean</span></span>| <span data-ttu-id="02743-p105">**true** gibt an, dass nur Sicherheitsgruppen, in denen die Person Mitglied ist, zurückgegeben werden sollen; **falsch** gibt an, dass alle Gruppen und Verzeichnisrollen, in denen die Person ein Mitglied ist, zurückgegeben werden sollen. **Hinweis**: Die Funktion kann nur für einen Benutzer aufgerufen werden, wenn der Parameter **true** lautet.</span><span class="sxs-lookup"><span data-stu-id="02743-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="02743-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="02743-140">Response</span></span>

<span data-ttu-id="02743-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02743-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02743-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="02743-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="02743-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="02743-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="02743-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="02743-144">Response</span></span>
<span data-ttu-id="02743-p106">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02743-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
