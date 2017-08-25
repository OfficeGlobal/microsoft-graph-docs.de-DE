# <a name="create-open-extension"></a><span data-ttu-id="b8418-101">Datenerweiterung erstellen</span><span class="sxs-lookup"><span data-stu-id="b8418-101">Create open extension</span></span>

<span data-ttu-id="b8418-102">Mit dieser API können Sie offene Erweiterungen (Objekte des Typs [openTypeExtension](../resources/openTypeExtension.md)) erstellen und einer neuen oder bereits vorhandenen Ressourceninstanz benutzerdefinierte Eigenschaften hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="b8418-102">Create an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) and add custom properties in a new or existing instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b8418-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b8418-103">Permissions</span></span>

<span data-ttu-id="b8418-p101">Zum Aufrufen dieser API ist eine der folgenden Berechtigungen erforderlich (je nachdem, in welchem Typ von Ressource Sie die Erweiterung erstellen möchten): Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b8418-p101">One of the following permissions is required to call this API, depending on the resource you're creating the extension in. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b8418-106">**Unterstützte Ressource**</span><span class="sxs-lookup"><span data-stu-id="b8418-106">**Supported resource**</span></span>|<span data-ttu-id="b8418-107">**Berechtigung**</span><span class="sxs-lookup"><span data-stu-id="b8418-107">**Permission**</span></span>|<span data-ttu-id="b8418-108">**Unterstützte Ressource**</span><span class="sxs-lookup"><span data-stu-id="b8418-108">**Supported resource**</span></span>|<span data-ttu-id="b8418-109">**Berechtigung**</span><span class="sxs-lookup"><span data-stu-id="b8418-109">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="b8418-110">device</span><span class="sxs-lookup"><span data-stu-id="b8418-110">device</span></span>](../resources/device.md) | <span data-ttu-id="b8418-111">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8418-111">Device.ReadWrite.All</span></span> | [<span data-ttu-id="b8418-112">event</span><span class="sxs-lookup"><span data-stu-id="b8418-112">event</span></span>](../resources/event.md) | <span data-ttu-id="b8418-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8418-113">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="b8418-114">group</span><span class="sxs-lookup"><span data-stu-id="b8418-114">group</span></span>](../resources/group.md) | <span data-ttu-id="b8418-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8418-115">Group.ReadWrite.All</span></span> | [<span data-ttu-id="b8418-116">group event</span><span class="sxs-lookup"><span data-stu-id="b8418-116">group event</span></span>](../resources/event.md) | <span data-ttu-id="b8418-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8418-117">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="b8418-118">group post</span><span class="sxs-lookup"><span data-stu-id="b8418-118">group post</span></span>](../resources/post.md) | <span data-ttu-id="b8418-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8418-119">Group.ReadWrite.All</span></span> | [<span data-ttu-id="b8418-120">message</span><span class="sxs-lookup"><span data-stu-id="b8418-120">message</span></span>](../resources/message.md) | <span data-ttu-id="b8418-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8418-121">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="b8418-122">organization</span><span class="sxs-lookup"><span data-stu-id="b8418-122">organization</span></span>](../resources/organization.md) | <span data-ttu-id="b8418-123">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b8418-123">Directory.AccessAsUser.All</span></span> | [<span data-ttu-id="b8418-124">personal contact</span><span class="sxs-lookup"><span data-stu-id="b8418-124">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="b8418-125">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8418-125">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="b8418-126">user</span><span class="sxs-lookup"><span data-stu-id="b8418-126">user</span></span>](../resources/user.md) | <span data-ttu-id="b8418-127">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b8418-127">Directory.AccessAsUser.All</span></span> | | |
 
## <a name="http-request"></a><span data-ttu-id="b8418-128">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8418-128">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="b8418-129">Erstellen einer Erweiterung in einer neuen Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="b8418-129">Create an extension in a new resource instance</span></span>

<span data-ttu-id="b8418-130">Verwenden Sie die gleiche REST-Anforderung wie zum Erstellen der Instanz.</span><span class="sxs-lookup"><span data-stu-id="b8418-130">Use the same REST request as creating the instance.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="b8418-p102">**Hinweis:** Die obige Syntax zeigt mehrere häufig verwendete Möglichkeiten zum Erstellen der unterstützten Ressourceninstanzen. Alle anderen POST-Syntaxen, mit denen Sie diese Ressourceninstanzen erstellen können, unterstützen das Erstellen offener Erweiterungen darin in einer ähnlichen Weise.</span><span class="sxs-lookup"><span data-stu-id="b8418-p102">**Note:** The above syntax shows some common ways to create the supported resource instances. All other POST syntax that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="b8418-133">Im Abschnitt [Anforderungstext](#request-body) ist beschrieben, wie Sie die Eigenschaften der neuen Ressourceninstanz _und die Erweiterung_ in den Anforderungstext einschließen können.</span><span class="sxs-lookup"><span data-stu-id="b8418-133">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="b8418-134">Erstellen einer Erweiterung in einer vorhandenen Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="b8418-134">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="b8418-135">Geben Sie die Ressourceninstanz in der Anforderung an, und wenden Sie den Befehl `POST` auf die Navigationseigenschaft **extensions** an.</span><span class="sxs-lookup"><span data-stu-id="b8418-135">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/extensions
POST /users/{id|userPrincipalName}/events/{id}/extensions
POST /groups/{id}/extensions
POST /groups/{id}/events/{id}/extensions
POST /groups/{id}/threads/{id}/posts/{id}/extensions
POST /users/{id|userPrincipalName}/messages/{id}/extensions
POST /organization/{id}/extensions
POST /users/{id|userPrincipalName}/contacts/{id}/extensions
POST /users/{id|userPrincipalName}/extensions
```

><span data-ttu-id="b8418-p103">**Hinweis:** Die obige Syntax zeigt mehrere häufig verwendete Möglichkeiten zum Identifizieren einer Ressourceninstanz, um eine Erweiterung darin zu erstellen. Alle anderen Syntaxen, mit denen Sie diese Ressourceninstanzen identifizieren können, unterstützen das Erstellen offener Erweiterungen darin in einer ähnlichen Weise.</span><span class="sxs-lookup"><span data-stu-id="b8418-p103">**Note:** The above syntax shows some common ways to identify a resource instance, in order to create an extension in it. All other syntax that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="b8418-138">Im Abschnitt [Anforderungstext](#request-body) wird beschrieben, wie Sie _die Erweiterung_ in den Anforderungstext einschließen können.</span><span class="sxs-lookup"><span data-stu-id="b8418-138">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="parameters"></a><span data-ttu-id="b8418-139">Parameter</span><span class="sxs-lookup"><span data-stu-id="b8418-139">Parameters</span></span>
|<span data-ttu-id="b8418-140">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="b8418-140">**Parameter**</span></span>|<span data-ttu-id="b8418-141">**Typ**</span><span class="sxs-lookup"><span data-stu-id="b8418-141">**Type**</span></span>|<span data-ttu-id="b8418-142">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="b8418-142">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b8418-143">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="b8418-143">_URL parameters_</span></span>|
|<span data-ttu-id="b8418-144">id</span><span class="sxs-lookup"><span data-stu-id="b8418-144">id</span></span>|<span data-ttu-id="b8418-145">string</span><span class="sxs-lookup"><span data-stu-id="b8418-145">string</span></span>|<span data-ttu-id="b8418-p104">Ein eindeutiger Bezeichner für ein Objekt in der entsprechenden Sammlung. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b8418-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="b8418-148">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8418-148">Request headers</span></span>
| <span data-ttu-id="b8418-149">Name</span><span class="sxs-lookup"><span data-stu-id="b8418-149">Name</span></span>       | <span data-ttu-id="b8418-150">Wert</span><span class="sxs-lookup"><span data-stu-id="b8418-150">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b8418-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8418-151">Authorization</span></span> | <span data-ttu-id="b8418-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b8418-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b8418-154">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8418-154">Content-Type</span></span> | <span data-ttu-id="b8418-155">application/json</span><span class="sxs-lookup"><span data-stu-id="b8418-155">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8418-156">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8418-156">Request body</span></span>

<span data-ttu-id="b8418-p106">Geben Sie den JSON-Text einer [openTypeExtension](../resources/openTypeExtension.md) an, mit den folgenden erforderlichen Name/Wert-Paaren und allen zusätzlichen benutzerdefinierten Daten. Die Daten in der JSON-Nutzlast können Grundtypen oder Arrays von Grundtypen sein.</span><span class="sxs-lookup"><span data-stu-id="b8418-p106">Provide a JSON body of an [openTypeExtension](../resources/openTypeExtension.md), with the following required name-value pairs, and any additional custom data. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="b8418-159">Name</span><span class="sxs-lookup"><span data-stu-id="b8418-159">Name</span></span>       | <span data-ttu-id="b8418-160">Wert</span><span class="sxs-lookup"><span data-stu-id="b8418-160">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b8418-161">@odata.type</span><span class="sxs-lookup"><span data-stu-id="b8418-161">@odata.type</span></span> | <span data-ttu-id="b8418-162">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="b8418-162">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="b8418-163">extensionName</span><span class="sxs-lookup"><span data-stu-id="b8418-163">extensionName</span></span> | <span data-ttu-id="b8418-164">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="b8418-164">%unique_string%</span></span> |

<span data-ttu-id="b8418-165">Beim Erstellen einer Erweiterung in einer _neuen_ Ressourceninstanz müssen Sie zusätzlich zu dem neuen **openTypeExtension**-Objekt eine JSON-Darstellung der zur Erstellung einer solchen Ressourceninstanz erforderlichen Eigenschaften angeben.</span><span class="sxs-lookup"><span data-stu-id="b8418-165">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="b8418-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8418-166">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="b8418-167">Antwortcode</span><span class="sxs-lookup"><span data-stu-id="b8418-167">Response code</span></span>
<span data-ttu-id="b8418-168">Je nach Vorgang lautet der Antwortcode `201 Created` oder `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="b8418-168">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="b8418-p107">Wenn Sie eine Erweiterung und eine Ressourceninstanz in ein und demselben Vorgang erstellen, wird bei erfolgreicher Durchführung des Vorgangs derselbe Antwortcode zurückgegeben, der auch zurückgegeben worden wäre, wenn Sie nur die Ressourceninstanz ohne die Erweiterung erstellt hätten. Weitere Informationen finden Sie in den [oben](#create-an-extension-in-a-new-resource-instance) aufgeführten Artikeln zum Thema Instanzenerstellung.</span><span class="sxs-lookup"><span data-stu-id="b8418-p107">When creating an extension in the same operation as creating a resource instance, a successful operation returns the same response code as when the operation is used to create only the resource instance without the extension. Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

#### <a name="response-body"></a><span data-ttu-id="b8418-171">Antworttext</span><span class="sxs-lookup"><span data-stu-id="b8418-171">Response body</span></span>
| <span data-ttu-id="b8418-172">Szenario</span><span class="sxs-lookup"><span data-stu-id="b8418-172">Scenario</span></span>       | <span data-ttu-id="b8418-173">Ressource</span><span class="sxs-lookup"><span data-stu-id="b8418-173">Resource</span></span>  | <span data-ttu-id="b8418-174">Antworttext</span><span class="sxs-lookup"><span data-stu-id="b8418-174">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="b8418-175">Erstellen einer Erweiterung bei gleichzeitiger expliziter Erstellung einer _neuen_ Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="b8418-175">Creating an extension while explicitly creating a _new_ resource instance</span></span> | [<span data-ttu-id="b8418-176">contact](../resources/contact.md), [event](../resources/event.md), [message</span><span class="sxs-lookup"><span data-stu-id="b8418-176">contact](../resources/contact.md), [event](../resources/event.md), [message</span></span>](../resources/message.md) | <span data-ttu-id="b8418-177">Enthält die neue Instanz, erweitert um das [openTypeExtension](../resources/openTypeExtension.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="b8418-177">Includes the new instance expanded with the [openTypeExtension](../resources/openTypeExtension.md) object.</span></span> |
| <span data-ttu-id="b8418-178">Erstellen einer Erweiterung bei gleichzeitiger impliziter Erstellung einer Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="b8418-178">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="b8418-179">post</span><span class="sxs-lookup"><span data-stu-id="b8418-179">post</span></span>](../resources/post.md) | <span data-ttu-id="b8418-180">Die Antwort enthält nur einen Antwortcode, keinen Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b8418-180">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="b8418-181">Erstellen einer Erweiterung in einer _vorhandenen_ Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="b8418-181">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="b8418-182">Alle unterstützten Ressourcen</span><span class="sxs-lookup"><span data-stu-id="b8418-182">All supported resources</span></span> | <span data-ttu-id="b8418-183">Enthält das **openTypeExtension**-Objekt.</span><span class="sxs-lookup"><span data-stu-id="b8418-183">Includes the **openTypeExtension** object.</span></span> |
 


## <a name="example"></a><span data-ttu-id="b8418-184">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8418-184">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="b8418-185">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="b8418-185">Request 1</span></span>

<span data-ttu-id="b8418-p108">Im ersten Beispiel werden mit ein und demselben Aufruf eine Nachricht und eine Erweiterung erstellt. Der Anforderungstext enthält Folgendes:</span><span class="sxs-lookup"><span data-stu-id="b8418-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="b8418-188">Die für eine neue Nachricht typischen Eigenschaften **subject**, **body** und **toRecipients**</span><span class="sxs-lookup"><span data-stu-id="b8418-188">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span> 
- <span data-ttu-id="b8418-189">Daneben die folgenden Parameter der Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="b8418-189">And for the extension:</span></span>

  - <span data-ttu-id="b8418-190">Den Typ `Microsoft.Graph.OpenTypeExtension`</span><span class="sxs-lookup"><span data-stu-id="b8418-190">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
  - <span data-ttu-id="b8418-191">Den Erweiterungsnamen „Com.Contoso.Referral“</span><span class="sxs-lookup"><span data-stu-id="b8418-191">The extension name "Com.Contoso.Referral".</span></span> 
  - <span data-ttu-id="b8418-192">Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `expirationDate` und `dealValue`</span><span class="sxs-lookup"><span data-stu-id="b8418-192">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>  

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages

{
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "You should be proud!"
  },
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com"
      }
    }
  ],
  "extensions": [
    {
      "@odata.type": "Microsoft.Graph.OpenTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="b8418-193">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="b8418-193">Response 1</span></span>

<span data-ttu-id="b8418-p109">Unten sehen Sie die Antwort für Beispiel 1. Der Antworttext enthält die Eigenschaften der neuen Nachricht sowie die folgenden Parameter der neuen Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="b8418-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="b8418-196">Die Eigenschaft **id** mit dem vollqualifizierten Namen `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`</span><span class="sxs-lookup"><span data-stu-id="b8418-196">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span> 
- <span data-ttu-id="b8418-197">Die in der Anforderung angegebene Standardeigenschaft **extensionName**</span><span class="sxs-lookup"><span data-stu-id="b8418-197">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="b8418-198">Die in der Anforderung angegebenen benutzerdefinierten Daten, gespeichert als 3 benutzerdefinierte Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b8418-198">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="b8418-p110">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8418-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')",
  "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj\"",
  "id": "AAMkAGEbs88AAB84uLuAAA=",
  "createdDateTime": "2015-10-30T03:03:43Z",
  "lastModifiedDateTime": "2015-10-30T03:03:43Z",
  "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj",
  "categories": [ ],
  "receivedDateTime": "2015-10-30T03:03:43Z",
  "sentDateTime": "2015-10-30T03:03:43Z",
  "hasAttachments": false,
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r
\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nYou should be proud!\r\n</body>\r
\n</html>\r\n"
  },
  "bodyPreview": "You should be proud!",
  "importance": "Normal",
  "parentFolderId": "AQMkAGEwAAAIBDwAAAA==",
  "sender": null,
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com",
        "name": "John Doe"
      }
    }
  ],
  "ccRecipients": [ ],
  "bccRecipients": [ ],
  "replyTo": [ ],
  "conversationId": "AAQkAGEFGugh3SVdMzzc=",
  "isDeliveryReceiptRequested": false,
  "isReadReceiptRequested": false,
  "isRead": true,
  "isDraft": true,
  "webLink": "https://outlook.office.com/owa/?
ItemID=AAMkAGEbs88AAB84uLuAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
  "inferenceClassification": "Focused",
  "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages
('AAMkAGEbs88AAB84uLuAAA%3D')/extensions",
  "extensions": [
    {
      "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
      "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
      "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```


****

##### <a name="request-2"></a><span data-ttu-id="b8418-201">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="b8418-201">Request 2</span></span>

<span data-ttu-id="b8418-p111">Das zweite Beispiel erstellt eine Erweiterung in der angegebenen Nachricht. Der Anforderungstext enthält die folgenden Parameter für die Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="b8418-p111">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="b8418-204">Den Typ `Microsoft.Graph.OpenTypeExtension`</span><span class="sxs-lookup"><span data-stu-id="b8418-204">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="b8418-205">Den Erweiterungsnamen „Com.Contoso.Referral“</span><span class="sxs-lookup"><span data-stu-id="b8418-205">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="b8418-206">Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `dealValue` und `expirationDate`</span><span class="sxs-lookup"><span data-stu-id="b8418-206">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>  

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions

{ 
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension", 
  "extensionName" : "Com.Contoso.Referral", 
  "companyName" : "Wingtip Toys", 
  "dealValue" : 500050, 
  "expirationDate" : "2015-12-03T10:00:00.000Z" 
} 
```

##### <a name="response-2"></a><span data-ttu-id="b8418-207">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="b8418-207">Response 2</span></span>

<span data-ttu-id="b8418-p112">Die Antwort für das zweite Beispiel sehen Sie unten. Der Antworttext enthält die folgenden Parameter für die neue Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="b8418-p112">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="b8418-210">Die Standardeigenschaft **extensionName**</span><span class="sxs-lookup"><span data-stu-id="b8418-210">The default property **extensionName**.</span></span>
- <span data-ttu-id="b8418-211">Die Eigenschaft **id** mit dem vollqualifizierten Namen `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`</span><span class="sxs-lookup"><span data-stu-id="b8418-211">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span> 
- <span data-ttu-id="b8418-212">Die benutzerdefinierten Daten, die gespeichert werden sollen</span><span class="sxs-lookup"><span data-stu-id="b8418-212">The custom data to be stored.</span></span>  

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
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
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

##### <a name="request-3"></a><span data-ttu-id="b8418-213">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="b8418-213">Request 3</span></span>

<span data-ttu-id="b8418-p113">Das dritte Beispiel erstellt eine Erweiterung in dem angegebenen Gruppenereignis. Der Anforderungstext enthält die folgenden Parameter für die Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="b8418-p113">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="b8418-216">Den Typ `Microsoft.Graph.OpenTypeExtension`</span><span class="sxs-lookup"><span data-stu-id="b8418-216">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="b8418-217">Den Erweiterungsnamen „Com.Contoso.Deal“</span><span class="sxs-lookup"><span data-stu-id="b8418-217">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="b8418-218">Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `dealValue` und `expirationDate`</span><span class="sxs-lookup"><span data-stu-id="b8418-218">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>  

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions 

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

##### <a name="response-3"></a><span data-ttu-id="b8418-219">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="b8418-219">Response 3</span></span>

<span data-ttu-id="b8418-220">Unten sehen Sie die Antwort auf die Anforderung im dritten Beispiel:</span><span class="sxs-lookup"><span data-stu-id="b8418-220">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
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

##### <a name="request-4"></a><span data-ttu-id="b8418-221">Anforderung 4</span><span class="sxs-lookup"><span data-stu-id="b8418-221">Request 4</span></span>

<span data-ttu-id="b8418-p114">Das vierte Beispiel erstellt eine Erweiterung in einem neuen Gruppenbeitrag, mit demselben **reply**-Aktionsaufruf, wie er für bereits vorhandene Gruppenbeiträge verwendet wird. Die Aktion **reply** erstellt einen neuen Beitrag und eine neue, in diesen Beitrag eingebettete Erweiterung. Der Antworttext enthält eine Eigenschaft **post** mit dem **Text** des neuen Beitrags sowie die folgenden Daten der neuen Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="b8418-p114">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="b8418-225">Den Typ `Microsoft.Graph.OpenTypeExtension`</span><span class="sxs-lookup"><span data-stu-id="b8418-225">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="b8418-226">Den Erweiterungsnamen „Com.Contoso.HR“</span><span class="sxs-lookup"><span data-stu-id="b8418-226">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="b8418-227">Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `expirationDate` und das Zeichenfolgen-Array `topPicks`</span><span class="sxs-lookup"><span data-stu-id="b8418-227">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=')/microsoft.graph.reply 

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
      "extensionName": "Com.Contoso.HR",
      "companyName": "Contoso",
      "expirationDate": "2015-07-03T13:04:00.000Z",
      "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
      ]
    }
  ]        
  }
}
```

##### <a name="response-4"></a><span data-ttu-id="b8418-228">Antwort 4</span><span class="sxs-lookup"><span data-stu-id="b8418-228">Response 4</span></span>

<span data-ttu-id="b8418-p115">Die Antwort für das vierte Beispiel sehen Sie unten. Wird eine Erweiterung in einem neuen Gruppenbeitrag erstellt, wird nur der Antwortcode „HTTP 202“ zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8418-p115">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Content-type: text/plain
Content-Length: 0
```


****

##### <a name="request-5"></a><span data-ttu-id="b8418-231">Anforderung 5</span><span class="sxs-lookup"><span data-stu-id="b8418-231">Request 5</span></span>

<span data-ttu-id="b8418-p116">Das fünfte Beispiel erstellt in ein und derselben POST-Operation eine Erweiterung in einem neuen Gruppenbeitrag und eine Unterhaltung. Die POST-Operation erstellt eine neue Unterhaltung, einen neuen Thread, einen neuen Beitrag und eine neue, in diesen Beitrag eingebettete Erweiterung. Der Anforderungstext enthält die Eigenschaften **Topic** und **Threads** sowie ein untergeordnetes Objekt des Typs **post** der neuen Unterhaltung. Das **post**-Objekt wiederum enthält den **Text** des neuen Beitrags sowie die folgenden Daten der Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="b8418-p116">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="b8418-236">Den Typ `Microsoft.Graph.OpenTypeExtension`</span><span class="sxs-lookup"><span data-stu-id="b8418-236">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="b8418-237">Den Erweiterungsnamen „Com.Contoso.HR“</span><span class="sxs-lookup"><span data-stu-id="b8418-237">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="b8418-238">Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `expirationDate` und das Zeichenfolgen-Array `topPicks`</span><span class="sxs-lookup"><span data-stu-id="b8418-238">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations

{
  "Topic": "Does anyone have a second?",
  "Threads": [
    {
      "Posts": [
        {
          "Body": {
            "ContentType": "HTML",
            "Content": "This is urgent!"
          },
          "Extensions": [
            {
              "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
              "extensionName": "Com.Contoso.Benefits",
              "companyName": "Contoso",
              "expirationDate": "2016-08-03T11:00:00.000Z",
              "topPicks": [
                "Employees only",
                "Add spouse or guest",
                "Add family"
              ]  
            }  
          ] 
        } 
      ]  
    } 
  ]
}
```

##### <a name="response-5"></a><span data-ttu-id="b8418-239">Antwort 5</span><span class="sxs-lookup"><span data-stu-id="b8418-239">Response 5</span></span>

<span data-ttu-id="b8418-p117">Unten sehen Sie die Antwort für das fünfte Beispiel mit der neuen Unterhaltung und einer Thread-ID. Dieser neue Thread enthält einen automatisch erstellten Beitrag, der wiederum die neue Erweiterung enthält.</span><span class="sxs-lookup"><span data-stu-id="b8418-p117">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span> 

<span data-ttu-id="b8418-p118">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b8418-p118">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="b8418-p119">Zum Abrufen der neuen Erweiterung [rufen Sie zunächst alle Beiträge](../api/conversationthread_list_posts.md) in diesem Thread ab. Anfangs sollte es nur einen Beitrag geben. Wenden Sie dann die Beitrags-ID und den Erweiterungsnamen `Com.Contoso.Benefits` an, um [die Erweiterung abzurufen](../api/opentypeextension_get.md).</span><span class="sxs-lookup"><span data-stu-id="b8418-p119">To get the new extension, first [get all the posts](../api/conversationthread_list_posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension_get.md).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
    "threads": [
        {
            "id": "AAQkADJDtMUzsf_PdhAAswJOhGVsnkyDtMUzsf_Pdg=="
        }
    ]
}

```


<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
