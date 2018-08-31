# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="0fd97-101">singleValueLegacyExtendedProperty abrufen</span><span class="sxs-lookup"><span data-stu-id="0fd97-101">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="0fd97-102">Sie können eine einzelne, mit einer bestimmten erweiterten Eigenschaft erweiterte Ressourceninstanz oder eine Sammlung von Ressourceninstanzen abrufen, die einem Filter entsprechende erweiterte Eigenschaften enthalten.</span><span class="sxs-lookup"><span data-stu-id="0fd97-102">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="0fd97-103">Mit dem Abfrageparameter `$expand` können Sie die angegebene Ressourceninstanz, erweitert um die angegebene erweiterte Eigenschaft, abrufen.</span><span class="sxs-lookup"><span data-stu-id="0fd97-103">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="0fd97-104">Wenden Sie einen `$filter`- und einen `eq`-Operator auf die **ID**-Eigenschaft an, um die erweiterte Eigenschaft anzugeben.</span><span class="sxs-lookup"><span data-stu-id="0fd97-104">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="0fd97-105">Dies ist derzeit die einzige Möglichkeit zum Abrufen des [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md)-Objekts, das eine erweiterte Eigenschaft darstellt.</span><span class="sxs-lookup"><span data-stu-id="0fd97-105">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="0fd97-106">Um Ressourceninstanzen mit bestimmten erweiterten Eigenschaften abzurufen, verwenden Sie den Abfrageparameter `$filter`, und wenden Sie einen `eq`-Operator auf die **ID**-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="0fd97-106">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="0fd97-107">Wenden Sie für nummerische erweiterte Eigenschaften zudem einen der folgenden Operatoren auf die Eigenschaft **Wert** an: `eq`, `ne`,`ge`, `gt`, `le` oder `lt`.</span><span class="sxs-lookup"><span data-stu-id="0fd97-107">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="0fd97-108">Für erweiterte Eigenschaften vom Typ Zeichenfolge wenden Sie einen `contains`-, `startswith`-, `eq`-, oder `ne`-Operator auf den **Wert** an.</span><span class="sxs-lookup"><span data-stu-id="0fd97-108">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span>

<span data-ttu-id="0fd97-109">Der Filter wird auf alle Instanzen der Ressource angewendet, die im Postfach eines angemeldeten Benutzers existieren.</span><span class="sxs-lookup"><span data-stu-id="0fd97-109">The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span> 

<span data-ttu-id="0fd97-110">Beim Filtern des Namens der Zeichenfolge (`Name`) in der **ID** einer erweiterten Eigenschaft wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="0fd97-110">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="0fd97-111">Beim Filtern der Eigenschaft **Wert** einer erweiterten Eigenschaft wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="0fd97-111">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="0fd97-112">Die folgenden Benutzerressourcen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="0fd97-112">The following user resources are supported:</span></span>

- [<span data-ttu-id="0fd97-113">message</span><span class="sxs-lookup"><span data-stu-id="0fd97-113">message</span></span>](../resources/message.md)
- [<span data-ttu-id="0fd97-114">mailFolder</span><span class="sxs-lookup"><span data-stu-id="0fd97-114">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="0fd97-115">event</span><span class="sxs-lookup"><span data-stu-id="0fd97-115">event</span></span>](../resources/event.md)
- [<span data-ttu-id="0fd97-116">calendar</span><span class="sxs-lookup"><span data-stu-id="0fd97-116">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="0fd97-117">contakt</span><span class="sxs-lookup"><span data-stu-id="0fd97-117">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="0fd97-118">contactFolder</span><span class="sxs-lookup"><span data-stu-id="0fd97-118">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="0fd97-119">Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="0fd97-119">As well as the following group resources:</span></span>

- <span data-ttu-id="0fd97-120">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="0fd97-120">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="0fd97-121">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="0fd97-121">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="0fd97-122">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="0fd97-122">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="0fd97-123">Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="0fd97-123">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fd97-124">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0fd97-124">Permissions</span></span>
<span data-ttu-id="0fd97-p104">Zum Aufrufen dieser API ist eine der folgenden Berechtigungen erforderlich (je nachdem, welche Ressource Sie abrufen möchten): Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0fd97-p104">One of the following permissions is required to call this API, depending on the resource you're getting. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="0fd97-127">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0fd97-127">Mail.Read</span></span>
- <span data-ttu-id="0fd97-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0fd97-128">Calendars.Read</span></span>
- <span data-ttu-id="0fd97-129">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0fd97-129">Contacts.Read</span></span>
- <span data-ttu-id="0fd97-130">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fd97-130">Group.Read.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="0fd97-131">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0fd97-131">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="0fd97-132">Abrufen einer Ressourceninstanz, erweitert um eine erweiterte Eigenschaft, die einem Filter entspricht</span><span class="sxs-lookup"><span data-stu-id="0fd97-132">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="0fd97-p105">Hier sehen Sie, wie Sie eine Ressourceninstanz abrufen können, erweitert um die erweiterte Eigenschaft, deren **id**-Eigenschaft dem definierten Filter entspricht. Stellen Sie sicher, dass Sie für die Leerzeichen in der Filterzeichenfolge die [URL-Codierung](http://www.w3schools.com/tags/ref_urlencode.asp) verwenden.</span><span class="sxs-lookup"><span data-stu-id="0fd97-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="0fd97-135">Abrufen einer **message**-Instanz: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-135">Get a **message** instance:</span></span>
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="0fd97-136">Abrufen einer **mailFolder**-Instanz: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-136">Get a **mailFolder** instance:</span></span>
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="0fd97-137">Abrufen einer **event**-Instanz <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-137">Get an **event** instance:</span></span>
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="0fd97-138">Abrufen einer **calendar**-Instanz: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-138">Get a **calendar** instance:</span></span>
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="0fd97-139">Abrufen einer **contakt**-Instanz: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-139">Get a **contact** instance:</span></span>
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="0fd97-140">Abrufen einer **contactFolder**-Instanz: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-140">Get a **contactFolder** instance:</span></span>
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="0fd97-141">Abrufen einer **event**-Instanz für eine Gruppe: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-141">Get a group **event** instance:</span></span>
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="0fd97-142">Abrufen einer **post**-Instanz für eine Gruppe: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-142">Get a group **post** instance:</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="0fd97-143">Abrufen von Ressourceninstanzen, die numerische erweiterte Eigenschaften enthalten, die einem Filter entsprechen</span><span class="sxs-lookup"><span data-stu-id="0fd97-143">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="0fd97-144">Rufen Sie Instanzen einer unterstützten Ressource ab, die eine numerische erweiterte Eigenschaft besitzen, die einem Filter entspricht.</span><span class="sxs-lookup"><span data-stu-id="0fd97-144">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="0fd97-145">Der Filter wendet einen `eq`-Operator auf die **ID**-Eigenschaft und einen der folgenden Operatoren auf die Eigenschaft **Wert** an: `eq`, `ne`,`ge`, `gt` , `le` oder `lt`.</span><span class="sxs-lookup"><span data-stu-id="0fd97-145">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="0fd97-146">Stellen Sie sicher, dass Sie für die folgenden Zeichen in der Filterzeichenfolge die [URL-Codierung](http://www.w3schools.com/tags/ref_urlencode.asp) verwenden: Doppelpunkte, Vorwärtsschrägstriche und Leerzeichen.</span><span class="sxs-lookup"><span data-stu-id="0fd97-146">Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="0fd97-147">Die folgenden Syntaxzeilen zeigen einen Filter, der den `eq`-Operator auf die ID anwendet, und einen `eq`-Operator, der auf den Eigenschaftswert angewandt wird.</span><span class="sxs-lookup"><span data-stu-id="0fd97-147">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="0fd97-148">Sie können den `eq`-Operator, der auf den **Wert** angewandt wird, durch einen der anderen Operatoren (`ne`,`ge`, `gt`, `le` oder `lt`) ersetzen, die auf numerische Werte angewandt werden.</span><span class="sxs-lookup"><span data-stu-id="0fd97-148">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="0fd97-149">Abrufen von **message**-Instanzen: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-149">Get **message** instances:</span></span>
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="0fd97-150">Abrufen von **mailFolder**-Instanzen: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-150">Get **mailFolder** instances:</span></span>
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="0fd97-151">Abrufen von **event**-Instanzen: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-151">Get **event** instances:</span></span>
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="0fd97-152">Abrufen von **calendar**-Instanzen: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-152">Get **calendar** instances:</span></span>
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="0fd97-153">Abrufen von **contact**-Instanzen: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-153">Get **contact** instances:</span></span>
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="0fd97-154">Abrufen von **contactFolder**-Instanzen: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-154">Get **contactFolder** instances:</span></span>
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="0fd97-155">Abrufen von **event**-Instanzen für Gruppen: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-155">Get group **event** instances:</span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="0fd97-156">Abrufen von **post**-Instanzen für Gruppen: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-156">Get group **post** instances:</span></span>
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="0fd97-157">Abrufen von Ressourceninstanzen mit erweiterten Eigenschaften des Typs Zeichenfolge, die einem Filter entsprechen</span><span class="sxs-lookup"><span data-stu-id="0fd97-157">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="0fd97-158">Rufen Sie Instanzen der Ressource **Nachricht** oder **Ereignis** mit einer erweiterten Eigenschaft des Typs Zeichenfolge ab, die einem Filter entspricht.</span><span class="sxs-lookup"><span data-stu-id="0fd97-158">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="0fd97-159">Der Filter wendet einen `eq`-Operator auf die **ID**-Eigenschaft und einen der folgenden Operatoren auf die Eigenschaft **Wert** an: `contains`, `startswith`, `eq` oder `ne`.</span><span class="sxs-lookup"><span data-stu-id="0fd97-159">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="0fd97-160">Stellen Sie sicher, dass Sie für die folgenden Zeichen in der Filterzeichenfolge die [URL-Codierung](http://www.w3schools.com/tags/ref_urlencode.asp) verwenden: Doppelpunkte, Vorwärtsschrägstriche und Leerzeichen.</span><span class="sxs-lookup"><span data-stu-id="0fd97-160">Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="0fd97-161">Abrufen von **message**-Instanzen: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-161">Get **message** instances:</span></span>
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="0fd97-162">Abrufen von **event**-Instanzen: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-162">Get **event** instances:</span></span>
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="0fd97-163">Abrufen von **event**-Instanzen für Gruppen: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0fd97-163">Get group **event** instances:</span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="parameters"></a><span data-ttu-id="0fd97-164">Parameter</span><span class="sxs-lookup"><span data-stu-id="0fd97-164">Parameters</span></span>
|<span data-ttu-id="0fd97-165">Parameter</span><span class="sxs-lookup"><span data-stu-id="0fd97-165">Parameter</span></span>|<span data-ttu-id="0fd97-166">Typ</span><span class="sxs-lookup"><span data-stu-id="0fd97-166">Type</span></span>|<span data-ttu-id="0fd97-167">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0fd97-167">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0fd97-168">id_value</span><span class="sxs-lookup"><span data-stu-id="0fd97-168">id_value</span></span>|<span data-ttu-id="0fd97-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0fd97-169">String</span></span>|<span data-ttu-id="0fd97-p109">Die ID der erweiterten Eigenschaft, nach der gefiltert wird. Sie muss eins der unterstützten Formate aufweisen. Weitere Informationen finden Sie unter [Überblick über erweiterte Eigenschaften in Outlook](../resources/extended-properties-overview.md). Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0fd97-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="0fd97-174">property_value</span><span class="sxs-lookup"><span data-stu-id="0fd97-174">property_value</span></span> |<span data-ttu-id="0fd97-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0fd97-175">String</span></span>|<span data-ttu-id="0fd97-176">Der Wert der erweiterten Eigenschaft, nach der gefiltert wird.</span><span class="sxs-lookup"><span data-stu-id="0fd97-176">The value of the extended property to match.</span></span> <span data-ttu-id="0fd97-177">Erforderlich, wo im Abschnitt **HTTP-Anforderung** oben aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="0fd97-177">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="0fd97-178">Wenn {property_value} keine Zeichenfolge ist, müssen Sie sicherstellen, dass `ep/value` explizit in den entsprechenden Edm-Datentyp beim Vergleich mit {property_value} umgewandelt wird.</span><span class="sxs-lookup"><span data-stu-id="0fd97-178">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="0fd97-179">Beispiele finden Sie unter [Anforderung 4](#request-4) weiter unter.</span><span class="sxs-lookup"><span data-stu-id="0fd97-179">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0fd97-180">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0fd97-180">Request headers</span></span>
| <span data-ttu-id="0fd97-181">Name</span><span class="sxs-lookup"><span data-stu-id="0fd97-181">Name</span></span>      |<span data-ttu-id="0fd97-182">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0fd97-182">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0fd97-183">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0fd97-183">Authorization</span></span>  | <span data-ttu-id="0fd97-p111">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0fd97-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fd97-186">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0fd97-186">Request body</span></span>
<span data-ttu-id="0fd97-187">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0fd97-187">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fd97-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="0fd97-188">Response</span></span>

<span data-ttu-id="0fd97-189">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0fd97-189">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-expanded-with-a-matching-extended-property"></a><span data-ttu-id="0fd97-190">Abrufen einer Ressourceninstanz, erweitert um eine übereinstimmende erweiterte Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0fd97-190">GET resource instance expanded with a matching extended property</span></span>
<span data-ttu-id="0fd97-191">Der Antworttext enthält ein Objekt, das die angeforderte Ressourceninstanz darstellt, erweitert um das dem Filter entsprechende [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="0fd97-191">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="0fd97-192">Abrufen von Ressourceninstanzen mit einer erweiterten Eigenschaft, die einem Filter entspricht</span><span class="sxs-lookup"><span data-stu-id="0fd97-192">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="0fd97-193">Der Antworttext enthält ein oder mehrere Objekte, die Ressourceninstanzen darstellen, die einem dem Filter entsprechende erweiterte Eigenschaft enthalten.</span><span class="sxs-lookup"><span data-stu-id="0fd97-193">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="0fd97-194">Der Antworttext enthält nicht die erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="0fd97-194">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="0fd97-195">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0fd97-195">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="0fd97-196">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="0fd97-196">Request 1</span></span>

<span data-ttu-id="0fd97-p113">Im ersten Beispiel wird die angegebene Nachricht abgerufen und um eine einwertige erweiterte Eigenschaft erweitert. Der Filter gibt die erweiterte Eigenschaft zurück, deren **id** der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` entspricht (URL-Codierung hier zur besseren Lesbarkeit entfernt).</span><span class="sxs-lookup"><span data-stu-id="0fd97-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2_bs88AACHsLqWAAA="],
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="0fd97-199">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="0fd97-199">Response 1</span></span>
<span data-ttu-id="0fd97-200">Der Antworttext enthält alle Eigenschaften der angegebenen Nachricht und die vom Filter zurückgegebene erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="0fd97-200">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="0fd97-p114">Hinweis: Das hier gezeigte **message**-Objekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0fd97-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="0fd97-203">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="0fd97-203">Request 2</span></span>

<span data-ttu-id="0fd97-204">Das zweite Beispiel ruft Nachrichten ab, die die im Filter spezifizierte einwertige erweiterte Eigenschaft vom Typ Zeichenfolge haben.</span><span class="sxs-lookup"><span data-stu-id="0fd97-204">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="0fd97-205">Der Filter sucht nach der erweiterten Eigenschaft, die folgende Merkmale hat:</span><span class="sxs-lookup"><span data-stu-id="0fd97-205">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="0fd97-206">Die **ID** entspricht der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (URL-Codierung hier zur besseren Lesbarkeit entfernt).</span><span class="sxs-lookup"><span data-stu-id="0fd97-206">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="0fd97-207">Der **Wert** ist gleich der Zeichenfolge `Green`.</span><span class="sxs-lookup"><span data-stu-id="0fd97-207">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="0fd97-208">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="0fd97-208">Response 2</span></span>

<span data-ttu-id="0fd97-p116">Eine erfolgreiche Antwort ist durch den Antwortcode `HTTP 200 OK` gekennzeichnet. Der Antworttext enthält alle Eigenschaften der Nachrichten, die die dem Filter entsprechende erweiterte Eigenschaft haben. Der Antworttext ähnelt der Antwort beim [Abrufen einer Nachrichtensammlung](../api/user_list_messages.md). Die Antwort enthält nicht die dem Filter entsprechende erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="0fd97-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user_list_messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="0fd97-212">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="0fd97-212">Request 3</span></span>

<span data-ttu-id="0fd97-213">Das dritte Beispiel ruft Nachrichten ab, die die im Filter spezifizierte einwertige erweiterte Eigenschaft vom Typ Zeichenfolge haben.</span><span class="sxs-lookup"><span data-stu-id="0fd97-213">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="0fd97-214">Der Filter sucht nach der erweiterten Eigenschaft, die folgende Merkmale hat:</span><span class="sxs-lookup"><span data-stu-id="0fd97-214">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="0fd97-215">Die **ID** entspricht der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (URL-Codierung hier zur besseren Lesbarkeit entfernt).</span><span class="sxs-lookup"><span data-stu-id="0fd97-215">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="0fd97-216">Die **Wert**, der die Zeichenfolge `green` enthält.</span><span class="sxs-lookup"><span data-stu-id="0fd97-216">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="0fd97-217">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="0fd97-217">Response 3</span></span>

<span data-ttu-id="0fd97-218">Eine erfolgreiche Antwort ist durch den Antwortcode `HTTP 200 OK` gekennzeichnet. Der Antworttext enthält alle Eigenschaften der Nachrichten, die die dem Filter entsprechende erweiterte Eigenschaft haben.</span><span class="sxs-lookup"><span data-stu-id="0fd97-218">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="0fd97-219">Wie zum Beispiel eine Nachricht, die eine einwertige erweiterte Eigenschaft mit einer **ID** besitzt, die der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` entspricht, und der **Wert** `Light green` stimmt mit dem Filter überein und ist in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="0fd97-219">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="0fd97-220">Der Antworttext ähnelt der Antwort beim [Abrufen einer Nachrichtensammlung](../api/user_list_messages.md).</span><span class="sxs-lookup"><span data-stu-id="0fd97-220">The response body is similar to the response from [getting a message collection](../api/user_list_messages.md).</span></span> <span data-ttu-id="0fd97-221">Die Antwort enthält nicht die dem Filter entsprechende erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="0fd97-221">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="0fd97-222">Anforderung 4</span><span class="sxs-lookup"><span data-stu-id="0fd97-222">Request 4</span></span>

<span data-ttu-id="0fd97-223">Die nächsten 2 Beispiele zeigen, wie Sie Nachrichten abrufen, die erweiterte einwertige Eigenschaften vom Typ Nicht-Zeichenfolge enthalten.</span><span class="sxs-lookup"><span data-stu-id="0fd97-223">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="0fd97-224">Zur besseren Lesbarkeit ist die erforderliche URL-Codierung dort nicht enthalten.</span><span class="sxs-lookup"><span data-stu-id="0fd97-224">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="0fd97-225">Das folgende Beispiel zeigt einen Filter, der nach der erweiterte Eigenschaft mit den folgenden Merkmalen sucht:</span><span class="sxs-lookup"><span data-stu-id="0fd97-225">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="0fd97-226">Die **id** entspricht der Zeichenfolge `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span><span class="sxs-lookup"><span data-stu-id="0fd97-226">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="0fd97-227">Der **Wert** ist die GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span><span class="sxs-lookup"><span data-stu-id="0fd97-227">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="0fd97-228">Wenn Sie den Eigenschaftswert mit einer GUID vergleichen möchten, ändern Sie `ep/value` in `Edm.Guid`.</span><span class="sxs-lookup"><span data-stu-id="0fd97-228">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="0fd97-229">Das folgende Beispiel zeigt einen Filter, der nach der erweiterte Eigenschaft mit den folgenden Merkmalen sucht:</span><span class="sxs-lookup"><span data-stu-id="0fd97-229">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="0fd97-230">Die **id** entspricht der Zeichenfolge `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span><span class="sxs-lookup"><span data-stu-id="0fd97-230">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="0fd97-231">Der **Wert** ist gleich der ganzen Zahl 12.</span><span class="sxs-lookup"><span data-stu-id="0fd97-231">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="0fd97-232">Um den Eigenschaftswert mit einer ganzen Zahl zu vergleichen, ändern Sie `ep/value` in `Edm.Int32`.</span><span class="sxs-lookup"><span data-stu-id="0fd97-232">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="0fd97-233">Antwort 4</span><span class="sxs-lookup"><span data-stu-id="0fd97-233">Response 4</span></span>

<span data-ttu-id="0fd97-234">Bei den zwei vorhergehenden Beispielen ist eine erfolgreiche Antwort durch den Antwortcode `HTTP 200 OK` gekennzeichnet. Der Antworttext enthält alle Eigenschaften der Nachrichten, die die dem Filter entsprechende erweiterte Eigenschaft haben.</span><span class="sxs-lookup"><span data-stu-id="0fd97-234">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="0fd97-235">Der Antworttext ähnelt der Antwort beim [Abrufen einer Nachrichtensammlung](../api/user_list_messages.md).</span><span class="sxs-lookup"><span data-stu-id="0fd97-235">The response body is similar to the response from [getting a message collection](../api/user_list_messages.md).</span></span> <span data-ttu-id="0fd97-236">Die Antwort enthält nicht die dem Filter entsprechende erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="0fd97-236">The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->