---
title: Anlagen auflisten
description: Mit dieser API können Sie eine Liste der einer Nachricht angefügten Objekte des Typs attachment abrufen.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b394b2f5bc81954467ebb315750087141936f3d5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509910"
---
# <a name="list-attachments"></a><span data-ttu-id="41818-103">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="41818-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41818-104">Mit dieser API können Sie eine Liste der einer Nachricht angefügten Objekte des Typs [attachment](../resources/attachment.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="41818-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="41818-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="41818-105">Permissions</span></span>
<span data-ttu-id="41818-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41818-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41818-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="41818-108">Permission type</span></span>      | <span data-ttu-id="41818-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="41818-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41818-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="41818-110">Delegated (work or school account)</span></span> | <span data-ttu-id="41818-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="41818-111">Mail.Read</span></span>    |
|<span data-ttu-id="41818-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="41818-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41818-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="41818-113">Mail.Read</span></span>    |
|<span data-ttu-id="41818-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="41818-114">Application</span></span> | <span data-ttu-id="41818-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="41818-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="41818-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="41818-116">HTTP request</span></span>
<span data-ttu-id="41818-117"><!-- { "blockType": "ignored" } -->Anlagen für eine [Nachricht](../resources/message.md) im Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="41818-117"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="41818-118">Anlagen für eine [Nachricht](../resources/message.md) in einem [MailFolder](../resources/mailfolder.md) der obersten Ebene im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="41818-118">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="41818-p102">Anlagen für eine [Nachricht](../resources/message.md) in einem untergeordneten [MailFolder](../resources/mailfolder.md) im Postfach eines Benutzers.  Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber eine Nachricht kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="41818-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="41818-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="41818-121">Optional query parameters</span></span>
<span data-ttu-id="41818-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="41818-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="41818-123">Insbesondere können Sie die $ Abfragezeichenfolgen-Parameter, um alle der Nachricht Anlagen Inline mit dem Rest der Nachrichteneigenschaften erweitern.</span><span class="sxs-lookup"><span data-stu-id="41818-123">In particular, you can use the $expand query parameter to include all of the message attachments inline with the rest of the message properties.</span></span> <span data-ttu-id="41818-124">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="41818-124">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/messages/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="41818-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="41818-125">Request headers</span></span>
| <span data-ttu-id="41818-126">Name</span><span class="sxs-lookup"><span data-stu-id="41818-126">Name</span></span>       | <span data-ttu-id="41818-127">Typ</span><span class="sxs-lookup"><span data-stu-id="41818-127">Type</span></span> | <span data-ttu-id="41818-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41818-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="41818-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="41818-129">Authorization</span></span>  | <span data-ttu-id="41818-130">string</span><span class="sxs-lookup"><span data-stu-id="41818-130">string</span></span>  | <span data-ttu-id="41818-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="41818-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41818-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="41818-133">Request body</span></span>
<span data-ttu-id="41818-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="41818-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41818-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="41818-135">Response</span></span>

<span data-ttu-id="41818-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Attachment](../resources/attachment.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="41818-136">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="41818-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="41818-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41818-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="41818-138">Request</span></span>
<span data-ttu-id="41818-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="41818-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="41818-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="41818-140">Response</span></span>
<span data-ttu-id="41818-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="41818-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-list-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
