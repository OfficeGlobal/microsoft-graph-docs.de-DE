---
title: Nachricht erstellen
description: Mit dieser API können Sie in einem Objekt des Typs „mailfolder“ neue Nachrichten erstellen.
ms.openlocfilehash: 4d901385559ed89b6215069b97ae2f323cc66cf6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016878"
---
# <a name="create-message"></a><span data-ttu-id="92c00-103">Nachricht erstellen</span><span class="sxs-lookup"><span data-stu-id="92c00-103">Create Message</span></span>

<span data-ttu-id="92c00-104">Mit dieser API können Sie in einem Objekt des Typs „mailfolder“ neue Nachrichten erstellen.</span><span class="sxs-lookup"><span data-stu-id="92c00-104">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="92c00-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="92c00-105">Permissions</span></span>
<span data-ttu-id="92c00-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92c00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92c00-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="92c00-108">Permission type</span></span>      | <span data-ttu-id="92c00-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="92c00-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92c00-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="92c00-110">Delegated (work or school account)</span></span> | <span data-ttu-id="92c00-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92c00-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="92c00-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="92c00-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92c00-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92c00-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="92c00-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="92c00-114">Application</span></span> | <span data-ttu-id="92c00-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92c00-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="92c00-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="92c00-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="92c00-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="92c00-117">Request headers</span></span>
| <span data-ttu-id="92c00-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="92c00-118">Header</span></span>       | <span data-ttu-id="92c00-119">Wert</span><span class="sxs-lookup"><span data-stu-id="92c00-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="92c00-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="92c00-120">Authorization</span></span>  | <span data-ttu-id="92c00-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="92c00-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="92c00-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="92c00-123">Content-Type</span></span>  | <span data-ttu-id="92c00-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="92c00-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="92c00-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="92c00-126">Request body</span></span>
<span data-ttu-id="92c00-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [Message](../resources/message.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="92c00-127">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="92c00-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="92c00-128">Response</span></span>

<span data-ttu-id="92c00-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [Message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="92c00-129">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92c00-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="92c00-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92c00-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="92c00-131">Request</span></span>
<span data-ttu-id="92c00-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="92c00-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```
<span data-ttu-id="92c00-133">Geben Sie im Anforderungstext eine JSON-Darstellung des [message](../resources/message.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="92c00-133">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="92c00-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="92c00-134">Response</span></span>
<span data-ttu-id="92c00-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="92c00-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
