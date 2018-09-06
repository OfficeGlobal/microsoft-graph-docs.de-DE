# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="366ba-101">Get multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="366ba-101">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="366ba-102">Dient zum Abrufen einer Ressourceninstanz mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="366ba-102">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="366ba-103">Mit dem Abfrageparameter `$expand` können Sie die angegebene Instanz abrufen, erweitert um die angegebene erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="366ba-103">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="366ba-104">Dies ist derzeit die einzige Möglichkeit zum Abrufen des [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md)-Objekts, das eine erweiterte Eigenschaft darstellt.</span><span class="sxs-lookup"><span data-stu-id="366ba-104">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="366ba-105">Die folgenden Benutzerressourcen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="366ba-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="366ba-106">message</span><span class="sxs-lookup"><span data-stu-id="366ba-106">message</span></span>](../resources/message.md)
- [<span data-ttu-id="366ba-107">mailFolder</span><span class="sxs-lookup"><span data-stu-id="366ba-107">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="366ba-108">event</span><span class="sxs-lookup"><span data-stu-id="366ba-108">event</span></span>](../resources/event.md)
- [<span data-ttu-id="366ba-109">calendar</span><span class="sxs-lookup"><span data-stu-id="366ba-109">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="366ba-110">contakt</span><span class="sxs-lookup"><span data-stu-id="366ba-110">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="366ba-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="366ba-111">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="366ba-112">Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="366ba-112">As well as the following group resources:</span></span>

- <span data-ttu-id="366ba-113">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="366ba-113">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="366ba-114">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="366ba-114">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="366ba-115">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="366ba-115">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="366ba-116">Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="366ba-116">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="366ba-117">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="366ba-117">Permissions</span></span>
<span data-ttu-id="366ba-p102">Zum Aufrufen dieser API ist eine der folgenden Berechtigungen erforderlich (je nachdem, welche Ressource Sie abrufen möchten): Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="366ba-p102">One of the following permissions is required to call this API, depending on the resource you're getting. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="366ba-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="366ba-120">Mail.Read</span></span>
- <span data-ttu-id="366ba-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="366ba-121">Calendars.Read</span></span>
- <span data-ttu-id="366ba-122">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="366ba-122">Contacts.Read</span></span>
- <span data-ttu-id="366ba-123">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="366ba-123">Group.Read.All</span></span> 
 
## <a name="http-request"></a><span data-ttu-id="366ba-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="366ba-124">HTTP request</span></span>

<span data-ttu-id="366ba-p103">Hier sehen Sie, wie Sie eine Ressourceninstanz abrufen können, erweitert um die erweiterte Eigenschaft, deren **id**-Eigenschaft dem definierten Filter entspricht. Stellen Sie sicher, dass Sie für die Leerzeichen in der Filterzeichenfolge die [URL-Codierung](http://www.w3schools.com/tags/ref_urlencode.asp) verwenden.</span><span class="sxs-lookup"><span data-stu-id="366ba-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="366ba-127">Abrufen einer **message**-Instanz: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="366ba-127">Get a **message** instance:</span></span>
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="366ba-128">Abrufen einer **mailFolder**-Instanz: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="366ba-128">Get a **mailFolder** instance:</span></span>
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="366ba-129">Abrufen einer **event**-Instanz <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="366ba-129">Get an **event** instance:</span></span>
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="366ba-130">Abrufen einer **calendar**-Instanz: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="366ba-130">Get a **calendar** instance:</span></span>
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="366ba-131">Abrufen einer **contakt**-Instanz: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="366ba-131">Get a **contact** instance:</span></span>
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="366ba-132">Abrufen einer **contactFolder**-Instanz: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="366ba-132">Get a **contactFolder** instance:</span></span>
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="366ba-133">Abrufen einer **event**-Instanz für eine Gruppe: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="366ba-133">Get a group **event** instance:</span></span>
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="366ba-134">Abrufen einer **post**-Instanz für eine Gruppe: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="366ba-134">Get a group **post** instance:</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="366ba-135">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="366ba-135">Path parameters</span></span>
|<span data-ttu-id="366ba-136">Parameter</span><span class="sxs-lookup"><span data-stu-id="366ba-136">Parameter</span></span>|<span data-ttu-id="366ba-137">Typ</span><span class="sxs-lookup"><span data-stu-id="366ba-137">Type</span></span>|<span data-ttu-id="366ba-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="366ba-138">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="366ba-139">id_value</span><span class="sxs-lookup"><span data-stu-id="366ba-139">id_value</span></span>|<span data-ttu-id="366ba-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="366ba-140">String</span></span>|<span data-ttu-id="366ba-p104">Die ID der erweiterten Eigenschaft, nach der gefiltert wird. Sie muss eins der unterstützten Formate aufweisen. Weitere Informationen finden Sie unter [Überblick über erweiterte Eigenschaften in Outlook](../resources/extended-properties-overview.md). Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="366ba-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="366ba-145">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="366ba-145">Request headers</span></span>
| <span data-ttu-id="366ba-146">Name</span><span class="sxs-lookup"><span data-stu-id="366ba-146">Name</span></span>      |<span data-ttu-id="366ba-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="366ba-147">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="366ba-148">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="366ba-148">Authorization</span></span>  | <span data-ttu-id="366ba-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="366ba-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="366ba-151">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="366ba-151">Request body</span></span>
<span data-ttu-id="366ba-152">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="366ba-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="366ba-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="366ba-153">Response</span></span>

<span data-ttu-id="366ba-154">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="366ba-154">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="366ba-155">Der Antworttext enthält ein Objekt, das die angeforderte Ressourceninstanz darstellt, und das übereinstimmende [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="366ba-155">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="366ba-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="366ba-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="366ba-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="366ba-157">Request</span></span>
<span data-ttu-id="366ba-p106">In diesem Beispiel wird das angegebene Ereignis abgerufen und um eine erweiterte mehrwertige Eigenschaften erwetiert. Der Filter gibt die erweiterte Eigenschaft mit der **ID** an, die mit der Zeichenfolge `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` übereinstimmt (URL-Codierung wurde zur besseren Lesbarkeit in diesem Beispiel entfernt).</span><span class="sxs-lookup"><span data-stu-id="366ba-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="366ba-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="366ba-160">Response</span></span>

<span data-ttu-id="366ba-161">Der Antworttext enthält alle Eigenschaften des angegebenen Ereignisses und erweiterte Eigenschaften, die von dem Filter zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="366ba-161">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="366ba-p107">Hinweis: Das hier gezeigte **event**-Objekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="366ba-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
    "@odata.etag": "W/\"mODEKWhc/Um6lA3uPm7PPAAAm8k15A==\"",
    "id": "AAMkAGE1M2_bs88AACbuFiiAAA=",
    "start": {
        "dateTime": "2015-11-26T17:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2015-11-30T05:00:00.0000000",
        "timeZone": "UTC"
    },
    "organizer": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
    "multiValueExtendedProperties": [
        {
            "id": "StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
            "value": [
                "Food",
                "Hiking",
                "Swimming"
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->