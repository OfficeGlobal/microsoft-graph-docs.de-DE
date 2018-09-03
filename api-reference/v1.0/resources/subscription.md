# <a name="subscription-resource-type"></a><span data-ttu-id="d1b16-101">Ressourcentyp Abonnement</span><span class="sxs-lookup"><span data-stu-id="d1b16-101">Subscription resource type</span></span>

<span data-ttu-id="d1b16-102">Mit einem Abonnement kann eine Client-App Benachrichtigungen zu Änderungen an den Daten in Microsoft Graph erhalten.</span><span class="sxs-lookup"><span data-stu-id="d1b16-102">A subscription allows a client app to receive notifications about data on the Microsoft Graph.</span></span> <span data-ttu-id="d1b16-103">Abonnements werden derzeit für die folgenden Ressourcen aktiviert:</span><span class="sxs-lookup"><span data-stu-id="d1b16-103">Currently, subscriptions are enabled for the following datasets:</span></span>

- <span data-ttu-id="d1b16-104">E-Mail, Ereignisse und Kontakte aus Outlook</span><span class="sxs-lookup"><span data-stu-id="d1b16-104">Mail, events, and contacts from Outlook</span></span>
- <span data-ttu-id="d1b16-105">Unterhaltungen aus Office-Gruppen</span><span class="sxs-lookup"><span data-stu-id="d1b16-105">Conversations from Office Groups.</span></span>
- <span data-ttu-id="d1b16-106">Laufwerk-Stammelemente aus OneDrive</span><span class="sxs-lookup"><span data-stu-id="d1b16-106">Drive root items from OneDrive</span></span>
- <span data-ttu-id="d1b16-107">Benutzer und Gruppen aus dem Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="d1b16-107">Users and Groups from Azure Active Directory</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1b16-108">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d1b16-108">JSON representation</span></span>

<span data-ttu-id="d1b16-109">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d1b16-109">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d1b16-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d1b16-110">Properties</span></span>

| <span data-ttu-id="d1b16-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d1b16-111">Property</span></span> | <span data-ttu-id="d1b16-112">Typ</span><span class="sxs-lookup"><span data-stu-id="d1b16-112">Type</span></span> | <span data-ttu-id="d1b16-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1b16-113">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="d1b16-114">changeType</span><span class="sxs-lookup"><span data-stu-id="d1b16-114">changeType</span></span> | <span data-ttu-id="d1b16-115">string</span><span class="sxs-lookup"><span data-stu-id="d1b16-115">string</span></span> | <span data-ttu-id="d1b16-116">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d1b16-116">Required.</span></span> <span data-ttu-id="d1b16-117">Gibt den Typ der Änderung in der abonnierten Ressource an, die eine Benachrichtigung auslöst.</span><span class="sxs-lookup"><span data-stu-id="d1b16-117">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="d1b16-118">Unterstützte Werte sind: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="d1b16-118">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="d1b16-119">Es können mehrere Werte mithilfe einer durch Komma getrennten Liste zusammen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="d1b16-119">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="d1b16-120">Hinweis: Laufwerk Stamm-Element Benachrichtigungs-Support unterstützen nur den `updated` ChangeType.</span><span class="sxs-lookup"><span data-stu-id="d1b16-120">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="d1b16-121">Support für Benutzer und Gruppen-Benachrichtigungen `updated` und `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="d1b16-121">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="d1b16-122">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="d1b16-122">notificationUrl</span></span> | <span data-ttu-id="d1b16-123">string</span><span class="sxs-lookup"><span data-stu-id="d1b16-123">string</span></span> | <span data-ttu-id="d1b16-124">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d1b16-124">Required.</span></span> <span data-ttu-id="d1b16-125">Die URL des Endpunkts, die Benachrichtigungen erhalten werden.</span><span class="sxs-lookup"><span data-stu-id="d1b16-125">The URL of the application that will receive the push notifications.</span></span> <span data-ttu-id="d1b16-126">Diese URL muss das HTTPS-Protokoll nutzen.</span><span class="sxs-lookup"><span data-stu-id="d1b16-126">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="d1b16-127">resource</span><span class="sxs-lookup"><span data-stu-id="d1b16-127">resource</span></span> | <span data-ttu-id="d1b16-128">string</span><span class="sxs-lookup"><span data-stu-id="d1b16-128">string</span></span> | <span data-ttu-id="d1b16-129">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d1b16-129">Required.</span></span> <span data-ttu-id="d1b16-130">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d1b16-130">Specifies the resource that will be monitored for changes. Do not include the base URL ("https://graph.microsoft.com/v1.0/").</span></span> <span data-ttu-id="d1b16-131">Die Basis-URL nicht einschließen (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="d1b16-131">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="d1b16-132">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d1b16-132">expirationDateTime</span></span> | [<span data-ttu-id="d1b16-133">dateTime</span><span class="sxs-lookup"><span data-stu-id="d1b16-133">dateTime</span></span>](http://tools.ietf.org/html/rfc3339) | <span data-ttu-id="d1b16-134">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d1b16-134">Required.</span></span> <span data-ttu-id="d1b16-135">Gibt Datum und Uhrzeit für das Ablaufen des Webhook-Abonnements an.</span><span class="sxs-lookup"><span data-stu-id="d1b16-135">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="d1b16-136">Die Zeit wird in UTC angegeben und kann eine Dauer aus der Erstellung des Abonnements sein, die von der abonnierten Ressource abweicht.</span><span class="sxs-lookup"><span data-stu-id="d1b16-136">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="d1b16-137">In der folgenden Tabelle finden Sie die maximale Dauer unterstützter Abonnements.</span><span class="sxs-lookup"><span data-stu-id="d1b16-137">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="d1b16-138">clientState</span><span class="sxs-lookup"><span data-stu-id="d1b16-138">clientState</span></span> | <span data-ttu-id="d1b16-139">string</span><span class="sxs-lookup"><span data-stu-id="d1b16-139">string</span></span> | <span data-ttu-id="d1b16-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="d1b16-140">Optional.</span></span> <span data-ttu-id="d1b16-141">Gibt den Wert der `clientState`-Eigenschaft an, die in jeder Benachrichtigung vom Dienst gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="d1b16-141">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="d1b16-142">Die Höchstlänge beträgt 128 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="d1b16-142">The maximum length is 128 characters.</span></span> <span data-ttu-id="d1b16-143">Der Client kann prüfen, ob die Benachrichtigung vom Dienst stammt, indem er den Wert der mit dem Abonnement gesendeten `clientState`-Eigenschaft mit dem Wert der mit jeder Benachrichtigung empfangenen `clientState`-Eigenschaft vergleicht.</span><span class="sxs-lookup"><span data-stu-id="d1b16-143">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="d1b16-144">ID</span><span class="sxs-lookup"><span data-stu-id="d1b16-144">id</span></span> | <span data-ttu-id="d1b16-145">string</span><span class="sxs-lookup"><span data-stu-id="d1b16-145">string</span></span> | <span data-ttu-id="d1b16-p108">Eindeutige ID für das Abonnement. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d1b16-p108">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="d1b16-148">applicationId</span><span class="sxs-lookup"><span data-stu-id="d1b16-148">applicationId</span></span> | <span data-ttu-id="d1b16-149">string</span><span class="sxs-lookup"><span data-stu-id="d1b16-149">string</span></span> | <span data-ttu-id="d1b16-150">Bezeichner der Anwendung, die verwendet wird, um das Abonnement zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="d1b16-150">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="d1b16-151">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d1b16-151">Read-only.</span></span> |
| <span data-ttu-id="d1b16-152">creatorId</span><span class="sxs-lookup"><span data-stu-id="d1b16-152">creatorId</span></span> | <span data-ttu-id="d1b16-153">string</span><span class="sxs-lookup"><span data-stu-id="d1b16-153">string</span></span> | <span data-ttu-id="d1b16-154">Bezeichner des Benutzers oder des Dienstprinzipals, der das Abonnement erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="d1b16-154">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="d1b16-155">Wenn die App zum Erstellen des Abonnements delegierte Berechtigungen verwendet hat, enthält dieses Feld die ID des angemeldeten Nutzers, für den die App im Auftrag von diesem Nutzer angerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="d1b16-155">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="d1b16-156">Wenn die App Anwendungsberechtigungen verwendet hat, enthält dieses Feld die Id des Dienstprinzipals entsprechend der App.</span><span class="sxs-lookup"><span data-stu-id="d1b16-156">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="d1b16-157">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d1b16-157">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="d1b16-158">Maximale Abonnementdauer pro Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d1b16-158">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="d1b16-159">Ressource</span><span class="sxs-lookup"><span data-stu-id="d1b16-159">Resource</span></span>            | <span data-ttu-id="d1b16-160">Maximal zulässige Ablaufzeit</span><span class="sxs-lookup"><span data-stu-id="d1b16-160">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="d1b16-161">Mail</span><span class="sxs-lookup"><span data-stu-id="d1b16-161">Mail</span></span>                | <span data-ttu-id="d1b16-162">4320 Minuten (3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d1b16-162">4320 minutes (3 days)</span></span>    |
| <span data-ttu-id="d1b16-163">Kalender</span><span class="sxs-lookup"><span data-stu-id="d1b16-163">Calendar</span></span>            | <span data-ttu-id="d1b16-164">4320 Minuten (3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d1b16-164">4320 minutes (3 days)</span></span>    |
| <span data-ttu-id="d1b16-165">Kontakte</span><span class="sxs-lookup"><span data-stu-id="d1b16-165">Contacts</span></span>            | <span data-ttu-id="d1b16-166">4320 Minuten (3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d1b16-166">4320 minutes (3 days)</span></span>    |
| <span data-ttu-id="d1b16-167">Gruppenunterhaltungen</span><span class="sxs-lookup"><span data-stu-id="d1b16-167">Group conversations</span></span> | <span data-ttu-id="d1b16-168">4320 Minuten (3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d1b16-168">4320 minutes (3 days)</span></span>    |
| <span data-ttu-id="d1b16-169">Laufwerkstammelemente</span><span class="sxs-lookup"><span data-stu-id="d1b16-169">Drive root items</span></span>    | <span data-ttu-id="d1b16-170">4320 Minuten (3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d1b16-170">4320 minutes (3 days)</span></span> |

> <span data-ttu-id="d1b16-171">**Hinweis:** Vorhandene Anwendungen und neue Anwendungen sollten den unterstützten Wert nicht überschreiten.</span><span class="sxs-lookup"><span data-stu-id="d1b16-171">Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="d1b16-172">In Zukunft werden alle Anforderungen zum Erstellen oder Erneuern eines Abonnements über den Maximalwert hinaus fehlschlagen.</span><span class="sxs-lookup"><span data-stu-id="d1b16-172">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="d1b16-173">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d1b16-173">Relationships</span></span>

<span data-ttu-id="d1b16-174">Keine</span><span class="sxs-lookup"><span data-stu-id="d1b16-174">None</span></span>

## <a name="methods"></a><span data-ttu-id="d1b16-175">Methoden</span><span class="sxs-lookup"><span data-stu-id="d1b16-175">Methods</span></span>

| <span data-ttu-id="d1b16-176">Methode</span><span class="sxs-lookup"><span data-stu-id="d1b16-176">Method</span></span> | <span data-ttu-id="d1b16-177">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d1b16-177">Return Type</span></span> | <span data-ttu-id="d1b16-178">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1b16-178">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="d1b16-179">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="d1b16-179">Create subscription</span></span>](../api/subscription_post_subscriptions.md) | [<span data-ttu-id="d1b16-180">subscription</span><span class="sxs-lookup"><span data-stu-id="d1b16-180">subscription</span></span>](subscription.md) | <span data-ttu-id="d1b16-181">Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Microsoft Graph-Daten geändert werden.</span><span class="sxs-lookup"><span data-stu-id="d1b16-181">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="d1b16-182">Abonnement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d1b16-182">Update subscription</span></span>](../api/subscription_update.md) | [<span data-ttu-id="d1b16-183">subscription</span><span class="sxs-lookup"><span data-stu-id="d1b16-183">subscription</span></span>](subscription.md) | <span data-ttu-id="d1b16-184">Erneuert ein Abonnement durch Aktualisierung der Ablaufzeit.</span><span class="sxs-lookup"><span data-stu-id="d1b16-184">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="d1b16-185">Liste von Abonnements</span><span class="sxs-lookup"><span data-stu-id="d1b16-185">List subscriptions</span></span>](../api/subscription_list.md) | [<span data-ttu-id="d1b16-186">subscription</span><span class="sxs-lookup"><span data-stu-id="d1b16-186">subscription</span></span>](subscription.md) | <span data-ttu-id="d1b16-187">Listen aktiver Abonnements.</span><span class="sxs-lookup"><span data-stu-id="d1b16-187">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="d1b16-188">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="d1b16-188">Get subscription</span></span>](../api/subscription_get.md) | [<span data-ttu-id="d1b16-189">subscription</span><span class="sxs-lookup"><span data-stu-id="d1b16-189">subscription</span></span>](subscription.md) | <span data-ttu-id="d1b16-190">Dient zum Lesen der Eigenschaften und der Beziehungen des subscription-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d1b16-190">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="d1b16-191">Abonnement löschen</span><span class="sxs-lookup"><span data-stu-id="d1b16-191">Delete subscription</span></span>](../api/subscription_delete.md) | <span data-ttu-id="d1b16-192">Keine</span><span class="sxs-lookup"><span data-stu-id="d1b16-192">None</span></span> |<span data-ttu-id="d1b16-193">Löscht ein subscription-Objekt.</span><span class="sxs-lookup"><span data-stu-id="d1b16-193">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
