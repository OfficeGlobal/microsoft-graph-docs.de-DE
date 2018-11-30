---
title: Benutzer abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des Benutzerobjekts.
ms.openlocfilehash: f5392e25736fb93fd112413e00012eea78dc2449
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065649"
---
# <a name="get-a-user"></a><span data-ttu-id="bfc5f-103">Benutzer abrufen</span><span class="sxs-lookup"><span data-stu-id="bfc5f-103">Get a user</span></span>

> <span data-ttu-id="bfc5f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bfc5f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfc5f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bfc5f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bfc5f-106">Dient zum Abrufen der Eigenschaften und der Beziehungen des Benutzerobjekts.</span><span class="sxs-lookup"><span data-stu-id="bfc5f-106">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="bfc5f-107">Da die Ressource **Benutzer** [Extensions](/graph/extensibility-overview)unterstützt, können Sie auch die `GET` Vorgang zum Abrufen von benutzerdefinierten Eigenschaften und Erweiterungsdaten in eine Instanz des **Benutzers** .</span><span class="sxs-lookup"><span data-stu-id="bfc5f-107">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfc5f-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bfc5f-108">Permissions</span></span>
<span data-ttu-id="bfc5f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfc5f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfc5f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bfc5f-111">Permission type</span></span>      | <span data-ttu-id="bfc5f-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bfc5f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfc5f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bfc5f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bfc5f-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bfc5f-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bfc5f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bfc5f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfc5f-116">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfc5f-116">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="bfc5f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bfc5f-117">Application</span></span> | <span data-ttu-id="bfc5f-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfc5f-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfc5f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfc5f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bfc5f-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bfc5f-120">Optional query parameters</span></span>
<span data-ttu-id="bfc5f-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bfc5f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bfc5f-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bfc5f-122">Request headers</span></span>
| <span data-ttu-id="bfc5f-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bfc5f-123">Header</span></span>       | <span data-ttu-id="bfc5f-124">Wert</span><span class="sxs-lookup"><span data-stu-id="bfc5f-124">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="bfc5f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfc5f-125">Authorization</span></span>  | <span data-ttu-id="bfc5f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bfc5f-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="bfc5f-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bfc5f-128">Content-Type</span></span>   | <span data-ttu-id="bfc5f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="bfc5f-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfc5f-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bfc5f-130">Request body</span></span>
<span data-ttu-id="bfc5f-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bfc5f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfc5f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfc5f-132">Response</span></span>

<span data-ttu-id="bfc5f-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bfc5f-133">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bfc5f-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bfc5f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfc5f-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfc5f-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/beta/me
```
##### <a name="response"></a><span data-ttu-id="bfc5f-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfc5f-136">Response</span></span>
<span data-ttu-id="bfc5f-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bfc5f-137">Here is an example of the response.</span></span> <span data-ttu-id="bfc5f-138">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="bfc5f-138">Note: The response object shown here may be truncated for brevity.</span></span> 

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

## <a name="see-also"></a><span data-ttu-id="bfc5f-139">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="bfc5f-139">See also</span></span>

- [<span data-ttu-id="bfc5f-140">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="bfc5f-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bfc5f-141">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="bfc5f-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="bfc5f-142">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="bfc5f-142">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
