# <a name="subscription-resource-type"></a><span data-ttu-id="d1d96-101">Ressourcentyp Abonnement</span><span class="sxs-lookup"><span data-stu-id="d1d96-101">Subscription resource type</span></span>

<span data-ttu-id="d1d96-102">Mit einem Abonnement kann eine Client-App Benachrichtigungen zu Änderungen an den Daten in Microsoft Graph erhalten.</span><span class="sxs-lookup"><span data-stu-id="d1d96-102">A subscription allows a client app to receive notifications about data on the Microsoft Graph.</span></span> <span data-ttu-id="d1d96-103">Abonnements werden derzeit für die folgenden Ressourcen aktiviert:</span><span class="sxs-lookup"><span data-stu-id="d1d96-103">Currently, subscriptions are enabled for the following datasets:</span></span>

- <span data-ttu-id="d1d96-104">E-Mail, Ereignisse und Kontakte aus Outlook</span><span class="sxs-lookup"><span data-stu-id="d1d96-104">Mail, events, and contacts from Outlook</span></span>
- <span data-ttu-id="d1d96-105">Unterhaltungen aus Office-Gruppen</span><span class="sxs-lookup"><span data-stu-id="d1d96-105">Conversations from Office Groups.</span></span>
- <span data-ttu-id="d1d96-106">Laufwerkstammelemente aus OneDrive</span><span class="sxs-lookup"><span data-stu-id="d1d96-106">Drive root items from OneDrive</span></span>
- <span data-ttu-id="d1d96-107">Benutzer und Gruppen aus dem Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="d1d96-107">Users and Groups from Azure Active Directory</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1d96-108">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d1d96-108">JSON representation</span></span>

<span data-ttu-id="d1d96-109">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d1d96-109">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d1d96-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d1d96-110">Properties</span></span>

| <span data-ttu-id="d1d96-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d1d96-111">Property</span></span> | <span data-ttu-id="d1d96-112">Typ</span><span class="sxs-lookup"><span data-stu-id="d1d96-112">Type</span></span> | <span data-ttu-id="d1d96-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1d96-113">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="d1d96-114">changeType</span><span class="sxs-lookup"><span data-stu-id="d1d96-114">changeType</span></span> | <span data-ttu-id="d1d96-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1d96-115">string</span></span> | <span data-ttu-id="d1d96-116">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d1d96-116">Required.</span></span> <span data-ttu-id="d1d96-117">Gibt den Typ der Änderung in der abonnierten Ressource an, die eine Benachrichtigung auslöst.</span><span class="sxs-lookup"><span data-stu-id="d1d96-117">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="d1d96-118">Unterstützte Werte sind: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="d1d96-118">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="d1d96-119">Es können mehrere Werte mithilfe einer durch Komma getrennten Liste zusammen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="d1d96-119">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="d1d96-120">Hinweis: Laufwerk Stamm-Element Benachrichtigungs-Support unterstützen nur den `updated` ChangeType.</span><span class="sxs-lookup"><span data-stu-id="d1d96-120">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="d1d96-121">Support für Benutzer und Gruppen-Benachrichtigungen `updated` und `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="d1d96-121">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="d1d96-122">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="d1d96-122">notificationUrl</span></span> | <span data-ttu-id="d1d96-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1d96-123">string</span></span> | <span data-ttu-id="d1d96-124">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d1d96-124">Required.</span></span> <span data-ttu-id="d1d96-125">Die URL des Endpunkts, die Benachrichtigungen erhalten werden.</span><span class="sxs-lookup"><span data-stu-id="d1d96-125">The URL of the application that will receive the push notifications.</span></span> <span data-ttu-id="d1d96-126">Diese URL muss das HTTPS-Protokoll nutzen.</span><span class="sxs-lookup"><span data-stu-id="d1d96-126">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="d1d96-127">Ressource</span><span class="sxs-lookup"><span data-stu-id="d1d96-127">resource</span></span> | <span data-ttu-id="d1d96-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1d96-128">string</span></span> | <span data-ttu-id="d1d96-129">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d1d96-129">Required.</span></span> <span data-ttu-id="d1d96-130">Gibt die Ressource ab, die für Änderungen überwacht wird.</span><span class="sxs-lookup"><span data-stu-id="d1d96-130">Specifies the resource that will be monitored for changes. Do not include the base URL ("https://graph.microsoft.com/v1.0/").</span></span> <span data-ttu-id="d1d96-131">Die Basis-URL nicht einschließen (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="d1d96-131">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="d1d96-132">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d1d96-132">expirationDateTime</span></span> | [<span data-ttu-id="d1d96-133">dateTime</span><span class="sxs-lookup"><span data-stu-id="d1d96-133">dateTime</span></span>](http://tools.ietf.org/html/rfc3339) | <span data-ttu-id="d1d96-134">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d1d96-134">Required.</span></span> <span data-ttu-id="d1d96-135">Gibt Datum und Uhrzeit für das Ablaufen des Webhook-Abonnements an.</span><span class="sxs-lookup"><span data-stu-id="d1d96-135">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="d1d96-136">Die Zeit wird in UTC angegeben und kann eine Dauer aus der Erstellung des Abonnements sein, die von der abonnierten Ressource abweicht.</span><span class="sxs-lookup"><span data-stu-id="d1d96-136">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="d1d96-137">In der folgenden Tabelle finden Sie die maximale Dauer unterstützter Abonnements.</span><span class="sxs-lookup"><span data-stu-id="d1d96-137">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="d1d96-138">clientState</span><span class="sxs-lookup"><span data-stu-id="d1d96-138">clientState</span></span> | <span data-ttu-id="d1d96-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1d96-139">string</span></span> | <span data-ttu-id="d1d96-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="d1d96-140">Optional.</span></span> <span data-ttu-id="d1d96-141">Gibt den Wert der `clientState`-Eigenschaft an, die in jeder Benachrichtigung vom Dienst gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="d1d96-141">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="d1d96-142">Die Höchstlänge beträgt 128 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="d1d96-142">The maximum length is 128 characters.</span></span> <span data-ttu-id="d1d96-143">Der Client kann prüfen, ob die Benachrichtigung vom Dienst stammt, indem er den Wert der mit dem Abonnement gesendeten `clientState`-Eigenschaft mit dem Wert der mit jeder Benachrichtigung empfangenen `clientState`-Eigenschaft vergleicht.</span><span class="sxs-lookup"><span data-stu-id="d1d96-143">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="d1d96-144">ID</span><span class="sxs-lookup"><span data-stu-id="d1d96-144">id</span></span> | <span data-ttu-id="d1d96-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1d96-145">string</span></span> | <span data-ttu-id="d1d96-p108">Eindeutige ID für das Abonnement. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d1d96-p108">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="d1d96-148">applicationId</span><span class="sxs-lookup"><span data-stu-id="d1d96-148">applicationId</span></span> | <span data-ttu-id="d1d96-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1d96-149">string</span></span> | <span data-ttu-id="d1d96-150">Bezeichner der Anwendung, die verwendet wird, um das Abonnement zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="d1d96-150">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="d1d96-151">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d1d96-151">Read-only.</span></span> |
| <span data-ttu-id="d1d96-152">creatorId</span><span class="sxs-lookup"><span data-stu-id="d1d96-152">creatorId</span></span> | <span data-ttu-id="d1d96-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1d96-153">string</span></span> | <span data-ttu-id="d1d96-154">Bezeichner des Benutzers oder des Dienstprinzipals, der das Abonnement erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="d1d96-154">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="d1d96-155">Wenn die App zum Erstellen des Abonnements delegierte Berechtigungen verwendet hat, enthält dieses Feld die ID des angemeldeten Nutzers, für den die App im Auftrag von diesem Nutzer angerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="d1d96-155">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="d1d96-156">Wenn die App Anwendungsberechtigungen verwendet hat, enthält dieses Feld die Id des Dienstprinzipals entsprechend der App.</span><span class="sxs-lookup"><span data-stu-id="d1d96-156">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="d1d96-157">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d1d96-157">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="d1d96-158">Maximale Abonnementdauer pro Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d1d96-158">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="d1d96-159">Ressource</span><span class="sxs-lookup"><span data-stu-id="d1d96-159">Resource</span></span>            | <span data-ttu-id="d1d96-160">Maximal zulässige Ablaufzeit</span><span class="sxs-lookup"><span data-stu-id="d1d96-160">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="d1d96-161">E-Mail</span><span class="sxs-lookup"><span data-stu-id="d1d96-161">Mail</span></span>                | <span data-ttu-id="d1d96-162">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d1d96-162">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="d1d96-163">Kalender</span><span class="sxs-lookup"><span data-stu-id="d1d96-163">Calendar</span></span>            | <span data-ttu-id="d1d96-164">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d1d96-164">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="d1d96-165">Kontakte</span><span class="sxs-lookup"><span data-stu-id="d1d96-165">Contacts</span></span>            | <span data-ttu-id="d1d96-166">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d1d96-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="d1d96-167">Gruppenunterhaltungen</span><span class="sxs-lookup"><span data-stu-id="d1d96-167">Group conversations</span></span> | <span data-ttu-id="d1d96-168">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d1d96-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="d1d96-169">Laufwerkstammelemente</span><span class="sxs-lookup"><span data-stu-id="d1d96-169">Drive root items</span></span>    | <span data-ttu-id="d1d96-170">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d1d96-170">4230 minutes (under 3 days)</span></span>    |

> <span data-ttu-id="d1d96-171">**Hinweis:** Vorhandene Anwendungen und neue Anwendungen sollten den unterstützten Wert nicht überschreiten.</span><span class="sxs-lookup"><span data-stu-id="d1d96-171">Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="d1d96-172">In Zukunft werden alle Anforderungen zum Erstellen oder Erneuern eines Abonnements über den Maximalwert hinaus fehlschlagen.</span><span class="sxs-lookup"><span data-stu-id="d1d96-172">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="d1d96-173">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d1d96-173">Relationships</span></span>

<span data-ttu-id="d1d96-174">Keine</span><span class="sxs-lookup"><span data-stu-id="d1d96-174">None</span></span>

## <a name="methods"></a><span data-ttu-id="d1d96-175">Methoden</span><span class="sxs-lookup"><span data-stu-id="d1d96-175">Methods</span></span>

| <span data-ttu-id="d1d96-176">Methode</span><span class="sxs-lookup"><span data-stu-id="d1d96-176">Method</span></span> | <span data-ttu-id="d1d96-177">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d1d96-177">Return Type</span></span> | <span data-ttu-id="d1d96-178">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1d96-178">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="d1d96-179">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="d1d96-179">Create subscription</span></span>](../api/subscription_post_subscriptions.md) | [<span data-ttu-id="d1d96-180">Abonnement</span><span class="sxs-lookup"><span data-stu-id="d1d96-180">subscription</span></span>](subscription.md) | <span data-ttu-id="d1d96-181">Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Microsoft Graph-Daten geändert werden.</span><span class="sxs-lookup"><span data-stu-id="d1d96-181">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="d1d96-182">Abonnement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d1d96-182">Update subscription</span></span>](../api/subscription_update.md) | [<span data-ttu-id="d1d96-183">Abonnement</span><span class="sxs-lookup"><span data-stu-id="d1d96-183">subscription</span></span>](subscription.md) | <span data-ttu-id="d1d96-184">Erneuert ein Abonnement durch Aktualisierung der Ablaufzeit.</span><span class="sxs-lookup"><span data-stu-id="d1d96-184">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="d1d96-185">Liste von Abonnements</span><span class="sxs-lookup"><span data-stu-id="d1d96-185">List subscriptions</span></span>](../api/subscription_list.md) | [<span data-ttu-id="d1d96-186">Abonnement</span><span class="sxs-lookup"><span data-stu-id="d1d96-186">subscription</span></span>](subscription.md) | <span data-ttu-id="d1d96-187">Listen aktiver Abonnements.</span><span class="sxs-lookup"><span data-stu-id="d1d96-187">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="d1d96-188">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="d1d96-188">Get subscription</span></span>](../api/subscription_get.md) | [<span data-ttu-id="d1d96-189">Abonnement</span><span class="sxs-lookup"><span data-stu-id="d1d96-189">subscription</span></span>](subscription.md) | <span data-ttu-id="d1d96-190">Dient zum Lesen der Eigenschaften und der Beziehungen des subscription-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d1d96-190">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="d1d96-191">Abonnement löschen</span><span class="sxs-lookup"><span data-stu-id="d1d96-191">Delete subscription</span></span>](../api/subscription_delete.md) | <span data-ttu-id="d1d96-192">Keine</span><span class="sxs-lookup"><span data-stu-id="d1d96-192">None</span></span> |<span data-ttu-id="d1d96-193">Löscht ein subscription-Objekt.</span><span class="sxs-lookup"><span data-stu-id="d1d96-193">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
