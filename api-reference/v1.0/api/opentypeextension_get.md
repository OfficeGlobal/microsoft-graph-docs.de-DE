# <a name="get-open-extension"></a><span data-ttu-id="a8633-101">Datenerweiterung abrufen</span><span class="sxs-lookup"><span data-stu-id="a8633-101">Get open extension</span></span>

<span data-ttu-id="a8633-102">Dieser Artikel beschreibt, wie Sie eine offene Erweiterung ([openTypeExtension](../resources/openTypeExtension.md)-Objekt) basierend auf ihrem Namen oder ihrem vollqualifizierten Namen abrufen können.</span><span class="sxs-lookup"><span data-stu-id="a8633-102">Get an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) identified by name or fully qualified name.</span></span>

<span data-ttu-id="a8633-103">In der folgenden Tabelle sind die drei Szenarien für den Abruf einer offenen Erweiterung aus einer unterstützten Ressourceninstanz aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="a8633-103">The following table lists the three scenarios where you can get an open extension from a supported resource instance.</span></span>

|<span data-ttu-id="a8633-104">**GET-Szenario**</span><span class="sxs-lookup"><span data-stu-id="a8633-104">**GET scenario**</span></span>|<span data-ttu-id="a8633-105">**Unterstützte Ressourcen**</span><span class="sxs-lookup"><span data-stu-id="a8633-105">**Supported resources**</span></span>|<span data-ttu-id="a8633-106">**Antworttext**</span><span class="sxs-lookup"><span data-stu-id="a8633-106">**Response body**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a8633-107">Abrufen einer bestimmen Erweiterung aus einer bekannten Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="a8633-107">Get a specific extension from a known resource instance.</span></span>| [<span data-ttu-id="a8633-108">Device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user</span><span class="sxs-lookup"><span data-stu-id="a8633-108">Device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user</span></span>](../resources/user.md) | <span data-ttu-id="a8633-109">Nur offene Erweiterung</span><span class="sxs-lookup"><span data-stu-id="a8633-109">Open extension only.</span></span>|
|<span data-ttu-id="a8633-110">Abrufen einer bekannten Ressourceninstanz, erweitert um eine bestimmte Erweiterung</span><span class="sxs-lookup"><span data-stu-id="a8633-110">Get a known resource instance expanded with a specific extension.</span></span>|<span data-ttu-id="a8633-111">Device, event, group, group event, group post, message, organization, personal contact, user</span><span class="sxs-lookup"><span data-stu-id="a8633-111">Device, event, group, group event, group post, message, organization, personal contact, user</span></span> |<span data-ttu-id="a8633-112">Eine um die offene Erweiterung erweiterte Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="a8633-112">A resource instance expanded with the open extension.</span></span>|
|<span data-ttu-id="a8633-113">Suchen und Erweitern von Ressourceninstanzen mit einer bestimmten Erweiterung</span><span class="sxs-lookup"><span data-stu-id="a8633-113">Find and expand resource instances with a specific extension.</span></span> |<span data-ttu-id="a8633-114">Event, group event, group post, message, personal contact</span><span class="sxs-lookup"><span data-stu-id="a8633-114">Event, group event, group post, message, personal contact</span></span>|<span data-ttu-id="a8633-115">Um die offene Erweiterung erweiterte Ressourceninstanzen</span><span class="sxs-lookup"><span data-stu-id="a8633-115">Resource instances expanded with the open extension.</span></span>|


## <a name="permissions"></a><span data-ttu-id="a8633-116">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a8633-116">Permissions</span></span>

<span data-ttu-id="a8633-p101">Zum Aufrufen dieser API ist eine der folgenden Berechtigungen erforderlich (je nach Typ der Ressource, die die Erweiterung enthält): Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a8633-p101">One of the following permissions is required to call this API, depending on the resource that contains the extension. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a8633-119">**Unterstützte Ressource**</span><span class="sxs-lookup"><span data-stu-id="a8633-119">**Supported resource**</span></span>|<span data-ttu-id="a8633-120">**Berechtigung**</span><span class="sxs-lookup"><span data-stu-id="a8633-120">**Permission**</span></span>|<span data-ttu-id="a8633-121">**Unterstützte Ressource**</span><span class="sxs-lookup"><span data-stu-id="a8633-121">**Supported resource**</span></span>|<span data-ttu-id="a8633-122">**Berechtigung**</span><span class="sxs-lookup"><span data-stu-id="a8633-122">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="a8633-123">Gerät</span><span class="sxs-lookup"><span data-stu-id="a8633-123">Device</span></span>](../resources/device.md) | <span data-ttu-id="a8633-124">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8633-124">Directory.Read.All</span></span> | [<span data-ttu-id="a8633-125">Ereignis</span><span class="sxs-lookup"><span data-stu-id="a8633-125">Event</span></span>](../resources/event.md) | <span data-ttu-id="a8633-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a8633-126">Calendars.Read</span></span> | 
| [<span data-ttu-id="a8633-127">Gruppe</span><span class="sxs-lookup"><span data-stu-id="a8633-127">Group</span></span>](../resources/group.md) | <span data-ttu-id="a8633-128">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8633-128">Group.Read.All</span></span> | [<span data-ttu-id="a8633-129">Gruppenereignis</span><span class="sxs-lookup"><span data-stu-id="a8633-129">Group event</span></span>](../resources/event.md) | <span data-ttu-id="a8633-130">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8633-130">Group.Read.All</span></span> | 
| [<span data-ttu-id="a8633-131">Gruppenbeitrag</span><span class="sxs-lookup"><span data-stu-id="a8633-131">Group post</span></span>](../resources/post.md) | <span data-ttu-id="a8633-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8633-132">Group.Read.All</span></span> | [<span data-ttu-id="a8633-133">Nachricht</span><span class="sxs-lookup"><span data-stu-id="a8633-133">Message</span></span>](../resources/message.md) | <span data-ttu-id="a8633-134">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a8633-134">Mail.Read</span></span> | 
| [<span data-ttu-id="a8633-135">Organisation</span><span class="sxs-lookup"><span data-stu-id="a8633-135">Organization</span></span>](../resources/organization.md) | <span data-ttu-id="a8633-136">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8633-136">Directory.Read.All</span></span> | [<span data-ttu-id="a8633-137">Privater Kontakt</span><span class="sxs-lookup"><span data-stu-id="a8633-137">Personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="a8633-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a8633-138">Contacts.Read</span></span> |
| [<span data-ttu-id="a8633-139">Benutzer</span><span class="sxs-lookup"><span data-stu-id="a8633-139">User</span></span>](../resources/user.md) | <span data-ttu-id="a8633-140">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8633-140">User.Read.All</span></span> | | |



## <a name="http-request"></a><span data-ttu-id="a8633-141">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8633-141">HTTP request</span></span>

<span data-ttu-id="a8633-142">In diesem Abschnitt finden Sie die Syntax für jedes der drei oben beschriebenen `GET`-Szenarien.</span><span class="sxs-lookup"><span data-stu-id="a8633-142">This section lists the syntax for each of the three `GET` scenarios described above.</span></span>

### <a name="get-a-specific-extension-in-a-known-resource-instance"></a><span data-ttu-id="a8633-143">Abrufen einer spezifischen Erweiterung in einer bekannten Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="a8633-143">Get a specific extension in a known resource instance</span></span>

<span data-ttu-id="a8633-144">Verwenden Sie die gleiche REST-Anforderung wie zum Abrufen der Ressourceninstanz, und geben Sie die Erweiterung in der Navigationseigenschaft **extensions** dieser Instanz an.</span><span class="sxs-lookup"><span data-stu-id="a8633-144">Use the same REST request as getting the resource instance, and identify the extension using the **extensions** navigation property of that instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/extensions/{extensionId}
GET /groups/{Id}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/threads/{Id}/posts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/messages/{Id}/extensions/{extensionId}
GET /organization/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/contacts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/extensions/{extensionId}
```


### <a name="get-a-known-resource-instance-expanded-with-a-matching-extension"></a><span data-ttu-id="a8633-145">Abrufen einer bekannten Ressourceninstanz, erweitert um eine übereinstimmende Erweiterung</span><span class="sxs-lookup"><span data-stu-id="a8633-145">Get a known resource instance expanded with a matching extension</span></span> 

<span data-ttu-id="a8633-p102">Für die Ressourcentypen „event“, „group event“, „group post“, „message“ und „personal contact“ können Sie die gleiche REST-Anforderung wie zum Abrufen der Ressourceninstanz verwenden. Suchen Sie zusätzlich per Filter nach einer Erweiterung mit dem gewünschten Wert in der Eigenschaft **id**, und erweitern Sie die Instanz mit der Erweiterung. Die Antwort enthält die meisten der Ressourceneigenschaften.</span><span class="sxs-lookup"><span data-stu-id="a8633-p102">For the event, group event, group post, message, personal contact resource types, you can use the same REST request as getting the resource instance, look for an extension that matches a filter on its **id** property, and expand the instance with the extension. The response includes most of the resource properties.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
```


<span data-ttu-id="a8633-148">Für die Ressourcentypen „device“, „group“, „organization“ und „user“ müssen Sie auch einen `$select`-Parameter verwenden, um die Eigenschaft **Id** und alle anderen gewünschten Eigenschaften aus der Ressourceninstanz einzuschließen:</span><span class="sxs-lookup"><span data-stu-id="a8633-148">For the device, group, organization, and user resource types, you must also use a `$select` parameter to include the **id** property and any other properties you want from the resource instance:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /groups/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /organization/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /users/{Id|userPrincipalName}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
```

### <a name="filter-for-resource-instances-expanded-with-a-matching-extension"></a><span data-ttu-id="a8633-149">Filtern nach Ressourceninstanzen, erweitert mit einer übereinstimmenden Erweiterung</span><span class="sxs-lookup"><span data-stu-id="a8633-149">Filter for resource instances expanded with a matching extension</span></span> 

<span data-ttu-id="a8633-150">Verwenden Sie die gleiche REST-Anforderung wie zum Abrufen einer Sammlung der unterstützten Ressource. Filtern Sie die Sammlung nach Instanzen mit einer Erweiterung, die den gewünschten Wert in der Eigenschaft **id** aufweist, und erweitern Sie die betreffenden Instanzen um diese Erweiterung.</span><span class="sxs-lookup"><span data-stu-id="a8633-150">Use the same REST request as getting a collection of the supported resource, filter the collection for instances that contain an extension with a matching **id** property, and expand these instances with the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
```

><span data-ttu-id="a8633-p103">**Hinweis:** Die obige Syntax zeigt mehrere häufig verwendete Möglichkeiten zum Identifizieren einer Ressourceninstanz oder -sammlung, um eine Erweiterung daraus zu löschen. Alle anderen Syntaxen, mit denen Sie diese Ressourceninstanzen oder -sammlungen identifizieren können, unterstützen das Löschen offener Erweiterungen daraus in einer ähnlichen Weise.</span><span class="sxs-lookup"><span data-stu-id="a8633-p103">**Note:** The above syntax shows some common ways to identify a resource instance or collection, in order to get an extension from it. All other syntax that allows you to identify these resource instances or collections supports getting open extensions from them in a similar way.</span></span>

## <a name="parameters"></a><span data-ttu-id="a8633-153">Parameter</span><span class="sxs-lookup"><span data-stu-id="a8633-153">Parameters</span></span>
|<span data-ttu-id="a8633-154">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="a8633-154">**Parameter**</span></span>|<span data-ttu-id="a8633-155">**Typ**</span><span class="sxs-lookup"><span data-stu-id="a8633-155">**Type**</span></span>|<span data-ttu-id="a8633-156">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="a8633-156">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a8633-157">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="a8633-157">_URL parameters_</span></span>|
|<span data-ttu-id="a8633-158">Id</span><span class="sxs-lookup"><span data-stu-id="a8633-158">Id</span></span>|<span data-ttu-id="a8633-159">string</span><span class="sxs-lookup"><span data-stu-id="a8633-159">string</span></span>|<span data-ttu-id="a8633-p104">Platzhalter für einen eindeutigen Bezeichner eines Objekts in der entsprechenden Sammlung, z. B. einer Nachricht, eines Ereignisses oder eines Kontakts. Erforderlich. Nicht zu verwechseln mit der **id**-Eigenschaft einer **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="a8633-p104">Placeholder for a unique identifier for an object in the corresponding collection such as messages, events, contacts. Required. Not to be confused with the **id** property of an **openTypeExtension**.</span></span>|
|<span data-ttu-id="a8633-163">extensionId</span><span class="sxs-lookup"><span data-stu-id="a8633-163">extensionId</span></span>|<span data-ttu-id="a8633-164">string</span><span class="sxs-lookup"><span data-stu-id="a8633-164">string</span></span>|<span data-ttu-id="a8633-p105">Platzhalter für einen Erweiterungsnamen. Ein Erweiterungsname ist der eindeutige Textbezeichner einer Erweiterung oder ein vollqualifizierter Name, der den Erweiterungstyp und den eindeutigen Textbezeichner verkettet. Der vollqualifizierte Name wird beim Erstellen der Erweiterung in der Eigenschaft **id** zurückgegeben. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a8633-p105">Placeholder for an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the **id** property when you create the extension. Required.</span></span>|


## <a name="optional-query-parameters"></a><span data-ttu-id="a8633-168">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a8633-168">Optional query parameters</span></span>

<span data-ttu-id="a8633-169">Stellen Sie sicher, dass Sie für die Leerzeichen in der `$filter`-Zeichenfolge die [URL-Codierung](http://www.w3schools.com/tags/ref_urlencode.asp) verwenden.</span><span class="sxs-lookup"><span data-stu-id="a8633-169">Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the `$filter` string.</span></span>

|<span data-ttu-id="a8633-170">**Name**</span><span class="sxs-lookup"><span data-stu-id="a8633-170">**Name**</span></span>|<span data-ttu-id="a8633-171">**Wert**</span><span class="sxs-lookup"><span data-stu-id="a8633-171">**Value**</span></span>|<span data-ttu-id="a8633-172">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="a8633-172">**Description**</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="a8633-173">$filter</span><span class="sxs-lookup"><span data-stu-id="a8633-173">$filter</span></span>|<span data-ttu-id="a8633-174">string</span><span class="sxs-lookup"><span data-stu-id="a8633-174">string</span></span>|<span data-ttu-id="a8633-175">Gibt Erweiterungen zurück, deren **id** dem Wert des Parameters `extensionId` entspricht.</span><span class="sxs-lookup"><span data-stu-id="a8633-175">Returns an extension with its **id** matching the `extensionId` parameter value.</span></span>|
|<span data-ttu-id="a8633-176">$filter with **any** operator</span><span class="sxs-lookup"><span data-stu-id="a8633-176">$filter with **any** operator</span></span>|<span data-ttu-id="a8633-177">string</span><span class="sxs-lookup"><span data-stu-id="a8633-177">string</span></span>|<span data-ttu-id="a8633-178">Gibt Instanzen einer Ressourcensammlung zurück, die eine Erweiterung enthalten, deren **id** dem Wert des Parameters `extensionId` entspricht.</span><span class="sxs-lookup"><span data-stu-id="a8633-178">Returns instances of a resource collection that contain an extension with its **id** matching the `extensionId` parameter value.</span></span>| 
|<span data-ttu-id="a8633-179">$expand</span><span class="sxs-lookup"><span data-stu-id="a8633-179">$expand</span></span>|<span data-ttu-id="a8633-180">string</span><span class="sxs-lookup"><span data-stu-id="a8633-180">string</span></span>|<span data-ttu-id="a8633-181">Erweitert eine Ressourceninstanz um eine Erweiterung.</span><span class="sxs-lookup"><span data-stu-id="a8633-181">Expands a resource instance to include an extension.</span></span> |


## <a name="request-headers"></a><span data-ttu-id="a8633-182">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8633-182">Request headers</span></span>
| <span data-ttu-id="a8633-183">Name</span><span class="sxs-lookup"><span data-stu-id="a8633-183">Name</span></span>       | <span data-ttu-id="a8633-184">Wert</span><span class="sxs-lookup"><span data-stu-id="a8633-184">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="a8633-185">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8633-185">Authorization</span></span> | <span data-ttu-id="a8633-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a8633-p106">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="a8633-188">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a8633-188">Request body</span></span>
<span data-ttu-id="a8633-189">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a8633-189">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8633-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8633-190">Response</span></span>

<span data-ttu-id="a8633-p107">Wird diese Methode erfolgreich ausgeführt, gibt Sie den Antwortcode `200 OK` und ein [openTypeExtension](../resources/opentypeextension.md)-Objekt im Antworttext zurück. Der genaue Antworttext ist je nach GET-Abfrage unterschiedlich.</span><span class="sxs-lookup"><span data-stu-id="a8633-p107">If successful, this method returns a `200 OK` response code and [openTypeExtension](../resources/opentypeextension.md) object in the response body. Depending on the GET query, the exact response body differs.</span></span>
## <a name="example"></a><span data-ttu-id="a8633-193">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8633-193">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="a8633-194">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="a8633-194">Request 1</span></span>

<span data-ttu-id="a8633-p108">Das erste Beispiel zeigt 2 Möglichkeiten zur Referenzierung einer Erweiterung und ruft die Erweiterung in der angegebenen Nachricht ab. Es wird unabhängig von der zur Referenzierung der Erweiterung verwendeten Methode jeweils die gleiche Antwort zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8633-p108">The first example shows 2 ways of referencing an extension and gets the extension in the specified message. The response is the same regardless of the way used to reference the extension.</span></span>

<span data-ttu-id="a8633-197">Die erste Möglichkeit ist der Abruf mithilfe des Namens:</span><span class="sxs-lookup"><span data-stu-id="a8633-197">First, by its name:</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="a8633-198">Die zweite Möglichkeit ist der Abruf mithilfe der ID (vollqualifizierter Name):</span><span class="sxs-lookup"><span data-stu-id="a8633-198">Second, by its ID (fully qualified name):</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```

#### <a name="response-1"></a><span data-ttu-id="a8633-199">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="a8633-199">Response 1</span></span>
<span data-ttu-id="a8633-200">Hier sehen Sie die Antwort für Beispiel 1:</span><span class="sxs-lookup"><span data-stu-id="a8633-200">Here is the response for the first example.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

****


#### <a name="request-2"></a><span data-ttu-id="a8633-201">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="a8633-201">Request 2</span></span>

<span data-ttu-id="a8633-202">Das zweite Beispiel referenziert eine Erweiterung über ihren Namen und ruft die Erweiterung im angegebenen Gruppenereignis ab.</span><span class="sxs-lookup"><span data-stu-id="a8633-202">The second example references an extension by its name and gets the extension in the specified group event.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions('Com.Contoso.Deal') 
```

#### <a name="response-2"></a><span data-ttu-id="a8633-203">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="a8633-203">Response 2</span></span>

<span data-ttu-id="a8633-204">Die Antwort für das zweite Beispiel sieht so aus:</span><span class="sxs-lookup"><span data-stu-id="a8633-204">Here is the response from the second example.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

#### <a name="request-3"></a><span data-ttu-id="a8633-205">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="a8633-205">Request 3</span></span>

<span data-ttu-id="a8633-p109">Im dritten Beispiel wird die angegebene Nachricht abgerufen und um eine von einem Filter zurückgegebene Erweiterung erweitert. Der Filter gibt die Erweiterung zurück, deren **id** dem angegebenen vollqualifizierten Namen entspricht.</span><span class="sxs-lookup"><span data-stu-id="a8633-p109">The third example gets and expands the specified message by including the extension returned from a filter. The filter returns the extension that has its **id** matching a fully qualified name.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')?$expand=extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```


#### <a name="response-3"></a><span data-ttu-id="a8633-208">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="a8633-208">Response 3</span></span>

<span data-ttu-id="a8633-p110">Unten sehen Sie die Antwort für das dritte Beispiel. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8633-p110">And here is the response from the third example. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM\"",
    "id": "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===",
    "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM",
    "categories": [
    ],
    "createDateTime": "2015-06-19T02:03:31Z",
    "lastModifiedDateTime": "2015-08-13T02:28:00Z",
    "subject": "Attached is the requested info",
    "bodyPreview": "See the images attached.",
    "body": {
        "contentType": "HTML",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<style type=\"text/css\" style=\"display:none;\"><!-- P {margin-top:0;margin-bottom:0;} --></style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" style=\"font-size:12pt;color:#000000;background-color:#FFFFFF;font-family:Calibri,Arial,Helvetica,sans-serif;\">\r\n<p>See the images attached. <br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "importance": "Normal",
    "hasAttachments": true,
    "parentFolderId": "AQMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===QAAAA==",
    "from": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "sender": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "address": "wendy@contoso.com",
                "name": "Wendy Molina"
            }
        }
    ],
    "ccRecipients": [
    ],
    "bccRecipients": [
    ],
    "replyTo": [
    ],
    "conversationId": "AAQkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===mivdTmQ=",
    "receivedDateTime": "2015-06-19T02:05:04Z",
    "sentDateTime": "2015-06-19T02:04:59Z",
    "isDeliveryReceiptRequested": false,
    "isReadReceiptRequested": false,
    "isDraft": false,
    "isRead": true,
    "webLink": "https://outlook.office.com/owa/?ItemID=AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===%2FNJTqt5NqHlVnKVBwCY4MQpaFz9SbqUDe4%2Bbs88AAAAAAEJAACY4MQpaFz9SbqUDe4%2Bbs88AAApA4JMAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "Focused",
    "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
        "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
        "extensionName": "Com.Contoso.Referral",
        "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "dealValue": 500050,
        "expirationDate": "2015-12-03T10:00:00Z"
      }
     ]
}
```

****

#### <a name="request-4"></a><span data-ttu-id="a8633-212">Anforderung 4</span><span class="sxs-lookup"><span data-stu-id="a8633-212">Request 4</span></span>

<span data-ttu-id="a8633-213">Das vierte Beispiel referenziert eine Erweiterung über ihren vollqualifizierten Namen und ruft die Erweiterung im angegebenen Gruppenbeitrag ab.</span><span class="sxs-lookup"><span data-stu-id="a8633-213">The fourth example references an extension by its fully qualified name and gets the extension in the specified group post.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_4"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate') 
```

#### <a name="response-4"></a><span data-ttu-id="a8633-214">Antwort 4</span><span class="sxs-lookup"><span data-stu-id="a8633-214">Response 4</span></span>

<span data-ttu-id="a8633-215">Die Antwort für das vierte Beispiel sieht wie folgt aus:</span><span class="sxs-lookup"><span data-stu-id="a8633-215">Here is the response from the fourth example.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```


#### <a name="request-5"></a><span data-ttu-id="a8633-216">Anforderung 5</span><span class="sxs-lookup"><span data-stu-id="a8633-216">Request 5</span></span>

<span data-ttu-id="a8633-p111">Das fünfte Beispiel sucht unter allen Nachrichten im Postfach des angemeldeten Benutzers diejenigen mit einer Erweiterung, die dem definierten Filter entspricht. Anschließend werden die Nachrichten um die Erweiterung erweitert. Der Filter gibt Erweiterungen zurück, deren **id**-Eigenschaft dem Erweiterungsnamen `Com.Contoso.Referral` entspricht.</span><span class="sxs-lookup"><span data-stu-id="a8633-p111">The fifth example looks at all messages in the signed-in user's mailbox to find those that contain an extension matching a filter, and expands them by including the extension. The filter returns extensions that has the **id** property matching the extension name `Com.Contoso.Referral`.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_5"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')&$expand=Extensions($filter=id%20eq%20'Com.Contoso.Referral')
```


####<a name="response-5"></a><span data-ttu-id="a8633-219">Antwort 5</span><span class="sxs-lookup"><span data-stu-id="a8633-219">Response 5</span></span>

<span data-ttu-id="a8633-220">In der Antwort aus Beispiel 5 gibt es im Postfach des Benutzers nur eine Nachricht mit einer Erweiterung, deren **id** `Com.Contoso.Referral` entspricht.</span><span class="sxs-lookup"><span data-stu-id="a8633-220">In this response for the fifth example, there is only one message in the user's mailbox that has an extension with its **id** equal to `Com.Contoso.Referral`.</span></span>

<span data-ttu-id="a8633-p112">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8633-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages",
  "value": [
  {

    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM\"",
    "id": "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===",
    "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM",
    "categories": [
    ],
    "createDateTime": "2015-06-19T02:03:31Z",
    "lastModifiedDateTime": "2015-08-13T02:28:00Z",
    "subject": "Attached is the requested info",
    "bodyPreview": "See the images attached.",
    "body": {
        "contentType": "HTML",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<style type=\"text/css\" style=\"display:none;\"><!-- P {margin-top:0;margin-bottom:0;} --></style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" style=\"font-size:12pt;color:#000000;background-color:#FFFFFF;font-family:Calibri,Arial,Helvetica,sans-serif;\">\r\n<p>See the images attached. <br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "importance": "Normal",
    "hasAttachments": true,
    "parentFolderId": "AQMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===QAAAA==",
    "from": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "sender": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "address": "wendy@contoso.com",
                "name": "Wendy Molina"
            }
        }
    ],
    "ccRecipients": [
    ],
    "bccRecipients": [
    ],
    "replyTo": [
    ],
    "conversationId": "AAQkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===mivdTmQ=",
    "receivedDateTime": "2015-06-19T02:05:04Z",
    "sentDateTime": "2015-06-19T02:04:59Z",
    "isDeliveryReceiptRequested": false,
    "isReadReceiptRequested": false,
    "isDraft": false,
    "isRead": true,
    "webLink": "https://outlook.office.com/owa/?ItemID=AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===%2FNJTqt5NqHlVnKVBwCY4MQpaFz9SbqUDe4%2Bbs88AAAAAAEJAACY4MQpaFz9SbqUDe4%2Bbs88AAApA4JMAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "Focused",
    "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
        "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
        "extensionName": "Com.Contoso.Referral",
        "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "dealValue": 500050,
        "expirationDate": "2015-12-03T10:00:00Z"
      }
     ]
  }
  ]
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get openTypeExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
