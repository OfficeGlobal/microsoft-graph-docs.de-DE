# <a name="user-getmailtips"></a><span data-ttu-id="2fe87-101">user: getMailTips</span><span class="sxs-lookup"><span data-stu-id="2fe87-101">user: getMailTips</span></span>

<span data-ttu-id="2fe87-102">Rufen Sie die E-Mail-Info für einen oder mehrere Empfänger als verfügbar für den angemeldeten [Benutzer](../resources/user.md)  ab.</span><span class="sxs-lookup"><span data-stu-id="2fe87-102">Return the MailTips of one or more recipients as available to the signed-in user.</span></span>

<span data-ttu-id="2fe87-103">Beachten Sie, dass Sie durch `POST` Aufruf der `getMailTips` Aktion bestimmte Typen von E-Mail-Infos anfordern können, dass diese für mehrere Empfänger gleichzeitig zurückgegeben werden sollen.</span><span class="sxs-lookup"><span data-stu-id="2fe87-103">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="2fe87-104">Die angeforderten E-Mail-Infos werden in einer [mailTips](../resources/mailtips.md) -Sammlung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2fe87-104">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fe87-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2fe87-105">Permissions</span></span>
<span data-ttu-id="2fe87-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2fe87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2fe87-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2fe87-108">Permission type</span></span>      | <span data-ttu-id="2fe87-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2fe87-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fe87-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2fe87-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2fe87-111">Mail.Read, Mail.Read.Shared</span><span class="sxs-lookup"><span data-stu-id="2fe87-111">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="2fe87-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2fe87-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fe87-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2fe87-113">Mail.Read</span></span>    |
|<span data-ttu-id="2fe87-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2fe87-114">Application</span></span> | <span data-ttu-id="2fe87-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2fe87-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fe87-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2fe87-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2fe87-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2fe87-117">Optional query parameters</span></span>
<span data-ttu-id="2fe87-118">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2fe87-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2fe87-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2fe87-119">Request headers</span></span>
| <span data-ttu-id="2fe87-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2fe87-120">Header</span></span>       | <span data-ttu-id="2fe87-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2fe87-121">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="2fe87-122">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2fe87-122">Authorization</span></span> | <span data-ttu-id="2fe87-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2fe87-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2fe87-125">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="2fe87-125">Content-Type</span></span>  | <span data-ttu-id="2fe87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2fe87-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2fe87-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2fe87-127">Request body</span></span>
<span data-ttu-id="2fe87-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="2fe87-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2fe87-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2fe87-129">Property</span></span>     | <span data-ttu-id="2fe87-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2fe87-130">Type</span></span>   |<span data-ttu-id="2fe87-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2fe87-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fe87-132">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="2fe87-132">EmailAddresses</span></span>|<span data-ttu-id="2fe87-133">Zeichenfolgesammlung</span><span class="sxs-lookup"><span data-stu-id="2fe87-133">String collection</span></span>|<span data-ttu-id="2fe87-134">Eine Sammlung von SMTP-Adressen von Empfängern, für die Sie E-Mail-Infos erhalten möchten.</span><span class="sxs-lookup"><span data-stu-id="2fe87-134">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="2fe87-135">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="2fe87-135">MailTipsOptions</span></span>|<span data-ttu-id="2fe87-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2fe87-136">String</span></span>|<span data-ttu-id="2fe87-137">Eine Enumeration von Kennzeichen, die die angeforderte E-Mail-Info repräsentiert.</span><span class="sxs-lookup"><span data-stu-id="2fe87-137">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="2fe87-138">Mögliche Werte sind: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, und `totalMemberCount`.</span><span class="sxs-lookup"><span data-stu-id="2fe87-138">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`,`mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="2fe87-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="2fe87-139">Response</span></span>

<span data-ttu-id="2fe87-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [mailTips](../resources/mailtips.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2fe87-140">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2fe87-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2fe87-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2fe87-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2fe87-142">Request</span></span>
<span data-ttu-id="2fe87-143">Das folgende Beispiel liefert E-Mail-Infos für die angegebenen Empfänger, für alle automatischen Antworteinstellungen und den Vollstatus des Postfachs.</span><span class="sxs-lookup"><span data-stu-id="2fe87-143">The following example gets MailTips for the specified recipients, for any automatic reply settings and mailbox full status.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmailtips"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMailTips
Content-Type: application/json

{
    "EmailAddresses": [
        "danas@contoso.onmicrosoft.com", 
        "fannyd@contoso.onmicrosoft.com"
    ],
    "MailTipsOptions": "automaticReplies, mailboxFullStatus"
}
```

##### <a name="response"></a><span data-ttu-id="2fe87-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="2fe87-144">Response</span></span>
<span data-ttu-id="2fe87-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2fe87-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.mailTips)",
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
