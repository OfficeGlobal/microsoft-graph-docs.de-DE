# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="5324e-101">singleValueLegacyExtendedProperty abrufen</span><span class="sxs-lookup"><span data-stu-id="5324e-101">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="5324e-102">Sie können eine einzelne, mit einer bestimmten erweiterten Eigenschaft erweiterte Ressourceninstanz oder eine Sammlung von Ressourceninstanzen abrufen, die einem Filter entsprechende erweiterte Eigenschaften enthalten.</span><span class="sxs-lookup"><span data-stu-id="5324e-102">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="5324e-103">Mit dem Abfrageparameter `$expand` können Sie die angegebene Ressourceninstanz, erweitert um die angegebene erweiterte Eigenschaft, abrufen.</span><span class="sxs-lookup"><span data-stu-id="5324e-103">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="5324e-104">Wenden Sie einen `$filter`- und einen `eq`-Operator auf die **ID**-Eigenschaft an, um die erweiterte Eigenschaft anzugeben.</span><span class="sxs-lookup"><span data-stu-id="5324e-104">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="5324e-105">Dies ist derzeit die einzige Möglichkeit zum Abrufen des [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md)-Objekts, das eine erweiterte Eigenschaft darstellt.</span><span class="sxs-lookup"><span data-stu-id="5324e-105">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="5324e-106">Um Ressourceninstanzen mit bestimmten erweiterten Eigenschaften abzurufen, verwenden Sie den Abfrageparameter `$filter`, und wenden Sie einen `eq`-Operator auf die **ID**-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="5324e-106">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="5324e-107">Wenden Sie für nummerische erweiterte Eigenschaften zudem einen der folgenden Operatoren auf die Eigenschaft **Wert** an: `eq`, `ne`,`ge`, `gt`, `le` oder `lt`.</span><span class="sxs-lookup"><span data-stu-id="5324e-107">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="5324e-108">Für erweiterte Eigenschaften vom Typ Zeichenfolge wenden Sie einen `contains`-, `startswith`-, `eq`-, oder `ne`-Operator auf den **Wert** an.</span><span class="sxs-lookup"><span data-stu-id="5324e-108">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span>

<span data-ttu-id="5324e-109">Der Filter wird auf alle Instanzen der Ressource angewendet, die im Postfach eines angemeldeten Benutzers existieren.</span><span class="sxs-lookup"><span data-stu-id="5324e-109">The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span> 

<span data-ttu-id="5324e-110">Beim Filtern des Namens der Zeichenfolge (`Name`) in der **ID** einer erweiterten Eigenschaft wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="5324e-110">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="5324e-111">Beim Filtern der Eigenschaft **Wert** einer erweiterten Eigenschaft wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="5324e-111">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="5324e-112">Die folgenden Benutzerressourcen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="5324e-112">The following user resources are supported:</span></span>

- [<span data-ttu-id="5324e-113">calendar</span><span class="sxs-lookup"><span data-stu-id="5324e-113">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="5324e-114">contact</span><span class="sxs-lookup"><span data-stu-id="5324e-114">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="5324e-115">contactFolder</span><span class="sxs-lookup"><span data-stu-id="5324e-115">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="5324e-116">Ereignis</span><span class="sxs-lookup"><span data-stu-id="5324e-116">event</span></span>](../resources/event.md)
- [<span data-ttu-id="5324e-117">mailFolder</span><span class="sxs-lookup"><span data-stu-id="5324e-117">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="5324e-118">Nachricht</span><span class="sxs-lookup"><span data-stu-id="5324e-118">message</span></span>](../resources/message.md) 

<span data-ttu-id="5324e-119">Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="5324e-119">As well as the following group resources:</span></span>

- <span data-ttu-id="5324e-120">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="5324e-120">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="5324e-121">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="5324e-121">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="5324e-122">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="5324e-122">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="5324e-123">Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="5324e-123">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="5324e-124">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5324e-124">Permissions</span></span>
<span data-ttu-id="5324e-125">Je nach der Ressource kommen die erweiterte Eigenschaft aus und geben Sie die Berechtigung (delegierte oder-Anwendung) Sie Anforderung, die Berechtigung, die in der folgenden Tabelle angegeben ist mindestens erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="5324e-125">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="5324e-126">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5324e-126">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="5324e-127">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="5324e-127">Supported resource</span></span> | <span data-ttu-id="5324e-128">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5324e-128">Delegated (work or school account)</span></span> | <span data-ttu-id="5324e-129">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5324e-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5324e-130">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5324e-130">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="5324e-131">Kalender</span><span class="sxs-lookup"><span data-stu-id="5324e-131">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="5324e-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-132">Calendars.Read</span></span> | <span data-ttu-id="5324e-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-133">Calendars.Read</span></span> | <span data-ttu-id="5324e-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-134">Calendars.Read</span></span> |
| [<span data-ttu-id="5324e-135">Kontakt</span><span class="sxs-lookup"><span data-stu-id="5324e-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="5324e-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-136">Contacts.Read</span></span> | <span data-ttu-id="5324e-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-137">Contacts.Read</span></span> | <span data-ttu-id="5324e-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-138">Contacts.Read</span></span> |
| [<span data-ttu-id="5324e-139">contactFolder</span><span class="sxs-lookup"><span data-stu-id="5324e-139">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="5324e-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-140">Contacts.Read</span></span> | <span data-ttu-id="5324e-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-141">Contacts.Read</span></span> | <span data-ttu-id="5324e-142">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-142">Contacts.Read</span></span> |
| [<span data-ttu-id="5324e-143">Ereignis</span><span class="sxs-lookup"><span data-stu-id="5324e-143">event</span></span>](../resources/event.md) | <span data-ttu-id="5324e-144">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-144">Calendars.Read</span></span> | <span data-ttu-id="5324e-145">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-145">Calendars.Read</span></span> |  <span data-ttu-id="5324e-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-146">Calendars.Read</span></span>|
| <span data-ttu-id="5324e-147">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="5324e-147">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="5324e-148">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5324e-148">Group.Read.All</span></span> | <span data-ttu-id="5324e-149">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5324e-149">Not supported</span></span> | <span data-ttu-id="5324e-150">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5324e-150">Not supported</span></span> |
| <span data-ttu-id="5324e-151">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="5324e-151">group [event](../resources/event.md)</span></span> | <span data-ttu-id="5324e-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5324e-152">Group.Read.All</span></span> | <span data-ttu-id="5324e-153">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5324e-153">Not supported</span></span> | <span data-ttu-id="5324e-154">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5324e-154">Not supported</span></span> |
| <span data-ttu-id="5324e-155">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="5324e-155">group [post](../resources/post.md)</span></span> | <span data-ttu-id="5324e-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5324e-156">Group.Read.All</span></span> | <span data-ttu-id="5324e-157">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5324e-157">Not supported</span></span> | <span data-ttu-id="5324e-158">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5324e-158">Group.Read.All</span></span> |
| [<span data-ttu-id="5324e-159">mailFolder</span><span class="sxs-lookup"><span data-stu-id="5324e-159">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="5324e-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-160">Mail.Read</span></span> | <span data-ttu-id="5324e-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-161">Mail.Read</span></span> | <span data-ttu-id="5324e-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-162">Mail.Read</span></span> |
| [<span data-ttu-id="5324e-163">Nachricht</span><span class="sxs-lookup"><span data-stu-id="5324e-163">message</span></span>](../resources/message.md) | <span data-ttu-id="5324e-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-164">Mail.Read</span></span> | <span data-ttu-id="5324e-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-165">Mail.Read</span></span> | <span data-ttu-id="5324e-166">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5324e-166">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="5324e-167">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5324e-167">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="5324e-168">Abrufen einer Ressourceninstanz, erweitert um eine erweiterte Eigenschaft, die einem Filter entspricht</span><span class="sxs-lookup"><span data-stu-id="5324e-168">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="5324e-p105">Hier sehen Sie, wie Sie eine Ressourceninstanz abrufen können, erweitert um die erweiterte Eigenschaft, deren **id**-Eigenschaft dem definierten Filter entspricht. Stellen Sie sicher, dass Sie für die Leerzeichen in der Filterzeichenfolge die [URL-Codierung](https://www.w3schools.com/tags/ref_urlencode.asp) verwenden.</span><span class="sxs-lookup"><span data-stu-id="5324e-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="5324e-171">Erhalten Sie eine Instanz der **Nachricht** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-171">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="5324e-172">Eine **MailFolder** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-172">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="5324e-173">Rufen Sie eine Instanz **Ereignis** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-173">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="5324e-174">Eine **Kalender** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-174">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="5324e-175">Abrufen einer Instanz **wenden Sie sich an** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-175">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="5324e-176">Eine **ContactFolder** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-176">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="5324e-177">Eine Gruppe **Ereignis** Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-177">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="5324e-178">Eine Gruppe **Buchen** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-178">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="5324e-179">Abrufen von Ressourceninstanzen, die numerische erweiterte Eigenschaften enthalten, die einem Filter entsprechen</span><span class="sxs-lookup"><span data-stu-id="5324e-179">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="5324e-180">Rufen Sie Instanzen einer unterstützten Ressource ab, die eine numerische erweiterte Eigenschaft besitzen, die einem Filter entspricht.</span><span class="sxs-lookup"><span data-stu-id="5324e-180">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="5324e-181">Der Filter wendet einen `eq`-Operator auf die **ID**-Eigenschaft und einen der folgenden Operatoren auf die Eigenschaft **Wert** an: `eq`, `ne`,`ge`, `gt` , `le` oder `lt`.</span><span class="sxs-lookup"><span data-stu-id="5324e-181">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="5324e-182">Stellen Sie sicher, dass Sie für die folgenden Zeichen in der Filterzeichenfolge die [URL-Codierung](https://www.w3schools.com/tags/ref_urlencode.asp) verwenden: Doppelpunkte, Vorwärtsschrägstriche und Leerzeichen.</span><span class="sxs-lookup"><span data-stu-id="5324e-182">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="5324e-183">Die folgenden Syntaxzeilen zeigen einen Filter, der den `eq`-Operator auf die ID anwendet, und einen `eq`-Operator, der auf den Eigenschaftswert angewandt wird.</span><span class="sxs-lookup"><span data-stu-id="5324e-183">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="5324e-184">Sie können den `eq`-Operator, der auf den **Wert** angewandt wird, durch einen der anderen Operatoren (`ne`,`ge`, `gt`, `le` oder `lt`) ersetzen, die auf numerische Werte angewandt werden.</span><span class="sxs-lookup"><span data-stu-id="5324e-184">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="5324e-185">**Nachricht** Instanzen abgerufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-185">Get **message** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="5324e-186">**MailFolder** Instanzen abgerufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-186">Get **mailFolder** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="5324e-187">**Ereignis** -Instanzen abzurufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-187">Get **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="5324e-188">**Kalender** -Instanzen abzurufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-188">Get **calendar** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="5324e-189">**Wenden Sie sich an** Instanzen abgerufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-189">Get **contact** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="5324e-190">**ContactFolder** Instanzen abgerufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-190">Get **contactFolder** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="5324e-191">Gruppe **Ereignis** Instanzen abgerufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-191">Get group **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="5324e-192">Gruppe **Buchen** Instanzen abgerufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-192">Get group **post** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="5324e-193">Abrufen von Ressourceninstanzen mit erweiterten Eigenschaften des Typs Zeichenfolge, die einem Filter entsprechen</span><span class="sxs-lookup"><span data-stu-id="5324e-193">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="5324e-194">Rufen Sie Instanzen der Ressource **Nachricht** oder **Ereignis** mit einer erweiterten Eigenschaft des Typs Zeichenfolge ab, die einem Filter entspricht.</span><span class="sxs-lookup"><span data-stu-id="5324e-194">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="5324e-195">Der Filter wendet einen `eq`-Operator auf die **ID**-Eigenschaft und einen der folgenden Operatoren auf die Eigenschaft **Wert** an: `contains`, `startswith`, `eq` oder `ne`.</span><span class="sxs-lookup"><span data-stu-id="5324e-195">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="5324e-196">Stellen Sie sicher, dass Sie für die folgenden Zeichen in der Filterzeichenfolge die [URL-Codierung](https://www.w3schools.com/tags/ref_urlencode.asp) verwenden: Doppelpunkte, Vorwärtsschrägstriche und Leerzeichen.</span><span class="sxs-lookup"><span data-stu-id="5324e-196">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="5324e-197">**Nachricht** Instanzen abgerufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-197">Get **message** instances: <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="5324e-198">**Ereignis** -Instanzen abzurufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-198">Get **event** instances: <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="5324e-199">Gruppe **Ereignis** Instanzen abgerufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5324e-199">Get group **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="5324e-200">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="5324e-200">Path parameters</span></span>
|<span data-ttu-id="5324e-201">Parameter</span><span class="sxs-lookup"><span data-stu-id="5324e-201">Parameter</span></span>|<span data-ttu-id="5324e-202">Typ</span><span class="sxs-lookup"><span data-stu-id="5324e-202">Type</span></span>|<span data-ttu-id="5324e-203">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5324e-203">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5324e-204">id_value</span><span class="sxs-lookup"><span data-stu-id="5324e-204">id_value</span></span>|<span data-ttu-id="5324e-205">String</span><span class="sxs-lookup"><span data-stu-id="5324e-205">String</span></span>|<span data-ttu-id="5324e-p109">Die ID der erweiterten Eigenschaft, nach der gefiltert wird. Sie muss eins der unterstützten Formate aufweisen. Weitere Informationen finden Sie unter [Überblick über erweiterte Eigenschaften in Outlook](../resources/extended-properties-overview.md). Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5324e-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="5324e-210">property_value</span><span class="sxs-lookup"><span data-stu-id="5324e-210">property_value</span></span> |<span data-ttu-id="5324e-211">String</span><span class="sxs-lookup"><span data-stu-id="5324e-211">String</span></span>|<span data-ttu-id="5324e-212">Der Wert der erweiterten Eigenschaft, nach der gefiltert wird.</span><span class="sxs-lookup"><span data-stu-id="5324e-212">The value of the extended property to match.</span></span> <span data-ttu-id="5324e-213">Erforderlich, wo im Abschnitt **HTTP-Anforderung** oben aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="5324e-213">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="5324e-214">Wenn {property_value} keine Zeichenfolge ist, müssen Sie sicherstellen, dass `ep/value` explizit in den entsprechenden Edm-Datentyp beim Vergleich mit {property_value} umgewandelt wird.</span><span class="sxs-lookup"><span data-stu-id="5324e-214">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="5324e-215">Beispiele finden Sie unter [Anforderung 4](#request-4) weiter unter.</span><span class="sxs-lookup"><span data-stu-id="5324e-215">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5324e-216">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5324e-216">Request headers</span></span>
| <span data-ttu-id="5324e-217">Name</span><span class="sxs-lookup"><span data-stu-id="5324e-217">Name</span></span>      |<span data-ttu-id="5324e-218">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5324e-218">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5324e-219">Authorization</span><span class="sxs-lookup"><span data-stu-id="5324e-219">Authorization</span></span>  | <span data-ttu-id="5324e-p111">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5324e-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5324e-222">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5324e-222">Request body</span></span>
<span data-ttu-id="5324e-223">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5324e-223">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5324e-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="5324e-224">Response</span></span>

<span data-ttu-id="5324e-225">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5324e-225">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-expanded-with-a-matching-extended-property"></a><span data-ttu-id="5324e-226">Abrufen einer Ressourceninstanz, erweitert um eine übereinstimmende erweiterte Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5324e-226">GET resource instance expanded with a matching extended property</span></span>
<span data-ttu-id="5324e-227">Der Antworttext enthält ein Objekt, das die angeforderte Ressourceninstanz darstellt, erweitert um das dem Filter entsprechende [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="5324e-227">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="5324e-228">Abrufen von Ressourceninstanzen mit einer erweiterten Eigenschaft, die einem Filter entspricht</span><span class="sxs-lookup"><span data-stu-id="5324e-228">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="5324e-229">Der Antworttext enthält ein oder mehrere Objekte, die Ressourceninstanzen darstellen, die einem dem Filter entsprechende erweiterte Eigenschaft enthalten.</span><span class="sxs-lookup"><span data-stu-id="5324e-229">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="5324e-230">Der Antworttext enthält nicht die erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="5324e-230">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="5324e-231">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5324e-231">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="5324e-232">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="5324e-232">Request 1</span></span>

<span data-ttu-id="5324e-p113">Im ersten Beispiel wird die angegebene Nachricht abgerufen und um eine einwertige erweiterte Eigenschaft erweitert. Der Filter gibt die erweiterte Eigenschaft zurück, deren **id** der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` entspricht (URL-Codierung hier zur besseren Lesbarkeit entfernt).</span><span class="sxs-lookup"><span data-stu-id="5324e-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2_bs88AACHsLqWAAA="],
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="5324e-235">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="5324e-235">Response 1</span></span>
<span data-ttu-id="5324e-236">Der Antworttext enthält alle Eigenschaften der angegebenen Nachricht und die vom Filter zurückgegebene erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="5324e-236">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="5324e-p114">Hinweis: Das hier gezeigte **message**-Objekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5324e-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="5324e-239">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="5324e-239">Request 2</span></span>

<span data-ttu-id="5324e-240">Das zweite Beispiel ruft Nachrichten ab, die die im Filter spezifizierte einwertige erweiterte Eigenschaft vom Typ Zeichenfolge haben.</span><span class="sxs-lookup"><span data-stu-id="5324e-240">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="5324e-241">Der Filter sucht nach der erweiterten Eigenschaft, die folgende Merkmale hat:</span><span class="sxs-lookup"><span data-stu-id="5324e-241">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="5324e-242">Die **ID** entspricht der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (URL-Codierung hier zur besseren Lesbarkeit entfernt).</span><span class="sxs-lookup"><span data-stu-id="5324e-242">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="5324e-243">Der **Wert** ist gleich der Zeichenfolge `Green`.</span><span class="sxs-lookup"><span data-stu-id="5324e-243">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="5324e-244">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="5324e-244">Response 2</span></span>

<span data-ttu-id="5324e-p116">Eine erfolgreiche Antwort ist durch den Antwortcode `HTTP 200 OK` gekennzeichnet. Der Antworttext enthält alle Eigenschaften der Nachrichten, die die dem Filter entsprechende erweiterte Eigenschaft haben. Der Antworttext ähnelt der Antwort beim [Abrufen einer Nachrichtensammlung](../api/user_list_messages.md). Die Antwort enthält nicht die dem Filter entsprechende erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="5324e-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user_list_messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="5324e-248">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="5324e-248">Request 3</span></span>

<span data-ttu-id="5324e-249">Das dritte Beispiel ruft Nachrichten ab, die die im Filter spezifizierte einwertige erweiterte Eigenschaft vom Typ Zeichenfolge haben.</span><span class="sxs-lookup"><span data-stu-id="5324e-249">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="5324e-250">Der Filter sucht nach der erweiterten Eigenschaft, die folgende Merkmale hat:</span><span class="sxs-lookup"><span data-stu-id="5324e-250">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="5324e-251">Die **ID** entspricht der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (URL-Codierung hier zur besseren Lesbarkeit entfernt).</span><span class="sxs-lookup"><span data-stu-id="5324e-251">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="5324e-252">Die **Wert**, der die Zeichenfolge `green` enthält.</span><span class="sxs-lookup"><span data-stu-id="5324e-252">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="5324e-253">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="5324e-253">Response 3</span></span>

<span data-ttu-id="5324e-254">Eine erfolgreiche Antwort ist durch den Antwortcode `HTTP 200 OK` gekennzeichnet. Der Antworttext enthält alle Eigenschaften der Nachrichten, die die dem Filter entsprechende erweiterte Eigenschaft haben.</span><span class="sxs-lookup"><span data-stu-id="5324e-254">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="5324e-255">Wie zum Beispiel eine Nachricht, die eine einwertige erweiterte Eigenschaft mit einer **ID** besitzt, die der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` entspricht, und der **Wert** `Light green` stimmt mit dem Filter überein und ist in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="5324e-255">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="5324e-256">Der Antworttext ähnelt der Antwort beim [Abrufen einer Nachrichtensammlung](../api/user_list_messages.md).</span><span class="sxs-lookup"><span data-stu-id="5324e-256">The response body is similar to the response from [getting a message collection](../api/user_list_messages.md).</span></span> <span data-ttu-id="5324e-257">Die Antwort enthält nicht die dem Filter entsprechende erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="5324e-257">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="5324e-258">Anforderung 4</span><span class="sxs-lookup"><span data-stu-id="5324e-258">Request 4</span></span>

<span data-ttu-id="5324e-259">Die nächsten 2 Beispiele zeigen, wie Sie Nachrichten abrufen, die erweiterte einwertige Eigenschaften vom Typ Nicht-Zeichenfolge enthalten.</span><span class="sxs-lookup"><span data-stu-id="5324e-259">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="5324e-260">Zur besseren Lesbarkeit ist die erforderliche URL-Codierung dort nicht enthalten.</span><span class="sxs-lookup"><span data-stu-id="5324e-260">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="5324e-261">Das folgende Beispiel zeigt einen Filter, der nach der erweiterte Eigenschaft mit den folgenden Merkmalen sucht:</span><span class="sxs-lookup"><span data-stu-id="5324e-261">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="5324e-262">Die **id** entspricht der Zeichenfolge `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span><span class="sxs-lookup"><span data-stu-id="5324e-262">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="5324e-263">Der **Wert** ist die GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span><span class="sxs-lookup"><span data-stu-id="5324e-263">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="5324e-264">Wenn Sie den Eigenschaftswert mit einer GUID vergleichen möchten, ändern Sie `ep/value` in `Edm.Guid`.</span><span class="sxs-lookup"><span data-stu-id="5324e-264">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="5324e-265">Das folgende Beispiel zeigt einen Filter, der nach der erweiterte Eigenschaft mit den folgenden Merkmalen sucht:</span><span class="sxs-lookup"><span data-stu-id="5324e-265">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="5324e-266">Die **id** entspricht der Zeichenfolge `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span><span class="sxs-lookup"><span data-stu-id="5324e-266">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="5324e-267">Der **Wert** ist gleich der ganzen Zahl 12.</span><span class="sxs-lookup"><span data-stu-id="5324e-267">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="5324e-268">Um den Eigenschaftswert mit einer ganzen Zahl zu vergleichen, ändern Sie `ep/value` in `Edm.Int32`.</span><span class="sxs-lookup"><span data-stu-id="5324e-268">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="5324e-269">Antwort 4</span><span class="sxs-lookup"><span data-stu-id="5324e-269">Response 4</span></span>

<span data-ttu-id="5324e-270">Bei den zwei vorhergehenden Beispielen ist eine erfolgreiche Antwort durch den Antwortcode `HTTP 200 OK` gekennzeichnet. Der Antworttext enthält alle Eigenschaften der Nachrichten, die die dem Filter entsprechende erweiterte Eigenschaft haben.</span><span class="sxs-lookup"><span data-stu-id="5324e-270">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="5324e-271">Der Antworttext ähnelt der Antwort beim [Abrufen einer Nachrichtensammlung](../api/user_list_messages.md).</span><span class="sxs-lookup"><span data-stu-id="5324e-271">The response body is similar to the response from [getting a message collection](../api/user_list_messages.md).</span></span> <span data-ttu-id="5324e-272">Die Antwort enthält nicht die dem Filter entsprechende erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="5324e-272">The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->