---
title: 'message: copy'
description: Mit dieser API können Sie Nachrichten in Ordner kopieren.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a5dfd92c6478414c8890b6c411b5a9385a992198
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514250"
---
# <a name="message-copy"></a><span data-ttu-id="94b38-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="94b38-103">message: copy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94b38-104">Mit dieser API können Sie Nachrichten in Ordner kopieren.</span><span class="sxs-lookup"><span data-stu-id="94b38-104">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="94b38-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="94b38-105">Permissions</span></span>

<span data-ttu-id="94b38-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94b38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94b38-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="94b38-108">Permission type</span></span> | <span data-ttu-id="94b38-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="94b38-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="94b38-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="94b38-110">Delegated (work or school account)</span></span> | <span data-ttu-id="94b38-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94b38-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="94b38-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="94b38-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94b38-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94b38-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="94b38-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="94b38-114">Application</span></span> | <span data-ttu-id="94b38-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94b38-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="94b38-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="94b38-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="94b38-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="94b38-117">Request headers</span></span>

| <span data-ttu-id="94b38-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="94b38-118">Header</span></span> | <span data-ttu-id="94b38-119">Wert</span><span class="sxs-lookup"><span data-stu-id="94b38-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="94b38-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="94b38-120">Authorization</span></span> | <span data-ttu-id="94b38-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="94b38-121"></span></span> <span data-ttu-id="94b38-122">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="94b38-122">Required.</span></span> |
| <span data-ttu-id="94b38-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94b38-123">Content-Type</span></span> | <span data-ttu-id="94b38-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="94b38-124"></span></span> <span data-ttu-id="94b38-125">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="94b38-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94b38-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="94b38-126">Request body</span></span>

<span data-ttu-id="94b38-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="94b38-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="94b38-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="94b38-128">Parameter</span></span> | <span data-ttu-id="94b38-129">Typ</span><span class="sxs-lookup"><span data-stu-id="94b38-129">Type</span></span> | <span data-ttu-id="94b38-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94b38-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="94b38-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="94b38-131">destinationId</span></span>|<span data-ttu-id="94b38-132">String</span><span class="sxs-lookup"><span data-stu-id="94b38-132">String</span></span>|<span data-ttu-id="94b38-133">Die Ziel-Ordner-ID oder den Ordnernamen einer bekannten.</span><span class="sxs-lookup"><span data-stu-id="94b38-133">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="94b38-134">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="94b38-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="94b38-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="94b38-135">Response</span></span>

<span data-ttu-id="94b38-136">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und eine [Nachricht](../resources/message.md) Ressource in den Antworttext.</span><span class="sxs-lookup"><span data-stu-id="94b38-136">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94b38-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="94b38-137">Example</span></span>

<span data-ttu-id="94b38-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="94b38-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="94b38-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="94b38-139">Request</span></span>

<span data-ttu-id="94b38-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="94b38-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="94b38-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="94b38-141">Response</span></span>

<span data-ttu-id="94b38-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="94b38-142">Here is an example of the response.</span></span>

> <span data-ttu-id="94b38-143">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="94b38-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="94b38-144">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="94b38-144">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-copy.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
