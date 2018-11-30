---
title: Ressourcentyp Abonnement
description: 'Ein Abonnement ermöglicht eine Client-app zum Empfangen von Benachrichtigungen zu Änderungen an Daten in Microsoft Graph. Abonnements werden derzeit für die folgenden Ressourcen aktiviert:'
ms.openlocfilehash: 5ece39954d661c6b7ef948d0ed7d514782fbceae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019839"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="b5545-104">Ressourcentyp Abonnement</span><span class="sxs-lookup"><span data-stu-id="b5545-104">subscription resource type</span></span>

<span data-ttu-id="b5545-105">Ein Abonnement ermöglicht eine Client-app zum Empfangen von Benachrichtigungen zu Änderungen an Daten in Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b5545-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="b5545-106">Abonnements werden derzeit für die folgenden Ressourcen aktiviert:</span><span class="sxs-lookup"><span data-stu-id="b5545-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="b5545-107">E-Mail-Nachrichten, Ereignisse und Kontakte aus Outlook.</span><span class="sxs-lookup"><span data-stu-id="b5545-107">Mail, events, and contacts from Outlook.</span></span>
- <span data-ttu-id="b5545-108">Unterhaltungen aus Office-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="b5545-108">Conversations from Office Groups.</span></span>
- <span data-ttu-id="b5545-109">Laufwerk Stammelemente aus OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b5545-109">Drive root items from OneDrive.</span></span>
- <span data-ttu-id="b5545-110">Benutzer und Gruppen aus dem Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b5545-110">Users and Groups from Azure Active Directory.</span></span>
- <span data-ttu-id="b5545-111">Benachrichtigungen über die Microsoft Graph-Sicherheit API.</span><span class="sxs-lookup"><span data-stu-id="b5545-111">Alerts from the Microsoft Graph Security API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5545-112">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b5545-112">JSON representation</span></span>

<span data-ttu-id="b5545-113">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b5545-113">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="b5545-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b5545-114">Properties</span></span>

| <span data-ttu-id="b5545-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5545-115">Property</span></span> | <span data-ttu-id="b5545-116">Typ</span><span class="sxs-lookup"><span data-stu-id="b5545-116">Type</span></span> | <span data-ttu-id="b5545-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5545-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="b5545-118">changeType</span><span class="sxs-lookup"><span data-stu-id="b5545-118">changeType</span></span> | <span data-ttu-id="b5545-119">string</span><span class="sxs-lookup"><span data-stu-id="b5545-119">string</span></span> | <span data-ttu-id="b5545-120">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b5545-120">Required.</span></span> <span data-ttu-id="b5545-121">Gibt den Typ der Änderung in der abonnierten Ressource an, die eine Benachrichtigung auslöst.</span><span class="sxs-lookup"><span data-stu-id="b5545-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="b5545-122">Unterstützte Werte sind: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="b5545-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="b5545-123">Es können mehrere Werte mithilfe einer durch Trennzeichen getrennten Liste zusammen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="b5545-123">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="b5545-124">Hinweis: Laufwerk Root Element Benachrichtigungen unterstützen nur die `updated` ChangeType.</span><span class="sxs-lookup"><span data-stu-id="b5545-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="b5545-125">Unterstützung von Benutzer- und Benachrichtigungen `updated` und `deleted` ChangeType.</span><span class="sxs-lookup"><span data-stu-id="b5545-125">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="b5545-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="b5545-126">notificationUrl</span></span> | <span data-ttu-id="b5545-127">string</span><span class="sxs-lookup"><span data-stu-id="b5545-127">string</span></span> | <span data-ttu-id="b5545-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b5545-128">Required.</span></span> <span data-ttu-id="b5545-129">Die URL des Endpunkts, die Benachrichtigungen erhalten werden.</span><span class="sxs-lookup"><span data-stu-id="b5545-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="b5545-130">Diese URL muss nutzen Sie die HTTPS Protokoll.</span><span class="sxs-lookup"><span data-stu-id="b5545-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="b5545-131">resource</span><span class="sxs-lookup"><span data-stu-id="b5545-131">resource</span></span> | <span data-ttu-id="b5545-132">string</span><span class="sxs-lookup"><span data-stu-id="b5545-132">string</span></span> | <span data-ttu-id="b5545-133">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b5545-133">Required.</span></span> <span data-ttu-id="b5545-134">Gibt die Ressource, die für Änderungen überwacht werden.</span><span class="sxs-lookup"><span data-stu-id="b5545-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="b5545-135">Die base-URL nicht einschließen (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="b5545-135">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="b5545-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b5545-136">expirationDateTime</span></span> | [<span data-ttu-id="b5545-137">dateTime</span><span class="sxs-lookup"><span data-stu-id="b5545-137">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="b5545-138">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b5545-138">Required.</span></span> <span data-ttu-id="b5545-139">Gibt Datum und Uhrzeit für das Ablaufen des Webhook-Abonnements an.</span><span class="sxs-lookup"><span data-stu-id="b5545-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="b5545-140">Die Zeit wird in UTC angegeben und kann eine Dauer aus der Erstellung des Abonnements sein, die von der abonnierten Ressource abweicht.</span><span class="sxs-lookup"><span data-stu-id="b5545-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="b5545-141">In der folgenden Tabelle finden Sie die maximale Dauer unterstützter Abonnements.</span><span class="sxs-lookup"><span data-stu-id="b5545-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="b5545-142">clientState</span><span class="sxs-lookup"><span data-stu-id="b5545-142">clientState</span></span> | <span data-ttu-id="b5545-143">string</span><span class="sxs-lookup"><span data-stu-id="b5545-143">string</span></span> | <span data-ttu-id="b5545-144">Optional.</span><span class="sxs-lookup"><span data-stu-id="b5545-144">Optional.</span></span> <span data-ttu-id="b5545-145">Gibt den Wert der `clientState`-Eigenschaft an, die in jeder Benachrichtigung vom Dienst gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="b5545-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="b5545-146">Die Höchstlänge beträgt 128 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="b5545-146">The maximum length is 128 characters.</span></span> <span data-ttu-id="b5545-147">Der Client kann prüfen, ob die Benachrichtigung vom Dienst stammt, indem er den Wert der mit dem Abonnement gesendeten `clientState`-Eigenschaft mit dem Wert der mit jeder Benachrichtigung empfangenen `clientState`-Eigenschaft vergleicht.</span><span class="sxs-lookup"><span data-stu-id="b5545-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="b5545-148">id</span><span class="sxs-lookup"><span data-stu-id="b5545-148">id</span></span> | <span data-ttu-id="b5545-149">string</span><span class="sxs-lookup"><span data-stu-id="b5545-149">string</span></span> | <span data-ttu-id="b5545-p109">Eindeutige ID für das Abonnement. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b5545-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="b5545-152">applicationId</span><span class="sxs-lookup"><span data-stu-id="b5545-152">applicationId</span></span> | <span data-ttu-id="b5545-153">string</span><span class="sxs-lookup"><span data-stu-id="b5545-153">string</span></span> | <span data-ttu-id="b5545-154">Bezeichner der Anwendung verwendet, um das Abonnement zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="b5545-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="b5545-155">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b5545-155">Read-only.</span></span> |
| <span data-ttu-id="b5545-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="b5545-156">creatorId</span></span> | <span data-ttu-id="b5545-157">string</span><span class="sxs-lookup"><span data-stu-id="b5545-157">string</span></span> | <span data-ttu-id="b5545-158">Bezeichner des Benutzers oder der Dienstprinzipalnamen, die das Abonnement erstellt.</span><span class="sxs-lookup"><span data-stu-id="b5545-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="b5545-159">Wenn die app verwendet Berechtigungen zum Erstellen des Abonnements delegiert, enthält dieses Feld die Id des angemeldeten Benutzers an, den die app im Auftrag von aufgerufen.</span><span class="sxs-lookup"><span data-stu-id="b5545-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="b5545-160">Wenn die app Anwendungsberechtigungen verwendet wird, enthält dieses Feld die Id des Prinzipals Service für die app.</span><span class="sxs-lookup"><span data-stu-id="b5545-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="b5545-161">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b5545-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="b5545-162">Maximale Abonnementdauer pro Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b5545-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="b5545-163">Ressource</span><span class="sxs-lookup"><span data-stu-id="b5545-163">Resource</span></span>            | <span data-ttu-id="b5545-164">Maximal zulässige Ablaufzeit</span><span class="sxs-lookup"><span data-stu-id="b5545-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="b5545-165">Mail</span><span class="sxs-lookup"><span data-stu-id="b5545-165">Mail</span></span>                | <span data-ttu-id="b5545-166">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="b5545-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b5545-167">Kalender</span><span class="sxs-lookup"><span data-stu-id="b5545-167">Calendar</span></span>            | <span data-ttu-id="b5545-168">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="b5545-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b5545-169">Kontakte</span><span class="sxs-lookup"><span data-stu-id="b5545-169">Contacts</span></span>            | <span data-ttu-id="b5545-170">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="b5545-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b5545-171">Gruppenunterhaltungen</span><span class="sxs-lookup"><span data-stu-id="b5545-171">Group conversations</span></span> | <span data-ttu-id="b5545-172">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="b5545-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b5545-173">Laufwerkstammelemente</span><span class="sxs-lookup"><span data-stu-id="b5545-173">Drive root items</span></span>    | <span data-ttu-id="b5545-174">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="b5545-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b5545-175">Sicherheitshinweise</span><span class="sxs-lookup"><span data-stu-id="b5545-175">Security alerts</span></span>     | <span data-ttu-id="b5545-176">43200 Minuten (unter 30 Tage)</span><span class="sxs-lookup"><span data-stu-id="b5545-176">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="b5545-177">**Hinweis:** Vorhandene Anwendungen und neuen Anwendungen sollte den unterstützten Wert nicht überschreiten.</span><span class="sxs-lookup"><span data-stu-id="b5545-177">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="b5545-178">In der Zukunft fehl alle Anforderungen zum Erstellen oder erneuern Sie ein Abonnement über den Höchstwert hinaus.</span><span class="sxs-lookup"><span data-stu-id="b5545-178">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="b5545-179">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b5545-179">Relationships</span></span>

<span data-ttu-id="b5545-180">Keine</span><span class="sxs-lookup"><span data-stu-id="b5545-180">None</span></span>

## <a name="methods"></a><span data-ttu-id="b5545-181">Methoden</span><span class="sxs-lookup"><span data-stu-id="b5545-181">Methods</span></span>

| <span data-ttu-id="b5545-182">Methode</span><span class="sxs-lookup"><span data-stu-id="b5545-182">Method</span></span> | <span data-ttu-id="b5545-183">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b5545-183">Return Type</span></span> | <span data-ttu-id="b5545-184">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5545-184">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="b5545-185">Create subscription</span><span class="sxs-lookup"><span data-stu-id="b5545-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="b5545-186">Abonnement</span><span class="sxs-lookup"><span data-stu-id="b5545-186">subscription</span></span>](subscription.md) | <span data-ttu-id="b5545-187">Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Microsoft Graph-Daten geändert werden.</span><span class="sxs-lookup"><span data-stu-id="b5545-187">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="b5545-188">Update subscription</span><span class="sxs-lookup"><span data-stu-id="b5545-188">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="b5545-189">Abonnement</span><span class="sxs-lookup"><span data-stu-id="b5545-189">subscription</span></span>](subscription.md) | <span data-ttu-id="b5545-190">Erneuert ein Abonnement durch Aktualisierung der Ablaufzeit.</span><span class="sxs-lookup"><span data-stu-id="b5545-190">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="b5545-191">Liste von Abonnements</span><span class="sxs-lookup"><span data-stu-id="b5545-191">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="b5545-192">subscription</span><span class="sxs-lookup"><span data-stu-id="b5545-192">subscription</span></span>](subscription.md) | <span data-ttu-id="b5545-193">Listen aktiver Abonnements.</span><span class="sxs-lookup"><span data-stu-id="b5545-193">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="b5545-194">Get subscription</span><span class="sxs-lookup"><span data-stu-id="b5545-194">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="b5545-195">Abonnement</span><span class="sxs-lookup"><span data-stu-id="b5545-195">subscription</span></span>](subscription.md) | <span data-ttu-id="b5545-196">Dient zum Lesen der Eigenschaften und der Beziehungen des subscription-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b5545-196">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="b5545-197">Delete subscription</span><span class="sxs-lookup"><span data-stu-id="b5545-197">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="b5545-198">Keine</span><span class="sxs-lookup"><span data-stu-id="b5545-198">None</span></span> |<span data-ttu-id="b5545-199">Löscht ein subscription-Objekt.</span><span class="sxs-lookup"><span data-stu-id="b5545-199">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
