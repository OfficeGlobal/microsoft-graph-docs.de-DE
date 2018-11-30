---
title: 'Benutzer: GetMailTips'
description: Rufen Sie die e-Mail-Infos für einen oder mehrere Empfänger als verfügbar für dem angemeldeten Benutzer.
ms.openlocfilehash: 2c439e5a2da2c5208157f11b2623107d511cdf44
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063494"
---
# <a name="user-getmailtips"></a><span data-ttu-id="6add9-103">Benutzer: GetMailTips</span><span class="sxs-lookup"><span data-stu-id="6add9-103">user: getMailTips</span></span>

> <span data-ttu-id="6add9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6add9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6add9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6add9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6add9-106">Rufen Sie die e-Mail-Infos für einen oder mehrere Empfänger als dem angemeldeten [Benutzer](../resources/user.md)zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="6add9-106">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="6add9-107">Beachten Sie, dass durch Erstellen einer `POST` aufrufen, um die `getMailTips` -Aktion können Sie bestimmte Typen von e-Mail-Infos für mehrere Empfänger gleichzeitig zurückgegeben werden soll anfordern.</span><span class="sxs-lookup"><span data-stu-id="6add9-107">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="6add9-108">Der angeforderte e-Mail-Infos werden in einer [e-Mail-Infos](../resources/mailtips.md) -Auflistung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6add9-108">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="6add9-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6add9-109">Permissions</span></span>
<span data-ttu-id="6add9-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6add9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6add9-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6add9-112">Permission type</span></span>      | <span data-ttu-id="6add9-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6add9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6add9-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6add9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6add9-115">Mail.Read Mail.Read.Shared</span><span class="sxs-lookup"><span data-stu-id="6add9-115">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="6add9-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6add9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6add9-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6add9-117">Mail.Read</span></span>    |
|<span data-ttu-id="6add9-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6add9-118">Application</span></span> | <span data-ttu-id="6add9-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6add9-119">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="6add9-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6add9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6add9-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6add9-121">Optional query parameters</span></span>
<span data-ttu-id="6add9-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6add9-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6add9-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6add9-123">Request headers</span></span>
| <span data-ttu-id="6add9-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6add9-124">Header</span></span>       | <span data-ttu-id="6add9-125">Wert</span><span class="sxs-lookup"><span data-stu-id="6add9-125">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="6add9-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6add9-126">Authorization</span></span> | <span data-ttu-id="6add9-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6add9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6add9-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6add9-129">Content-Type</span></span>  | <span data-ttu-id="6add9-130">application/json</span><span class="sxs-lookup"><span data-stu-id="6add9-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6add9-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6add9-131">Request body</span></span>
<span data-ttu-id="6add9-132">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="6add9-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6add9-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6add9-133">Property</span></span>     | <span data-ttu-id="6add9-134">Typ</span><span class="sxs-lookup"><span data-stu-id="6add9-134">Type</span></span>   |<span data-ttu-id="6add9-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6add9-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6add9-136">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="6add9-136">EmailAddresses</span></span>|<span data-ttu-id="6add9-137">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="6add9-137">String collection</span></span>|<span data-ttu-id="6add9-138">Eine Auflistung von SMTP-Adressen der Empfänger für e-Mail-Infos zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="6add9-138">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="6add9-139">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="6add9-139">MailTipsOptions</span></span>|<span data-ttu-id="6add9-140">String</span><span class="sxs-lookup"><span data-stu-id="6add9-140">String</span></span>|<span data-ttu-id="6add9-141">Eine Flags-Enumeration, die die angeforderten e-Mail-Infos darstellt.</span><span class="sxs-lookup"><span data-stu-id="6add9-141">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="6add9-142">Mögliche Werte sind: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, und `totalMemberCount`.</span><span class="sxs-lookup"><span data-stu-id="6add9-142">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="6add9-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="6add9-143">Response</span></span>

<span data-ttu-id="6add9-144">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [e-Mail-Infos](../resources/mailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="6add9-144">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6add9-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6add9-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6add9-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6add9-146">Request</span></span>
<span data-ttu-id="6add9-147">Im folgenden Beispiel wird die e-Mail-Infos für die angegebenen Empfänger, für alle Einstellungen für automatische Antworten und den vollständigen Postfach-Status.</span><span class="sxs-lookup"><span data-stu-id="6add9-147">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmailtips"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMailTips
Content-Type: application/json

{
    "EmailAddresses": [
        "danas@contoso.onmicrosoft.com", 
        "fannyd@contoso.onmicrosoft.com"
    ],
    "MailTipsOptions": "automaticReplies, mailboxFullStatus"
}
```

##### <a name="response"></a><span data-ttu-id="6add9-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="6add9-148">Response</span></span>
<span data-ttu-id="6add9-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6add9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailTips",
  isCollection: true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailTips)",
    "value":[
        {
            "emailAddress":{
                "name":"",
                "address":"danas@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":"<style type=\"text/css\" style=\"\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n<div dir=\"ltr\">\r\n<div id=\"x_divtagdefaultwrapper\" style=\"font-size:12pt; color:#000000; background-color:#FFFFFF; font-family:Calibri,Arial,Helvetica,sans-serif\">\r\n<p>Hi, I am on vacation right now. I'll get back to you after I return.<br>\r\n</p>\r\n</div>\r\n</div>",
                "messageLanguage":{
                    "locale":"en-US",
                    "displayName":"English (United States)"
                },
                "scheduledStartTime": {
                    "dateTime": "2018-08-07T02:00:00.0000000",
                    "timeZone": "UTC"
                },
                "scheduledEndTime": {
                    "dateTime": "2018-08-09T02:00:00.0000000",
                    "timeZone": "UTC"
                }
            },
            "mailboxFull":false
        },
        {
            "emailAddress":{
                "name":"",
                "address":"fannyd@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":""
            },
            "mailboxFull":false
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
