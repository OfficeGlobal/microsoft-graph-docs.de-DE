# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="b38d7-101">singleValueLegacyExtendedProperty abrufen</span><span class="sxs-lookup"><span data-stu-id="b38d7-101">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="b38d7-102">In diesem Artikel erfahren Sie, wie Sie mithilfe von `$expand` oder `$filter` Ressourceninstanzen abrufen können, die eine einwertige erweiterte Eigenschaft enthalten.</span><span class="sxs-lookup"><span data-stu-id="b38d7-102">Get resource instances that contain a single-value extended property by using `$expand` or `$filter`.</span></span>

<span data-ttu-id="b38d7-p101">Mit dem Abfrageparameter `$expand` können Sie die angegebene Instanz abrufen, erweitert um die angegebene erweiterte Eigenschaft. Dies ist derzeit die einzige Möglichkeit zum Abrufen des [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md)-Objekts, das eine erweiterte Eigenschaft darstellt.</span><span class="sxs-lookup"><span data-stu-id="b38d7-p101">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property. This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="b38d7-p102">Mithilfe des Abfrageparameters `$filter` können Sie alle Instanzen der angegebenen Ressource abrufen, die eine erweiterte Eigenschaft haben, deren Eigenschaften **id** und **value** dem festgelegten Filter entsprechen. Der Filter wird auf alle Instanzen der Ressource angewendet, die im Postfach eines angemeldeten Benutzers existieren.</span><span class="sxs-lookup"><span data-stu-id="b38d7-p102">Using the query parameter `$filter` allows you to get all the instances of the specified resource that have an extended property matching a filter on the **id** and **value** properties. The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span>

<span data-ttu-id="b38d7-107">Die folgenden Benutzerressourcen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="b38d7-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="b38d7-108">message</span><span class="sxs-lookup"><span data-stu-id="b38d7-108">message</span></span>](../resources/message.md)
- [<span data-ttu-id="b38d7-109">mailFolder</span><span class="sxs-lookup"><span data-stu-id="b38d7-109">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="b38d7-110">event</span><span class="sxs-lookup"><span data-stu-id="b38d7-110">event</span></span>](../resources/event.md)
- [<span data-ttu-id="b38d7-111">calendar</span><span class="sxs-lookup"><span data-stu-id="b38d7-111">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="b38d7-112">contact</span><span class="sxs-lookup"><span data-stu-id="b38d7-112">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="b38d7-113">contactFolder</span><span class="sxs-lookup"><span data-stu-id="b38d7-113">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="b38d7-114">Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="b38d7-114">As well as the following group resources:</span></span>

- <span data-ttu-id="b38d7-115">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="b38d7-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="b38d7-116">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="b38d7-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="b38d7-117">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="b38d7-117">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="b38d7-118">Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="b38d7-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="b38d7-119">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b38d7-119">Permissions</span></span>
<span data-ttu-id="b38d7-p103">Zum Aufrufen dieser API ist eine der folgenden Berechtigungen erforderlich (je nachdem, welche Ressource Sie abrufen möchten): Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b38d7-p103">One of the following permissions is required to call this API, depending on the resource you're getting. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="b38d7-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b38d7-122">Mail.Read</span></span>
- <span data-ttu-id="b38d7-123">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b38d7-123">Calendars.Read</span></span>
- <span data-ttu-id="b38d7-124">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b38d7-124">Contacts.Read</span></span>
- <span data-ttu-id="b38d7-125">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b38d7-125">Group.Read.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="b38d7-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b38d7-126">HTTP request</span></span>

#### <a name="get-a-resource-instance-using-expand"></a><span data-ttu-id="b38d7-127">Abrufen einer Ressourceninstanz mithilfe von `$expand`</span><span class="sxs-lookup"><span data-stu-id="b38d7-127">GET a resource instance using `$expand`</span></span>
<span data-ttu-id="b38d7-p104">Hier sehen Sie, wie Sie eine Ressourceninstanz abrufen können, erweitert um die erweiterte Eigenschaft, deren **id**-Eigenschaft dem definierten Filter entspricht. Stellen Sie sicher, dass Sie für die Leerzeichen in der Filterzeichenfolge die [URL-Codierung](http://www.w3schools.com/tags/ref_urlencode.asp) verwenden.</span><span class="sxs-lookup"><span data-stu-id="b38d7-p104">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="b38d7-130">Abrufen einer **message**-Instanz:</span><span class="sxs-lookup"><span data-stu-id="b38d7-130">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="b38d7-131">Abrufen einer **mailFolder**-Instanz:</span><span class="sxs-lookup"><span data-stu-id="b38d7-131">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="b38d7-132">Abrufen einer **event**-Instanz</span><span class="sxs-lookup"><span data-stu-id="b38d7-132">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="b38d7-133">Abrufen einer **calendar**-Instanz:</span><span class="sxs-lookup"><span data-stu-id="b38d7-133">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="b38d7-134">Abrufen einer **contact**-Instanz:</span><span class="sxs-lookup"><span data-stu-id="b38d7-134">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="b38d7-135">Abrufen einer **contactFolder**-Instanz:</span><span class="sxs-lookup"><span data-stu-id="b38d7-135">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="b38d7-136">Abrufen einer **event**-Instanz für eine Gruppe:</span><span class="sxs-lookup"><span data-stu-id="b38d7-136">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="b38d7-137">Abrufen einer **post**-Instanz für eine Gruppe:</span><span class="sxs-lookup"><span data-stu-id="b38d7-137">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-using-filter"></a><span data-ttu-id="b38d7-138">Abrufen von Ressourceninstanzen mithilfe von `$filter`</span><span class="sxs-lookup"><span data-stu-id="b38d7-138">GET resource instances using `$filter`</span></span>

<span data-ttu-id="b38d7-p105">Hier sehen Sie, wie Sie alle Instanzen einer unterstützten Ressource abrufen, die eine erweiterte Eigenschaft haben, deren Eigenschaften **id** und **value** dem definierten Filter entsprechen. Stellen Sie sicher, dass Sie für die folgenden Zeichen in der Filterzeichenfolge die [URL-Codierung](http://www.w3schools.com/tags/ref_urlencode.asp) verwenden: Vorwärtsschrägstriche und Leerzeichen.</span><span class="sxs-lookup"><span data-stu-id="b38d7-p105">Get instances of a supported resource that have the extended property matching a filter on the **id** and **value** properties. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - forward slash and space.</span></span>


<span data-ttu-id="b38d7-141">Abrufen von **message**-Instanzen:</span><span class="sxs-lookup"><span data-stu-id="b38d7-141">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="b38d7-142">Abrufen von **mailFolder**-Instanzen:</span><span class="sxs-lookup"><span data-stu-id="b38d7-142">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="b38d7-143">Abrufen von **event**-Instanzen:</span><span class="sxs-lookup"><span data-stu-id="b38d7-143">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="b38d7-144">Abrufen von **calendar**-Instanzen:</span><span class="sxs-lookup"><span data-stu-id="b38d7-144">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="b38d7-145">Abrufen von **contact**-Instanzen:</span><span class="sxs-lookup"><span data-stu-id="b38d7-145">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="b38d7-146">Abrufen von **contactFolder**-Instanzen:</span><span class="sxs-lookup"><span data-stu-id="b38d7-146">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="b38d7-147">Abrufen von **event**-Instanzen für Gruppen:</span><span class="sxs-lookup"><span data-stu-id="b38d7-147">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="b38d7-148">Abrufen von **post**-Instanzen für Gruppen:</span><span class="sxs-lookup"><span data-stu-id="b38d7-148">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

## <a name="parameters"></a><span data-ttu-id="b38d7-149">Parameter</span><span class="sxs-lookup"><span data-stu-id="b38d7-149">Parameters</span></span>
|<span data-ttu-id="b38d7-150">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="b38d7-150">**Parameter**</span></span>|<span data-ttu-id="b38d7-151">**Typ**</span><span class="sxs-lookup"><span data-stu-id="b38d7-151">**Type**</span></span>|<span data-ttu-id="b38d7-152">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="b38d7-152">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b38d7-153">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="b38d7-153">_URL parameters_</span></span>|
|<span data-ttu-id="b38d7-154">id_value</span><span class="sxs-lookup"><span data-stu-id="b38d7-154">id_value</span></span>|<span data-ttu-id="b38d7-155">String</span><span class="sxs-lookup"><span data-stu-id="b38d7-155">String</span></span>|<span data-ttu-id="b38d7-p106">Die ID der erweiterten Eigenschaft, nach der gefiltert wird. Sie muss eins der unterstützten Formate aufweisen. Weitere Informationen finden Sie unter [Überblick über erweiterte Eigenschaften in Outlook](../resources/extended-properties-overview.md). Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b38d7-p106">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="b38d7-160">property_value</span><span class="sxs-lookup"><span data-stu-id="b38d7-160">property_value</span></span>|<span data-ttu-id="b38d7-161">String</span><span class="sxs-lookup"><span data-stu-id="b38d7-161">String</span></span>|<span data-ttu-id="b38d7-p107">Der Wert der erweiterten Eigenschaft, nach der gefiltert wird. Erforderlich, wo im Abschnitt **HTTP-Anforderung** oben aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="b38d7-p107">The value of the extended property to match. Required where listed in the **HTTP request** section above.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b38d7-164">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b38d7-164">Request headers</span></span>
| <span data-ttu-id="b38d7-165">Name</span><span class="sxs-lookup"><span data-stu-id="b38d7-165">Name</span></span>      |<span data-ttu-id="b38d7-166">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b38d7-166">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b38d7-167">Authorization</span><span class="sxs-lookup"><span data-stu-id="b38d7-167">Authorization</span></span>  | <span data-ttu-id="b38d7-p108">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b38d7-p108">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b38d7-170">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b38d7-170">Request body</span></span>
<span data-ttu-id="b38d7-171">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b38d7-171">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b38d7-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="b38d7-172">Response</span></span>

<span data-ttu-id="b38d7-173">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b38d7-173">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="b38d7-174">Abrufen von Ressourceninstanzen mithilfe von `$expand`</span><span class="sxs-lookup"><span data-stu-id="b38d7-174">GET resource instance using `$expand`</span></span>
<span data-ttu-id="b38d7-175">Der Antworttext enthält ein Objekt, das die angeforderte Ressourceninstanz darstellt, erweitert um das dem Filter entsprechende [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="b38d7-175">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-using-filter"></a><span data-ttu-id="b38d7-176">Abrufen von Ressourceninstanzen mithilfe von `$filter`</span><span class="sxs-lookup"><span data-stu-id="b38d7-176">GET resource instances using `$filter`</span></span>
<span data-ttu-id="b38d7-p109">Der Antworttext enthält ein oder mehrere Objekte, die Ressourceninstanzen darstellen, die die dem Filter entsprechende erweiterte Eigenschaft enthalten. Der Antworttext enthält nicht die erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="b38d7-p109">The response body includes one or more objects representing the resource instances that contain the matching extended property. The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="b38d7-179">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b38d7-179">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="b38d7-180">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="b38d7-180">Request 1</span></span>

<span data-ttu-id="b38d7-p110">Im ersten Beispiel wird die angegebene Nachricht abgerufen und um eine einwertige erweiterte Eigenschaft erweitert. Der Filter gibt die erweiterte Eigenschaft zurück, deren **id** der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` entspricht (URL-Codierung hier zur besseren Lesbarkeit entfernt).</span><span class="sxs-lookup"><span data-stu-id="b38d7-p110">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
##### <a name="response-1"></a><span data-ttu-id="b38d7-183">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="b38d7-183">Response 1</span></span>
<span data-ttu-id="b38d7-184">Der Antworttext enthält alle Eigenschaften der angegebenen Nachricht und die vom Filter zurückgegebene erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="b38d7-184">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="b38d7-p111">Hinweis: Das hier gezeigte **message**-Objekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b38d7-p111">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AACbyS4H\"",
    "id": "AAMkAGE1M2_bs88AACHsLqWAAA=",
    "subject": "RE: Talk about emergency prep",
    "sender": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "from": null,
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Christine Irwin",
                "address": "christine@contoso.com"
            }
        }
    ],
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```

****

#### <a name="request-2"></a><span data-ttu-id="b38d7-187">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="b38d7-187">Request 2</span></span>

<span data-ttu-id="b38d7-p112">Das zweite Beispiel ruft Nachrichten ab, die die im Filter spezifizierte einwertige erweiterte Eigenschaft haben. Der Filter gibt die erweiterte Eigenschaft zurück, die folgende Merkmale hat:</span><span class="sxs-lookup"><span data-stu-id="b38d7-p112">The second example gets messages that have the single-value extended property specified in the filter. The filter returns the extended property that has:</span></span>
- <span data-ttu-id="b38d7-190">Die **id** entspricht der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (URL-Codierung hier zur besseren Lesbarkeit entfernt).</span><span class="sxs-lookup"><span data-stu-id="b38d7-190">Its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>
- <span data-ttu-id="b38d7-191">Für **value** ist `Green` festgelegt.</span><span class="sxs-lookup"><span data-stu-id="b38d7-191">Its **value** being `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/api/v1.0/Me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

##### <a name="response-2"></a><span data-ttu-id="b38d7-192">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="b38d7-192">Response 2</span></span>

<span data-ttu-id="b38d7-p113">Eine erfolgreiche Antwort ist durch den Antwortcode `HTTP 200 OK` gekennzeichnet. Der Antworttext enthält alle Eigenschaften der Nachrichten, die die dem Filter entsprechende erweiterte Eigenschaft haben. Der Antworttext ähnelt der Antwort beim [Abrufen einer Nachrichtensammlung](../api/user_list_messages.md). Die Antwort enthält nicht die dem Filter entsprechende erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="b38d7-p113">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user_list_messages.md). The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->