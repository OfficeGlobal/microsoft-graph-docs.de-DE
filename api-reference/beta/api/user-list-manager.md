---
title: Manager auflisten
description: Ruft den Vorgesetzten des Benutzers ab. Gibt den Benutzer oder Kontakt zurück, der als Vorgesetzter des Benutzers zugewiesen ist.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3818d72ea024ff06697f123d9a1fb5b3d534152d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933772"
---
# <a name="list-manager"></a><span data-ttu-id="f6521-104">Manager auflisten</span><span class="sxs-lookup"><span data-stu-id="f6521-104">List manager</span></span>

> <span data-ttu-id="f6521-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f6521-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6521-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6521-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f6521-p103">Ruft den Vorgesetzten des Benutzers ab. Gibt den Benutzer oder Kontakt zurück, der als Vorgesetzter des Benutzers zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="f6521-p103">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="f6521-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f6521-109">Permissions</span></span>
<span data-ttu-id="f6521-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6521-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6521-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f6521-112">Permission type</span></span>      | <span data-ttu-id="f6521-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f6521-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6521-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f6521-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f6521-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f6521-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f6521-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f6521-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6521-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6521-117">Not supported.</span></span>    |
|<span data-ttu-id="f6521-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f6521-118">Application</span></span> | <span data-ttu-id="f6521-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6521-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6521-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6521-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f6521-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f6521-121">Optional query parameters</span></span>
<span data-ttu-id="f6521-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f6521-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f6521-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f6521-123">Request headers</span></span>
| <span data-ttu-id="f6521-124">Header</span><span class="sxs-lookup"><span data-stu-id="f6521-124">Header</span></span>       | <span data-ttu-id="f6521-125">Wert</span><span class="sxs-lookup"><span data-stu-id="f6521-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="f6521-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6521-126">Authorization</span></span>  | <span data-ttu-id="f6521-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f6521-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f6521-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6521-129">Content-Type</span></span>   | <span data-ttu-id="f6521-130">application/json</span><span class="sxs-lookup"><span data-stu-id="f6521-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f6521-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f6521-131">Request body</span></span>
<span data-ttu-id="f6521-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f6521-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6521-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6521-133">Response</span></span>

<span data-ttu-id="f6521-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6521-134">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f6521-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f6521-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6521-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6521-136">Request</span></span>
<span data-ttu-id="f6521-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f6521-137">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="f6521-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6521-138">Response</span></span>
<span data-ttu-id="f6521-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f6521-139">Here is an example of the response.</span></span>
<!-- { "blockType": "ignored" } -->
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
