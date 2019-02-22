---
title: Abonnement Ressourcentyp
description: 'Ein Abonnement ermöglicht einer Client-App, Benachrichtigungen zu Änderungen an Daten in Microsoft Graph zu erhalten. Derzeit werden Abonnements für die folgenden Ressourcen aktiviert:'
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9de48cc6a3e5dde459673117d9ee00a34477faf6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163938"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="92994-104">Abonnement Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="92994-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92994-105">Ein Abonnement ermöglicht einer Client-App, Benachrichtigungen zu Änderungen an Daten in Microsoft Graph zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="92994-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="92994-106">Derzeit werden Abonnements für die folgenden Ressourcen aktiviert:</span><span class="sxs-lookup"><span data-stu-id="92994-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="92994-107">[Nachricht][], [Ereignis][]oder [Kontakt][] in Outlook</span><span class="sxs-lookup"><span data-stu-id="92994-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="92994-108">Eine unter [Haltung][] einer Office 365-Gruppe</span><span class="sxs-lookup"><span data-stu-id="92994-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="92994-109">Inhalt in der Hierarchie eines Stammordners [driveItem][] in OneDrive for Business oder eines Stammordners oder Unterordners [driveItem][] in der persönlichen OneDrive eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="92994-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="92994-110">Ein [Benutzer][] oder eine [Gruppe][] in Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="92994-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="92994-111">Eine [Warnung][] aus der Sicherheits-API von Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="92994-111">An [alert][] from the Microsoft Graph Security API</span></span>


## <a name="json-representation"></a><span data-ttu-id="92994-112">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="92994-112">JSON representation</span></span>

<span data-ttu-id="92994-113">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="92994-113">Here is a JSON representation of the resource.</span></span>

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
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="92994-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="92994-114">Properties</span></span>

| <span data-ttu-id="92994-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="92994-115">Property</span></span> | <span data-ttu-id="92994-116">Typ</span><span class="sxs-lookup"><span data-stu-id="92994-116">Type</span></span> | <span data-ttu-id="92994-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92994-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="92994-118">changeType</span><span class="sxs-lookup"><span data-stu-id="92994-118">changeType</span></span> | <span data-ttu-id="92994-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92994-119">string</span></span> | <span data-ttu-id="92994-120">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="92994-120">Required.</span></span> <span data-ttu-id="92994-121">Gibt den Typ der Änderung in der abonnierten Ressource an, die eine Benachrichtigung auslöst.</span><span class="sxs-lookup"><span data-stu-id="92994-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="92994-122">Unterstützte Werte sind: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="92994-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="92994-123">Es können mehrere Werte mithilfe einer durch Trennzeichen getrennten Liste zusammen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="92994-123">Multiple values can be combined using a comma-separated list.</span></span> <br><br><span data-ttu-id="92994-124">Hinweis: Drive-Stammelement Benachrichtigungen unterstützen `updated` nur den ChangeType.</span><span class="sxs-lookup"><span data-stu-id="92994-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="92994-125">Unterstützung `updated` von Benutzer-und `deleted` Gruppenbenachrichtigungen und ChangeType.</span><span class="sxs-lookup"><span data-stu-id="92994-125">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="92994-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="92994-126">notificationUrl</span></span> | <span data-ttu-id="92994-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92994-127">string</span></span> | <span data-ttu-id="92994-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="92994-128">Required.</span></span> <span data-ttu-id="92994-129">Die URL des Endpunkts, der die Benachrichtigungen empfängt.</span><span class="sxs-lookup"><span data-stu-id="92994-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="92994-130">Diese URL muss das HTTPS-Protokoll verwenden.</span><span class="sxs-lookup"><span data-stu-id="92994-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="92994-131">resource</span><span class="sxs-lookup"><span data-stu-id="92994-131">resource</span></span> | <span data-ttu-id="92994-132">Die Ressource, auf die Sie zugreifen möchten.</span><span class="sxs-lookup"><span data-stu-id="92994-132">string</span></span> | <span data-ttu-id="92994-133">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="92994-133">Required.</span></span> <span data-ttu-id="92994-134">Gibt die Ressource an, die auf Änderungen überwacht wird.</span><span class="sxs-lookup"><span data-stu-id="92994-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="92994-135">Die Basis-URL darf nicht eingeschlossen`https://graph.microsoft.com/beta/`werden ().</span><span class="sxs-lookup"><span data-stu-id="92994-135">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> |
| <span data-ttu-id="92994-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="92994-136">expirationDateTime</span></span> | <span data-ttu-id="92994-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92994-137">DateTimeOffset</span></span> | <span data-ttu-id="92994-138">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="92994-138">Required.</span></span> <span data-ttu-id="92994-139">Gibt Datum und Uhrzeit für das Ablaufen des Webhook-Abonnements an.</span><span class="sxs-lookup"><span data-stu-id="92994-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="92994-140">Die Zeit wird in UTC angegeben und kann eine Dauer aus der Erstellung des Abonnements sein, die von der abonnierten Ressource abweicht.</span><span class="sxs-lookup"><span data-stu-id="92994-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="92994-141">In der folgenden Tabelle finden Sie die maximale Dauer unterstützter Abonnements.</span><span class="sxs-lookup"><span data-stu-id="92994-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="92994-142">clientState</span><span class="sxs-lookup"><span data-stu-id="92994-142">clientState</span></span> | <span data-ttu-id="92994-143">string</span><span class="sxs-lookup"><span data-stu-id="92994-143">string</span></span> | <span data-ttu-id="92994-144">Optional.</span><span class="sxs-lookup"><span data-stu-id="92994-144">Optional.</span></span> <span data-ttu-id="92994-145">Gibt den Wert der `clientState`-Eigenschaft an, die in jeder Benachrichtigung vom Dienst gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="92994-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="92994-146">Die maximale Länge ist 255 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="92994-146">The maximum length is 255 characters.</span></span> <span data-ttu-id="92994-147">Der Client kann prüfen, ob die Benachrichtigung vom Dienst stammt, indem er den Wert der mit dem Abonnement gesendeten `clientState`-Eigenschaft mit dem Wert der mit jeder Benachrichtigung empfangenen `clientState`-Eigenschaft vergleicht.</span><span class="sxs-lookup"><span data-stu-id="92994-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="92994-148">id</span><span class="sxs-lookup"><span data-stu-id="92994-148">id</span></span> | <span data-ttu-id="92994-149">string</span><span class="sxs-lookup"><span data-stu-id="92994-149">string</span></span> | <span data-ttu-id="92994-p109">Eindeutige ID für das Abonnement. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="92994-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="92994-152">applicationId</span><span class="sxs-lookup"><span data-stu-id="92994-152">applicationId</span></span> | <span data-ttu-id="92994-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92994-153">string</span></span> | <span data-ttu-id="92994-154">Der Bezeichner der Anwendung, die zum Erstellen des Abonnements verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="92994-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="92994-155">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="92994-155">Read-only.</span></span> |
| <span data-ttu-id="92994-156">Creator-Nr.</span><span class="sxs-lookup"><span data-stu-id="92994-156">creatorId</span></span> | <span data-ttu-id="92994-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92994-157">string</span></span> | <span data-ttu-id="92994-158">Der Bezeichner des Benutzers oder Dienst Prinzipals, der das Abonnement erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="92994-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="92994-159">Wenn die APP Delegierte Berechtigungen zum Erstellen des Abonnements verwendet hat, enthält dieses Feld die ID des signierten Benutzers, für den die app aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="92994-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="92994-160">Wenn die APP Anwendungsberechtigungen verwendet, enthält dieses Feld die ID des Dienst Prinzipals, der der APP entspricht.</span><span class="sxs-lookup"><span data-stu-id="92994-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="92994-161">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="92994-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="92994-162">Maximale Abonnementdauer pro Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="92994-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="92994-163">Ressource</span><span class="sxs-lookup"><span data-stu-id="92994-163">Resource</span></span>            | <span data-ttu-id="92994-164">Maximal zulässige Ablaufzeit</span><span class="sxs-lookup"><span data-stu-id="92994-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="92994-165">Mail</span><span class="sxs-lookup"><span data-stu-id="92994-165">Mail</span></span>                | <span data-ttu-id="92994-166">4230 Minuten (weniger als 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="92994-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="92994-167">Kalender</span><span class="sxs-lookup"><span data-stu-id="92994-167">Calendar</span></span>            | <span data-ttu-id="92994-168">4230 Minuten (weniger als 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="92994-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="92994-169">Kontakte</span><span class="sxs-lookup"><span data-stu-id="92994-169">Contacts</span></span>            | <span data-ttu-id="92994-170">4230 Minuten (weniger als 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="92994-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="92994-171">Gruppenunterhaltungen</span><span class="sxs-lookup"><span data-stu-id="92994-171">Group conversations</span></span> | <span data-ttu-id="92994-172">4230 Minuten (weniger als 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="92994-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="92994-173">Laufwerkstammelemente</span><span class="sxs-lookup"><span data-stu-id="92994-173">Drive root items</span></span>    | <span data-ttu-id="92994-174">4230 Minuten (weniger als 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="92994-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="92994-175">Sicherheitswarnungen</span><span class="sxs-lookup"><span data-stu-id="92994-175">Security alerts</span></span>     | <span data-ttu-id="92994-176">43200 Minuten (weniger als 30 Tage)</span><span class="sxs-lookup"><span data-stu-id="92994-176">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="92994-177">**Hinweis:** Vorhandene Anwendungen und neue Anwendungen sollten den unterstützten Wert nicht überschreiten.</span><span class="sxs-lookup"><span data-stu-id="92994-177">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="92994-178">In Zukunft schlagen alle Anforderungen zum Erstellen oder Erneuern eines Abonnements, die den Maximalwert überschreiten, fehl.</span><span class="sxs-lookup"><span data-stu-id="92994-178">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="92994-179">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="92994-179">Relationships</span></span>

<span data-ttu-id="92994-180">Keine</span><span class="sxs-lookup"><span data-stu-id="92994-180">None</span></span>

## <a name="methods"></a><span data-ttu-id="92994-181">Methoden</span><span class="sxs-lookup"><span data-stu-id="92994-181">Methods</span></span>

| <span data-ttu-id="92994-182">Methode</span><span class="sxs-lookup"><span data-stu-id="92994-182">Method</span></span> | <span data-ttu-id="92994-183">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="92994-183">Return Type</span></span> | <span data-ttu-id="92994-184">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92994-184">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="92994-185">Create subscription</span><span class="sxs-lookup"><span data-stu-id="92994-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="92994-186">Abonnement</span><span class="sxs-lookup"><span data-stu-id="92994-186">subscription</span></span>](subscription.md) | <span data-ttu-id="92994-187">Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Microsoft Graph-Daten geändert werden.</span><span class="sxs-lookup"><span data-stu-id="92994-187">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="92994-188">Update subscription</span><span class="sxs-lookup"><span data-stu-id="92994-188">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="92994-189">subscription</span><span class="sxs-lookup"><span data-stu-id="92994-189">subscription</span></span>](subscription.md) | <span data-ttu-id="92994-190">Erneuern Sie ein Abonnement, indem Sie dessen Ablaufzeit aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="92994-190">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="92994-191">Listen Abonnements</span><span class="sxs-lookup"><span data-stu-id="92994-191">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="92994-192">subscription</span><span class="sxs-lookup"><span data-stu-id="92994-192">subscription</span></span>](subscription.md) | <span data-ttu-id="92994-193">Listet aktive Abonnements auf.</span><span class="sxs-lookup"><span data-stu-id="92994-193">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="92994-194">Get subscription</span><span class="sxs-lookup"><span data-stu-id="92994-194">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="92994-195">Abonnement</span><span class="sxs-lookup"><span data-stu-id="92994-195">subscription</span></span>](subscription.md) | <span data-ttu-id="92994-196">Lesen von Eigenschaften und Beziehungen des Subscription-Objekts.</span><span class="sxs-lookup"><span data-stu-id="92994-196">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="92994-197">Delete subscription</span><span class="sxs-lookup"><span data-stu-id="92994-197">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="92994-198">Keine</span><span class="sxs-lookup"><span data-stu-id="92994-198">None</span></span> | <span data-ttu-id="92994-199">Löscht ein Subscription-Objekt.</span><span class="sxs-lookup"><span data-stu-id="92994-199">Delete a subscription object.</span></span> |

[Kontakt]: ./contact.md
[contact]: ./contact.md
[Unterhaltung]: ./conversation.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[Warnung]: ./alert.md
[alert]: ./alert.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/subscription.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
