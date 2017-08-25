# <a name="create-single-value-extended-property"></a><span data-ttu-id="f2e78-101">Erweiterte einwertige Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="f2e78-101">Create single-value extended property</span></span>

<span data-ttu-id="f2e78-102">Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource.</span><span class="sxs-lookup"><span data-stu-id="f2e78-102">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="f2e78-103">Die folgenden Benutzerressourcen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="f2e78-103">The following user resources are supported:</span></span>

- [<span data-ttu-id="f2e78-104">message</span><span class="sxs-lookup"><span data-stu-id="f2e78-104">message</span></span>](../resources/message.md)
- [<span data-ttu-id="f2e78-105">mailFolder</span><span class="sxs-lookup"><span data-stu-id="f2e78-105">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="f2e78-106">event</span><span class="sxs-lookup"><span data-stu-id="f2e78-106">event</span></span>](../resources/event.md)
- [<span data-ttu-id="f2e78-107">calendar</span><span class="sxs-lookup"><span data-stu-id="f2e78-107">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="f2e78-108">contact</span><span class="sxs-lookup"><span data-stu-id="f2e78-108">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="f2e78-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="f2e78-109">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="f2e78-110">Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="f2e78-110">As well as the following group resources:</span></span>

- <span data-ttu-id="f2e78-111">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="f2e78-111">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="f2e78-112">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="f2e78-112">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="f2e78-113">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="f2e78-113">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="f2e78-114">Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="f2e78-114">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2e78-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f2e78-115">Permissions</span></span>
<span data-ttu-id="f2e78-p101">Zum Aufrufen dieser API ist eine der folgenden Berechtigungen erforderlich (je nachdem, in welchem Typ von Ressource Sie die erweiterte Eigenschaft erstellen möchten): Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f2e78-p101">One of the following permissions is required to call this API, depending on the resource you're creating the extended property in. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="f2e78-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2e78-118">Mail.ReadWrite</span></span>
- <span data-ttu-id="f2e78-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2e78-119">Calendars.ReadWrite</span></span>
- <span data-ttu-id="f2e78-120">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2e78-120">Contacts.ReadWrite</span></span>
- <span data-ttu-id="f2e78-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2e78-121">Group.ReadWrite.All</span></span>
 
## <a name="http-request"></a><span data-ttu-id="f2e78-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2e78-122">HTTP request</span></span>
<span data-ttu-id="f2e78-123">Sie können erweiterte Eigenschaften in einer neuen oder vorhandenen Ressourceninstanz erstellen.</span><span class="sxs-lookup"><span data-stu-id="f2e78-123">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="f2e78-p102">Verwenden Sie zum Erstellen einer oder mehrerer erweiterter Eigenschaften in einer _neuen_ Ressourceninstanz die gleiche REST-Anforderung wie zum Erstellen der Instanz, und fügen Sie die Eigenschaften der neuen Ressourceninstanz _und die erweiterte Eigenschaft_ zum Anforderungstext hinzu. Beachten Sie, dass für einige Ressourcen die Erstellung auf mehrere Weisen erfolgen kann. Weitere Informationen zum Erstellen dieser Ressourceninstanzen finden Sie unter den entsprechenden Themen zum Erstellen einer [Nachricht](../resources/message.md), eines [MailFolder](../api/user_post_mailfolders.md)-Elements, [Ereignisses](../api/user_post_events.md), [Kalenders](../api/user_post_calendars.md), [Kontakts](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md)-Elements, [Gruppenereignisses](../api/group_post_events.md) und eines [Gruppenbeitrags](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="f2e78-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user_post_mailfolders.md), [event](../api/user_post_events.md), [calendar](../api/user_post_calendars.md), [contact](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md), [group event](../api/group_post_events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="f2e78-127">So sieht die Syntax der Anforderungen aus:</span><span class="sxs-lookup"><span data-stu-id="f2e78-127">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="f2e78-128">Um eine oder mehrere erweiterte Eigenschaften in einer vorhandenen Ressourceninstanz zu erstellen,müssen Sie die Instanz in der Anforderung angeben und die erweiterte-Eigenschaft zum Anforderungstext hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="f2e78-128">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="f2e78-129">**Hinweis:** Sie können keine erweiterte Eigenschaft in einem vorhandenen Gruppenbeitrag erstellen.</span><span class="sxs-lookup"><span data-stu-id="f2e78-129">**Note** You cannot create an extended property in an existing group post.</span></span>

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


## <a name="parameters"></a><span data-ttu-id="f2e78-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="f2e78-130">Parameters</span></span>
|<span data-ttu-id="f2e78-131">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="f2e78-131">**Parameter**</span></span>|<span data-ttu-id="f2e78-132">**Typ**</span><span class="sxs-lookup"><span data-stu-id="f2e78-132">**Type**</span></span>|<span data-ttu-id="f2e78-133">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="f2e78-133">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f2e78-134">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="f2e78-134">_URL parameters_</span></span>|
|<span data-ttu-id="f2e78-135">id</span><span class="sxs-lookup"><span data-stu-id="f2e78-135">id</span></span>|<span data-ttu-id="f2e78-136">string</span><span class="sxs-lookup"><span data-stu-id="f2e78-136">string</span></span>|<span data-ttu-id="f2e78-p103">Ein eindeutiger Bezeichner für ein Objekt in der entsprechenden Sammlung. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f2e78-p103">A unique identifier for an object in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="f2e78-139">_Body parameters_</span><span class="sxs-lookup"><span data-stu-id="f2e78-139">_Body parameters_</span></span>|
|<span data-ttu-id="f2e78-140">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="f2e78-140">singleValueExtendedProperties</span></span>|<span data-ttu-id="f2e78-141">[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f2e78-141">[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) collection</span></span>| <span data-ttu-id="f2e78-142">Ein Array aus erweiterten mehrwertigen Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="f2e78-142">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="f2e78-143">id</span><span class="sxs-lookup"><span data-stu-id="f2e78-143">id</span></span>|<span data-ttu-id="f2e78-144">String</span><span class="sxs-lookup"><span data-stu-id="f2e78-144">String</span></span>|<span data-ttu-id="f2e78-p104">Geben Sie diese für jede Eigenschaft in der **singleValueExtendedProperties**-Sammlung an, um die Eigenschaft zu identifizieren. Sie muss eins der unterstützten Formate aufweisen. Weitere Informationen finden Sie unter [Überblick über erweiterte Eigenschaften in Outlook](../resources/extended-properties-overview.md). Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f2e78-p104">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="f2e78-149">value</span><span class="sxs-lookup"><span data-stu-id="f2e78-149">value</span></span>|<span data-ttu-id="f2e78-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f2e78-150">string</span></span>|<span data-ttu-id="f2e78-p105">Geben Sie für jede Eigenschaft in der **singleValueExtendedProperties**-Sammlung den Eigenschaftswert an. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f2e78-p105">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="f2e78-153">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f2e78-153">Request headers</span></span>
| <span data-ttu-id="f2e78-154">Name</span><span class="sxs-lookup"><span data-stu-id="f2e78-154">Name</span></span>       | <span data-ttu-id="f2e78-155">Wert</span><span class="sxs-lookup"><span data-stu-id="f2e78-155">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="f2e78-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2e78-156">Authorization</span></span> | <span data-ttu-id="f2e78-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f2e78-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2e78-159">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f2e78-159">Content-Type</span></span> | <span data-ttu-id="f2e78-160">application/json</span><span class="sxs-lookup"><span data-stu-id="f2e78-160">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2e78-161">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f2e78-161">Request body</span></span>

<span data-ttu-id="f2e78-162">Stellen Sie einen JSON-Text für jedes [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md)-Objekt in der **singleValueExtendedProperties**-Sammlungseigenschaft der Ressourceninstanz bereit.</span><span class="sxs-lookup"><span data-stu-id="f2e78-162">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

<span data-ttu-id="f2e78-163">Beim Erstellen einer erweiterten Eigenschaft in einer _neuen_ Ressourceninstanz müssen Sie zusätzlich zu der neuen **singleValueExtendedProperties**-Sammlung eine JSON-Darstellung der betreffenden Ressourceninstanz spezifizieren (d. h. eine Ressource des Typs [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md) usw.).</span><span class="sxs-lookup"><span data-stu-id="f2e78-163">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="f2e78-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2e78-164">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="f2e78-165">Antwortcode</span><span class="sxs-lookup"><span data-stu-id="f2e78-165">Response code</span></span>
<span data-ttu-id="f2e78-166">Ist die Operation zur Erstellung einer erweiterten Eigenschaft in einer neuen Ressourceninstanz erfolgreich, wird `201 Created` zurückgegeben. Ausnahme: In einem neuen Gruppenbeitrag kann die Operation je nach verwendeter Methode `200 OK` oder `202 Accepted` zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="f2e78-166">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="f2e78-167">Eine erfolgreiche Erstellungsoperation in einer vorhandenen Ressourceninstanz gibt `200 OK` zurück.</span><span class="sxs-lookup"><span data-stu-id="f2e78-167">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="f2e78-168">Antworttext</span><span class="sxs-lookup"><span data-stu-id="f2e78-168">Response body</span></span>

<span data-ttu-id="f2e78-p107">Wenn Sie eine erweiterte Eigenschaft erstellen, enthält die Antwort nur die neue oder bereits vorhandene Instanz, nicht jedoch die neue erweiterte Eigenschaft. Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie die um die erweiterte Eigenschaft erweiterte Instanz abrufen](../api/singlevaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="f2e78-p107">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>

<span data-ttu-id="f2e78-171">Beim Erstellen einer erweiterten Eigenschaft in einem _neuen_ [Gruppenbeitrag](../resources/post.md) durch Antwort auf einen Thread oder Beitrag enthält die Antwort nur einen Antwortcode, nicht aber den neuen Beitrag oder die erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="f2e78-171">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="f2e78-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f2e78-172">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="f2e78-173">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="f2e78-173">Request 1</span></span>

<span data-ttu-id="f2e78-p108">Im ersten Beispiel wird mit einer einzigen POST-Operation ein neuer Ereignis und eine einwertige erweiterte Eigenschaft erstellt. Abgesehen von den Eigenschaften, die Sie normalerweise für ein neues Ereignis definieren würden, enthält der Anforderungstext die **singleValueExtendedProperties**-Sammlung. Diese wiederum enthält eine erweiterte einwertige Eigenschaft und folgende Angaben für die Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="f2e78-p108">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>
- <span data-ttu-id="f2e78-176">**ID** Gibt den Eigenschaftstyp als `String`, die GUID und die Eigenschaft mit dem Namen `Fun` an.</span><span class="sxs-lookup"><span data-stu-id="f2e78-176">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="f2e78-177">**Wert** Gibt `Food` als den Wert der `Fun`-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="f2e78-177">**value** specifies `Food` as the value of the `Fun` property.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-Type: application/json

{
  "subject": "Celebrate Thanksgiving",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together!"
  },
  "start": {
      "dateTime": "2015-11-26T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-26T23:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    }
  ],
  "singleValueExtendedProperties": [
     {
           "id":"String {66f5a359-4659-4830-9070-00040ec6ac6e} Name Fun",
           "value":"Food"
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="f2e78-178">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="f2e78-178">Response 1</span></span>

<span data-ttu-id="f2e78-p109">Eine erfolgreiche Antwort wird mit dem Antwortcode `HTTP 201 Created` gekennzeichnet und enthält das neue Ereignis im Antworttext, ähnlich wie die Antwort, die zurückgegeben wird, wenn Sie [nur ein Ereignis erstellen](../api/user_post_events.md). Die Antwort enthält keine neu erstellten erweiterten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="f2e78-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user_post_events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="f2e78-181">Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie das um die erweiterte Eigenschaft erweiterte Ereignis abrufen](../api/singlevaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="f2e78-181">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="f2e78-182">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="f2e78-182">Request 2</span></span>

<span data-ttu-id="f2e78-p110">Das zweite Beispiel erstellt eine einwertige erweiterte Eigenschaft für die angegebene vorhandene Nachricht. Diese erweiterte Eigenschaft ist das einzige Element in dem **singleValueExtendedProperties**-Array. Der Anforderungstext enthält die folgenden Parameter für diese erweiterte Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="f2e78-p110">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="f2e78-186">**ID** Gibt den Eigenschaftstyp als `String`, die GUID und die `Color`-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="f2e78-186">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="f2e78-187">**Wert** Gibt `Green` als den Wert der `Color`-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="f2e78-187">**value** specifies `Green` as the value of the `Color` property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')

Content-Type: application/json

{
  "singleValueExtendedProperties": [
      {
         "id":"String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
         "value":"Green"
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="f2e78-188">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="f2e78-188">Response 2</span></span>

<span data-ttu-id="f2e78-p111">Eine erfolgreiche Antwort wird mit dem Antwortcode `HTTP 200 OK` gekennzeichnet und enthält die angegebene Nachricht im Antworttext, ähnlich wie die Antwort, die zurückgegeben wird, wenn Sie [eine Nachricht aktualisieren](../api/message_update.md). Die Antwort enthält nicht die neu erstellte erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="f2e78-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message_update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="f2e78-191">Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie die um die erweiterte Eigenschaft erweiterte Nachricht abrufen](../api/singlevaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="f2e78-191">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>

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

