---
title: mailFolder abrufen
description: Mit dieser Methode können Sie die Eigenschaften und Beziehungen eines Nachrichtenordnerobjekts abrufen.
author: angelgolfer-ms
ms.openlocfilehash: e1394c6bf97a3c5d65bda0ee7b8f29d8a29643bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357813"
---
# <a name="get-mailfolder"></a><span data-ttu-id="0efa1-103">mailFolder abrufen</span><span class="sxs-lookup"><span data-stu-id="0efa1-103">Get mailFolder</span></span>

> <span data-ttu-id="0efa1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0efa1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0efa1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0efa1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0efa1-106">Mit dieser Methode können Sie die Eigenschaften und Beziehungen eines Nachrichtenordnerobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="0efa1-106">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="0efa1-107">Es gibt zwei Szenarien, in dem eine app e-Mail-Ordner eines anderen Benutzers abgerufen werden kann:</span><span class="sxs-lookup"><span data-stu-id="0efa1-107">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="0efa1-108">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="0efa1-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="0efa1-109">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer der Benutzer einen e-Mail-Ordner freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="0efa1-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="0efa1-110">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="0efa1-110">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="0efa1-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0efa1-111">Permissions</span></span>
<span data-ttu-id="0efa1-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0efa1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0efa1-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0efa1-114">Permission type</span></span>      | <span data-ttu-id="0efa1-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0efa1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0efa1-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0efa1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="0efa1-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0efa1-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0efa1-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0efa1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0efa1-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0efa1-119">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0efa1-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0efa1-120">Application</span></span> | <span data-ttu-id="0efa1-121">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0efa1-121">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0efa1-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0efa1-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0efa1-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0efa1-123">Optional query parameters</span></span>
<span data-ttu-id="0efa1-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0efa1-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0efa1-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0efa1-125">Request headers</span></span>
| <span data-ttu-id="0efa1-126">Name</span><span class="sxs-lookup"><span data-stu-id="0efa1-126">Name</span></span>       | <span data-ttu-id="0efa1-127">Typ</span><span class="sxs-lookup"><span data-stu-id="0efa1-127">Type</span></span> | <span data-ttu-id="0efa1-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0efa1-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0efa1-129">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0efa1-129">Authorization</span></span>  | <span data-ttu-id="0efa1-130">string</span><span class="sxs-lookup"><span data-stu-id="0efa1-130">string</span></span>  | <span data-ttu-id="0efa1-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0efa1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0efa1-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0efa1-133">Request body</span></span>
<span data-ttu-id="0efa1-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0efa1-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0efa1-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="0efa1-135">Response</span></span>
<span data-ttu-id="0efa1-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [MailFolder](../resources/mailfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0efa1-136">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="0efa1-137">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="0efa1-137">Example 1</span></span>
#### <a name="request-1"></a><span data-ttu-id="0efa1-138">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="0efa1-138">Request 1</span></span>
<span data-ttu-id="0efa1-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0efa1-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

#### <a name="response-1"></a><span data-ttu-id="0efa1-140">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="0efa1-140">Response 1</span></span>
<span data-ttu-id="0efa1-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0efa1-141">The following is an example of the response.</span></span>
 ><span data-ttu-id="0efa1-142">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="0efa1-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0efa1-143">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0efa1-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "Inbox",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

## <a name="example-2"></a><span data-ttu-id="0efa1-144">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="0efa1-144">Example 2</span></span>
#### <a name="request-2"></a><span data-ttu-id="0efa1-145">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="0efa1-145">Request 2</span></span>
<span data-ttu-id="0efa1-146">Es folgt ein Beispiel für Ordner suchen der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0efa1-146">The following is a search folder example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailSearchfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

#### <a name="response-2"></a><span data-ttu-id="0efa1-147">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="0efa1-147">Response 2</span></span>
<span data-ttu-id="0efa1-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0efa1-148">The following is an example of the response.</span></span>
 ><span data-ttu-id="0efa1-149">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="0efa1-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0efa1-150">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0efa1-150">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "Inbox",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
