---
title: Nachricht abrufen
description: Rufen Sie die Eigenschaften und Beziehungen des Message-Objekts ab.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e5f7b8c73ac9e121a1f0cbe1bf4200326d2d4e29
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526032"
---
# <a name="get-message"></a><span data-ttu-id="0f6f6-103">Nachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="0f6f6-103">Get message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f6f6-104">Rufen Sie die Eigenschaften und Beziehungen des [Message](../resources/message.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-104">Retrieve the properties and relationships of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="0f6f6-105">Beispielsweise können Sie eine Nachricht erhalten möchten, und erweitern Sie alle [erwähnen](../resources/mention.md) Instanzen in der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-105">For example, you can get a message and expand all the [mention](../resources/mention.md) instances in the message.</span></span>

<span data-ttu-id="0f6f6-106">Es gibt zwei Szenarien, in dem eine app eine Nachricht in einen anderen Benutzer e-Mail-Ordner abrufen:</span><span class="sxs-lookup"><span data-stu-id="0f6f6-106">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="0f6f6-107">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="0f6f6-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="0f6f6-108">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer der Benutzer einen e-Mail-Ordner freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="0f6f6-109">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="0f6f6-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="0f6f6-110">Da die **message**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **message**-Instanzen abrufen.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-110">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="0f6f6-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0f6f6-111">Permissions</span></span>
<span data-ttu-id="0f6f6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f6f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f6f6-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0f6f6-114">Permission type</span></span>      | <span data-ttu-id="0f6f6-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0f6f6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f6f6-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0f6f6-116">Delegated (work or school account)</span></span> | <span data-ttu-id="0f6f6-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0f6f6-117">Mail.Read</span></span>    |
|<span data-ttu-id="0f6f6-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0f6f6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f6f6-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0f6f6-119">Mail.Read</span></span>    |
|<span data-ttu-id="0f6f6-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f6f6-120">Application</span></span> | <span data-ttu-id="0f6f6-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0f6f6-121">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f6f6-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f6f6-122">HTTP request</span></span>

<span data-ttu-id="0f6f6-123">Um die angegebene ausgegeben werden:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0f6f6-123">To get the specified message: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="0f6f6-124">Zum Abrufen einer Nachricht, und erweitern alle Vorkommnisse in der Nachricht:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0f6f6-124">To get a message and expand all mentions in the message: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/messages/{id}?$expand=mentions
GET /me/mailFolders/{id}/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}?$expand=mentions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0f6f6-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0f6f6-125">Optional query parameters</span></span>
<span data-ttu-id="0f6f6-126">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="0f6f6-127">Sie können die `$expand` erweitert Abfragezeichenfolgen-Parameter auf Navigationseigenschaft **erwähnt** , wird eine Meldung mit den Details jeder [erwähnen](../resources/mention.md) in der Nachricht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-127">You can use the `$expand` query parameter on the **mentions** navigation property to get a message with the details of each [mention](../resources/mention.md) in the message expanded.</span></span>



## <a name="request-headers"></a><span data-ttu-id="0f6f6-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0f6f6-128">Request headers</span></span>
| <span data-ttu-id="0f6f6-129">Name</span><span class="sxs-lookup"><span data-stu-id="0f6f6-129">Name</span></span>       | <span data-ttu-id="0f6f6-130">Typ</span><span class="sxs-lookup"><span data-stu-id="0f6f6-130">Type</span></span> | <span data-ttu-id="0f6f6-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f6f6-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0f6f6-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f6f6-132">Authorization</span></span>  | <span data-ttu-id="0f6f6-133">String</span><span class="sxs-lookup"><span data-stu-id="0f6f6-133">string</span></span>  | <span data-ttu-id="0f6f6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0f6f6-136">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="0f6f6-136">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="0f6f6-137">string</span><span class="sxs-lookup"><span data-stu-id="0f6f6-137">string</span></span> | <span data-ttu-id="0f6f6-138">Das Format, in der die **body**- und **uniqueBody**-Eigenschaften zurückgegeben werden sollen.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-138">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="0f6f6-139">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-139">Values can be "text" or "html".</span></span> <span data-ttu-id="0f6f6-140">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-140">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="0f6f6-141">Wenn die Kopfzeile nicht angegeben ist, werden die **body**- und **uniqueBody**-Eigenschaften im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-141">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="0f6f6-142">Optional.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f6f6-143">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0f6f6-143">Request body</span></span>
<span data-ttu-id="0f6f6-144">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f6f6-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f6f6-145">Response</span></span>

<span data-ttu-id="0f6f6-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-146">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0f6f6-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f6f6-147">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="0f6f6-148">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="0f6f6-148">Request 1</span></span>
<span data-ttu-id="0f6f6-149">Im erste Beispiel ruft die angegebenen Nachricht ab.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-149">The first example gets the specified message.</span></span> <span data-ttu-id="0f6f6-150">Es gibt keine Header, um das gewünschte Format des Textkörpers zurückzugebenden anzugeben.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-150">It does not specify any header to indicate the desired format of the body to be returned.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGI1AAAoZCfHAAA=')
```
##### <a name="response-1"></a><span data-ttu-id="0f6f6-151">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="0f6f6-151">Response 1</span></span>
<span data-ttu-id="0f6f6-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-152">Here is an example of the response.</span></span> <span data-ttu-id="0f6f6-153">Die Eigenschaften **Body** und **UniqueBody** werden in der Standard-HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-153">The **body** and **uniqueBody** properties are returned in the default HTML format.</span></span>
<span data-ttu-id="0f6f6-154">Hinweis: Das hier gezeigte Response-Objekt wird aus Platzgründen Zahl gekürzt.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-154">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="0f6f6-155">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-155">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 523

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
    "id":"AAMkAGI1AAAoZCfHAAA=",
    "subject":"Welcome to our group!",
    "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head></head><body><p>Welcome to our group, Dana! Hope you will enjoy working with us </p></body></html>\r\n"
    },
    "uniqueBody":{
        "contentType":"html",
        "content":"<html>\r\n<head></head><body><p>Welcome to our group, Dana! Hope you will enjoy working with us </p></body></html>\r\n"
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="0f6f6-156">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="0f6f6-156">Request 2</span></span>
<span data-ttu-id="0f6f6-157">Im nächsten Beispiel wird die angemeldeten Benutzers Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-157">In the next example, the signed-in user is Dana Swope.</span></span> <span data-ttu-id="0f6f6-158">Das Beispiel zeigt die Details der alle Vorkommnisse in der angegebenen Nachricht im Postfach des Dana abrufen.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-158">The example shows getting the details of all the mentions in the specified message in Dana's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADJmMTUAAAgVZAAAA"],
  "name": "get_mentions_in_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/('AQMkADJmMTUAAAgVZAAAA')?$expand=mentions
```
##### <a name="response-2"></a><span data-ttu-id="0f6f6-159">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="0f6f6-159">Response 2</span></span>
<span data-ttu-id="0f6f6-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2248

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages/$entity",
  "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')",
  "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAATI\"",
  "id":"AQMkADJmMTUAAAgVZAAAA",
  "subject":"Start planning soon",
  "body":{
    "contentType":"HTML",
    "content":"<html><head></head><body><p><a href=\"mailto:danas@contoso.onmicrosoft.com\">@Dana Swope</a>,<a href=\"mailto:randiw@contoso.onmicrosoft.com\">@Randi Welch</a>, forgot to mention, I will be away&nbsp;this weekend. I can start on Monday though.</p></body></html>"
  },
  "bodyPreview":"@Dana Swope<mailto:danas@contoso.onmicrosoft.com>, @Randi Welch, forgot to mention, I will be away this weekend. I can start on Monday though.",
  "sender":{
    "emailAddress":{
      "name":"Samantha Booth",
      "address":"samanthab@contoso.onmicrosoft.com"
    }
  },
  "from":{
    "emailAddress":{
      "name":"Samantha Booth",
      "address":"samanthab@contoso.onmicrosoft.com"
    }
  },
  "toRecipients":[
    {
      "emailAddress":{
        "name":"Dana Swope",
        "address":"danas@contoso.onmicrosoft.com"
      }
    },
    {
      "emailAddress":{
        "name":"Randi Welch",
        "address":"randiw@contoso.onmicrosoft.com"
      }
    }
  ],
  "ccRecipients":[
  ],
  "bccRecipients":[
  ],
  "mentionsPreview":{
    "isMentioned":true
  },
  "mentions@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages('AQMkADJmMTUAAAgVZAAAA')/mentions",
  "mentions":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')/mentions('138f4c0a-1130-4776-b780-bf79d73abb3f')",
      "id":"138f4c0a-1130-4776-b780-bf79d73abb3f",
      "mentioned":{
        "name":"Dana Swope",
        "address":"danas@contoso.onmicrosoft.com"
      },
      "mentionText":null,
      "clientReference":null,
      "createdBy":{
        "name":"Samantha Booth",
        "address":"samanthab@contoso.onmicrosoft.com"
      },
      "createdDateTime":"2016-07-21T07:40:20.152Z",
      "serverCreatedDateTime":"2016-07-21T07:40:20.152Z",
      "deepLink":null,
      "application":null
    },
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')/mentions('7b94df1a-0086-482a-b0da-e62fae12f983')",
      "id":"7b94df1a-0086-482a-b0da-e62fae12f983",
      "mentioned":{
        "name":"Randi Welch",
        "address":"randiw@contoso.onmicrosoft.com"
      },
      "mentionText":null,
      "clientReference":null,
      "createdBy":{
        "name":"Samantha Booth",
        "address":"samanthab@contoso.onmicrosoft.com"
      },
      "createdDateTime":"2016-07-21T07:40:20.158Z",
      "serverCreatedDateTime":"2016-07-21T07:40:20.158Z",
      "deepLink":null,
      "application":null
    }
  ]
}
```


##### <a name="request-3"></a><span data-ttu-id="0f6f6-163">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="0f6f6-163">Request 3</span></span>

<span data-ttu-id="0f6f6-164">Im dritten Beispiel wird gezeigt, wie mit einem `Prefer: outlook.body-content-type="text"` Header, um den **Text** und den **UniqueBody** der angegebenen Nachricht im Textformat erhalten möchten.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-164">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGI1AAAoZCfHAAA=')?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```

##### <a name="response-3"></a><span data-ttu-id="0f6f6-165">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="0f6f6-165">Response 3</span></span>

<span data-ttu-id="0f6f6-166">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-166">Here is an example of the response.</span></span> <span data-ttu-id="0f6f6-167">Hinweis: Die Antwort enthält eine `Preference-Applied: outlook.body-content-type` Header Bestätigen der `Prefer: outlook.body-content-type` Anforderungsheader.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-167">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"
Content-length: 1550

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)/$entity",
    "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
    "id":"AAMkAGI1AAAoZCfHAAA=",
    "subject":"Welcome to our group!",
    "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nTh",
    "body":{
        "contentType":"text",
        "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nThanks!\r\n\r\n"
    },
    "uniqueBody":{
        "contentType":"text",
        "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\nThanks!\r\n"
    }
}
```

##### <a name="request-4"></a><span data-ttu-id="0f6f6-168">Anforderung 4</span><span class="sxs-lookup"><span data-stu-id="0f6f6-168">Request 4</span></span>

<span data-ttu-id="0f6f6-169">Im vierte Beispiel veranschaulicht das Internetkopfzeilen Nachricht einer bestimmten Nachricht erhalten möchten.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-169">The fourth example shows how to get the Internet message headers of a specific message.</span></span>  

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEz"],
  "name": "get_message_internet_headers"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGVmMDEz')?$select=internetMessageHeaders
```

##### <a name="response-4"></a><span data-ttu-id="0f6f6-170">Antwort 4</span><span class="sxs-lookup"><span data-stu-id="0f6f6-170">Response 4</span></span>

<span data-ttu-id="0f6f6-171">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-171">Here is an example of the response.</span></span> <span data-ttu-id="0f6f6-172">Hinweis: Die Anzahl der Internet Nachrichtenköpfe in das Antwortobjekt wurde der Kürze halber reduziert.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-172">Note: The number of Internet message headers in the response object has been reduced for brevity.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('48d31887-5fad-4d73-a9f5-3c356e68a038')/messages(internetMessageHeaders)/$entity",
  "@odata.type":"#microsoft.graph.eventMessageRequest",
  "@odata.etag":"W/\"CwAAABYAAAAiIsqMbYjsT5e/T7KzowPTAAAa/qUB\"",
  "id":"AAMkAGVmMDEz",
  "internetMessageHeaders":[
    {
      "name":"Content-Type",
      "value":"application/ms-tnef"
    },
    {
      "name":"Content-Transfer-Encoding",
      "value":"binary"
    },
    {
      "name":"Subject",
      "value":"Cloud and Mobile Working Group"
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

## <a name="see-also"></a><span data-ttu-id="0f6f6-173">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="0f6f6-173">See also</span></span>

- [<span data-ttu-id="0f6f6-174">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="0f6f6-174">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0f6f6-175">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="0f6f6-175">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="0f6f6-176">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="0f6f6-176">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
