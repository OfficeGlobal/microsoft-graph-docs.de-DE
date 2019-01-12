---
title: 'user: getMemberObjects'
description: Gibt alle Gruppen, Verzeichnisrollen und administrativen Einheiten zurück, bei denen der Benutzer ein Mitglied ist. Die Überprüfung ist transitiv.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f4a2b01096b271b26f89c83f22a65246d02023c2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957816"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="0c10a-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="0c10a-104">user: getMemberObjects</span></span>

> <span data-ttu-id="0c10a-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0c10a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c10a-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0c10a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c10a-p103">Gibt alle Gruppen, Verzeichnisrollen und administrativen Einheiten zurück, bei denen der Benutzer ein Mitglied ist. Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="0c10a-p103">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c10a-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0c10a-109">Permissions</span></span>
<span data-ttu-id="0c10a-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c10a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0c10a-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0c10a-112">Permission type</span></span>      | <span data-ttu-id="0c10a-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0c10a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c10a-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0c10a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0c10a-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0c10a-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0c10a-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0c10a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c10a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c10a-117">Not supported.</span></span>    |
|<span data-ttu-id="0c10a-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0c10a-118">Application</span></span> | <span data-ttu-id="0c10a-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c10a-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c10a-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c10a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="0c10a-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0c10a-121">Request headers</span></span>
| <span data-ttu-id="0c10a-122">Header</span><span class="sxs-lookup"><span data-stu-id="0c10a-122">Header</span></span>       | <span data-ttu-id="0c10a-123">Wert</span><span class="sxs-lookup"><span data-stu-id="0c10a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0c10a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c10a-124">Authorization</span></span>  | <span data-ttu-id="0c10a-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0c10a-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0c10a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0c10a-127">Content-Type</span></span>  | <span data-ttu-id="0c10a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0c10a-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0c10a-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0c10a-129">Request body</span></span>
<span data-ttu-id="0c10a-130">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="0c10a-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0c10a-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="0c10a-131">Parameter</span></span>    | <span data-ttu-id="0c10a-132">Typ</span><span class="sxs-lookup"><span data-stu-id="0c10a-132">Type</span></span>   |<span data-ttu-id="0c10a-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c10a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c10a-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="0c10a-134">securityEnabledOnly</span></span>|<span data-ttu-id="0c10a-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0c10a-135">Boolean</span></span>|<span data-ttu-id="0c10a-p106">**true** gibt an, dass nur Sicherheitsgruppen, in denen der Benutzer Mitglied ist, zurückgegeben werden sollen; **false** gibt an, dass alle Gruppen, von denen der Benutzer ein Mitglied ist, zurückgegeben werden sollen. Hinweis: Dieser Parameter darf nur auf **true** gesetzt werden, wenn diese Methode auf einen Benutzer angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="0c10a-p106">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="0c10a-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c10a-138">Response</span></span>

<span data-ttu-id="0c10a-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Zeichenfolgensammlung im Antworttext zurückgegeben, der die IDs der Gruppen und Verzeichnisrollen enthält, von denen der Benutzer ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="0c10a-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="0c10a-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0c10a-140">Example</span></span>
<span data-ttu-id="0c10a-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="0c10a-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0c10a-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c10a-142">Request</span></span>
<span data-ttu-id="0c10a-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0c10a-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="0c10a-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c10a-144">Response</span></span>
<span data-ttu-id="0c10a-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0c10a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
