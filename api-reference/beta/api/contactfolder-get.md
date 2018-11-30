---
title: contactFolder abrufen
description: Dient zum Abrufen eines Kontaktordners anhand der Kontaktordner-ID.
ms.openlocfilehash: f57471da55ea10128d0eaec4503c4f323a751fc0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058316"
---
# <a name="get-contactfolder"></a><span data-ttu-id="062a3-103">contactFolder abrufen</span><span class="sxs-lookup"><span data-stu-id="062a3-103">Get contactFolder</span></span>

> <span data-ttu-id="062a3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="062a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="062a3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="062a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="062a3-106">Dient zum Abrufen eines Kontaktordners anhand der Kontaktordner-ID.</span><span class="sxs-lookup"><span data-stu-id="062a3-106">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="062a3-107">Es gibt zwei Szenarien, in dem eine app Kontaktordner eines anderen Benutzers abgerufen werden kann:</span><span class="sxs-lookup"><span data-stu-id="062a3-107">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="062a3-108">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="062a3-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="062a3-109">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer diesen Benutzer einen Kontaktordner freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="062a3-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="062a3-110">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="062a3-110">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="062a3-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="062a3-111">Permissions</span></span>
<span data-ttu-id="062a3-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="062a3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="062a3-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="062a3-114">Permission type</span></span>      | <span data-ttu-id="062a3-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="062a3-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="062a3-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="062a3-116">Delegated (work or school account)</span></span> | <span data-ttu-id="062a3-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="062a3-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="062a3-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="062a3-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="062a3-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="062a3-119">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="062a3-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="062a3-120">Application</span></span> | <span data-ttu-id="062a3-121">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="062a3-121">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="062a3-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="062a3-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="062a3-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="062a3-123">Optional query parameters</span></span>
<span data-ttu-id="062a3-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="062a3-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="062a3-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="062a3-125">Request headers</span></span>
| <span data-ttu-id="062a3-126">Name</span><span class="sxs-lookup"><span data-stu-id="062a3-126">Name</span></span>       | <span data-ttu-id="062a3-127">Typ</span><span class="sxs-lookup"><span data-stu-id="062a3-127">Type</span></span> | <span data-ttu-id="062a3-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="062a3-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="062a3-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="062a3-129">Authorization</span></span>  | <span data-ttu-id="062a3-130">string</span><span class="sxs-lookup"><span data-stu-id="062a3-130">string</span></span>  | <span data-ttu-id="062a3-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="062a3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="062a3-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="062a3-133">Request body</span></span>
<span data-ttu-id="062a3-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="062a3-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="062a3-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="062a3-135">Response</span></span>

<span data-ttu-id="062a3-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [contactFolder](../resources/contactfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="062a3-136">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="062a3-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="062a3-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="062a3-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="062a3-138">Request</span></span>
<span data-ttu-id="062a3-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="062a3-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="062a3-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="062a3-140">Response</span></span>
<span data-ttu-id="062a3-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="062a3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "wellKnownName": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
