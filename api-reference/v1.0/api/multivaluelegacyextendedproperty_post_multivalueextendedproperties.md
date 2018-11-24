# <a name="create-multi-value-extended-property"></a><span data-ttu-id="c0008-101">Mehrwertige erweiterte Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="c0008-101">Create multi-value extended property</span></span>

<span data-ttu-id="c0008-102">In diesem Artikel erläutern wir Ihnen,wie Sie eine oder mehrere mehrwertige erweiterte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource erstellen können.</span><span class="sxs-lookup"><span data-stu-id="c0008-102">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="c0008-103">Die folgenden Benutzerressourcen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="c0008-103">The following user resources are supported:</span></span>

- [<span data-ttu-id="c0008-104">calendar</span><span class="sxs-lookup"><span data-stu-id="c0008-104">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="c0008-105">contact</span><span class="sxs-lookup"><span data-stu-id="c0008-105">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="c0008-106">contactFolder</span><span class="sxs-lookup"><span data-stu-id="c0008-106">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="c0008-107">Ereignis</span><span class="sxs-lookup"><span data-stu-id="c0008-107">event</span></span>](../resources/event.md)
- [<span data-ttu-id="c0008-108">mailFolder</span><span class="sxs-lookup"><span data-stu-id="c0008-108">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="c0008-109">Nachricht</span><span class="sxs-lookup"><span data-stu-id="c0008-109">message</span></span>](../resources/message.md)

<span data-ttu-id="c0008-110">Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="c0008-110">As well as the following group resources:</span></span>

- <span data-ttu-id="c0008-111">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="c0008-111">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="c0008-112">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="c0008-112">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="c0008-113">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="c0008-113">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="c0008-114">Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="c0008-114">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0008-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c0008-115">Permissions</span></span>
<span data-ttu-id="c0008-116">Erstellen Sie je nach der Ressource in die erweiterte Eigenschaft und die Berechtigung geben (delegierte oder-Anwendung) Sie Anforderung, die Berechtigung, die in der folgenden Tabelle angegeben ist mindestens erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="c0008-116">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="c0008-117">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c0008-117">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="c0008-118">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="c0008-118">Supported resource</span></span> | <span data-ttu-id="c0008-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0008-119">Delegated (work or school account)</span></span> | <span data-ttu-id="c0008-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0008-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0008-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0008-121">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="c0008-122">Kalender</span><span class="sxs-lookup"><span data-stu-id="c0008-122">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="c0008-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-123">Calendars.ReadWrite</span></span> | <span data-ttu-id="c0008-124">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-124">Calendars.ReadWrite</span></span> | <span data-ttu-id="c0008-125">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-125">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="c0008-126">Kontakt</span><span class="sxs-lookup"><span data-stu-id="c0008-126">contact</span></span>](../resources/contact.md) | <span data-ttu-id="c0008-127">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-127">Contacts.ReadWrite</span></span> | <span data-ttu-id="c0008-128">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-128">Contacts.ReadWrite</span></span> | <span data-ttu-id="c0008-129">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-129">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="c0008-130">contactFolder</span><span class="sxs-lookup"><span data-stu-id="c0008-130">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="c0008-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="c0008-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-132">Contacts.ReadWrite</span></span> | <span data-ttu-id="c0008-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-133">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="c0008-134">event</span><span class="sxs-lookup"><span data-stu-id="c0008-134">event</span></span>](../resources/event.md) | <span data-ttu-id="c0008-135">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-135">Calendars.ReadWrite</span></span> | <span data-ttu-id="c0008-136">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-136">Calendars.ReadWrite</span></span> |  <span data-ttu-id="c0008-137">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-137">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="c0008-138">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="c0008-138">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="c0008-139">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0008-139">Group.ReadWrite.All</span></span> | <span data-ttu-id="c0008-140">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0008-140">Not supported</span></span> | <span data-ttu-id="c0008-141">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0008-141">Not supported</span></span> |
| <span data-ttu-id="c0008-142">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="c0008-142">group [event](../resources/event.md)</span></span> | <span data-ttu-id="c0008-143">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0008-143">Group.ReadWrite.All</span></span> | <span data-ttu-id="c0008-144">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0008-144">Not supported</span></span> | <span data-ttu-id="c0008-145">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0008-145">Not supported</span></span> |
| <span data-ttu-id="c0008-146">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="c0008-146">group [post](../resources/post.md)</span></span> | <span data-ttu-id="c0008-147">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0008-147">Group.ReadWrite.All</span></span> | <span data-ttu-id="c0008-148">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0008-148">Not supported</span></span> | <span data-ttu-id="c0008-149">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0008-149">Not supported</span></span> |
| [<span data-ttu-id="c0008-150">mailFolder</span><span class="sxs-lookup"><span data-stu-id="c0008-150">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="c0008-151">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-151">Mail.ReadWrite</span></span> | <span data-ttu-id="c0008-152">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-152">Mail.ReadWrite</span></span> | <span data-ttu-id="c0008-153">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-153">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="c0008-154">message</span><span class="sxs-lookup"><span data-stu-id="c0008-154">message</span></span>](../resources/message.md) | <span data-ttu-id="c0008-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-155">Mail.ReadWrite</span></span> | <span data-ttu-id="c0008-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-156">Mail.ReadWrite</span></span> | <span data-ttu-id="c0008-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0008-157">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0008-158">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0008-158">HTTP request</span></span>
<span data-ttu-id="c0008-159">Sie können erweiterte Eigenschaften in einer neuen oder vorhandenen Ressourceninstanz erstellen.</span><span class="sxs-lookup"><span data-stu-id="c0008-159">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="c0008-p102">Verwenden Sie zum Erstellen einer oder mehrerer erweiterter Eigenschaften in einer _neuen_ Ressourceninstanz die gleiche REST-Anforderung wie zum Erstellen der Instanz, und fügen Sie die Eigenschaften der neuen Ressourceninstanz _und die erweiterte Eigenschaft_ zum Anforderungstext hinzu. Beachten Sie, dass für einige Ressourcen die Erstellung auf mehrere Weisen erfolgen kann. Weitere Informationen zum Erstellen dieser Ressourceninstanzen finden Sie unter den entsprechenden Themen zum Erstellen einer [Nachricht](../resources/message.md), eines [MailFolder](../api/user_post_mailfolders.md)-Elements, [Ereignisses](../api/user_post_events.md), [Kalenders](../api/user_post_calendars.md), [Kontakts](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md)-Elements, [Gruppenereignisses](../api/group_post_events.md) und eines [Gruppenbeitrags](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="c0008-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user_post_mailfolders.md), [event](../api/user_post_events.md), [calendar](../api/user_post_calendars.md), [contact](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md), [group event](../api/group_post_events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="c0008-163">So sieht die Syntax der Anforderungen aus:</span><span class="sxs-lookup"><span data-stu-id="c0008-163">The following is the syntax of the requests.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages

POST /me/mailFolders
POST /users/{id|userPrincipalName}/mailFolders

POST /me/events
POST /users/{id|userPrincipalName}/events

POST /me/calendars
POST /users/{id|userPrincipalName}/calendars

POST /me/contacts
POST /users/{id|userPrincipalName}/contacts

POST /me/contactFolders
POST /users/{id|userPrincipalName}/contactFolders

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

<span data-ttu-id="c0008-164">Um eine oder mehrere erweiterte Eigenschaften in einer vorhandenen Ressourceninstanz zu erstellen,müssen Sie die Instanz in der Anforderung angeben und die erweiterte-Eigenschaft zum Anforderungstext hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="c0008-164">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="c0008-165">**Hinweis:** Sie können keine erweiterte Eigenschaft in einem vorhandenen Gruppenbeitrag erstellen.</span><span class="sxs-lookup"><span data-stu-id="c0008-165">**Note** You cannot create an extended property in an existing group post.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id|userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}

PATCH /me/mailFolders/{id}
PATCH /users/{id|userPrincipalName}/mailFolders/{id}

PATCH /me/events/{id}
PATCH /users/{id|userPrincipalName}/events/{id}

PATCH /me/calendars/{id}
PATCH /users/{id|userPrincipalName}/calendars/{id}

PATCH /me/contacts/{id}
PATCH /users/{id|userPrincipalName}/contacts/{id}

PATCH /me/contactFolders/{id}
PATCH /users/{id|userPrincipalName}/contactFolders/{id}

PATCH /groups/{id}/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c0008-166">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0008-166">Request headers</span></span>
| <span data-ttu-id="c0008-167">Name</span><span class="sxs-lookup"><span data-stu-id="c0008-167">Name</span></span>       | <span data-ttu-id="c0008-168">Wert</span><span class="sxs-lookup"><span data-stu-id="c0008-168">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="c0008-169">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0008-169">Authorization</span></span> | <span data-ttu-id="c0008-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c0008-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c0008-172">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0008-172">Content-Type</span></span> | <span data-ttu-id="c0008-173">application/json</span><span class="sxs-lookup"><span data-stu-id="c0008-173">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0008-174">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0008-174">Request body</span></span>

<span data-ttu-id="c0008-175">Geben Sie einen JSON-Text für jedes [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md)-Objekt in der **multiValueExtendedProperties**-Sammlung der Ressourceninstanz an.</span><span class="sxs-lookup"><span data-stu-id="c0008-175">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) object in the **multiValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="c0008-176">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c0008-176">Property</span></span>|<span data-ttu-id="c0008-177">Typ</span><span class="sxs-lookup"><span data-stu-id="c0008-177">Type</span></span>|<span data-ttu-id="c0008-178">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0008-178">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c0008-179">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="c0008-179">multiValueExtendedProperties</span></span>|<span data-ttu-id="c0008-180">[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="c0008-180">[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection</span></span>| <span data-ttu-id="c0008-181">Ein Array aus einer oder mehreren mehrwertigen erweiterten Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c0008-181">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="c0008-182">id</span><span class="sxs-lookup"><span data-stu-id="c0008-182">id</span></span>|<span data-ttu-id="c0008-183">String</span><span class="sxs-lookup"><span data-stu-id="c0008-183">String</span></span>|<span data-ttu-id="c0008-p104">Geben Sie diesen Parameter für jede Eigenschaft in der **multiValueExtendedProperties**-Sammlung an, um die Eigenschaft zu identifizieren. Der Parameter muss einem der unterstützten Formate entsprechen. Weitere Informationen finden Sie unter [Outlook extended properties overview](../resources/extended-properties-overview.md) (Überblick über erweiterte Outlook-Eigenschaften). Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c0008-p104">For each property in the **multiValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="c0008-188">value</span><span class="sxs-lookup"><span data-stu-id="c0008-188">value</span></span>|<span data-ttu-id="c0008-189">string</span><span class="sxs-lookup"><span data-stu-id="c0008-189">string</span></span>|<span data-ttu-id="c0008-p105">Geben Sie für jede Eigenschaft in der **multiValueExtendedProperties**-Sammlung den Eigenschaftswert an. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c0008-p105">For each property in the **multiValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="c0008-192">Beim Erstellen einer erweiterten Eigenschaft in eine _neue_ Instanz der Ressource, zusätzlich zu der neuen **MultiValueExtendedProperties** Auflistung bieten Sie eine JSON-Darstellung, wie diese Ressource Instanz sowie (d. h., eine [Nachricht](../resources/message.md), [mailFolder ](../resources/mailfolder.md), [Ereignis](../resources/event.md)usw..).</span><span class="sxs-lookup"><span data-stu-id="c0008-192">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueExtendedProperties** collection, provide a JSON representation of that resource instance as well (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.).</span></span>


## <a name="response"></a><span data-ttu-id="c0008-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0008-193">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="c0008-194">Antwortcode</span><span class="sxs-lookup"><span data-stu-id="c0008-194">Response code</span></span>
<span data-ttu-id="c0008-195">Ist die Operation zur Erstellung einer erweiterten Eigenschaft in einer neuen Ressourceninstanz erfolgreich, wird `201 Created` zurückgegeben. Ausnahme: In einem neuen Gruppenbeitrag kann die Operation je nach verwendeter Methode `200 OK` oder `202 Accepted` zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="c0008-195">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="c0008-196">Eine erfolgreiche Erstellungsoperation in einer vorhandenen Ressourceninstanz gibt `200 OK` zurück.</span><span class="sxs-lookup"><span data-stu-id="c0008-196">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="c0008-197">Antworttext</span><span class="sxs-lookup"><span data-stu-id="c0008-197">Response body</span></span>

<span data-ttu-id="c0008-p106">Für alle unterstützten Ressourcen außer [Gruppenbeiträge](../resources/post.md) gilt: Wenn Sie eine erweiterte Eigenschaft erstellen, enthält die Antwort nur die neue oder bereits vorhandene Instanz, nicht jedoch die neue erweiterte Eigenschaft. Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie die um die erweiterte Eigenschaft erweiterte Instanz abrufen](../api/multivaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="c0008-p106">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty_get.md).</span></span>

<span data-ttu-id="c0008-p107">Beim Erstellen einer erweiterten Eigenschaft in einem _neuen_ Gruppenbeitrag enthält die Antwort nur einen Antwortcode, nicht aber den neuen Beitrag oder die erweiterte Eigenschaft. In bereits vorhandenen Gruppenbeiträgen können Sie keine erweiterten Eigenschaften erstellen.</span><span class="sxs-lookup"><span data-stu-id="c0008-p107">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="c0008-202">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0008-202">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="c0008-203">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="c0008-203">Request 1</span></span>

<span data-ttu-id="c0008-p108">Im ersten Beispiel wird mit einer einzigen POST-Operation eine mehrwertige erweiterte Eigenschaft in einem neuen Ereignis erstellt. Abgesehen von den Eigenschaften, die Sie normalerweise für ein neues Ereignis definieren würden, enthält der Anforderungstext die **multiValueExtendedProperties**-Sammlung. Diese wiederum enthält eine erweiterte Eigenschaft. Der Anforderungstext enthält die folgenden Parameter für diese mehrwertige erweiterte Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="c0008-p108">The first example creates a multi-value extended property in a new event all in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **multiValueExtendedProperties** collection which contains one extended property. The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="c0008-207">**id**: Dieser Parameter definiert die Eigenschaft als ein Array von Zeichenfolgen mit der angegebenen GUID und dem Namen `Recreation`.</span><span class="sxs-lookup"><span data-stu-id="c0008-207">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span> 
- <span data-ttu-id="c0008-208">**value**: Dieser Parameter definiert `Recreation` als ein Array von 3 Zeichenfolgewerten, `["Food", "Hiking", "Swimming"]`.</span><span class="sxs-lookup"><span data-stu-id="c0008-208">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>
 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-Type: application/json

{
  "subject": "Family reunion",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together this Thanksgiving!"
  },
  "start": {
      "dateTime": "2015-11-26T09:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-29T21:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    },
    {
      "emailAddress": {
        "address": "Lauren@contoso.com",
        "name": "Lauren Solis"
      },
      "type": "Required"
    }
  ],
  "multiValueExtendedProperties": [
     {
           "id":"StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
           "value": ["Food", "Hiking", "Swimming"]
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="c0008-209">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="c0008-209">Response 1</span></span>

<span data-ttu-id="c0008-p109">Eine erfolgreiche Antwort wird mit dem Antwortcode `HTTP 201 Created` gekennzeichnet und enthält das neue Ereignis im Antworttext, ähnlich wie die Antwort, die zurückgegeben wird, wenn Sie [nur ein Ereignis erstellen](../api/user_post_events.md). Die Antwort enthält keine neu erstellten erweiterten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="c0008-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user_post_events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="c0008-212">Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie das um die erweiterte Eigenschaft erweiterte Ereignis abrufen](../api/multivaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="c0008-212">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty_get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="c0008-213">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="c0008-213">Request 2</span></span>

<span data-ttu-id="c0008-p110">Das zweite Beispiel erstellt eine mehrwertige erweiterte Eigenschaft für die angegebene Nachricht. Diese erweiterte Eigenschaft ist das einzige Element in der **multiValueExtendedProperties**-Sammlung. Der Anforderungstext enthält die folgenden Parameter für diese erweiterte Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="c0008-p110">The second example creates one multi-value extended property for the specified message. That extended property is the only element in the **multiValueExtendedProperties** collection. The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="c0008-217">**id**: Dieser Parameter definiert die Eigenschaft als ein Array von Zeichenfolgen mit der angegebenen GUID und dem Namen `Palette`.</span><span class="sxs-lookup"><span data-stu-id="c0008-217">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="c0008-218">**value**: Dieser Parameter definiert `Palette` als ein Array von 3 Zeichenfolgewerten, `["Green", "Aqua", "Blue"]`.</span><span class="sxs-lookup"><span data-stu-id="c0008-218">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_as77AACHsLrBBBA=')

Content-Type: application/json

{
  "multiValueExtendedProperties": [
      {
         "id":"StringArray {66f5a359-4659-4830-9070-00049ec6ac6e} Name Palette",
         "value":["Green", "Aqua", "Blue"]
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="c0008-219">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="c0008-219">Response 2</span></span>

<span data-ttu-id="c0008-p111">Eine erfolgreiche Antwort wird mit dem Antwortcode `HTTP 200 OK` gekennzeichnet und enthält die angegebene Nachricht im Antworttext, ähnlich wie die Antwort, die zurückgegeben wird, wenn Sie [eine Nachricht aktualisieren](../api/message_update.md). Die Antwort enthält nicht die neu erstellte erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="c0008-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message_update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="c0008-222">Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie die um die erweiterte Eigenschaft erweiterte Nachricht abrufen](../api/multivaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="c0008-222">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty_get.md).</span></span>


<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->




