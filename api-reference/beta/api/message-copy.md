---
title: 'message: copy'
description: Mit dieser API können Sie Nachrichten in Ordner kopieren.
ms.openlocfilehash: c0c5428ff2f661d865a6cb2cd17bc0a48e177a52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060386"
---
# <a name="message-copy"></a><span data-ttu-id="99005-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="99005-103">message: copy</span></span>

> <span data-ttu-id="99005-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="99005-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99005-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="99005-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99005-106">Mit dieser API können Sie Nachrichten in Ordner kopieren.</span><span class="sxs-lookup"><span data-stu-id="99005-106">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="99005-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="99005-107">Permissions</span></span>

<span data-ttu-id="99005-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99005-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="99005-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="99005-110">Permission type</span></span> | <span data-ttu-id="99005-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="99005-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="99005-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="99005-112">Delegated (work or school account)</span></span> | <span data-ttu-id="99005-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99005-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="99005-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="99005-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99005-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99005-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="99005-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="99005-116">Application</span></span> | <span data-ttu-id="99005-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99005-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="99005-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="99005-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="99005-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="99005-119">Request headers</span></span>

| <span data-ttu-id="99005-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="99005-120">Header</span></span> | <span data-ttu-id="99005-121">Wert</span><span class="sxs-lookup"><span data-stu-id="99005-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="99005-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="99005-122">Authorization</span></span> | <span data-ttu-id="99005-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="99005-123"></span></span> <span data-ttu-id="99005-124">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="99005-124">Required.</span></span> |
| <span data-ttu-id="99005-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="99005-125">Content-Type</span></span> | <span data-ttu-id="99005-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="99005-126"></span></span> <span data-ttu-id="99005-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="99005-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99005-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="99005-128">Request body</span></span>

<span data-ttu-id="99005-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="99005-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="99005-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="99005-130">Parameter</span></span> | <span data-ttu-id="99005-131">Typ</span><span class="sxs-lookup"><span data-stu-id="99005-131">Type</span></span> | <span data-ttu-id="99005-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99005-132">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="99005-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="99005-133">destinationId</span></span>|<span data-ttu-id="99005-134">String</span><span class="sxs-lookup"><span data-stu-id="99005-134">String</span></span>|<span data-ttu-id="99005-135">Die Ziel-Ordner-ID oder den Ordnernamen einer bekannten.</span><span class="sxs-lookup"><span data-stu-id="99005-135">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="99005-136">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="99005-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="99005-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="99005-137">Response</span></span>

<span data-ttu-id="99005-138">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und eine [Nachricht](../resources/message.md) Ressource in den Antworttext.</span><span class="sxs-lookup"><span data-stu-id="99005-138">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99005-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="99005-139">Example</span></span>

<span data-ttu-id="99005-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="99005-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="99005-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="99005-141">Request</span></span>

<span data-ttu-id="99005-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="99005-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="99005-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="99005-143">Response</span></span>

<span data-ttu-id="99005-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="99005-144">Here is an example of the response.</span></span>

> <span data-ttu-id="99005-145">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="99005-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="99005-146">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="99005-146">All the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
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
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
