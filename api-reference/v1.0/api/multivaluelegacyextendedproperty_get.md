# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="6347e-101">Get multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="6347e-101">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="6347e-102">Dient zum Abrufen einer Ressourceninstanz mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="6347e-102">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="6347e-103">Mit dem Abfrageparameter `$expand` können Sie die angegebene Instanz abrufen, erweitert um die angegebene erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="6347e-103">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="6347e-104">Dies ist derzeit die einzige Möglichkeit zum Abrufen des [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md)-Objekts, das eine erweiterte Eigenschaft darstellt.</span><span class="sxs-lookup"><span data-stu-id="6347e-104">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="6347e-105">Die folgenden Benutzerressourcen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="6347e-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="6347e-106">calendar</span><span class="sxs-lookup"><span data-stu-id="6347e-106">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="6347e-107">contact</span><span class="sxs-lookup"><span data-stu-id="6347e-107">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="6347e-108">contactFolder</span><span class="sxs-lookup"><span data-stu-id="6347e-108">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="6347e-109">Ereignis</span><span class="sxs-lookup"><span data-stu-id="6347e-109">event</span></span>](../resources/event.md)
- [<span data-ttu-id="6347e-110">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6347e-110">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="6347e-111">Nachricht</span><span class="sxs-lookup"><span data-stu-id="6347e-111">message</span></span>](../resources/message.md) 

<span data-ttu-id="6347e-112">Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="6347e-112">As well as the following group resources:</span></span>

- <span data-ttu-id="6347e-113">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="6347e-113">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="6347e-114">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="6347e-114">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="6347e-115">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="6347e-115">group [post](../resources/post.md)</span></span>

<span data-ttu-id="6347e-116">Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="6347e-116">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="6347e-117">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6347e-117">Permissions</span></span>
<span data-ttu-id="6347e-118">Je nach der Ressource kommen die erweiterte Eigenschaft aus und geben Sie die Berechtigung (delegierte oder-Anwendung) Sie Anforderung, die Berechtigung, die in der folgenden Tabelle angegeben ist mindestens erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="6347e-118">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="6347e-119">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6347e-119">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="6347e-120">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="6347e-120">Supported resource</span></span> | <span data-ttu-id="6347e-121">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6347e-121">Delegated (work or school account)</span></span> | <span data-ttu-id="6347e-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6347e-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6347e-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6347e-123">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="6347e-124">Kalender</span><span class="sxs-lookup"><span data-stu-id="6347e-124">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="6347e-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-125">Calendars.Read</span></span> | <span data-ttu-id="6347e-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-126">Calendars.Read</span></span> | <span data-ttu-id="6347e-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-127">Calendars.Read</span></span> |
| [<span data-ttu-id="6347e-128">Kontakt</span><span class="sxs-lookup"><span data-stu-id="6347e-128">contact</span></span>](../resources/contact.md) | <span data-ttu-id="6347e-129">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-129">Contacts.Read</span></span> | <span data-ttu-id="6347e-130">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-130">Contacts.Read</span></span> | <span data-ttu-id="6347e-131">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-131">Contacts.Read</span></span> |
| [<span data-ttu-id="6347e-132">contactFolder</span><span class="sxs-lookup"><span data-stu-id="6347e-132">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="6347e-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-133">Contacts.Read</span></span> | <span data-ttu-id="6347e-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-134">Contacts.Read</span></span> | <span data-ttu-id="6347e-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-135">Contacts.Read</span></span> |
| [<span data-ttu-id="6347e-136">Ereignis</span><span class="sxs-lookup"><span data-stu-id="6347e-136">event</span></span>](../resources/event.md) | <span data-ttu-id="6347e-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-137">Calendars.Read</span></span> | <span data-ttu-id="6347e-138">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-138">Calendars.Read</span></span> |  <span data-ttu-id="6347e-139">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-139">Calendars.Read</span></span>|
| <span data-ttu-id="6347e-140">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="6347e-140">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="6347e-141">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6347e-141">Group.Read.All</span></span> | <span data-ttu-id="6347e-142">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6347e-142">Not supported</span></span> | <span data-ttu-id="6347e-143">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6347e-143">Not supported</span></span> |
| <span data-ttu-id="6347e-144">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="6347e-144">group [event](../resources/event.md)</span></span> | <span data-ttu-id="6347e-145">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6347e-145">Group.Read.All</span></span> | <span data-ttu-id="6347e-146">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6347e-146">Not supported</span></span> | <span data-ttu-id="6347e-147">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6347e-147">Not supported</span></span> |
| <span data-ttu-id="6347e-148">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="6347e-148">group [post](../resources/post.md)</span></span> | <span data-ttu-id="6347e-149">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6347e-149">Group.Read.All</span></span> | <span data-ttu-id="6347e-150">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6347e-150">Not supported</span></span> | <span data-ttu-id="6347e-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6347e-151">Group.Read.All</span></span> |
| [<span data-ttu-id="6347e-152">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6347e-152">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="6347e-153">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-153">Mail.Read</span></span> | <span data-ttu-id="6347e-154">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-154">Mail.Read</span></span> | <span data-ttu-id="6347e-155">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-155">Mail.Read</span></span> |
| [<span data-ttu-id="6347e-156">Nachricht</span><span class="sxs-lookup"><span data-stu-id="6347e-156">message</span></span>](../resources/message.md) | <span data-ttu-id="6347e-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-157">Mail.Read</span></span> | <span data-ttu-id="6347e-158">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-158">Mail.Read</span></span> | <span data-ttu-id="6347e-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6347e-159">Mail.Read</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="6347e-160">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6347e-160">HTTP request</span></span>

<span data-ttu-id="6347e-p103">Rufen Sie eine erweiterte Ressourceninstanz mit erweiterter Eigenschaft ab, die einem Filter für die **id**-Eigenschaft entspricht. Stellen Sie sicher, dass Sie die [URL-Codierung](https://www.w3schools.com/tags/ref_urlencode.asp) auf die Leerzeichen in der Filterzeichenfolge anwenden.</span><span class="sxs-lookup"><span data-stu-id="6347e-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="6347e-163">Erhalten Sie eine Instanz der **Nachricht** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6347e-163">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="6347e-164">Eine **MailFolder** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6347e-164">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="6347e-165">Rufen Sie eine Instanz **Ereignis** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6347e-165">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="6347e-166">Eine **Kalender** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6347e-166">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="6347e-167">Abrufen einer Instanz **wenden Sie sich an** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6347e-167">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="6347e-168">Eine **ContactFolder** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6347e-168">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="6347e-169">Eine Gruppe **Ereignis** Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6347e-169">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="6347e-170">Eine Gruppe **Buchen** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6347e-170">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="6347e-171">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="6347e-171">Path parameters</span></span>
|<span data-ttu-id="6347e-172">Parameter</span><span class="sxs-lookup"><span data-stu-id="6347e-172">Parameter</span></span>|<span data-ttu-id="6347e-173">Typ</span><span class="sxs-lookup"><span data-stu-id="6347e-173">Type</span></span>|<span data-ttu-id="6347e-174">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6347e-174">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6347e-175">id_value</span><span class="sxs-lookup"><span data-stu-id="6347e-175">id_value</span></span>|<span data-ttu-id="6347e-176">String</span><span class="sxs-lookup"><span data-stu-id="6347e-176">String</span></span>|<span data-ttu-id="6347e-p104">Die ID der erweiterten übereinstimmenden Eigenschaft. Sie muss eins der unterstützten Formate aufweisen. Weitere Informationen finden Sie unter [Überblick über erweiterte Eigenschaften in Outlook](../resources/extended-properties-overview.md). Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6347e-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="6347e-181">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6347e-181">Request headers</span></span>
| <span data-ttu-id="6347e-182">Name</span><span class="sxs-lookup"><span data-stu-id="6347e-182">Name</span></span>      |<span data-ttu-id="6347e-183">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6347e-183">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6347e-184">Authorization</span><span class="sxs-lookup"><span data-stu-id="6347e-184">Authorization</span></span>  | <span data-ttu-id="6347e-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6347e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6347e-187">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6347e-187">Request body</span></span>
<span data-ttu-id="6347e-188">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6347e-188">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6347e-189">Antwort</span><span class="sxs-lookup"><span data-stu-id="6347e-189">Response</span></span>

<span data-ttu-id="6347e-190">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6347e-190">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="6347e-191">Der Antworttext enthält ein Objekt, das die angeforderte Ressourceninstanz darstellt, und das übereinstimmende [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="6347e-191">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="6347e-192">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6347e-192">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6347e-193">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6347e-193">Request</span></span>
<span data-ttu-id="6347e-p106">In diesem Beispiel wird das angegebene Ereignis abgerufen und um eine erweiterte mehrwertige Eigenschaften erwetiert. Der Filter gibt die erweiterte Eigenschaft mit der **ID** an, die mit der Zeichenfolge `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` übereinstimmt (URL-Codierung wurde zur besseren Lesbarkeit in diesem Beispiel entfernt).</span><span class="sxs-lookup"><span data-stu-id="6347e-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="6347e-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="6347e-196">Response</span></span>

<span data-ttu-id="6347e-197">Der Antworttext enthält alle Eigenschaften des angegebenen Ereignisses und erweiterte Eigenschaften, die von dem Filter zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="6347e-197">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="6347e-p107">Hinweis: Das hier gezeigte **event**-Objekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6347e-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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