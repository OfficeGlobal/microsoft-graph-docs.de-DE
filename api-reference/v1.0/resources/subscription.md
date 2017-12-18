# <a name="subscription-resource-type"></a><span data-ttu-id="41503-101">Abonnementressourcentyp</span><span class="sxs-lookup"><span data-stu-id="41503-101">Subscription Resource Type</span></span>
<span data-ttu-id="41503-102">Mit einem Abonnement kann eine Client-App Benachrichtigungen zu Daten in Microsoft Graph erhalten.</span><span class="sxs-lookup"><span data-stu-id="41503-102">A subscription allows a client app to receive notifications about data on the Microsoft Graph. Currently subscriptions are enabled for the following datasets:</span></span> <span data-ttu-id="41503-103">Für die folgenden Datensätze sind derzeit Abonnements aktiviert:</span><span class="sxs-lookup"><span data-stu-id="41503-103">Currently, subscriptions are enabled for the following datasets:</span></span>

1. <span data-ttu-id="41503-104">E-Mail, Ereignisse und Kontakte aus Outlook</span><span class="sxs-lookup"><span data-stu-id="41503-104">Mail, events, and contacts from Outlook</span></span>
1. <span data-ttu-id="41503-105">Unterhaltungen aus Office-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="41503-105">Conversations from Office Groups.</span></span>
1. <span data-ttu-id="41503-106">Laufwerkstammelemente aus OneDrive</span><span class="sxs-lookup"><span data-stu-id="41503-106">Drive root items from OneDrive</span></span> 


## <a name="json-representation"></a><span data-ttu-id="41503-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="41503-107">JSON representation</span></span>

<span data-ttu-id="41503-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="41503-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscription"
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string"
}

```
## <a name="properties"></a><span data-ttu-id="41503-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="41503-109">Properties</span></span>
| <span data-ttu-id="41503-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="41503-110">Property</span></span>     | <span data-ttu-id="41503-111">Typ</span><span class="sxs-lookup"><span data-stu-id="41503-111">Type</span></span>   |<span data-ttu-id="41503-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41503-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41503-113">changeType</span><span class="sxs-lookup"><span data-stu-id="41503-113">changeType</span></span>|<span data-ttu-id="41503-114">string</span><span class="sxs-lookup"><span data-stu-id="41503-114">string</span></span>|<span data-ttu-id="41503-115">Gibt den Typ der Änderung in der abonnierten Ressource an, die eine Benachrichtigung auslöst.</span><span class="sxs-lookup"><span data-stu-id="41503-115">Indicates the type of change in the subscribed resource that will raise a notification. The supported values are: , , . Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="41503-116">Unterstützte Werte sind: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="41503-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="41503-117">Es können mehrere Werte mithilfe einer durch Trennzeichen getrennten Liste zusammen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="41503-117">Multiple values can be combined using a comma-separated list.</span></span>|
|<span data-ttu-id="41503-118">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="41503-118">notificationUrl</span></span>|<span data-ttu-id="41503-119">string</span><span class="sxs-lookup"><span data-stu-id="41503-119">string</span></span>|<span data-ttu-id="41503-p103">Die URL des Endpunkts, der die Benachrichtigungen erhält. Diese URL muss das HTTPS-Protokoll verwenden.</span><span class="sxs-lookup"><span data-stu-id="41503-p103">The URL of the endpoint that will receive the notifications. This URL has to make use of the HTTPS protocol.</span></span>|
|<span data-ttu-id="41503-122">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="41503-122">resource</span></span>|<span data-ttu-id="41503-123">string</span><span class="sxs-lookup"><span data-stu-id="41503-123">string</span></span>|<span data-ttu-id="41503-p104">Gibt die Ressource an, deren Änderungen überwacht werden. Schließen Sie die Basis-URL nicht mit ein („https://graph.microsoft.com/v1.0/“).</span><span class="sxs-lookup"><span data-stu-id="41503-p104">Specifies the resource that will be monitored for changes. Do not include the base URL ("https://graph.microsoft.com/v1.0/").</span></span>|
|<span data-ttu-id="41503-126">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="41503-126">expirationDateTime</span></span>|[<span data-ttu-id="41503-127">dateTime</span><span class="sxs-lookup"><span data-stu-id="41503-127">dateTime</span></span>](http://tools.ietf.org/html/rfc3339)|<span data-ttu-id="41503-128">Gibt Datum und Uhrzeit für das Ablaufen des Webhook-Abonnements an.</span><span class="sxs-lookup"><span data-stu-id="41503-128">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="41503-129">Die Zeit wird in UTC angegeben und kann eine Dauer aus der Erstellung des Abonnements sein, die von der abonnierten Ressource abweicht.</span><span class="sxs-lookup"><span data-stu-id="41503-129">Specifies the date and time when the webhook subscription expires. The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.  See the table below for maximum values.</span></span>  <span data-ttu-id="41503-130">In der folgenden Tabelle finden Sie die maximale Dauer unterstützter Abonnements.</span><span class="sxs-lookup"><span data-stu-id="41503-130">See the table below for maximum supported subscription length of time.</span></span> |
|<span data-ttu-id="41503-131">clientState</span><span class="sxs-lookup"><span data-stu-id="41503-131">clientState</span></span>|<span data-ttu-id="41503-132">string</span><span class="sxs-lookup"><span data-stu-id="41503-132">string</span></span>|<span data-ttu-id="41503-133">Gibt den Wert der `clientState`-Eigenschaft an, die in jeder Benachrichtigung vom Dienst gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="41503-133">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="41503-134">Die Höchstlänge beträgt 128 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="41503-134">The maximum length is 255 characters.</span></span> <span data-ttu-id="41503-135">Der Client kann prüfen, ob die Benachrichtigung vom Dienst stammt, indem er den Wert der mit dem Abonnement gesendeten `clientState`-Eigenschaft mit dem Wert der mit jeder Benachrichtigung empfangenen `clientState`-Eigenschaft vergleicht.</span><span class="sxs-lookup"><span data-stu-id="41503-135">Specifies the value of the  property sent by the service in each notification. The maximum length is 128 characters. The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span>|
|<span data-ttu-id="41503-136">id</span><span class="sxs-lookup"><span data-stu-id="41503-136">id</span></span>|<span data-ttu-id="41503-137">string</span><span class="sxs-lookup"><span data-stu-id="41503-137">string</span></span>|<span data-ttu-id="41503-p107">Eindeutige ID für das Abonnement. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="41503-p107">Unique identifier for the subscription. Read-only.</span></span>|

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="41503-140">Maximale Abonnementdauer pro Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="41503-140">Maximum length of subscription per resource type</span></span>
| <span data-ttu-id="41503-141">Ressource</span><span class="sxs-lookup"><span data-stu-id="41503-141">Resource</span></span> | <span data-ttu-id="41503-142">Maximal zulässige Ablaufzeit</span><span class="sxs-lookup"><span data-stu-id="41503-142">Maximum Expiration Time</span></span> |
|:---------------------|:--------------------|
|<span data-ttu-id="41503-143">Mail</span><span class="sxs-lookup"><span data-stu-id="41503-143">Mail</span></span>| <span data-ttu-id="41503-144">4230 Minuten.</span><span class="sxs-lookup"><span data-stu-id="41503-144">4230 minutes.</span></span>|
|<span data-ttu-id="41503-145">Kalender</span><span class="sxs-lookup"><span data-stu-id="41503-145">Calendar</span></span>| <span data-ttu-id="41503-146">4230 Minuten.</span><span class="sxs-lookup"><span data-stu-id="41503-146">4230 minutes.</span></span>|
|<span data-ttu-id="41503-147">Kontakte</span><span class="sxs-lookup"><span data-stu-id="41503-147">Contacts</span></span>| <span data-ttu-id="41503-148">4230 Minuten.</span><span class="sxs-lookup"><span data-stu-id="41503-148">4230 minutes.</span></span>|
|<span data-ttu-id="41503-149">Gruppenunterhaltungen</span><span class="sxs-lookup"><span data-stu-id="41503-149">Group conversations</span></span>| <span data-ttu-id="41503-150">4230 Minuten.</span><span class="sxs-lookup"><span data-stu-id="41503-150">4230 minutes.</span></span>|
|<span data-ttu-id="41503-151">Laufwerkstammelemente</span><span class="sxs-lookup"><span data-stu-id="41503-151">Drive root items</span></span>| <span data-ttu-id="41503-152">43200  Minuten</span><span class="sxs-lookup"><span data-stu-id="41503-152">43200 minutes.</span></span> <span data-ttu-id="41503-153">Vorhandene Anwendungen und neue Anwendungen sollten den unterstützten Wert nicht überschreiten.</span><span class="sxs-lookup"><span data-stu-id="41503-153">Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="41503-154">In künftigen Versionen sind keine höheren Werte zulässig.</span><span class="sxs-lookup"><span data-stu-id="41503-154">Higher values won't be permitted in upcoming releases.</span></span> |

## <a name="relationships"></a><span data-ttu-id="41503-155">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="41503-155">Relationships</span></span>
<span data-ttu-id="41503-156">Keine</span><span class="sxs-lookup"><span data-stu-id="41503-156">None</span></span>


## <a name="methods"></a><span data-ttu-id="41503-157">Methoden</span><span class="sxs-lookup"><span data-stu-id="41503-157">Methods</span></span>

| <span data-ttu-id="41503-158">Methode</span><span class="sxs-lookup"><span data-stu-id="41503-158">Method</span></span>           | <span data-ttu-id="41503-159">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="41503-159">Return Type</span></span>    |<span data-ttu-id="41503-160">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41503-160">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="41503-161">Create subscription</span><span class="sxs-lookup"><span data-stu-id="41503-161">Create subscription</span></span>](../api/subscription_post_subscriptions.md) | [<span data-ttu-id="41503-162">Abonnement</span><span class="sxs-lookup"><span data-stu-id="41503-162">subscription</span></span>](subscription.md) |<span data-ttu-id="41503-163">Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Microsoft Graph-Daten geändert werden.</span><span class="sxs-lookup"><span data-stu-id="41503-163">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span>|
|[<span data-ttu-id="41503-164">Update subscription</span><span class="sxs-lookup"><span data-stu-id="41503-164">Update subscription</span></span>](../api/subscription_update.md) | [<span data-ttu-id="41503-165">Abonnement</span><span class="sxs-lookup"><span data-stu-id="41503-165">subscription</span></span>](subscription.md) |<span data-ttu-id="41503-166">Erneuert ein Abonnement durch Aktualisierung der Ablaufzeit.</span><span class="sxs-lookup"><span data-stu-id="41503-166">Renews a subscription by updating its expiration time.</span></span>|
|[<span data-ttu-id="41503-167">Get subscription</span><span class="sxs-lookup"><span data-stu-id="41503-167">Get subscription</span></span>](../api/subscription_get.md) | [<span data-ttu-id="41503-168">Abonnement</span><span class="sxs-lookup"><span data-stu-id="41503-168">subscription</span></span>](subscription.md) |<span data-ttu-id="41503-169">Dient zum Lesen der Eigenschaften und der Beziehungen des subscription-Objekts.</span><span class="sxs-lookup"><span data-stu-id="41503-169">Reads properties and relationships of subscription object.</span></span>|
|[<span data-ttu-id="41503-170">Delete subscription</span><span class="sxs-lookup"><span data-stu-id="41503-170">Delete subscription</span></span>](../api/subscription_delete.md) | <span data-ttu-id="41503-171">Keine</span><span class="sxs-lookup"><span data-stu-id="41503-171">None</span></span> |<span data-ttu-id="41503-172">Löscht ein subscription-Objekt.</span><span class="sxs-lookup"><span data-stu-id="41503-172">Deletes a subscription object.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
