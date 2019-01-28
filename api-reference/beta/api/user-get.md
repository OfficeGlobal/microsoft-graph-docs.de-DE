---
title: Benutzer abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des Benutzerobjekts.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b0a05ee2e2bd2b4f5d2e66f5c2e0efcf27efb59
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523946"
---
# <a name="get-a-user"></a><span data-ttu-id="6dc5f-103">Benutzer abrufen</span><span class="sxs-lookup"><span data-stu-id="6dc5f-103">Get a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dc5f-104">Dient zum Abrufen der Eigenschaften und der Beziehungen des Benutzerobjekts.</span><span class="sxs-lookup"><span data-stu-id="6dc5f-104">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="6dc5f-105">Da die **user**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **user**-Instanzen abrufen.</span><span class="sxs-lookup"><span data-stu-id="6dc5f-105">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dc5f-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6dc5f-106">Permissions</span></span>
<span data-ttu-id="6dc5f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dc5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dc5f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6dc5f-109">Permission type</span></span>      | <span data-ttu-id="6dc5f-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6dc5f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dc5f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6dc5f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6dc5f-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6dc5f-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6dc5f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6dc5f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dc5f-114">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6dc5f-114">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="6dc5f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6dc5f-115">Application</span></span> | <span data-ttu-id="6dc5f-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dc5f-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6dc5f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6dc5f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6dc5f-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6dc5f-118">Optional query parameters</span></span>
<span data-ttu-id="6dc5f-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6dc5f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6dc5f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6dc5f-120">Request headers</span></span>
| <span data-ttu-id="6dc5f-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6dc5f-121">Header</span></span>       | <span data-ttu-id="6dc5f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6dc5f-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="6dc5f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dc5f-123">Authorization</span></span>  | <span data-ttu-id="6dc5f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6dc5f-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="6dc5f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6dc5f-126">Content-Type</span></span>   | <span data-ttu-id="6dc5f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6dc5f-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6dc5f-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6dc5f-128">Request body</span></span>
<span data-ttu-id="6dc5f-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6dc5f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dc5f-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="6dc5f-130">Response</span></span>

<span data-ttu-id="6dc5f-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6dc5f-131">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6dc5f-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6dc5f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6dc5f-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6dc5f-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/beta/me
```
##### <a name="response"></a><span data-ttu-id="6dc5f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6dc5f-134">Response</span></span>
<span data-ttu-id="6dc5f-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6dc5f-135">Here is an example of the response.</span></span> <span data-ttu-id="6dc5f-136">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="6dc5f-136">Note: The response object shown here may be truncated for brevity.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```

## <a name="see-also"></a><span data-ttu-id="6dc5f-137">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="6dc5f-137">See also</span></span>

- [<span data-ttu-id="6dc5f-138">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="6dc5f-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6dc5f-139">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="6dc5f-139">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="6dc5f-140">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="6dc5f-140">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
