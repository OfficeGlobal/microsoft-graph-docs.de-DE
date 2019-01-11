---
title: Nachrichten auflisten
description: Mit dieser API können Sie alle Nachrichten im Postfach des angemeldeten Benutzers abrufen oder alle Nachrichten in einem bestimmten Ordner in diesem Postfach.
localization_priority: Priority
ms.openlocfilehash: a58d6e3c51cf85992129b3ba9c8e3996fa9841f8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825368"
---
# <a name="list-messages"></a><span data-ttu-id="74bcd-103">Nachrichten auflisten</span><span class="sxs-lookup"><span data-stu-id="74bcd-103">List messages</span></span>

<span data-ttu-id="74bcd-104">Mit dieser API können Sie alle Nachrichten im Postfach des angemeldeten Benutzers abrufen oder alle Nachrichten in einem bestimmten Ordner in diesem Postfach.</span><span class="sxs-lookup"><span data-stu-id="74bcd-104">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="74bcd-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="74bcd-105">Permissions</span></span>
<span data-ttu-id="74bcd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74bcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74bcd-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="74bcd-108">Permission type</span></span>      | <span data-ttu-id="74bcd-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="74bcd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74bcd-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="74bcd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="74bcd-111">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74bcd-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="74bcd-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="74bcd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74bcd-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74bcd-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="74bcd-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="74bcd-114">Application</span></span> | <span data-ttu-id="74bcd-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74bcd-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="74bcd-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="74bcd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="74bcd-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="74bcd-117">Optional query parameters</span></span>
<span data-ttu-id="74bcd-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="74bcd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="74bcd-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="74bcd-119">Request headers</span></span>
| <span data-ttu-id="74bcd-120">Name</span><span class="sxs-lookup"><span data-stu-id="74bcd-120">Name</span></span>       | <span data-ttu-id="74bcd-121">Typ</span><span class="sxs-lookup"><span data-stu-id="74bcd-121">Type</span></span> | <span data-ttu-id="74bcd-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74bcd-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="74bcd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74bcd-123">Authorization</span></span>  | <span data-ttu-id="74bcd-124">string</span><span class="sxs-lookup"><span data-stu-id="74bcd-124">string</span></span>  | <span data-ttu-id="74bcd-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="74bcd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74bcd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="74bcd-127">Request body</span></span>
<span data-ttu-id="74bcd-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="74bcd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74bcd-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="74bcd-129">Response</span></span>

<span data-ttu-id="74bcd-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Message](../resources/message.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74bcd-130">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="74bcd-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="74bcd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74bcd-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74bcd-132">Request</span></span>
<span data-ttu-id="74bcd-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="74bcd-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="74bcd-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="74bcd-134">Response</span></span>
<span data-ttu-id="74bcd-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74bcd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
