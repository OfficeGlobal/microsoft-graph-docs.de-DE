---
title: subscription-Ressourcentyp
description: 'Mit einem Abonnement kann eine Client-App Benachrichtigungen zu Datenänderungen in Microsoft Graph erhalten. Für die folgenden Ressourcen sind derzeit Abonnements aktiviert:'
localization_priority: Priority
author: piotrci
ms.openlocfilehash: db3a536395f327115af69f769f37c823013ec7fa
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155762"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="dcbef-104">subscription-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dcbef-104">Subscription resource type</span></span>

<span data-ttu-id="dcbef-105">Mit einem Abonnement kann eine Client-App Benachrichtigungen zu Datenänderungen in Microsoft Graph erhalten.</span><span class="sxs-lookup"><span data-stu-id="dcbef-105">A subscription allows a client app to receive notifications about data on the Microsoft Graph.</span></span> <span data-ttu-id="dcbef-106">Für die folgenden Ressourcen sind derzeit Abonnements aktiviert:</span><span class="sxs-lookup"><span data-stu-id="dcbef-106">Currently, subscriptions are enabled for the following datasets:</span></span>

- <span data-ttu-id="dcbef-107">[Nachrichten][], [Ereignisse][] oder [Kontakte][] in Outlook</span><span class="sxs-lookup"><span data-stu-id="dcbef-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="dcbef-108">[Unterhaltungen][] einer Office 365-Gruppe</span><span class="sxs-lookup"><span data-stu-id="dcbef-108">[post][] of an Office 365 group</span></span>
- <span data-ttu-id="dcbef-109">Inhalte in der Hierarchie eines [driveItem][]-Stammordners in OneDrive for Business bzw. eines [driveItem][]-Stammordners oder -Unterordners im persönlichen OneDrive eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="dcbef-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="dcbef-110">[Benutzer][] oder [Gruppen][] in Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="dcbef-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="dcbef-111">[Warnungen][] aus der Microsoft Graph-Sicherheits-API</span><span class="sxs-lookup"><span data-stu-id="dcbef-111">An [alert][] from the Microsoft Graph Security API</span></span>

## <a name="json-representation"></a><span data-ttu-id="dcbef-112">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dcbef-112">JSON representation</span></span>

<span data-ttu-id="dcbef-113">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dcbef-113">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="dcbef-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dcbef-114">Properties</span></span>

| <span data-ttu-id="dcbef-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dcbef-115">Property</span></span> | <span data-ttu-id="dcbef-116">Typ</span><span class="sxs-lookup"><span data-stu-id="dcbef-116">Type</span></span> | <span data-ttu-id="dcbef-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dcbef-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="dcbef-118">changeType</span><span class="sxs-lookup"><span data-stu-id="dcbef-118">changeType</span></span> | <span data-ttu-id="dcbef-119">string</span><span class="sxs-lookup"><span data-stu-id="dcbef-119">string</span></span> | <span data-ttu-id="dcbef-120">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dcbef-120">Required.</span></span> <span data-ttu-id="dcbef-121">Gibt den Typ der Änderung in der abonnierten Ressource an, die eine Benachrichtigung auslöst.</span><span class="sxs-lookup"><span data-stu-id="dcbef-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="dcbef-122">Unterstützte Werte sind: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="dcbef-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="dcbef-123">Es können mehrere Werte mithilfe einer durch Trennzeichen getrennten Liste zusammen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="dcbef-123">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="dcbef-124">Hinweis: Benachrichtigungen für Laufwerkstammelemente unterstützen nur den `updated`-changeType.</span><span class="sxs-lookup"><span data-stu-id="dcbef-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="dcbef-125">Benachrichtigungen für Benutzer und Gruppen unterstützen den `updated`- und den `deleted`-changeType.</span><span class="sxs-lookup"><span data-stu-id="dcbef-125">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="dcbef-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="dcbef-126">notificationUrl</span></span> | <span data-ttu-id="dcbef-127">string</span><span class="sxs-lookup"><span data-stu-id="dcbef-127">string</span></span> | <span data-ttu-id="dcbef-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dcbef-128">Required.</span></span> <span data-ttu-id="dcbef-129">Die URL des Endpunkts, der die Benachrichtigungen erhält.</span><span class="sxs-lookup"><span data-stu-id="dcbef-129">The URL of the endpoint that will receive the notifications. This URL has to make use of the HTTPS protocol.</span></span> <span data-ttu-id="dcbef-130">Diese URL muss das HTTPS-Protokoll verwenden.</span><span class="sxs-lookup"><span data-stu-id="dcbef-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="dcbef-131">resource</span><span class="sxs-lookup"><span data-stu-id="dcbef-131">resource</span></span> | <span data-ttu-id="dcbef-132">string</span><span class="sxs-lookup"><span data-stu-id="dcbef-132">string</span></span> | <span data-ttu-id="dcbef-133">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dcbef-133">Required.</span></span> <span data-ttu-id="dcbef-134">Gibt die Ressource an, deren Änderungen überwacht werden.</span><span class="sxs-lookup"><span data-stu-id="dcbef-134">The  property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="dcbef-135">Fügen Sie nicht die Basis-URL hinzu (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="dcbef-135">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="dcbef-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dcbef-136">expirationDateTime</span></span> | [<span data-ttu-id="dcbef-137">dateTime</span><span class="sxs-lookup"><span data-stu-id="dcbef-137">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="dcbef-138">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dcbef-138">Required.</span></span> <span data-ttu-id="dcbef-139">Gibt Datum und Uhrzeit für das Ablaufen des Webhook-Abonnements an.</span><span class="sxs-lookup"><span data-stu-id="dcbef-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="dcbef-140">Die Zeit wird in UTC angegeben und kann eine Dauer aus der Erstellung des Abonnements sein, die von der abonnierten Ressource abweicht.</span><span class="sxs-lookup"><span data-stu-id="dcbef-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="dcbef-141">In der folgenden Tabelle finden Sie die maximale Dauer unterstützter Abonnements.</span><span class="sxs-lookup"><span data-stu-id="dcbef-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="dcbef-142">clientState</span><span class="sxs-lookup"><span data-stu-id="dcbef-142">clientState</span></span> | <span data-ttu-id="dcbef-143">string</span><span class="sxs-lookup"><span data-stu-id="dcbef-143">string</span></span> | <span data-ttu-id="dcbef-144">Optional.</span><span class="sxs-lookup"><span data-stu-id="dcbef-144">Optional.</span></span> <span data-ttu-id="dcbef-145">Gibt den Wert der `clientState`-Eigenschaft an, die in jeder Benachrichtigung vom Dienst gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="dcbef-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="dcbef-146">Die Höchstlänge beträgt 128 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="dcbef-146">The maximum length is 128 characters.</span></span> <span data-ttu-id="dcbef-147">Der Client kann prüfen, ob die Benachrichtigung vom Dienst stammt, indem er den Wert der mit dem Abonnement gesendeten `clientState`-Eigenschaft mit dem Wert der mit jeder Benachrichtigung empfangenen `clientState`-Eigenschaft vergleicht.</span><span class="sxs-lookup"><span data-stu-id="dcbef-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="dcbef-148">id</span><span class="sxs-lookup"><span data-stu-id="dcbef-148">id</span></span> | <span data-ttu-id="dcbef-149">string</span><span class="sxs-lookup"><span data-stu-id="dcbef-149">string</span></span> | <span data-ttu-id="dcbef-p109">Eindeutige ID für das Abonnement. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dcbef-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="dcbef-152">applicationId</span><span class="sxs-lookup"><span data-stu-id="dcbef-152">applicationId</span></span> | <span data-ttu-id="dcbef-153">string</span><span class="sxs-lookup"><span data-stu-id="dcbef-153">string</span></span> | <span data-ttu-id="dcbef-154">Bezeichner der Anwendung, die zum Erstellen des Abonnements verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="dcbef-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="dcbef-155">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dcbef-155">Read-only.</span></span> |
| <span data-ttu-id="dcbef-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="dcbef-156">creatorId</span></span> | <span data-ttu-id="dcbef-157">string</span><span class="sxs-lookup"><span data-stu-id="dcbef-157">string</span></span> | <span data-ttu-id="dcbef-158">Bezeichner des Benutzers oder Dienstprinzipals, der das Abonnement erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="dcbef-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="dcbef-159">Wenn die App delegierte Berechtigungen zum Erstellen des Abonnements verwendet hat, enthält dieses Feld die ID des angemeldeten Benutzers, für den die App den Aufruf ausgeführt hat.</span><span class="sxs-lookup"><span data-stu-id="dcbef-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="dcbef-160">Wenn die App Anwendungsberechtigungen verwendet hat, enthält dieses Feld die ID des Dienstprinzipals, der der App entspricht.</span><span class="sxs-lookup"><span data-stu-id="dcbef-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="dcbef-161">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dcbef-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="dcbef-162">Maximale Abonnementdauer pro Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dcbef-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="dcbef-163">Ressource</span><span class="sxs-lookup"><span data-stu-id="dcbef-163">Resource</span></span>            | <span data-ttu-id="dcbef-164">Maximal zulässige Ablaufzeit</span><span class="sxs-lookup"><span data-stu-id="dcbef-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="dcbef-165">Mail</span><span class="sxs-lookup"><span data-stu-id="dcbef-165">Mail</span></span>                | <span data-ttu-id="dcbef-166">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="dcbef-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dcbef-167">Kalender</span><span class="sxs-lookup"><span data-stu-id="dcbef-167">Calendar</span></span>            | <span data-ttu-id="dcbef-168">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="dcbef-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dcbef-169">Kontakte</span><span class="sxs-lookup"><span data-stu-id="dcbef-169">Contacts</span></span>            | <span data-ttu-id="dcbef-170">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="dcbef-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dcbef-171">Gruppenunterhaltungen</span><span class="sxs-lookup"><span data-stu-id="dcbef-171">Group conversations</span></span> | <span data-ttu-id="dcbef-172">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="dcbef-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dcbef-173">Laufwerkstammelemente</span><span class="sxs-lookup"><span data-stu-id="dcbef-173">Drive root items</span></span>    | <span data-ttu-id="dcbef-174">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="dcbef-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dcbef-175">Sicherheitswarnungen</span><span class="sxs-lookup"><span data-stu-id="dcbef-175">Security Alerts</span></span>     | <span data-ttu-id="dcbef-176">43200 Minuten (unter 30 Tage)</span><span class="sxs-lookup"><span data-stu-id="dcbef-176">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="dcbef-177">**Hinweis:** Vorhandene Anwendungen und neue Anwendungen sollten den unterstützten Wert nicht überschreiten.</span><span class="sxs-lookup"><span data-stu-id="dcbef-177">Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="dcbef-178">In Zukunft schlagen alle Anforderungen zur Erstellung oder Verlängerung eines Abonnements, die über den Maximalwert hinausgehen, fehl.</span><span class="sxs-lookup"><span data-stu-id="dcbef-178">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="dcbef-179">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dcbef-179">Relationships</span></span>

<span data-ttu-id="dcbef-180">Keine</span><span class="sxs-lookup"><span data-stu-id="dcbef-180">None</span></span>

## <a name="methods"></a><span data-ttu-id="dcbef-181">Methoden</span><span class="sxs-lookup"><span data-stu-id="dcbef-181">Methods</span></span>

| <span data-ttu-id="dcbef-182">Methode</span><span class="sxs-lookup"><span data-stu-id="dcbef-182">Method</span></span> | <span data-ttu-id="dcbef-183">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="dcbef-183">Return Type</span></span> | <span data-ttu-id="dcbef-184">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dcbef-184">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="dcbef-185">Create subscription</span><span class="sxs-lookup"><span data-stu-id="dcbef-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="dcbef-186">Abonnement</span><span class="sxs-lookup"><span data-stu-id="dcbef-186">subscription</span></span>](subscription.md) | <span data-ttu-id="dcbef-187">Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Microsoft Graph-Daten geändert werden.</span><span class="sxs-lookup"><span data-stu-id="dcbef-187">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="dcbef-188">Update subscription</span><span class="sxs-lookup"><span data-stu-id="dcbef-188">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="dcbef-189">Abonnement</span><span class="sxs-lookup"><span data-stu-id="dcbef-189">subscription</span></span>](subscription.md) | <span data-ttu-id="dcbef-190">Erneuert ein Abonnement durch Aktualisierung der Ablaufzeit.</span><span class="sxs-lookup"><span data-stu-id="dcbef-190">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="dcbef-191">Abonnements auflisten</span><span class="sxs-lookup"><span data-stu-id="dcbef-191">List current subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="dcbef-192">subscription</span><span class="sxs-lookup"><span data-stu-id="dcbef-192">subscription</span></span>](subscription.md) | <span data-ttu-id="dcbef-193">Listet aktive Abonnements auf.</span><span class="sxs-lookup"><span data-stu-id="dcbef-193">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="dcbef-194">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="dcbef-194">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="dcbef-195">Abonnement</span><span class="sxs-lookup"><span data-stu-id="dcbef-195">subscription</span></span>](subscription.md) | <span data-ttu-id="dcbef-196">Dient zum Lesen der Eigenschaften und der Beziehungen des subscription-Objekts.</span><span class="sxs-lookup"><span data-stu-id="dcbef-196">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="dcbef-197">Delete subscription</span><span class="sxs-lookup"><span data-stu-id="dcbef-197">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="dcbef-198">Keine</span><span class="sxs-lookup"><span data-stu-id="dcbef-198">None</span></span> |<span data-ttu-id="dcbef-199">Löscht ein subscription-Objekt.</span><span class="sxs-lookup"><span data-stu-id="dcbef-199">Deletes a subscription object.</span></span> |

[contact]: ./contact.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
[Alert]: ./alert.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
