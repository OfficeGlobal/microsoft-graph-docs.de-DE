---
title: 'Benutzer: GetMailTips'
description: Rufen Sie die e-Mail-Infos für einen oder mehrere Empfänger als verfügbar für dem angemeldeten Benutzer.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e3397bade518cde6e17759096601f364f84e918e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516140"
---
# <a name="user-getmailtips"></a><span data-ttu-id="057d3-103">Benutzer: GetMailTips</span><span class="sxs-lookup"><span data-stu-id="057d3-103">user: getMailTips</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="057d3-104">Rufen Sie die e-Mail-Infos für einen oder mehrere Empfänger als dem angemeldeten [Benutzer](../resources/user.md)zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="057d3-104">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="057d3-105">Beachten Sie, dass durch Erstellen einer `POST` aufrufen, um die `getMailTips` -Aktion können Sie bestimmte Typen von e-Mail-Infos für mehrere Empfänger gleichzeitig zurückgegeben werden soll anfordern.</span><span class="sxs-lookup"><span data-stu-id="057d3-105">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="057d3-106">Der angeforderte e-Mail-Infos werden in einer [e-Mail-Infos](../resources/mailtips.md) -Auflistung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="057d3-106">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="057d3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="057d3-107">Permissions</span></span>
<span data-ttu-id="057d3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="057d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="057d3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="057d3-110">Permission type</span></span>      | <span data-ttu-id="057d3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="057d3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="057d3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="057d3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="057d3-113">Mail.Read Mail.Read.Shared</span><span class="sxs-lookup"><span data-stu-id="057d3-113">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="057d3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="057d3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="057d3-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="057d3-115">Mail.Read</span></span>    |
|<span data-ttu-id="057d3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="057d3-116">Application</span></span> | <span data-ttu-id="057d3-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="057d3-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="057d3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="057d3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="057d3-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="057d3-119">Optional query parameters</span></span>
<span data-ttu-id="057d3-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="057d3-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="057d3-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="057d3-121">Request headers</span></span>
| <span data-ttu-id="057d3-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="057d3-122">Header</span></span>       | <span data-ttu-id="057d3-123">Wert</span><span class="sxs-lookup"><span data-stu-id="057d3-123">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="057d3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="057d3-124">Authorization</span></span> | <span data-ttu-id="057d3-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="057d3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="057d3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="057d3-127">Content-Type</span></span>  | <span data-ttu-id="057d3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="057d3-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="057d3-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="057d3-129">Request body</span></span>
<span data-ttu-id="057d3-130">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="057d3-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="057d3-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="057d3-131">Property</span></span>     | <span data-ttu-id="057d3-132">Typ</span><span class="sxs-lookup"><span data-stu-id="057d3-132">Type</span></span>   |<span data-ttu-id="057d3-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="057d3-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="057d3-134">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="057d3-134">EmailAddresses</span></span>|<span data-ttu-id="057d3-135">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="057d3-135">String collection</span></span>|<span data-ttu-id="057d3-136">Eine Auflistung von SMTP-Adressen der Empfänger für e-Mail-Infos zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="057d3-136">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="057d3-137">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="057d3-137">MailTipsOptions</span></span>|<span data-ttu-id="057d3-138">String</span><span class="sxs-lookup"><span data-stu-id="057d3-138">String</span></span>|<span data-ttu-id="057d3-139">Eine Flags-Enumeration, die die angeforderten e-Mail-Infos darstellt.</span><span class="sxs-lookup"><span data-stu-id="057d3-139">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="057d3-140">Mögliche Werte sind: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, und `totalMemberCount`.</span><span class="sxs-lookup"><span data-stu-id="057d3-140">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="057d3-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="057d3-141">Response</span></span>

<span data-ttu-id="057d3-142">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [e-Mail-Infos](../resources/mailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="057d3-142">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="057d3-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="057d3-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="057d3-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="057d3-144">Request</span></span>
<span data-ttu-id="057d3-145">Im folgenden Beispiel wird die e-Mail-Infos für die angegebenen Empfänger, für alle Einstellungen für automatische Antworten und den vollständigen Postfach-Status.</span><span class="sxs-lookup"><span data-stu-id="057d3-145">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>

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

##### <a name="response"></a><span data-ttu-id="057d3-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="057d3-146">Response</span></span>
<span data-ttu-id="057d3-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="057d3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-getmailtips.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
