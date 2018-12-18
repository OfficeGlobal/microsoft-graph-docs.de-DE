---
title: Nachricht erstellen
description: Mit dieser API können Sie in einem Objekt des Typs „mailfolder“ neue Nachrichten erstellen.
author: angelgolfer-ms
ms.openlocfilehash: bb88a061a8e867f4cc15470073925c51fe6a3cf6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332543"
---
# <a name="create-message"></a><span data-ttu-id="39673-103">Nachricht erstellen</span><span class="sxs-lookup"><span data-stu-id="39673-103">Create Message</span></span>

<span data-ttu-id="39673-104">Mit dieser API können Sie in einem Objekt des Typs „mailfolder“ neue Nachrichten erstellen.</span><span class="sxs-lookup"><span data-stu-id="39673-104">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="39673-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="39673-105">Permissions</span></span>
<span data-ttu-id="39673-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39673-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39673-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="39673-108">Permission type</span></span>      | <span data-ttu-id="39673-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="39673-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39673-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="39673-110">Delegated (work or school account)</span></span> | <span data-ttu-id="39673-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39673-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="39673-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="39673-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39673-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39673-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="39673-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="39673-114">Application</span></span> | <span data-ttu-id="39673-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39673-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="39673-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="39673-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="39673-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="39673-117">Request headers</span></span>
| <span data-ttu-id="39673-118">Header</span><span class="sxs-lookup"><span data-stu-id="39673-118">Header</span></span>       | <span data-ttu-id="39673-119">Wert</span><span class="sxs-lookup"><span data-stu-id="39673-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="39673-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="39673-120">Authorization</span></span>  | <span data-ttu-id="39673-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="39673-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="39673-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="39673-123">Content-Type</span></span>  | <span data-ttu-id="39673-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="39673-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="39673-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="39673-126">Request body</span></span>
<span data-ttu-id="39673-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [Message](../resources/message.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="39673-127">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="39673-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="39673-128">Response</span></span>

<span data-ttu-id="39673-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [Message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39673-129">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39673-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="39673-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39673-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39673-131">Request</span></span>
<span data-ttu-id="39673-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="39673-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="39673-133">Geben Sie im Anforderungstext eine JSON-Darstellung des [message](../resources/message.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="39673-133">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="39673-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="39673-134">Response</span></span>
<span data-ttu-id="39673-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39673-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
