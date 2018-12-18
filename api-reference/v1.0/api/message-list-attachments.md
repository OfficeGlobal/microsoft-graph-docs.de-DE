---
title: Anlagen auflisten
description: Mit dieser API können Sie eine Liste der einer Nachricht angefügten Objekte des Typs attachment abrufen.
author: angelgolfer-ms
ms.openlocfilehash: 740616e0f2da0a941f6dc49944d81168dcc7d2c3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352679"
---
# <a name="list-attachments"></a><span data-ttu-id="93878-103">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="93878-103">List attachments</span></span>

<span data-ttu-id="93878-104">Mit dieser API können Sie eine Liste der einer Nachricht angefügten Objekte des Typs [attachment](../resources/attachment.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="93878-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="93878-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="93878-105">Permissions</span></span>
<span data-ttu-id="93878-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93878-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93878-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="93878-108">Permission type</span></span>      | <span data-ttu-id="93878-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="93878-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93878-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="93878-110">Delegated (work or school account)</span></span> | <span data-ttu-id="93878-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="93878-111">Mail.Read</span></span>    |
|<span data-ttu-id="93878-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="93878-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93878-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="93878-113">Mail.Read</span></span>    |
|<span data-ttu-id="93878-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="93878-114">Application</span></span> | <span data-ttu-id="93878-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="93878-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="93878-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="93878-116">HTTP request</span></span>
<span data-ttu-id="93878-117"><!-- { "blockType": "ignored" } -->Anlagen für eine [Nachricht](../resources/message.md) im Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="93878-117"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="93878-118">Anlagen für eine [Nachricht](../resources/message.md) in einem [MailFolder](../resources/mailfolder.md) der obersten Ebene im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="93878-118">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="93878-p102">Anlagen für eine [Nachricht](../resources/message.md) in einem untergeordneten [MailFolder](../resources/mailfolder.md) im Postfach eines Benutzers.  Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber eine Nachricht kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="93878-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="93878-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="93878-121">Optional query parameters</span></span>
<span data-ttu-id="93878-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="93878-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="93878-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="93878-123">Request headers</span></span>
| <span data-ttu-id="93878-124">Name</span><span class="sxs-lookup"><span data-stu-id="93878-124">Name</span></span>       | <span data-ttu-id="93878-125">Typ</span><span class="sxs-lookup"><span data-stu-id="93878-125">Type</span></span> | <span data-ttu-id="93878-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93878-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="93878-127">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="93878-127">Authorization</span></span>  | <span data-ttu-id="93878-128">string</span><span class="sxs-lookup"><span data-stu-id="93878-128">string</span></span>  | <span data-ttu-id="93878-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="93878-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93878-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="93878-131">Request body</span></span>
<span data-ttu-id="93878-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="93878-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93878-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="93878-133">Response</span></span>

<span data-ttu-id="93878-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Attachment](../resources/attachment.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="93878-134">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93878-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="93878-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93878-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="93878-136">Request</span></span>
<span data-ttu-id="93878-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="93878-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="93878-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="93878-138">Response</span></span>
<span data-ttu-id="93878-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="93878-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
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