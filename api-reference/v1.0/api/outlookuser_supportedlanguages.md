# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="ba1d4-101">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="ba1d4-101">outlookUser: supportedLanguages</span></span>

<span data-ttu-id="ba1d4-102">Abrufen der Liste von Gebietsschemas und Sprachen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="ba1d4-102">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="ba1d4-103">Beim Einrichten eines Outlook-Clients wählt der Benutzer die bevorzugte Sprache aus dieser unterstützten Liste aus.</span><span class="sxs-lookup"><span data-stu-id="ba1d4-103">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="ba1d4-104">Sie können anschließend die bevorzugte Sprache abrufen, indem Sie [die Postfacheinstellungen des Benutzers abrufen](user_get_mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="ba1d4-104">You can subsequently get the preferred language by [getting the user's mailbox settings](user_get_mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="ba1d4-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ba1d4-105">Permissions</span></span>
<span data-ttu-id="ba1d4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ba1d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ba1d4-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ba1d4-108">Permission type</span></span>      | <span data-ttu-id="ba1d4-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ba1d4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba1d4-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ba1d4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ba1d4-111">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="ba1d4-111">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="ba1d4-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ba1d4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba1d4-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="ba1d4-113">User.Read</span></span>    |
|<span data-ttu-id="ba1d4-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ba1d4-114">Application</span></span> | <span data-ttu-id="ba1d4-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba1d4-115">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba1d4-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba1d4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="ba1d4-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ba1d4-117">Request headers</span></span>
| <span data-ttu-id="ba1d4-118">Name</span><span class="sxs-lookup"><span data-stu-id="ba1d4-118">Name</span></span>       | <span data-ttu-id="ba1d4-119">Typ</span><span class="sxs-lookup"><span data-stu-id="ba1d4-119">Type</span></span> | <span data-ttu-id="ba1d4-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ba1d4-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ba1d4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba1d4-121">Authorization</span></span>  | <span data-ttu-id="ba1d4-122">string</span><span class="sxs-lookup"><span data-stu-id="ba1d4-122">string</span></span>  | <span data-ttu-id="ba1d4-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ba1d4-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="ba1d4-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ba1d4-125">Request body</span></span>
<span data-ttu-id="ba1d4-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ba1d4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba1d4-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba1d4-127">Response</span></span>
<span data-ttu-id="ba1d4-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [localeInfo](../resources/localeinfo.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ba1d4-128">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba1d4-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ba1d4-129">Example</span></span>
<span data-ttu-id="ba1d4-130">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="ba1d4-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ba1d4-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba1d4-131">Request</span></span>
<span data-ttu-id="ba1d4-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ba1d4-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedLanguages
```

##### <a name="response"></a><span data-ttu-id="ba1d4-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba1d4-133">Response</span></span>
<span data-ttu-id="ba1d4-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ba1d4-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.localeInfo",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.localeInfo)",
  "value":[
    {
      "locale":"af-ZA",
      "displayName":"Afrikaans (Suid-Afrika)"
    },
    {
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    {
       "locale":"en-CA",
       "displayName":"English (Canada)"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedLanguages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->