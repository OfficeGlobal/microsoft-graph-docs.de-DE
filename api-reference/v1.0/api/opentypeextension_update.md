# <a name="update-open-extension"></a><span data-ttu-id="9703b-101">Datenerweiterung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9703b-101">Update open extension</span></span>

<span data-ttu-id="9703b-102">Aktualisieren Sie eine offene Erweiterung ([openTypeExtension](../resources/openTypeExtension.md)-Objekt) mit den Eigenschaften im Anforderungsheader:</span><span class="sxs-lookup"><span data-stu-id="9703b-102">Update an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="9703b-103">Wenn eine Eigenschaft im Anforderungsheader mit dem Name einer vorhandenen Eigenschaft in der Erweiterung übereinstimmt, werden die Daten in die Erweiterung aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="9703b-103">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="9703b-104">Andernfalls werden die Eigenschaft und die entsprechenden Daten zur Erweiterung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="9703b-104">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="9703b-105">Die Daten in einer Erweiterung können Grundtypen oder Arrays von Grundtypen sein.</span><span class="sxs-lookup"><span data-stu-id="9703b-105">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

## <a name="permissions"></a><span data-ttu-id="9703b-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9703b-106">Permissions</span></span>

<span data-ttu-id="9703b-p101">Zum Aufrufen dieser API ist eine der folgenden Berechtigungen erforderlich (je nach dem Typ der Ressource, in der die Erweiterung erstellt wurde): Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9703b-p101">One of the following permissions is required to call this API, depending on the resource that the extension was created in. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9703b-109">**Unterstützte Ressource**</span><span class="sxs-lookup"><span data-stu-id="9703b-109">**Supported resource**</span></span>|<span data-ttu-id="9703b-110">**Berechtigung**</span><span class="sxs-lookup"><span data-stu-id="9703b-110">**Permission**</span></span>|<span data-ttu-id="9703b-111">**Unterstützte Ressource**</span><span class="sxs-lookup"><span data-stu-id="9703b-111">**Supported resource**</span></span>|<span data-ttu-id="9703b-112">**Berechtigung**</span><span class="sxs-lookup"><span data-stu-id="9703b-112">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="9703b-113">device</span><span class="sxs-lookup"><span data-stu-id="9703b-113">device</span></span>](../resources/device.md) | <span data-ttu-id="9703b-114">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9703b-114">Device.ReadWrite.All</span></span> | [<span data-ttu-id="9703b-115">event</span><span class="sxs-lookup"><span data-stu-id="9703b-115">event</span></span>](../resources/event.md) | <span data-ttu-id="9703b-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9703b-116">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="9703b-117">group</span><span class="sxs-lookup"><span data-stu-id="9703b-117">group</span></span>](../resources/group.md) | <span data-ttu-id="9703b-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9703b-118">Group.ReadWrite.All</span></span> | [<span data-ttu-id="9703b-119">group event</span><span class="sxs-lookup"><span data-stu-id="9703b-119">group event</span></span>](../resources/event.md) | <span data-ttu-id="9703b-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9703b-120">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="9703b-121">group post</span><span class="sxs-lookup"><span data-stu-id="9703b-121">group post</span></span>](../resources/post.md) | <span data-ttu-id="9703b-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9703b-122">Group.ReadWrite.All</span></span> | [<span data-ttu-id="9703b-123">message</span><span class="sxs-lookup"><span data-stu-id="9703b-123">message</span></span>](../resources/message.md) | <span data-ttu-id="9703b-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9703b-124">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="9703b-125">organization</span><span class="sxs-lookup"><span data-stu-id="9703b-125">organization</span></span>](../resources/organization.md) | <span data-ttu-id="9703b-126">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9703b-126">Directory.AccessAsUser.All</span></span> | [<span data-ttu-id="9703b-127">personal contact</span><span class="sxs-lookup"><span data-stu-id="9703b-127">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="9703b-128">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9703b-128">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="9703b-129">user</span><span class="sxs-lookup"><span data-stu-id="9703b-129">user</span></span>](../resources/user.md) | <span data-ttu-id="9703b-130">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9703b-130">Directory.AccessAsUser.All</span></span> | | |

## <a name="http-request"></a><span data-ttu-id="9703b-131">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9703b-131">HTTP request</span></span>
<span data-ttu-id="9703b-132">In der Anforderung geben Sie die Ressourceninstanz an, spezifizieren in der Navigationseigenschaft **extensions** dieser Instanz die Erweiterung und wenden anschließend den Befehl `PATCH` auf diese Erweiterungsinstanz an.</span><span class="sxs-lookup"><span data-stu-id="9703b-132">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/extensions/{extensionId}
PATCH /groups/{id}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
PATCH /organization/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/extensions/{extensionId}
```

><span data-ttu-id="9703b-p102">**Hinweis:** Die obige Syntax zeigt mehrere häufig verwendete Möglichkeiten zum Identifizieren einer Ressourceninstanz, um eine Erweiterung darin zu aktualisieren. Alle anderen Syntaxen, mit denen Sie diese Ressourceninstanzen identifizieren können, unterstützen das Aktualisieren offener Erweiterungen darin in einer ähnlichen Weise.</span><span class="sxs-lookup"><span data-stu-id="9703b-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it. All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="9703b-135">Im Abschnitt [Anforderungstext](#request-body) wird beschrieben, wie Sie benutzerdefinierte Daten zur Änderung oder Ergänzung der Erweiterung in den Anforderungstext einschließen können.</span><span class="sxs-lookup"><span data-stu-id="9703b-135">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>


## <a name="parameters"></a><span data-ttu-id="9703b-136">Parameter</span><span class="sxs-lookup"><span data-stu-id="9703b-136">Parameters</span></span>
|<span data-ttu-id="9703b-137">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="9703b-137">**Parameter**</span></span>|<span data-ttu-id="9703b-138">**Typ**</span><span class="sxs-lookup"><span data-stu-id="9703b-138">**Type**</span></span>|<span data-ttu-id="9703b-139">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="9703b-139">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9703b-140">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="9703b-140">_URL parameters_</span></span>|
|<span data-ttu-id="9703b-141">id</span><span class="sxs-lookup"><span data-stu-id="9703b-141">id</span></span>|<span data-ttu-id="9703b-142">string</span><span class="sxs-lookup"><span data-stu-id="9703b-142">string</span></span>|<span data-ttu-id="9703b-p103">Ein eindeutiger Bezeichner für eine Instanz der entsprechenden Sammlung. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="9703b-p103">A unique identifier for an instance of the corresponding collection. Required.</span></span>|
|<span data-ttu-id="9703b-145">extensionId</span><span class="sxs-lookup"><span data-stu-id="9703b-145">extensionId</span></span>|<span data-ttu-id="9703b-146">string</span><span class="sxs-lookup"><span data-stu-id="9703b-146">string</span></span>|<span data-ttu-id="9703b-p104">Dies kann ein Erweiterungsname sein. Der Erweiterungsname ist ein eindeutiger Textbezeichner einer Erweiterung oder ein vollqualifizierter Name, der den Erweiterungstyp und den eindeutigen Textbezeichner verkettet. Der vollqualifizierte Name wird beim Erstellen der Erweiterung in der `id`-Eigenschaft zurückgegeben. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="9703b-p104">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="9703b-150">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9703b-150">Request headers</span></span>
| <span data-ttu-id="9703b-151">Name</span><span class="sxs-lookup"><span data-stu-id="9703b-151">Name</span></span>       | <span data-ttu-id="9703b-152">Wert</span><span class="sxs-lookup"><span data-stu-id="9703b-152">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="9703b-153">Authorization</span><span class="sxs-lookup"><span data-stu-id="9703b-153">Authorization</span></span> | <span data-ttu-id="9703b-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9703b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9703b-156">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9703b-156">Content-Type</span></span> | <span data-ttu-id="9703b-157">application/json</span><span class="sxs-lookup"><span data-stu-id="9703b-157">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9703b-158">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9703b-158">Request body</span></span>

<span data-ttu-id="9703b-p106">Stellen Sie den JSON-Text eines [openTypeExtension](../resources/openTypeExtension.md)-Objekts mit den folgenden erforderlichen Name-Wert-Paaren und allen benutzerdefinierten Daten bereit, die geändert oder zu dieser Erweiterung hinzugefügt werden sollen. Die Daten in der JSON-Nutzlast können Grundtypen oder Arrays von Grundtypen sein.</span><span class="sxs-lookup"><span data-stu-id="9703b-p106">Provide a JSON body of an [openTypeExtension](../resources/openTypeExtension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="9703b-161">Name</span><span class="sxs-lookup"><span data-stu-id="9703b-161">Name</span></span>       | <span data-ttu-id="9703b-162">Wert</span><span class="sxs-lookup"><span data-stu-id="9703b-162">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="9703b-163">@odata.type</span><span class="sxs-lookup"><span data-stu-id="9703b-163">@odata.type</span></span> | <span data-ttu-id="9703b-164">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="9703b-164">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="9703b-165">extensionName</span><span class="sxs-lookup"><span data-stu-id="9703b-165">extensionName</span></span> | <span data-ttu-id="9703b-166">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="9703b-166">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="9703b-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="9703b-167">Response</span></span>

<span data-ttu-id="9703b-168">Bei Erfolg gibt diese Methode den Antwortcode `200 OK` und das aktualisierte [openTypeExtension](../resources/openTypeExtension.md)-Objekt zurück.</span><span class="sxs-lookup"><span data-stu-id="9703b-168">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/openTypeExtension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="9703b-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9703b-169">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="9703b-170">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="9703b-170">Request 1</span></span>

<span data-ttu-id="9703b-p107">Im ersten Beispiel wird gezeigt, wie eine Erweiterung in einer Nachricht aktualisiert wird. Die Erweiterung wird anfänglich durch die folgende JSON-Nutzlast dargestellt:</span><span class="sxs-lookup"><span data-stu-id="9703b-p107">The first example shows how to update an extension in a message. The extension is initially represented by the following JSON payload:</span></span>

<!-- { "blockType": "ignored" } -->
```http
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

<span data-ttu-id="9703b-173">Sie können anhand des Namens auf die Erweiterung verweisen:</span><span class="sxs-lookup"><span data-stu-id="9703b-173">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="9703b-174">Sie können auch anhand des vollqualifizierten Namens auf die Erweiterung verweisen:</span><span class="sxs-lookup"><span data-stu-id="9703b-174">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```

<span data-ttu-id="9703b-175">Sie können die Beispielanforderung und den folgenden Anforderungstext verwenden, um die oben genannte Erweiterung auf folgende Weise zu aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="9703b-175">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="9703b-176">Durch Ändern des `companyName` von `Wingtip Toys` zu `Wingtip Toys (USA)`</span><span class="sxs-lookup"><span data-stu-id="9703b-176">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="9703b-177">Durch Ändern des `dealValue` von `500050` zu `500100`</span><span class="sxs-lookup"><span data-stu-id="9703b-177">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="9703b-178">Durch Hinzufügen neuer Daten als die benutzerdefinierte `updated`-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9703b-178">Adding new data as the custom property `updated`</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.type": "Microsoft.Graph.OpenTypeExtension",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": "500100",
    "expirationDate": "2015-12-03T10:00:00.000Z",
    "updated": "2015-10-29T11:00:00.000Z"
} 
```


#### <a name="response-1"></a><span data-ttu-id="9703b-179">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="9703b-179">Response 1</span></span>

<span data-ttu-id="9703b-180">Es wird unabhängig von der zur Referenzierung der Erweiterung verwendeten Methode jeweils die gleiche Antwort zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9703b-180">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": 500100,
    "expirationDate": "2015-12-03T10:00:00Z",
    "updated": "2015-10-29T11:00:00.000Z"
}
```

****

#### <a name="request-2"></a><span data-ttu-id="9703b-181">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="9703b-181">Request 2</span></span>

<span data-ttu-id="9703b-p108">Im zweiten Beispiel wird gezeigt, wie eine Erweiterung in einem Gruppenbeitrag aktualisiert wird. Die Erweiterung wird anfänglich durch die folgende JSON-Nutzlast mit einem `expirationDate`-Wert von `2015-07-03T13:04:00Z` dargestellt:</span><span class="sxs-lookup"><span data-stu-id="9703b-p108">The second example shows how to update an extension in a group post. The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<span data-ttu-id="9703b-184">Im Folgenden werden die Anforderung und Anforderungstext zum Ändern von `expirationDate` zu `2016-07-30T11:00:00Z` dargestellt:</span><span class="sxs-lookup"><span data-stu-id="9703b-184">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>

<!-- {
  "blockType": "request",
  "name": "update_opentypeextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate')
Content-type: application/json

{
   "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
   "extensionName": "Com.Contoso.Estimate",
   "companyName": "Contoso",
   "expirationDate": "2016-07-30T11:00:00.000Z",
   "DealValue": 1010100,
   "topPicks": [
       "Employees only",
       "Add spouse or guest",
       "Add family"
    ]
}
```

#### <a name="response-2"></a><span data-ttu-id="9703b-185">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="9703b-185">Response 2</span></span>

<span data-ttu-id="9703b-186">Im Folgenden wird die Antwort des zweiten Beispiels dargestellt, welche das aktualisierte `expirationDate`-Element in die Erweiterung zeigt.</span><span class="sxs-lookup"><span data-stu-id="9703b-186">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

<!-- {  
  "blockType": "response",  
  "truncated": true,  
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
    "expirationDate": "2016-07-30T11:00:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
} -->
