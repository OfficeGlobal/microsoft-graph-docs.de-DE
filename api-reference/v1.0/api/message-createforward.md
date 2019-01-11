---
title: 'message: createForward'
description: Erstellen Sie einen Entwurf, um die angegebene Nachricht weiterzuleiten. Anschließend können Sie den Entwurf aktualisieren, um den Inhalt zum **Text** hinzuzufügen, oder andere Nachrichteneigenschaften ändern. Sie können den Entwurf auch einfach senden.
localization_priority: Normal
ms.openlocfilehash: 230fdfd4a1700e5bcbe2e1cb364de08d86c7be39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888263"
---
# <a name="message-createforward"></a><span data-ttu-id="1ec6e-104">message: createForward</span><span class="sxs-lookup"><span data-stu-id="1ec6e-104">message: createForward</span></span>

<span data-ttu-id="1ec6e-105">Erstellen Sie einen Entwurf, um die angegebene [Nachricht](../resources/message.md) weiterzuleiten.</span><span class="sxs-lookup"><span data-stu-id="1ec6e-105">Create a draft to forward the specified [message](../resources/message.md).</span></span> <span data-ttu-id="1ec6e-106">Anschließend können Sie den Entwurf [aktualisieren](../api/message-update.md), um den Inhalt zum **Text** hinzuzufügen, oder andere Nachrichteneigenschaften ändern. Sie können den Entwurf auch einfach [senden](../api/message-send.md).</span><span class="sxs-lookup"><span data-stu-id="1ec6e-106">You can then [update](../api/message-update.md) the draft to add content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ec6e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1ec6e-107">Permissions</span></span>

<span data-ttu-id="1ec6e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ec6e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ec6e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1ec6e-110">Permission type</span></span>      | <span data-ttu-id="1ec6e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1ec6e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ec6e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1ec6e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1ec6e-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ec6e-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1ec6e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1ec6e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ec6e-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ec6e-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1ec6e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1ec6e-116">Application</span></span> | <span data-ttu-id="1ec6e-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ec6e-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ec6e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ec6e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```

## <a name="request-headers"></a><span data-ttu-id="1ec6e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1ec6e-119">Request headers</span></span>

| <span data-ttu-id="1ec6e-120">Name</span><span class="sxs-lookup"><span data-stu-id="1ec6e-120">Name</span></span>       | <span data-ttu-id="1ec6e-121">Typ</span><span class="sxs-lookup"><span data-stu-id="1ec6e-121">Type</span></span> | <span data-ttu-id="1ec6e-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ec6e-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1ec6e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ec6e-123">Authorization</span></span>  | <span data-ttu-id="1ec6e-124">string</span><span class="sxs-lookup"><span data-stu-id="1ec6e-124">string</span></span>  | <span data-ttu-id="1ec6e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1ec6e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ec6e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1ec6e-127">Request body</span></span>

<span data-ttu-id="1ec6e-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1ec6e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ec6e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ec6e-129">Response</span></span>

<span data-ttu-id="1ec6e-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [Message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ec6e-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ec6e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1ec6e-131">Example</span></span>

<span data-ttu-id="1ec6e-132">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="1ec6e-132">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1ec6e-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ec6e-133">Request</span></span>

<span data-ttu-id="1ec6e-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1ec6e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createForward
```

##### <a name="response"></a><span data-ttu-id="1ec6e-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ec6e-135">Response</span></span>

<span data-ttu-id="1ec6e-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ec6e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
