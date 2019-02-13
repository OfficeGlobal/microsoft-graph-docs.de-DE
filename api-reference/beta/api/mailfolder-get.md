---
title: mailFolder abrufen
description: Mit dieser Methode können Sie die Eigenschaften und Beziehungen eines Nachrichtenordnerobjekts abrufen.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: af2cc42c2ee72f1a57a1e0f9402209c107e259f4
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967298"
---
# <a name="get-mailfolder"></a><span data-ttu-id="aab30-103">mailFolder abrufen</span><span class="sxs-lookup"><span data-stu-id="aab30-103">Get mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aab30-104">Mit dieser Methode können Sie die Eigenschaften und Beziehungen eines Nachrichtenordnerobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="aab30-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="aab30-105">Es gibt zwei Szenarien, in dem eine app e-Mail-Ordner eines anderen Benutzers abgerufen werden kann:</span><span class="sxs-lookup"><span data-stu-id="aab30-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="aab30-106">Wenn die App Anwendungsberechtigungen besitzt oder</span><span class="sxs-lookup"><span data-stu-id="aab30-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="aab30-107">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer der Benutzer einen e-Mail-Ordner freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="aab30-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="aab30-108">Hier finden Sie [weitere Informationen und ein Beispiel](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="aab30-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="aab30-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aab30-109">Permissions</span></span>

<span data-ttu-id="aab30-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aab30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aab30-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aab30-112">Permission type</span></span>      | <span data-ttu-id="aab30-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aab30-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aab30-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aab30-114">Delegated (work or school account)</span></span> | <span data-ttu-id="aab30-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aab30-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="aab30-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aab30-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aab30-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aab30-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="aab30-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aab30-118">Application</span></span> | <span data-ttu-id="aab30-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aab30-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="aab30-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aab30-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aab30-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="aab30-121">Optional query parameters</span></span>

<span data-ttu-id="aab30-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aab30-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aab30-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aab30-123">Request headers</span></span>

| <span data-ttu-id="aab30-124">Name</span><span class="sxs-lookup"><span data-stu-id="aab30-124">Name</span></span>          | <span data-ttu-id="aab30-125">Typ</span><span class="sxs-lookup"><span data-stu-id="aab30-125">Type</span></span>   | <span data-ttu-id="aab30-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aab30-126">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="aab30-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="aab30-127">Authorization</span></span> | <span data-ttu-id="aab30-128">string</span><span class="sxs-lookup"><span data-stu-id="aab30-128">string</span></span> | <span data-ttu-id="aab30-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aab30-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aab30-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aab30-131">Request body</span></span>

<span data-ttu-id="aab30-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aab30-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aab30-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="aab30-133">Response</span></span>

<span data-ttu-id="aab30-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [MailFolder](../resources/mailfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aab30-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aab30-135">Beispiele</span><span class="sxs-lookup"><span data-stu-id="aab30-135">Examples</span></span>

### <a name="example-1-get-a-mail-folder"></a><span data-ttu-id="aab30-136">In Beispiel 1: Abrufen von e-Mail-Ordnern</span><span class="sxs-lookup"><span data-stu-id="aab30-136">Example 1: Get a mail folder</span></span>

#### <a name="request"></a><span data-ttu-id="aab30-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aab30-137">Request</span></span>

<span data-ttu-id="aab30-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aab30-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="aab30-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="aab30-139">Response</span></span>

<span data-ttu-id="aab30-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aab30-140">The following is an example of the response.</span></span>

> <span data-ttu-id="aab30-141">**Hinweis:**  Das hier gezeigte Antwortobjekt ist möglicherweise zur besseren Lesbarkeit gekürzt worden.</span><span class="sxs-lookup"><span data-stu-id="aab30-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="aab30-142">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="aab30-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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

### <a name="example-2-get-a-mail-search-folder"></a><span data-ttu-id="aab30-143">Beispiel 2: Abrufen von Ordnern e-Mail-Suche</span><span class="sxs-lookup"><span data-stu-id="aab30-143">Example 2: Get a mail search folder</span></span>

#### <a name="request"></a><span data-ttu-id="aab30-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aab30-144">Request</span></span>

<span data-ttu-id="aab30-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aab30-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mailSearchfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzN
```

#### <a name="response"></a><span data-ttu-id="aab30-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="aab30-146">Response</span></span>

<span data-ttu-id="aab30-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aab30-147">The following is an example of the response.</span></span>

> <span data-ttu-id="aab30-148">**Hinweis:**  Das hier gezeigte Antwortobjekt ist möglicherweise zur besseren Lesbarkeit gekürzt worden.</span><span class="sxs-lookup"><span data-stu-id="aab30-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="aab30-149">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="aab30-149">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzN",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzI",
  "childFolderCount": 0,
  "unreadItemCount": 6,
  "totalItemCount": 6,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
    "AAMkAGVmMDEzM"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
