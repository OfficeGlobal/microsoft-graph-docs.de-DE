---
title: mailFolder abrufen
description: Mit dieser Methode können Sie die Eigenschaften und Beziehungen eines Nachrichtenordnerobjekts abrufen.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: d2f61152b8edd98aa11fc7c6b34d2c2b04b72f55
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990124"
---
# <a name="get-mailfolder"></a><span data-ttu-id="94a4a-103">mailFolder abrufen</span><span class="sxs-lookup"><span data-stu-id="94a4a-103">Get mailFolder</span></span>

<span data-ttu-id="94a4a-104">Mit dieser Methode können Sie die Eigenschaften und Beziehungen eines Nachrichtenordnerobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="94a4a-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="94a4a-105">Es gibt zwei Szenarien, in dem eine app e-Mail-Ordner eines anderen Benutzers abgerufen werden kann:</span><span class="sxs-lookup"><span data-stu-id="94a4a-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="94a4a-106">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="94a4a-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="94a4a-107">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer der Benutzer einen e-Mail-Ordner freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="94a4a-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="94a4a-108">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="94a4a-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="94a4a-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="94a4a-109">Permissions</span></span>
<span data-ttu-id="94a4a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94a4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94a4a-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="94a4a-112">Permission type</span></span>      | <span data-ttu-id="94a4a-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="94a4a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94a4a-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="94a4a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="94a4a-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94a4a-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="94a4a-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="94a4a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94a4a-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94a4a-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="94a4a-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="94a4a-118">Application</span></span> | <span data-ttu-id="94a4a-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94a4a-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="94a4a-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="94a4a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="94a4a-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="94a4a-121">Optional query parameters</span></span>
<span data-ttu-id="94a4a-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="94a4a-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="94a4a-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="94a4a-123">Request headers</span></span>
| <span data-ttu-id="94a4a-124">Name</span><span class="sxs-lookup"><span data-stu-id="94a4a-124">Name</span></span>       | <span data-ttu-id="94a4a-125">Typ</span><span class="sxs-lookup"><span data-stu-id="94a4a-125">Type</span></span> | <span data-ttu-id="94a4a-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94a4a-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="94a4a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="94a4a-127">Authorization</span></span>  | <span data-ttu-id="94a4a-128">string</span><span class="sxs-lookup"><span data-stu-id="94a4a-128">string</span></span>  | <span data-ttu-id="94a4a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="94a4a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94a4a-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="94a4a-131">Request body</span></span>
<span data-ttu-id="94a4a-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="94a4a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94a4a-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="94a4a-133">Response</span></span>

<span data-ttu-id="94a4a-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [MailFolder](../resources/mailfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="94a4a-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94a4a-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="94a4a-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94a4a-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="94a4a-136">Request</span></span>
<span data-ttu-id="94a4a-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="94a4a-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="94a4a-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="94a4a-138">Response</span></span>
<span data-ttu-id="94a4a-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="94a4a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
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
