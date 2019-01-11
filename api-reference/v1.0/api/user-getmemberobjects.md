---
title: 'user: getMemberObjects'
description: Gibt alle Gruppen, Verzeichnisrollen und administrativen Einheiten zurück, bei denen der Benutzer ein Mitglied ist. Die Überprüfung ist transitiv.
localization_priority: Priority
ms.openlocfilehash: 2d2c28ab41e7f9798ff1f77e1750e6303a52de34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811382"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="fe30c-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="fe30c-104">user: getMemberObjects</span></span>
<span data-ttu-id="fe30c-p102">Gibt alle Gruppen, Verzeichnisrollen und administrativen Einheiten zurück, bei denen der Benutzer ein Mitglied ist. Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="fe30c-p102">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe30c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fe30c-107">Permissions</span></span>
<span data-ttu-id="fe30c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe30c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fe30c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fe30c-110">Permission type</span></span>      | <span data-ttu-id="fe30c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fe30c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe30c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fe30c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fe30c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fe30c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fe30c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fe30c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe30c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe30c-115">Not supported.</span></span>    |
|<span data-ttu-id="fe30c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fe30c-116">Application</span></span> | <span data-ttu-id="fe30c-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe30c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe30c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe30c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="fe30c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fe30c-119">Request headers</span></span>
| <span data-ttu-id="fe30c-120">Header</span><span class="sxs-lookup"><span data-stu-id="fe30c-120">Header</span></span>       | <span data-ttu-id="fe30c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="fe30c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fe30c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe30c-122">Authorization</span></span>  | <span data-ttu-id="fe30c-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fe30c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fe30c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe30c-125">Content-Type</span></span>  | <span data-ttu-id="fe30c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe30c-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fe30c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fe30c-127">Request body</span></span>
<span data-ttu-id="fe30c-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="fe30c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fe30c-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="fe30c-129">Parameter</span></span>    | <span data-ttu-id="fe30c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fe30c-130">Type</span></span>   |<span data-ttu-id="fe30c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe30c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe30c-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="fe30c-132">securityEnabledOnly</span></span>|<span data-ttu-id="fe30c-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe30c-133">Boolean</span></span>|<span data-ttu-id="fe30c-p105">**true** gibt an, dass nur Sicherheitsgruppen, in denender Benutzer Mitglied ist, zurückgegeben werden sollen; **false** gibt an, dass alle Gruppen und Verzeichnisrollen, in denen der Benutzer ein Mitglied ist, zurückgegeben werden sollen. Hinweis: Dieser Parameter darf nur auf **true** gesetzt werden, wenn diese Methode auf einen Benutzer angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="fe30c-p105">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups and directory roles that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="fe30c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe30c-136">Response</span></span>

<span data-ttu-id="fe30c-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Zeichenfolgensammlung im Antworttext zurückgegeben, der die IDs der Gruppen und Verzeichnisrollen enthält, von denen der Benutzer ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="fe30c-137">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="fe30c-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fe30c-138">Example</span></span>
<span data-ttu-id="fe30c-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="fe30c-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fe30c-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe30c-140">Request</span></span>
<span data-ttu-id="fe30c-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fe30c-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="fe30c-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe30c-142">Response</span></span>
<span data-ttu-id="fe30c-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe30c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
