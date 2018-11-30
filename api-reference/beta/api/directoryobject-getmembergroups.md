---
title: Mitgliedergruppen abrufen
description: Zurückgeben aller Gruppen, dass die angegebenen Benutzer, Gruppe, Dienstprinzipal oder Directory-Objekt ein Mitglied ist der. Diese Funktion ist transitiv.
ms.openlocfilehash: 9dc6af54ba364e1c5c82dc7e14a5d2571e29ef12
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062709"
---
# <a name="get-member-groups"></a><span data-ttu-id="4bd5f-104">Mitgliedergruppen abrufen</span><span class="sxs-lookup"><span data-stu-id="4bd5f-104">Get member groups</span></span>

> <span data-ttu-id="4bd5f-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4bd5f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bd5f-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4bd5f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4bd5f-107">Zurückgeben aller Gruppen, dass die angegebenen Benutzer, Gruppe, Dienstprinzipal oder Directory-Objekt ein Mitglied ist der.</span><span class="sxs-lookup"><span data-stu-id="4bd5f-107">Return all the groups that the specified user, group, service principal or directory object is a member of.</span></span> <span data-ttu-id="4bd5f-108">Diese Funktion ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="4bd5f-108">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bd5f-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4bd5f-109">Permissions</span></span>
<span data-ttu-id="4bd5f-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bd5f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4bd5f-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4bd5f-112">Permission type</span></span>      | <span data-ttu-id="4bd5f-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4bd5f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bd5f-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4bd5f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4bd5f-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bd5f-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="4bd5f-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4bd5f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bd5f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4bd5f-117">Not supported.</span></span>    |
|<span data-ttu-id="4bd5f-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4bd5f-118">Application</span></span> | <span data-ttu-id="4bd5f-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bd5f-119">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bd5f-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4bd5f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /servicePrincipals/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="4bd5f-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4bd5f-121">Request headers</span></span>
| <span data-ttu-id="4bd5f-122">Name</span><span class="sxs-lookup"><span data-stu-id="4bd5f-122">Name</span></span>       | <span data-ttu-id="4bd5f-123">Typ</span><span class="sxs-lookup"><span data-stu-id="4bd5f-123">Type</span></span> | <span data-ttu-id="4bd5f-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4bd5f-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4bd5f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bd5f-125">Authorization</span></span>  | <span data-ttu-id="4bd5f-126">string</span><span class="sxs-lookup"><span data-stu-id="4bd5f-126">string</span></span>  | <span data-ttu-id="4bd5f-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4bd5f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4bd5f-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4bd5f-129">Content-Type</span></span>  | <span data-ttu-id="4bd5f-130">application/json</span><span class="sxs-lookup"><span data-stu-id="4bd5f-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4bd5f-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4bd5f-131">Request body</span></span>
<span data-ttu-id="4bd5f-132">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="4bd5f-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4bd5f-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="4bd5f-133">Parameter</span></span>    | <span data-ttu-id="4bd5f-134">Typ</span><span class="sxs-lookup"><span data-stu-id="4bd5f-134">Type</span></span>   |<span data-ttu-id="4bd5f-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4bd5f-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bd5f-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="4bd5f-136">securityEnabledOnly</span></span>|<span data-ttu-id="4bd5f-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bd5f-137">Boolean</span></span>| <span data-ttu-id="4bd5f-p106">**true** gibt an, dass nur Sicherheitsgruppen, in denen die Person Mitglied ist, zurückgegeben werden sollen; **falsch** gibt an, dass alle Gruppen und Verzeichnisrollen, in denen die Person ein Mitglied ist, zurückgegeben werden sollen. **Hinweis**: Die Funktion kann nur für einen Benutzer aufgerufen werden, wenn der Parameter **true** lautet.</span><span class="sxs-lookup"><span data-stu-id="4bd5f-p106">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="4bd5f-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="4bd5f-140">Response</span></span>

<span data-ttu-id="4bd5f-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4bd5f-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bd5f-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4bd5f-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4bd5f-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4bd5f-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="4bd5f-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="4bd5f-144">Response</span></span>
<span data-ttu-id="4bd5f-p107">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4bd5f-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
