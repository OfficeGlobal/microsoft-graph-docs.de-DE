---
title: Mitgliedsobjekte abrufen
description: " Gibt alle Gruppen, administrative Einheiten und Directory Rollen, denen ein Benutzer, Gruppe, Dienstprinzipale oder Directory-Objekt ein Mitglied ist. Diese Funktion ist transitiv. "
localization_priority: Normal
ms.openlocfilehash: f63c077414f656df168db5c5af498cec0f79e703
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874802"
---
# <a name="get-member-objects"></a><span data-ttu-id="bdbb3-104">Mitgliedsobjekte abrufen</span><span class="sxs-lookup"><span data-stu-id="bdbb3-104">Get member objects</span></span>

> <span data-ttu-id="bdbb3-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bdbb3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdbb3-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bdbb3-106">Use of these APIs in production applications is not supported.</span></span>

 <span data-ttu-id="bdbb3-107">Gibt alle Gruppen, administrative Einheiten und Directory Rollen, denen ein Benutzer, Gruppe, Dienstprinzipale oder Directory-Objekt ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="bdbb3-107">Returns all the groups, administrative units and directory roles that a user, group, service principals or directory object is a member of.</span></span> <span data-ttu-id="bdbb3-108">Diese Funktion ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="bdbb3-108">This function is transitive.</span></span> 
 > <span data-ttu-id="bdbb3-109">Hinweis: Nur Benutzer können Verzeichnisrollen angehören.</span><span class="sxs-lookup"><span data-stu-id="bdbb3-109">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdbb3-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bdbb3-110">Permissions</span></span>
<span data-ttu-id="bdbb3-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdbb3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bdbb3-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bdbb3-113">Permission type</span></span>      | <span data-ttu-id="bdbb3-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bdbb3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdbb3-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bdbb3-115">Delegated (work or school account)</span></span> | <span data-ttu-id="bdbb3-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdbb3-116">Directory.Read.All</span></span>    |
|<span data-ttu-id="bdbb3-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bdbb3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdbb3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bdbb3-118">Not supported.</span></span>    |
|<span data-ttu-id="bdbb3-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bdbb3-119">Application</span></span> | <span data-ttu-id="bdbb3-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdbb3-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdbb3-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bdbb3-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberObjects
POST /servicePrincipals/{id}/getMemberObjects
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="bdbb3-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bdbb3-122">Request headers</span></span>
| <span data-ttu-id="bdbb3-123">Name</span><span class="sxs-lookup"><span data-stu-id="bdbb3-123">Name</span></span>       | <span data-ttu-id="bdbb3-124">Typ</span><span class="sxs-lookup"><span data-stu-id="bdbb3-124">Type</span></span> | <span data-ttu-id="bdbb3-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bdbb3-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bdbb3-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdbb3-126">Authorization</span></span>  | <span data-ttu-id="bdbb3-127">string</span><span class="sxs-lookup"><span data-stu-id="bdbb3-127">string</span></span>  | <span data-ttu-id="bdbb3-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bdbb3-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bdbb3-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bdbb3-130">Content-Type</span></span>  | <span data-ttu-id="bdbb3-131">application/json</span><span class="sxs-lookup"><span data-stu-id="bdbb3-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bdbb3-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bdbb3-132">Request body</span></span>
<span data-ttu-id="bdbb3-133">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="bdbb3-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bdbb3-134">Parameter</span><span class="sxs-lookup"><span data-stu-id="bdbb3-134">Parameter</span></span>    | <span data-ttu-id="bdbb3-135">Typ</span><span class="sxs-lookup"><span data-stu-id="bdbb3-135">Type</span></span>   |<span data-ttu-id="bdbb3-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bdbb3-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdbb3-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="bdbb3-137">securityEnabledOnly</span></span>|<span data-ttu-id="bdbb3-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdbb3-138">Boolean</span></span>| <span data-ttu-id="bdbb3-p106">**true** gibt an, dass nur Sicherheitsgruppen, in denen die Person Mitglied ist, zurückgegeben werden sollen; **falsch** gibt an, dass alle Gruppen und Verzeichnisrollen, in denen die Person ein Mitglied ist, zurückgegeben werden sollen. **Hinweis**: Die Funktion kann nur für einen Benutzer aufgerufen werden, wenn der Parameter **true** lautet.</span><span class="sxs-lookup"><span data-stu-id="bdbb3-p106">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="bdbb3-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="bdbb3-141">Response</span></span>

<span data-ttu-id="bdbb3-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bdbb3-142">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdbb3-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bdbb3-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bdbb3-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bdbb3-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="bdbb3-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="bdbb3-145">Response</span></span>
<span data-ttu-id="bdbb3-p107">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bdbb3-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
