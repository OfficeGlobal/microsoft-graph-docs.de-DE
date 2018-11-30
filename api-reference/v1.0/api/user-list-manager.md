---
title: Manager auflisten
description: Ruft den Vorgesetzten des Benutzers ab. Gibt den Benutzer oder Kontakt zurück, der als Vorgesetzter des Benutzers zugewiesen ist.
ms.openlocfilehash: eb25449970311ceb7790b54c64191c669daeb004
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016032"
---
# <a name="list-manager"></a><span data-ttu-id="29e01-104">Manager auflisten</span><span class="sxs-lookup"><span data-stu-id="29e01-104">List manager</span></span>

<span data-ttu-id="29e01-p102">Ruft den Vorgesetzten des Benutzers ab. Gibt den Benutzer oder Kontakt zurück, der als Vorgesetzter des Benutzers zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="29e01-p102">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="29e01-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="29e01-107">Permissions</span></span>
<span data-ttu-id="29e01-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29e01-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29e01-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="29e01-110">Permission type</span></span>      | <span data-ttu-id="29e01-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="29e01-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29e01-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="29e01-112">Delegated (work or school account)</span></span> | <span data-ttu-id="29e01-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="29e01-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="29e01-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="29e01-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29e01-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29e01-115">Not supported.</span></span>    |
|<span data-ttu-id="29e01-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="29e01-116">Application</span></span> | <span data-ttu-id="29e01-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29e01-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29e01-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="29e01-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="29e01-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="29e01-119">Optional query parameters</span></span>
<span data-ttu-id="29e01-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="29e01-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="29e01-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="29e01-121">Request headers</span></span>
| <span data-ttu-id="29e01-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="29e01-122">Header</span></span>       | <span data-ttu-id="29e01-123">Wert</span><span class="sxs-lookup"><span data-stu-id="29e01-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="29e01-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="29e01-124">Authorization</span></span>  | <span data-ttu-id="29e01-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="29e01-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="29e01-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29e01-127">Content-Type</span></span>   | <span data-ttu-id="29e01-128">application/json</span><span class="sxs-lookup"><span data-stu-id="29e01-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29e01-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="29e01-129">Request body</span></span>
<span data-ttu-id="29e01-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="29e01-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29e01-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="29e01-131">Response</span></span>

<span data-ttu-id="29e01-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29e01-132">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29e01-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="29e01-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29e01-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="29e01-134">Request</span></span>
<span data-ttu-id="29e01-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="29e01-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="29e01-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="29e01-136">Response</span></span>
<span data-ttu-id="29e01-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="29e01-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->