---
title: Anlagen auflisten
description: Mit dieser API können Sie eine Liste der einer Nachricht angefügten Objekte des Typs attachment abrufen.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 0d89d05c80a8d2437f4940ace2a046f93ba67b82
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806685"
---
# <a name="list-attachments"></a><span data-ttu-id="aa067-103">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="aa067-103">List attachments</span></span>

> <span data-ttu-id="aa067-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aa067-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa067-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aa067-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa067-106">Mit dieser API können Sie eine Liste der einer Nachricht angefügten Objekte des Typs [attachment](../resources/attachment.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="aa067-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa067-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aa067-107">Permissions</span></span>
<span data-ttu-id="aa067-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa067-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa067-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aa067-110">Permission type</span></span>      | <span data-ttu-id="aa067-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aa067-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa067-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aa067-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aa067-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="aa067-113">Mail.Read</span></span>    |
|<span data-ttu-id="aa067-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aa067-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa067-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="aa067-115">Mail.Read</span></span>    |
|<span data-ttu-id="aa067-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aa067-116">Application</span></span> | <span data-ttu-id="aa067-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="aa067-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa067-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa067-118">HTTP request</span></span>
<span data-ttu-id="aa067-119"><!-- { "blockType": "ignored" } -->Anlagen für eine [Nachricht](../resources/message.md) im Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="aa067-119"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="aa067-120">Anlagen für eine [Nachricht](../resources/message.md) in einem [MailFolder](../resources/mailfolder.md) der obersten Ebene im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="aa067-120">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="aa067-p103">Anlagen für eine [Nachricht](../resources/message.md) in einem untergeordneten [MailFolder](../resources/mailfolder.md) im Postfach eines Benutzers.  Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber eine Nachricht kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="aa067-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aa067-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="aa067-123">Optional query parameters</span></span>
<span data-ttu-id="aa067-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aa067-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="aa067-125">Insbesondere können Sie die $ Abfragezeichenfolgen-Parameter, um alle der Nachricht Anlagen Inline mit dem Rest der Nachrichteneigenschaften erweitern.</span><span class="sxs-lookup"><span data-stu-id="aa067-125">In particular, you can use the $expand query parameter to include all of the message attachments inline with the rest of the message properties.</span></span> <span data-ttu-id="aa067-126">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="aa067-126">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/messages/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="aa067-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aa067-127">Request headers</span></span>
| <span data-ttu-id="aa067-128">Name</span><span class="sxs-lookup"><span data-stu-id="aa067-128">Name</span></span>       | <span data-ttu-id="aa067-129">Typ</span><span class="sxs-lookup"><span data-stu-id="aa067-129">Type</span></span> | <span data-ttu-id="aa067-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa067-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aa067-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa067-131">Authorization</span></span>  | <span data-ttu-id="aa067-132">string</span><span class="sxs-lookup"><span data-stu-id="aa067-132">string</span></span>  | <span data-ttu-id="aa067-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aa067-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa067-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aa067-135">Request body</span></span>
<span data-ttu-id="aa067-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aa067-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa067-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa067-137">Response</span></span>

<span data-ttu-id="aa067-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Attachment](../resources/attachment.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa067-138">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aa067-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aa067-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa067-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa067-140">Request</span></span>
<span data-ttu-id="aa067-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aa067-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="aa067-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa067-142">Response</span></span>
<span data-ttu-id="aa067-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa067-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
