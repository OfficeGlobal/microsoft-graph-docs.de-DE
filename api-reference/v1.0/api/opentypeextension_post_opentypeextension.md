# <a name="create-open-extension"></a><span data-ttu-id="6118d-101">Datenerweiterung erstellen</span><span class="sxs-lookup"><span data-stu-id="6118d-101">Create open extension</span></span>

<span data-ttu-id="6118d-102">Mit dieser API können Sie offene Erweiterungen (Objekte des Typs [openTypeExtension](../resources/openTypeExtension.md)) erstellen und einer neuen oder bereits vorhandenen Ressourceninstanz benutzerdefinierte Eigenschaften hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="6118d-102">Create an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) and add custom properties in a new or existing instance of a resource.</span></span>

> <span data-ttu-id="6118d-103">**Hinweis:** Wenn beim Erstellen von open Extensions auf Outlook-Ressourcen finden Sie in [OpenTypeExtension Ressourcentyp](../resources/opentypeextension.md#outlook-specific-considerations) **Outlook-spezifischen Aspekte** .</span><span class="sxs-lookup"><span data-stu-id="6118d-103">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="6118d-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6118d-104">Permissions</span></span>

<span data-ttu-id="6118d-105">Je nach der Ressource, die Sie die Erweiterung im erstellen und die Berechtigung Typ (delegierte oder-Anwendung) angefordert, die Berechtigung, die in der folgenden Tabelle angegebenen mit den geringsten ist erforderlich, um diese API aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="6118d-105">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="6118d-106">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6118d-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="6118d-107">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="6118d-107">Supported resource</span></span> | <span data-ttu-id="6118d-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6118d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6118d-109">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6118d-109">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6118d-110">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6118d-110">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="6118d-111">Gerät</span><span class="sxs-lookup"><span data-stu-id="6118d-111">device</span></span>](../resources/device.md) | <span data-ttu-id="6118d-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6118d-112">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="6118d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6118d-113">Not supported</span></span> | <span data-ttu-id="6118d-114">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6118d-114">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="6118d-115">event</span><span class="sxs-lookup"><span data-stu-id="6118d-115">event</span></span>](../resources/event.md) | <span data-ttu-id="6118d-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6118d-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="6118d-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6118d-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="6118d-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6118d-118">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="6118d-119">group</span><span class="sxs-lookup"><span data-stu-id="6118d-119">group</span></span>](../resources/group.md) | <span data-ttu-id="6118d-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6118d-120">Group.ReadWrite.All</span></span> | <span data-ttu-id="6118d-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6118d-121">Not supported</span></span> | <span data-ttu-id="6118d-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6118d-122">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="6118d-123">group event</span><span class="sxs-lookup"><span data-stu-id="6118d-123">group event</span></span>](../resources/event.md) | <span data-ttu-id="6118d-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6118d-124">Group.ReadWrite.All</span></span> | <span data-ttu-id="6118d-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6118d-125">Not supported</span></span> | <span data-ttu-id="6118d-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6118d-126">Not supported</span></span> |
| [<span data-ttu-id="6118d-127">group post</span><span class="sxs-lookup"><span data-stu-id="6118d-127">group post</span></span>](../resources/post.md) | <span data-ttu-id="6118d-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6118d-128">Group.ReadWrite.All</span></span> | <span data-ttu-id="6118d-129">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6118d-129">Not supported</span></span> | <span data-ttu-id="6118d-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6118d-130">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="6118d-131">message</span><span class="sxs-lookup"><span data-stu-id="6118d-131">message</span></span>](../resources/message.md) | <span data-ttu-id="6118d-132">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6118d-132">Mail.ReadWrite</span></span> | <span data-ttu-id="6118d-133">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6118d-133">Mail.ReadWrite</span></span> | <span data-ttu-id="6118d-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6118d-134">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="6118d-135">organization</span><span class="sxs-lookup"><span data-stu-id="6118d-135">organization</span></span>](../resources/organization.md) | <span data-ttu-id="6118d-136">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6118d-136">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="6118d-137">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6118d-137">Not supported</span></span> | <span data-ttu-id="6118d-138">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6118d-138">Not supported</span></span> |
| [<span data-ttu-id="6118d-139">personal contact</span><span class="sxs-lookup"><span data-stu-id="6118d-139">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="6118d-140">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6118d-140">Contacts.ReadWrite</span></span> | <span data-ttu-id="6118d-141">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6118d-141">Contacts.ReadWrite</span></span> | <span data-ttu-id="6118d-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6118d-142">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="6118d-143">user</span><span class="sxs-lookup"><span data-stu-id="6118d-143">user</span></span>](../resources/user.md) | <span data-ttu-id="6118d-144">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6118d-144">User.ReadWrite.All</span></span> | <span data-ttu-id="6118d-145">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6118d-145">User.ReadWrite</span></span> | <span data-ttu-id="6118d-146">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6118d-146">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6118d-147">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6118d-147">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="6118d-148">Erstellen einer Erweiterung in einer neuen Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="6118d-148">Create an extension in a new resource instance</span></span>

<span data-ttu-id="6118d-149">Verwenden Sie die gleiche REST-Anforderung, die Sie verwenden, um die Instanz zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="6118d-149">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="6118d-150">**Hinweis:** Diese Syntax enthält einige allgemeinen Bereitstellungsmethoden für die Ressourceninstanzen unterstützte zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="6118d-150">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="6118d-151">Andere POST-Syntax, die Sie erstellen diese Ressourceninstanzen können unterstützt erstellen open Erweiterungen in diese auf ähnliche Weise.</span><span class="sxs-lookup"><span data-stu-id="6118d-151">All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="6118d-152">Im Abschnitt [Anforderungstext](#request-body) ist beschrieben, wie Sie die Eigenschaften der neuen Ressourceninstanz _und die Erweiterung_ in den Anforderungstext einschließen können.</span><span class="sxs-lookup"><span data-stu-id="6118d-152">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="6118d-153">Erstellen einer Erweiterung in einer vorhandenen Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="6118d-153">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="6118d-154">Geben Sie die Ressourceninstanz in der Anforderung an, und wenden Sie den Befehl `POST` auf die Navigationseigenschaft **extensions** an.</span><span class="sxs-lookup"><span data-stu-id="6118d-154">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

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

><span data-ttu-id="6118d-155">**Hinweis:** Diese Syntax enthält einige allgemeinen Bereitstellungsmethoden für eine Ressourceninstanz identifizieren, um eine Erweiterung in es zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="6118d-155">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it.</span></span> <span data-ttu-id="6118d-156">Alle anderen Syntax, die Ihnen ermöglicht, diese Ressourceninstanzen identifizieren unterstützt das Erstellen von open Extensions darin auf ähnliche Weise.</span><span class="sxs-lookup"><span data-stu-id="6118d-156">All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="6118d-157">Im Abschnitt [Anforderungstext](#request-body) wird beschrieben, wie Sie _die Erweiterung_ in den Anforderungstext einschließen können.</span><span class="sxs-lookup"><span data-stu-id="6118d-157">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="6118d-158">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="6118d-158">Path parameters</span></span>
|<span data-ttu-id="6118d-159">Parameter</span><span class="sxs-lookup"><span data-stu-id="6118d-159">Parameter</span></span>|<span data-ttu-id="6118d-160">Typ</span><span class="sxs-lookup"><span data-stu-id="6118d-160">Type</span></span>|<span data-ttu-id="6118d-161">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6118d-161">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6118d-162">id</span><span class="sxs-lookup"><span data-stu-id="6118d-162">id</span></span>|<span data-ttu-id="6118d-163">string</span><span class="sxs-lookup"><span data-stu-id="6118d-163">string</span></span>|<span data-ttu-id="6118d-p104">Ein eindeutiger Bezeichner für ein Objekt in der entsprechenden Sammlung. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6118d-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="6118d-166">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6118d-166">Request headers</span></span>

| <span data-ttu-id="6118d-167">Name</span><span class="sxs-lookup"><span data-stu-id="6118d-167">Name</span></span>       | <span data-ttu-id="6118d-168">Wert</span><span class="sxs-lookup"><span data-stu-id="6118d-168">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="6118d-169">Authorization</span><span class="sxs-lookup"><span data-stu-id="6118d-169">Authorization</span></span> | <span data-ttu-id="6118d-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6118d-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6118d-172">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6118d-172">Content-Type</span></span> | <span data-ttu-id="6118d-173">application/json</span><span class="sxs-lookup"><span data-stu-id="6118d-173">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6118d-174">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6118d-174">Request body</span></span>

<span data-ttu-id="6118d-p106">Geben Sie den JSON-Text einer [openTypeExtension](../resources/openTypeExtension.md) an, mit den folgenden erforderlichen Name/Wert-Paaren und allen zusätzlichen benutzerdefinierten Daten. Die Daten in der JSON-Nutzlast können Grundtypen oder Arrays von Grundtypen sein.</span><span class="sxs-lookup"><span data-stu-id="6118d-p106">Provide a JSON body of an [openTypeExtension](../resources/openTypeExtension.md), with the following required name-value pairs, and any additional custom data. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="6118d-177">Name</span><span class="sxs-lookup"><span data-stu-id="6118d-177">Name</span></span>       | <span data-ttu-id="6118d-178">Wert</span><span class="sxs-lookup"><span data-stu-id="6118d-178">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="6118d-179">@odata.type</span><span class="sxs-lookup"><span data-stu-id="6118d-179">@odata.type</span></span> | <span data-ttu-id="6118d-180">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="6118d-180">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="6118d-181">extensionName</span><span class="sxs-lookup"><span data-stu-id="6118d-181">extensionName</span></span> | <span data-ttu-id="6118d-182">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="6118d-182">%unique_string%</span></span> |

<span data-ttu-id="6118d-183">Beim Erstellen einer Erweiterung in einer _neuen_ Ressourceninstanz müssen Sie zusätzlich zu dem neuen **openTypeExtension**-Objekt eine JSON-Darstellung der zur Erstellung einer solchen Ressourceninstanz erforderlichen Eigenschaften angeben.</span><span class="sxs-lookup"><span data-stu-id="6118d-183">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="6118d-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="6118d-184">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="6118d-185">Antwortcode</span><span class="sxs-lookup"><span data-stu-id="6118d-185">Response code</span></span>

<span data-ttu-id="6118d-186">Je nach Vorgang lautet der Antwortcode `201 Created` oder `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="6118d-186">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="6118d-187">Beim Erstellen einer Erweiterungs mit den gleichen Vorgang, mit denen Sie eine Ressourceninstanz zu erstellen, gibt der Vorgang den gleichen Antwortcode, den es zurückgibt, wenn Sie den Vorgang zum Erstellen der Ressourceninstanz ohne die Erweiterung verwenden.</span><span class="sxs-lookup"><span data-stu-id="6118d-187">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension.</span></span>
<span data-ttu-id="6118d-188">Finden Sie in den entsprechenden Themen für die Instanz als aufgeführten [oben](#create-an-extension-in-a-new-resource-instance)zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="6118d-188">Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="6118d-189">Antworttext</span><span class="sxs-lookup"><span data-stu-id="6118d-189">Response body</span></span>

| <span data-ttu-id="6118d-190">Szenario</span><span class="sxs-lookup"><span data-stu-id="6118d-190">Scenario</span></span>       | <span data-ttu-id="6118d-191">Ressource</span><span class="sxs-lookup"><span data-stu-id="6118d-191">Resource</span></span>  | <span data-ttu-id="6118d-192">Antworttext</span><span class="sxs-lookup"><span data-stu-id="6118d-192">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="6118d-193">Erstellen einer Erweiterung bei gleichzeitiger expliziter Erstellung einer _neuen_ Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="6118d-193">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="6118d-194">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="6118d-194">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="6118d-195">Enthält die neue Instanz, erweitert um das [openTypeExtension](../resources/openTypeExtension.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="6118d-195">Includes the new instance expanded with the [openTypeExtension](../resources/openTypeExtension.md) object.</span></span> |
| <span data-ttu-id="6118d-196">Erstellen einer Erweiterung bei gleichzeitiger impliziter Erstellung einer Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="6118d-196">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="6118d-197">post</span><span class="sxs-lookup"><span data-stu-id="6118d-197">post</span></span>](../resources/post.md) | <span data-ttu-id="6118d-198">Die Antwort enthält nur einen Antwortcode, keinen Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6118d-198">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="6118d-199">Erstellen einer Erweiterung in einer _vorhandenen_ Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="6118d-199">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="6118d-200">Alle unterstützten Ressourcen</span><span class="sxs-lookup"><span data-stu-id="6118d-200">All supported resources</span></span> | <span data-ttu-id="6118d-201">Enthält das **openTypeExtension**-Objekt.</span><span class="sxs-lookup"><span data-stu-id="6118d-201">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="6118d-202">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6118d-202">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="6118d-203">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="6118d-203">Request 1</span></span>

<span data-ttu-id="6118d-p108">Im ersten Beispiel werden mit ein und demselben Aufruf eine Nachricht und eine Erweiterung erstellt. Der Anforderungstext enthält Folgendes:</span><span class="sxs-lookup"><span data-stu-id="6118d-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="6118d-206">Die für eine neue Nachricht typischen Eigenschaften **subject**, **body** und **toRecipients**</span><span class="sxs-lookup"><span data-stu-id="6118d-206">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="6118d-207">Daneben die folgenden Parameter der Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="6118d-207">And for the extension:</span></span>

  - <span data-ttu-id="6118d-208">Den Typ `microsoft.graph.openTypeExtension`</span><span class="sxs-lookup"><span data-stu-id="6118d-208">The type `microsoft.graph.openTypeExtension`.</span></span>
  - <span data-ttu-id="6118d-209">Den Erweiterungsnamen „Com.Contoso.Referral“</span><span class="sxs-lookup"><span data-stu-id="6118d-209">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="6118d-210">Zusätzliche Daten, die als drei benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden: `companyName`, `expirationDate`, und `dealValue`.</span><span class="sxs-lookup"><span data-stu-id="6118d-210">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>

<!-- {
  "blockType": "ignored",
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
      "@odata.type": "microsoft.graph.openTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

### <a name="response-1"></a><span data-ttu-id="6118d-211">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="6118d-211">Response 1</span></span>

<span data-ttu-id="6118d-p109">Unten sehen Sie die Antwort für Beispiel 1. Der Antworttext enthält die Eigenschaften der neuen Nachricht sowie die folgenden Parameter der neuen Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="6118d-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="6118d-214">Die Eigenschaft **id** mit dem vollqualifizierten Namen `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`</span><span class="sxs-lookup"><span data-stu-id="6118d-214">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="6118d-215">Die in der Anforderung angegebene Standardeigenschaft **extensionName**</span><span class="sxs-lookup"><span data-stu-id="6118d-215">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="6118d-216">Die in der Anforderung angegebenen benutzerdefinierten Daten, gespeichert als 3 benutzerdefinierte Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6118d-216">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="6118d-p110">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6118d-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.openTypeExtension",
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

### <a name="request-2"></a><span data-ttu-id="6118d-219">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="6118d-219">Request 2</span></span>

<span data-ttu-id="6118d-p111">Das zweite Beispiel erstellt eine Erweiterung in der angegebenen Nachricht. Der Anforderungstext enthält die folgenden Parameter für die Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="6118d-p111">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="6118d-222">Den Typ `microsoft.graph.openTypeExtension`</span><span class="sxs-lookup"><span data-stu-id="6118d-222">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="6118d-223">Den Erweiterungsnamen „Com.Contoso.Referral“</span><span class="sxs-lookup"><span data-stu-id="6118d-223">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="6118d-224">Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `dealValue` und `expirationDate`</span><span class="sxs-lookup"><span data-stu-id="6118d-224">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```

### <a name="response-2"></a><span data-ttu-id="6118d-225">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="6118d-225">Response 2</span></span>

<span data-ttu-id="6118d-p112">Die Antwort für das zweite Beispiel sehen Sie unten. Der Antworttext enthält die folgenden Parameter für die neue Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="6118d-p112">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="6118d-228">Die Standardeigenschaft **extensionName**</span><span class="sxs-lookup"><span data-stu-id="6118d-228">The default property **extensionName**.</span></span>
- <span data-ttu-id="6118d-229">Die Eigenschaft **id** mit dem vollqualifizierten Namen `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`</span><span class="sxs-lookup"><span data-stu-id="6118d-229">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="6118d-230">Die benutzerdefinierten Daten, die gespeichert werden sollen</span><span class="sxs-lookup"><span data-stu-id="6118d-230">The custom data to be stored.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
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

### <a name="request-3"></a><span data-ttu-id="6118d-231">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="6118d-231">Request 3</span></span>

<span data-ttu-id="6118d-p113">Das dritte Beispiel erstellt eine Erweiterung in dem angegebenen Gruppenereignis. Der Anforderungstext enthält die folgenden Parameter für die Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="6118d-p113">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="6118d-234">Den Typ `microsoft.graph.openTypeExtension`</span><span class="sxs-lookup"><span data-stu-id="6118d-234">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="6118d-235">Den Erweiterungsnamen „Com.Contoso.Deal“</span><span class="sxs-lookup"><span data-stu-id="6118d-235">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="6118d-236">Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `dealValue` und `expirationDate`</span><span class="sxs-lookup"><span data-stu-id="6118d-236">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

### <a name="response-3"></a><span data-ttu-id="6118d-237">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="6118d-237">Response 3</span></span>

<span data-ttu-id="6118d-238">Unten sehen Sie die Antwort auf die Anforderung im dritten Beispiel:</span><span class="sxs-lookup"><span data-stu-id="6118d-238">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

### <a name="request-4"></a><span data-ttu-id="6118d-239">Anforderung 4</span><span class="sxs-lookup"><span data-stu-id="6118d-239">Request 4</span></span>

<span data-ttu-id="6118d-p114">Das vierte Beispiel erstellt eine Erweiterung in einem neuen Gruppenbeitrag, mit demselben **reply**-Aktionsaufruf, wie er für bereits vorhandene Gruppenbeiträge verwendet wird. Die Aktion **reply** erstellt einen neuen Beitrag und eine neue, in diesen Beitrag eingebettete Erweiterung. Der Antworttext enthält eine Eigenschaft **post** mit dem **Text** des neuen Beitrags sowie die folgenden Daten der neuen Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="6118d-p114">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="6118d-243">Den Typ `microsoft.graph.openTypeExtension`</span><span class="sxs-lookup"><span data-stu-id="6118d-243">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="6118d-244">Den Erweiterungsnamen „Com.Contoso.HR“</span><span class="sxs-lookup"><span data-stu-id="6118d-244">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="6118d-245">Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `expirationDate` und das Zeichenfolgen-Array `topPicks`</span><span class="sxs-lookup"><span data-stu-id="6118d-245">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=/reply

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

### <a name="response-4"></a><span data-ttu-id="6118d-246">Antwort 4</span><span class="sxs-lookup"><span data-stu-id="6118d-246">Response 4</span></span>

<span data-ttu-id="6118d-p115">Die Antwort für das vierte Beispiel sehen Sie unten. Wird eine Erweiterung in einem neuen Gruppenbeitrag erstellt, wird nur der Antwortcode „HTTP 202“ zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6118d-p115">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

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

### <a name="request-5"></a><span data-ttu-id="6118d-249">Anforderung 5</span><span class="sxs-lookup"><span data-stu-id="6118d-249">Request 5</span></span>

<span data-ttu-id="6118d-p116">Das fünfte Beispiel erstellt in ein und derselben POST-Operation eine Erweiterung in einem neuen Gruppenbeitrag und eine Unterhaltung. Die POST-Operation erstellt eine neue Unterhaltung, einen neuen Thread, einen neuen Beitrag und eine neue, in diesen Beitrag eingebettete Erweiterung. Der Anforderungstext enthält die Eigenschaften **Topic** und **Threads** sowie ein untergeordnetes Objekt des Typs **post** der neuen Unterhaltung. Das **post**-Objekt wiederum enthält den **Text** des neuen Beitrags sowie die folgenden Daten der Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="6118d-p116">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="6118d-254">Den Typ `microsoft.graph.openTypeExtension`</span><span class="sxs-lookup"><span data-stu-id="6118d-254">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="6118d-255">Den Erweiterungsnamen „Com.Contoso.HR“</span><span class="sxs-lookup"><span data-stu-id="6118d-255">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="6118d-256">Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `expirationDate` und das Zeichenfolgen-Array `topPicks`</span><span class="sxs-lookup"><span data-stu-id="6118d-256">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/conversations

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

### <a name="response-5"></a><span data-ttu-id="6118d-257">Antwort 5</span><span class="sxs-lookup"><span data-stu-id="6118d-257">Response 5</span></span>

<span data-ttu-id="6118d-p117">Unten sehen Sie die Antwort für das fünfte Beispiel mit der neuen Unterhaltung und einer Thread-ID. Dieser neue Thread enthält einen automatisch erstellten Beitrag, der wiederum die neue Erweiterung enthält.</span><span class="sxs-lookup"><span data-stu-id="6118d-p117">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="6118d-p118">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6118d-p118">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="6118d-p119">Zum Abrufen der neuen Erweiterung [rufen Sie zunächst alle Beiträge](../api/conversationthread_list_posts.md) in diesem Thread ab. Anfangs sollte es nur einen Beitrag geben. Wenden Sie dann die Beitrags-ID und den Erweiterungsnamen `Com.Contoso.Benefits` an, um [die Erweiterung abzurufen](../api/opentypeextension_get.md).</span><span class="sxs-lookup"><span data-stu-id="6118d-p119">To get the new extension, first [get all the posts](../api/conversationthread_list_posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension_get.md).</span></span>

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
