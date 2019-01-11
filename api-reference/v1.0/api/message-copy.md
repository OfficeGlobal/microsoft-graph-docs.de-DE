---
title: 'message: copy'
description: Mit dieser API können Sie Nachrichten in Ordner kopieren.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 38ff866ac6464f53adc021fabb05ad3ad7d435c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854929"
---
# <a name="message-copy"></a><span data-ttu-id="9dc4d-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="9dc4d-103">message: copy</span></span>

<span data-ttu-id="9dc4d-104">Mit dieser API können Sie Nachrichten in Ordner kopieren.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-104">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="9dc4d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9dc4d-105">Permissions</span></span>

<span data-ttu-id="9dc4d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dc4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9dc4d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9dc4d-108">Permission type</span></span> | <span data-ttu-id="9dc4d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9dc4d-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="9dc4d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9dc4d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9dc4d-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9dc4d-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9dc4d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9dc4d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dc4d-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9dc4d-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9dc4d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9dc4d-114">Application</span></span> | <span data-ttu-id="9dc4d-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9dc4d-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9dc4d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9dc4d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="9dc4d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9dc4d-117">Request headers</span></span>

| <span data-ttu-id="9dc4d-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9dc4d-118">Header</span></span> | <span data-ttu-id="9dc4d-119">Wert</span><span class="sxs-lookup"><span data-stu-id="9dc4d-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="9dc4d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9dc4d-120">Authorization</span></span> | <span data-ttu-id="9dc4d-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-121"></span></span> <span data-ttu-id="9dc4d-122">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-122">Required.</span></span> |
| <span data-ttu-id="9dc4d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9dc4d-123">Content-Type</span></span> | <span data-ttu-id="9dc4d-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-124"></span></span> <span data-ttu-id="9dc4d-125">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9dc4d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9dc4d-126">Request body</span></span>

<span data-ttu-id="9dc4d-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9dc4d-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="9dc4d-128">Parameter</span></span> | <span data-ttu-id="9dc4d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="9dc4d-129">Type</span></span> | <span data-ttu-id="9dc4d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9dc4d-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="9dc4d-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="9dc4d-131">destinationId</span></span>|<span data-ttu-id="9dc4d-132">String</span><span class="sxs-lookup"><span data-stu-id="9dc4d-132">String</span></span>|<span data-ttu-id="9dc4d-133">Die Ziel-Ordner-ID oder den Ordnernamen einer bekannten.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-133">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="9dc4d-134">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="9dc4d-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="9dc4d-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="9dc4d-135">Response</span></span>

<span data-ttu-id="9dc4d-136">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und eine [Nachricht](../resources/message.md) Ressource in den Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-136">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dc4d-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9dc4d-137">Example</span></span>

<span data-ttu-id="9dc4d-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9dc4d-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9dc4d-139">Request</span></span>
<span data-ttu-id="9dc4d-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="9dc4d-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="9dc4d-141">Response</span></span>

<span data-ttu-id="9dc4d-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-142">Here is an example of the response.</span></span>

> <span data-ttu-id="9dc4d-143">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9dc4d-144">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-144">All the properties will be returned from an actual call.</span></span>
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
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
