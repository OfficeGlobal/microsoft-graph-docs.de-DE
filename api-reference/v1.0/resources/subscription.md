# <a name="subscription-resource-type"></a><span data-ttu-id="d4af9-101">Ressourcentyp Abonnement</span><span class="sxs-lookup"><span data-stu-id="d4af9-101">subscription resource type</span></span>

<span data-ttu-id="d4af9-102">Ein Abonnement ermöglicht eine Client-app zum Empfangen von Benachrichtigungen zu Änderungen an Daten in Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d4af9-102">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="d4af9-103">Abonnements werden derzeit für die folgenden Ressourcen aktiviert:</span><span class="sxs-lookup"><span data-stu-id="d4af9-103">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="d4af9-104">E-Mail-Nachrichten, Ereignisse und Kontakte aus Outlook.</span><span class="sxs-lookup"><span data-stu-id="d4af9-104">Mail, events, and contacts from Outlook.</span></span>
- <span data-ttu-id="d4af9-105">Unterhaltungen aus Office-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="d4af9-105">Conversations from Office Groups.</span></span>
- <span data-ttu-id="d4af9-106">Laufwerk Stammelemente aus OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d4af9-106">Drive root items from OneDrive.</span></span>
- <span data-ttu-id="d4af9-107">Benutzer und Gruppen aus dem Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d4af9-107">Users and Groups from Azure Active Directory.</span></span>
- <span data-ttu-id="d4af9-108">Benachrichtigungen über die Microsoft Graph-Sicherheit API.</span><span class="sxs-lookup"><span data-stu-id="d4af9-108">Alerts from the Microsoft Graph Security API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4af9-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d4af9-109">JSON representation</span></span>

<span data-ttu-id="d4af9-110">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d4af9-110">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscription",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false,
        "sortable": false
      }
    }
  ]
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="d4af9-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d4af9-111">Properties</span></span>

| <span data-ttu-id="d4af9-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4af9-112">Property</span></span> | <span data-ttu-id="d4af9-113">Typ</span><span class="sxs-lookup"><span data-stu-id="d4af9-113">Type</span></span> | <span data-ttu-id="d4af9-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4af9-114">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="d4af9-115">changeType</span><span class="sxs-lookup"><span data-stu-id="d4af9-115">changeType</span></span> | <span data-ttu-id="d4af9-116">string</span><span class="sxs-lookup"><span data-stu-id="d4af9-116">string</span></span> | <span data-ttu-id="d4af9-117">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d4af9-117">Required.</span></span> <span data-ttu-id="d4af9-118">Gibt den Typ der Änderung in der abonnierten Ressource an, die eine Benachrichtigung auslöst.</span><span class="sxs-lookup"><span data-stu-id="d4af9-118">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="d4af9-119">Unterstützte Werte sind: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="d4af9-119">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="d4af9-120">Es können mehrere Werte mithilfe einer durch Trennzeichen getrennten Liste zusammen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="d4af9-120">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="d4af9-121">Hinweis: Laufwerk Root Element Benachrichtigungen unterstützen nur die `updated` ChangeType.</span><span class="sxs-lookup"><span data-stu-id="d4af9-121">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="d4af9-122">Unterstützung von Benutzer- und Benachrichtigungen `updated` und `deleted` ChangeType.</span><span class="sxs-lookup"><span data-stu-id="d4af9-122">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="d4af9-123">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="d4af9-123">notificationUrl</span></span> | <span data-ttu-id="d4af9-124">string</span><span class="sxs-lookup"><span data-stu-id="d4af9-124">string</span></span> | <span data-ttu-id="d4af9-125">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d4af9-125">Required.</span></span> <span data-ttu-id="d4af9-126">Die URL des Endpunkts, die Benachrichtigungen erhalten werden.</span><span class="sxs-lookup"><span data-stu-id="d4af9-126">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="d4af9-127">Diese URL muss nutzen Sie die HTTPS Protokoll.</span><span class="sxs-lookup"><span data-stu-id="d4af9-127">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="d4af9-128">resource</span><span class="sxs-lookup"><span data-stu-id="d4af9-128">resource</span></span> | <span data-ttu-id="d4af9-129">string</span><span class="sxs-lookup"><span data-stu-id="d4af9-129">string</span></span> | <span data-ttu-id="d4af9-130">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d4af9-130">Required.</span></span> <span data-ttu-id="d4af9-131">Gibt die Ressource, die für Änderungen überwacht werden.</span><span class="sxs-lookup"><span data-stu-id="d4af9-131">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="d4af9-132">Die base-URL nicht einschließen (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="d4af9-132">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="d4af9-133">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d4af9-133">expirationDateTime</span></span> | [<span data-ttu-id="d4af9-134">dateTime</span><span class="sxs-lookup"><span data-stu-id="d4af9-134">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="d4af9-135">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d4af9-135">Required.</span></span> <span data-ttu-id="d4af9-136">Gibt Datum und Uhrzeit für das Ablaufen des Webhook-Abonnements an.</span><span class="sxs-lookup"><span data-stu-id="d4af9-136">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="d4af9-137">Die Zeit wird in UTC angegeben und kann eine Dauer aus der Erstellung des Abonnements sein, die von der abonnierten Ressource abweicht.</span><span class="sxs-lookup"><span data-stu-id="d4af9-137">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="d4af9-138">In der folgenden Tabelle finden Sie die maximale Dauer unterstützter Abonnements.</span><span class="sxs-lookup"><span data-stu-id="d4af9-138">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="d4af9-139">clientState</span><span class="sxs-lookup"><span data-stu-id="d4af9-139">clientState</span></span> | <span data-ttu-id="d4af9-140">string</span><span class="sxs-lookup"><span data-stu-id="d4af9-140">string</span></span> | <span data-ttu-id="d4af9-141">Optional.</span><span class="sxs-lookup"><span data-stu-id="d4af9-141">Optional.</span></span> <span data-ttu-id="d4af9-142">Gibt den Wert der `clientState`-Eigenschaft an, die in jeder Benachrichtigung vom Dienst gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="d4af9-142">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="d4af9-143">Die Höchstlänge beträgt 128 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="d4af9-143">The maximum length is 128 characters.</span></span> <span data-ttu-id="d4af9-144">Der Client kann prüfen, ob die Benachrichtigung vom Dienst stammt, indem er den Wert der mit dem Abonnement gesendeten `clientState`-Eigenschaft mit dem Wert der mit jeder Benachrichtigung empfangenen `clientState`-Eigenschaft vergleicht.</span><span class="sxs-lookup"><span data-stu-id="d4af9-144">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="d4af9-145">id</span><span class="sxs-lookup"><span data-stu-id="d4af9-145">id</span></span> | <span data-ttu-id="d4af9-146">string</span><span class="sxs-lookup"><span data-stu-id="d4af9-146">string</span></span> | <span data-ttu-id="d4af9-p108">Eindeutige ID für das Abonnement. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4af9-p108">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="d4af9-149">applicationId</span><span class="sxs-lookup"><span data-stu-id="d4af9-149">applicationId</span></span> | <span data-ttu-id="d4af9-150">string</span><span class="sxs-lookup"><span data-stu-id="d4af9-150">string</span></span> | <span data-ttu-id="d4af9-151">Bezeichner der Anwendung verwendet, um das Abonnement zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="d4af9-151">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="d4af9-152">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4af9-152">Read-only.</span></span> |
| <span data-ttu-id="d4af9-153">creatorId</span><span class="sxs-lookup"><span data-stu-id="d4af9-153">creatorId</span></span> | <span data-ttu-id="d4af9-154">string</span><span class="sxs-lookup"><span data-stu-id="d4af9-154">string</span></span> | <span data-ttu-id="d4af9-155">Bezeichner des Benutzers oder der Dienstprinzipalnamen, die das Abonnement erstellt.</span><span class="sxs-lookup"><span data-stu-id="d4af9-155">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="d4af9-156">Wenn die app verwendet Berechtigungen zum Erstellen des Abonnements delegiert, enthält dieses Feld die Id des angemeldeten Benutzers an, den die app im Auftrag von aufgerufen.</span><span class="sxs-lookup"><span data-stu-id="d4af9-156">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="d4af9-157">Wenn die app Anwendungsberechtigungen verwendet wird, enthält dieses Feld die Id des Prinzipals Service für die app.</span><span class="sxs-lookup"><span data-stu-id="d4af9-157">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="d4af9-158">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4af9-158">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="d4af9-159">Maximale Abonnementdauer pro Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d4af9-159">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="d4af9-160">Ressource</span><span class="sxs-lookup"><span data-stu-id="d4af9-160">Resource</span></span>            | <span data-ttu-id="d4af9-161">Maximal zulässige Ablaufzeit</span><span class="sxs-lookup"><span data-stu-id="d4af9-161">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="d4af9-162">Mail</span><span class="sxs-lookup"><span data-stu-id="d4af9-162">Mail</span></span>                | <span data-ttu-id="d4af9-163">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d4af9-163">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="d4af9-164">Kalender</span><span class="sxs-lookup"><span data-stu-id="d4af9-164">Calendar</span></span>            | <span data-ttu-id="d4af9-165">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d4af9-165">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="d4af9-166">Kontakte</span><span class="sxs-lookup"><span data-stu-id="d4af9-166">Contacts</span></span>            | <span data-ttu-id="d4af9-167">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d4af9-167">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="d4af9-168">Gruppenunterhaltungen</span><span class="sxs-lookup"><span data-stu-id="d4af9-168">Group conversations</span></span> | <span data-ttu-id="d4af9-169">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d4af9-169">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="d4af9-170">Laufwerkstammelemente</span><span class="sxs-lookup"><span data-stu-id="d4af9-170">Drive root items</span></span>    | <span data-ttu-id="d4af9-171">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d4af9-171">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="d4af9-172">Sicherheitshinweise</span><span class="sxs-lookup"><span data-stu-id="d4af9-172">Security alerts</span></span>     | <span data-ttu-id="d4af9-173">43200 Minuten (unter 30 Tage)</span><span class="sxs-lookup"><span data-stu-id="d4af9-173">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="d4af9-174">**Hinweis:** Vorhandene Anwendungen und neuen Anwendungen sollte den unterstützten Wert nicht überschreiten.</span><span class="sxs-lookup"><span data-stu-id="d4af9-174">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="d4af9-175">In der Zukunft fehl alle Anforderungen zum Erstellen oder erneuern Sie ein Abonnement über den Höchstwert hinaus.</span><span class="sxs-lookup"><span data-stu-id="d4af9-175">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="d4af9-176">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d4af9-176">Relationships</span></span>

<span data-ttu-id="d4af9-177">Keine</span><span class="sxs-lookup"><span data-stu-id="d4af9-177">None</span></span>

## <a name="methods"></a><span data-ttu-id="d4af9-178">Methoden</span><span class="sxs-lookup"><span data-stu-id="d4af9-178">Methods</span></span>

| <span data-ttu-id="d4af9-179">Methode</span><span class="sxs-lookup"><span data-stu-id="d4af9-179">Method</span></span> | <span data-ttu-id="d4af9-180">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d4af9-180">Return Type</span></span> | <span data-ttu-id="d4af9-181">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4af9-181">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="d4af9-182">Create subscription</span><span class="sxs-lookup"><span data-stu-id="d4af9-182">Create subscription</span></span>](../api/subscription_post_subscriptions.md) | [<span data-ttu-id="d4af9-183">Abonnement</span><span class="sxs-lookup"><span data-stu-id="d4af9-183">subscription</span></span>](subscription.md) | <span data-ttu-id="d4af9-184">Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Microsoft Graph-Daten geändert werden.</span><span class="sxs-lookup"><span data-stu-id="d4af9-184">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="d4af9-185">Update subscription</span><span class="sxs-lookup"><span data-stu-id="d4af9-185">Update subscription</span></span>](../api/subscription_update.md) | [<span data-ttu-id="d4af9-186">Abonnement</span><span class="sxs-lookup"><span data-stu-id="d4af9-186">subscription</span></span>](subscription.md) | <span data-ttu-id="d4af9-187">Erneuert ein Abonnement durch Aktualisierung der Ablaufzeit.</span><span class="sxs-lookup"><span data-stu-id="d4af9-187">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="d4af9-188">Liste von Abonnements</span><span class="sxs-lookup"><span data-stu-id="d4af9-188">List subscriptions</span></span>](../api/subscription_list.md) | [<span data-ttu-id="d4af9-189">subscription</span><span class="sxs-lookup"><span data-stu-id="d4af9-189">subscription</span></span>](subscription.md) | <span data-ttu-id="d4af9-190">Listen aktiver Abonnements.</span><span class="sxs-lookup"><span data-stu-id="d4af9-190">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="d4af9-191">Get subscription</span><span class="sxs-lookup"><span data-stu-id="d4af9-191">Get subscription</span></span>](../api/subscription_get.md) | [<span data-ttu-id="d4af9-192">Abonnement</span><span class="sxs-lookup"><span data-stu-id="d4af9-192">subscription</span></span>](subscription.md) | <span data-ttu-id="d4af9-193">Dient zum Lesen der Eigenschaften und der Beziehungen des subscription-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4af9-193">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="d4af9-194">Delete subscription</span><span class="sxs-lookup"><span data-stu-id="d4af9-194">Delete subscription</span></span>](../api/subscription_delete.md) | <span data-ttu-id="d4af9-195">Keine</span><span class="sxs-lookup"><span data-stu-id="d4af9-195">None</span></span> |<span data-ttu-id="d4af9-196">Löscht ein subscription-Objekt.</span><span class="sxs-lookup"><span data-stu-id="d4af9-196">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
