---
title: Nachricht abrufen
description: Mit dieser Methode können Sie die Eigenschaften und Beziehungen eines message-Objekts abrufen.
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 8ff0e85fcfc23a42aaf9219b2248804ffeea9751
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825690"
---
# <a name="get-message"></a><span data-ttu-id="18edf-103">Nachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="18edf-103">Get message</span></span>

<span data-ttu-id="18edf-104">Mit dieser Methode können Sie die Eigenschaften und Beziehungen eines [message](../resources/message.md)-Objekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="18edf-104">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="18edf-105">Zurzeit gibt dieser Vorgang Nachrichtentext ausschließlich im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="18edf-105">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="18edf-106">Es gibt zwei Szenarien, in dem eine app eine Nachricht in einen anderen Benutzer e-Mail-Ordner abrufen:</span><span class="sxs-lookup"><span data-stu-id="18edf-106">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="18edf-107">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="18edf-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="18edf-108">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer der Benutzer einen e-Mail-Ordner freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="18edf-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="18edf-109">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="18edf-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="18edf-110">Da die **message**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **message**-Instanzen abrufen.</span><span class="sxs-lookup"><span data-stu-id="18edf-110">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="18edf-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="18edf-111">Permissions</span></span>
<span data-ttu-id="18edf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18edf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18edf-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18edf-114">Permission type</span></span>      | <span data-ttu-id="18edf-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18edf-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18edf-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18edf-116">Delegated (work or school account)</span></span> | <span data-ttu-id="18edf-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="18edf-117">Mail.Read</span></span>    |
|<span data-ttu-id="18edf-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18edf-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18edf-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="18edf-119">Mail.Read</span></span>    |
|<span data-ttu-id="18edf-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18edf-120">Application</span></span> | <span data-ttu-id="18edf-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="18edf-121">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="18edf-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18edf-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="18edf-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="18edf-123">Optional query parameters</span></span>
<span data-ttu-id="18edf-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="18edf-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="18edf-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18edf-125">Request headers</span></span>
| <span data-ttu-id="18edf-126">Name</span><span class="sxs-lookup"><span data-stu-id="18edf-126">Name</span></span>       | <span data-ttu-id="18edf-127">Typ</span><span class="sxs-lookup"><span data-stu-id="18edf-127">Type</span></span> | <span data-ttu-id="18edf-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18edf-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="18edf-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="18edf-129">Authorization</span></span>  | <span data-ttu-id="18edf-130">string</span><span class="sxs-lookup"><span data-stu-id="18edf-130">string</span></span>  | <span data-ttu-id="18edf-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="18edf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18edf-133">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="18edf-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="18edf-134">string</span><span class="sxs-lookup"><span data-stu-id="18edf-134">string</span></span> | <span data-ttu-id="18edf-135">Das Format, in der die **body**- und **uniqueBody**-Eigenschaften zurückgegeben werden sollen.</span><span class="sxs-lookup"><span data-stu-id="18edf-135">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="18edf-136">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="18edf-136">Values can be "text" or "html".</span></span> <span data-ttu-id="18edf-137">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="18edf-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="18edf-138">Wenn die Kopfzeile nicht angegeben ist, werden die **body**- und **uniqueBody**-Eigenschaften im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18edf-138">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="18edf-139">Optional.</span><span class="sxs-lookup"><span data-stu-id="18edf-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18edf-140">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18edf-140">Request body</span></span>
<span data-ttu-id="18edf-141">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="18edf-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18edf-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="18edf-142">Response</span></span>

<span data-ttu-id="18edf-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18edf-143">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18edf-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18edf-144">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="18edf-145">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="18edf-145">Request 1</span></span>
<span data-ttu-id="18edf-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18edf-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
##### <a name="response-1"></a><span data-ttu-id="18edf-147">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="18edf-147">Response 1</span></span>
<span data-ttu-id="18edf-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18edf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuZ\"",
    "id":"AAMkADhMGAAA=",
    "createdDateTime":"2018-09-09T03:15:05Z",
    "lastModifiedDateTime":"2018-09-09T03:15:08Z",
    "changeKey":"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuZ",
    "categories":[

    ],
    "receivedDateTime":"2018-09-09T03:15:08Z",
    "sentDateTime":"2018-09-09T03:15:06Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR6E1BE060@MWHPR1120.namprd22.prod.outlook.com>",
    "subject":"9/9/2018: concert",
    "bodyPreview":"The group represents Nevada.",
    "importance":"normal",
    "parentFolderId":"AAMkADcbAAAAAAEJAAA=",
    "conversationId":"AAQkADOUpag6yWs=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADMGAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThe group represents Nevada.\r\n</body>\r\n</html>\r\n"
    },
    "sender":{
        "emailAddress":{
            "name":"Adele Vance",
            "address":"adelev@contoso.OnMicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Adele Vance",
            "address":"adelev@contoso.OnMicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="18edf-151">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="18edf-151">Request 2</span></span>
<span data-ttu-id="18edf-152">Im nächste Beispiel wird mit einer `$select` Abfragen Parameter, um die Nachrichtenkopfzeilen Internet eine Nachricht zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="18edf-152">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
##### <a name="response-2"></a><span data-ttu-id="18edf-153">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="18edf-153">Response 2</span></span>
<span data-ttu-id="18edf-154">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="18edf-154">Here is an example of the response.</span></span> <span data-ttu-id="18edf-155">Hinweis: Die Gruppe von Nachrichtenköpfe in der Response-Objekt wird aus Platzgründen Zahl gekürzt.</span><span class="sxs-lookup"><span data-stu-id="18edf-155">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="18edf-156">Alle Header wird von einem tatsächlichen Aufruf zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="18edf-156">All of the headers will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages(internetMessageHeaders)/$entity",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "internetMessageHeaders":[
        {
            "name":"MIME-Version",
            "value":"1.0"
        },
        {
            "name":"Content-Type",
            "value":"multipart/report"
        },
        {
            "name":"x-custom-header-group-name",
            "value":"Washington"
        },
        {
            "name":"x-custom-header-group-id",
            "value":"WA001"
        }
    ]
}
```


## <a name="see-also"></a><span data-ttu-id="18edf-157">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="18edf-157">See also</span></span>

- [<span data-ttu-id="18edf-158">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="18edf-158">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="18edf-159">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="18edf-159">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
