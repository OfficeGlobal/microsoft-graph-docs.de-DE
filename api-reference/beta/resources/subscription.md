---
title: Subscription-Ressourcentyp
description: 'Ein Abonnement ermöglicht eine Client-app zum Empfangen von Benachrichtigungen zu Änderungen an Daten in Microsoft Graph. Abonnements werden derzeit für die folgenden Ressourcen aktiviert:'
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 265ea807330f833edf0d7b1f6a640e0a1f6f4634
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517267"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="d0fce-104">Abonnementressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d0fce-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0fce-105">Ein Abonnement ermöglicht eine Client-app zum Empfangen von Benachrichtigungen zu Änderungen an Daten in Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d0fce-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="d0fce-106">Abonnements werden derzeit für die folgenden Ressourcen aktiviert:</span><span class="sxs-lookup"><span data-stu-id="d0fce-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="d0fce-107">E-Mail, Ereignisse und Kontakte aus Outlook</span><span class="sxs-lookup"><span data-stu-id="d0fce-107">Mail, events, and contacts from Outlook.</span></span>
- <span data-ttu-id="d0fce-108">Unterhaltungen aus Office-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="d0fce-108">Conversations from Office Groups.</span></span>
- <span data-ttu-id="d0fce-109">Laufwerkstammelemente aus OneDrive</span><span class="sxs-lookup"><span data-stu-id="d0fce-109">Drive root items from OneDrive.</span></span>
- <span data-ttu-id="d0fce-110">Benutzer und Gruppen aus dem Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d0fce-110">Users and Groups from Azure Active Directory.</span></span>
- <span data-ttu-id="d0fce-111">Benachrichtigungen über die Microsoft Graph-Sicherheit API.</span><span class="sxs-lookup"><span data-stu-id="d0fce-111">Alerts from the Microsoft Graph Security API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0fce-112">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d0fce-112">JSON representation</span></span>

<span data-ttu-id="d0fce-113">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d0fce-113">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d0fce-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d0fce-114">Properties</span></span>

| <span data-ttu-id="d0fce-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d0fce-115">Property</span></span> | <span data-ttu-id="d0fce-116">Typ</span><span class="sxs-lookup"><span data-stu-id="d0fce-116">Type</span></span> | <span data-ttu-id="d0fce-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0fce-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="d0fce-118">changeType</span><span class="sxs-lookup"><span data-stu-id="d0fce-118">changeType</span></span> | <span data-ttu-id="d0fce-119">string</span><span class="sxs-lookup"><span data-stu-id="d0fce-119">string</span></span> | <span data-ttu-id="d0fce-120">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d0fce-120">Required.</span></span> <span data-ttu-id="d0fce-121">Gibt den Typ der Änderung in der abonnierten Ressource an, die eine Benachrichtigung auslöst.</span><span class="sxs-lookup"><span data-stu-id="d0fce-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="d0fce-122">Unterstützte Werte sind: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="d0fce-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="d0fce-123">Es können mehrere Werte mithilfe einer durch Trennzeichen getrennten Liste zusammen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="d0fce-123">Multiple values can be combined using a comma-separated list.</span></span> <br><br><span data-ttu-id="d0fce-124">Hinweis: Laufwerk Root Element Benachrichtigungen unterstützen nur die `updated` ChangeType.</span><span class="sxs-lookup"><span data-stu-id="d0fce-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="d0fce-125">Unterstützung von Benutzer- und Benachrichtigungen `updated` und `deleted` ChangeType.</span><span class="sxs-lookup"><span data-stu-id="d0fce-125">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="d0fce-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="d0fce-126">notificationUrl</span></span> | <span data-ttu-id="d0fce-127">string</span><span class="sxs-lookup"><span data-stu-id="d0fce-127">string</span></span> | <span data-ttu-id="d0fce-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d0fce-128">Required.</span></span> <span data-ttu-id="d0fce-129">Die URL des Endpunkts, die Benachrichtigungen erhalten werden.</span><span class="sxs-lookup"><span data-stu-id="d0fce-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="d0fce-130">Diese URL muss nutzen Sie die HTTPS Protokoll.</span><span class="sxs-lookup"><span data-stu-id="d0fce-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="d0fce-131">resource</span><span class="sxs-lookup"><span data-stu-id="d0fce-131">resource</span></span> | <span data-ttu-id="d0fce-132">Die Ressource, auf die Sie zugreifen möchten.</span><span class="sxs-lookup"><span data-stu-id="d0fce-132">string</span></span> | <span data-ttu-id="d0fce-133">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d0fce-133">Required.</span></span> <span data-ttu-id="d0fce-134">Gibt die Ressource, die für Änderungen überwacht werden.</span><span class="sxs-lookup"><span data-stu-id="d0fce-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="d0fce-135">Die base-URL nicht einschließen (`https://graph.microsoft.com/beta/`).</span><span class="sxs-lookup"><span data-stu-id="d0fce-135">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> |
| <span data-ttu-id="d0fce-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d0fce-136">expirationDateTime</span></span> | <span data-ttu-id="d0fce-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0fce-137">DateTimeOffset</span></span> | <span data-ttu-id="d0fce-138">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d0fce-138">Required.</span></span> <span data-ttu-id="d0fce-139">Gibt Datum und Uhrzeit für das Ablaufen des Webhook-Abonnements an.</span><span class="sxs-lookup"><span data-stu-id="d0fce-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="d0fce-140">Die Zeit wird in UTC angegeben und kann eine Dauer aus der Erstellung des Abonnements sein, die von der abonnierten Ressource abweicht.</span><span class="sxs-lookup"><span data-stu-id="d0fce-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="d0fce-141">In der folgenden Tabelle finden Sie die maximale Dauer unterstützter Abonnements.</span><span class="sxs-lookup"><span data-stu-id="d0fce-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="d0fce-142">clientState</span><span class="sxs-lookup"><span data-stu-id="d0fce-142">clientState</span></span> | <span data-ttu-id="d0fce-143">string</span><span class="sxs-lookup"><span data-stu-id="d0fce-143">string</span></span> | <span data-ttu-id="d0fce-144">Optional.</span><span class="sxs-lookup"><span data-stu-id="d0fce-144">Optional.</span></span> <span data-ttu-id="d0fce-145">Gibt den Wert der `clientState`-Eigenschaft an, die in jeder Benachrichtigung vom Dienst gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="d0fce-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="d0fce-146">Die maximale Länge ist 255 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="d0fce-146">The maximum length is 255 characters.</span></span> <span data-ttu-id="d0fce-147">Der Client kann prüfen, ob die Benachrichtigung vom Dienst stammt, indem er den Wert der mit dem Abonnement gesendeten `clientState`-Eigenschaft mit dem Wert der mit jeder Benachrichtigung empfangenen `clientState`-Eigenschaft vergleicht.</span><span class="sxs-lookup"><span data-stu-id="d0fce-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="d0fce-148">id</span><span class="sxs-lookup"><span data-stu-id="d0fce-148">id</span></span> | <span data-ttu-id="d0fce-149">string</span><span class="sxs-lookup"><span data-stu-id="d0fce-149">string</span></span> | <span data-ttu-id="d0fce-p109">Eindeutige ID für das Abonnement. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d0fce-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="d0fce-152">applicationId</span><span class="sxs-lookup"><span data-stu-id="d0fce-152">applicationId</span></span> | <span data-ttu-id="d0fce-153">string</span><span class="sxs-lookup"><span data-stu-id="d0fce-153">string</span></span> | <span data-ttu-id="d0fce-154">Bezeichner der Anwendung verwendet, um das Abonnement zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="d0fce-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="d0fce-155">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d0fce-155">Read-only.</span></span> |
| <span data-ttu-id="d0fce-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="d0fce-156">creatorId</span></span> | <span data-ttu-id="d0fce-157">string</span><span class="sxs-lookup"><span data-stu-id="d0fce-157">string</span></span> | <span data-ttu-id="d0fce-158">Bezeichner des Benutzers oder der Dienstprinzipalnamen, die das Abonnement erstellt.</span><span class="sxs-lookup"><span data-stu-id="d0fce-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="d0fce-159">Wenn die app verwendet Berechtigungen zum Erstellen des Abonnements delegiert, enthält dieses Feld die Id des angemeldeten Benutzers an, den die app im Auftrag von aufgerufen.</span><span class="sxs-lookup"><span data-stu-id="d0fce-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="d0fce-160">Wenn die app Anwendungsberechtigungen verwendet wird, enthält dieses Feld die Id des Prinzipals Service für die app.</span><span class="sxs-lookup"><span data-stu-id="d0fce-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="d0fce-161">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d0fce-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="d0fce-162">Maximale Abonnementdauer pro Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d0fce-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="d0fce-163">Ressource</span><span class="sxs-lookup"><span data-stu-id="d0fce-163">Resource</span></span>            | <span data-ttu-id="d0fce-164">Maximal zulässige Ablaufzeit</span><span class="sxs-lookup"><span data-stu-id="d0fce-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="d0fce-165">Mail</span><span class="sxs-lookup"><span data-stu-id="d0fce-165">Mail</span></span>                | <span data-ttu-id="d0fce-166">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d0fce-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="d0fce-167">Kalender</span><span class="sxs-lookup"><span data-stu-id="d0fce-167">Calendar</span></span>            | <span data-ttu-id="d0fce-168">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d0fce-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="d0fce-169">Kontakte</span><span class="sxs-lookup"><span data-stu-id="d0fce-169">Contacts</span></span>            | <span data-ttu-id="d0fce-170">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d0fce-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="d0fce-171">Gruppenunterhaltungen</span><span class="sxs-lookup"><span data-stu-id="d0fce-171">Group conversations</span></span> | <span data-ttu-id="d0fce-172">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d0fce-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="d0fce-173">Laufwerkstammelemente</span><span class="sxs-lookup"><span data-stu-id="d0fce-173">Drive root items</span></span>    | <span data-ttu-id="d0fce-174">4230 Minuten (unter 3 Tage)</span><span class="sxs-lookup"><span data-stu-id="d0fce-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="d0fce-175">Sicherheitswarnungen</span><span class="sxs-lookup"><span data-stu-id="d0fce-175">Security alerts</span></span>     | <span data-ttu-id="d0fce-176">43200 Minuten (unter 30 Tage)</span><span class="sxs-lookup"><span data-stu-id="d0fce-176">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="d0fce-177">**Hinweis:** Vorhandene Anwendungen und neuen Anwendungen sollte den unterstützten Wert nicht überschreiten.</span><span class="sxs-lookup"><span data-stu-id="d0fce-177">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="d0fce-178">In der Zukunft fehl alle Anforderungen zum Erstellen oder erneuern Sie ein Abonnement über den Höchstwert hinaus.</span><span class="sxs-lookup"><span data-stu-id="d0fce-178">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="d0fce-179">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d0fce-179">Relationships</span></span>

<span data-ttu-id="d0fce-180">Keine</span><span class="sxs-lookup"><span data-stu-id="d0fce-180">None</span></span>

## <a name="methods"></a><span data-ttu-id="d0fce-181">Methoden</span><span class="sxs-lookup"><span data-stu-id="d0fce-181">Methods</span></span>

| <span data-ttu-id="d0fce-182">Methode</span><span class="sxs-lookup"><span data-stu-id="d0fce-182">Method</span></span> | <span data-ttu-id="d0fce-183">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d0fce-183">Return Type</span></span> | <span data-ttu-id="d0fce-184">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0fce-184">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="d0fce-185">Create subscription</span><span class="sxs-lookup"><span data-stu-id="d0fce-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="d0fce-186">Abonnement</span><span class="sxs-lookup"><span data-stu-id="d0fce-186">subscription</span></span>](subscription.md) | <span data-ttu-id="d0fce-187">Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Microsoft Graph-Daten geändert werden.</span><span class="sxs-lookup"><span data-stu-id="d0fce-187">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="d0fce-188">Update subscription</span><span class="sxs-lookup"><span data-stu-id="d0fce-188">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="d0fce-189">subscription</span><span class="sxs-lookup"><span data-stu-id="d0fce-189">subscription</span></span>](subscription.md) | <span data-ttu-id="d0fce-190">Erneuern eines Abonnements durch den Ablaufzeitpunkt aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="d0fce-190">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="d0fce-191">Liste von Abonnements</span><span class="sxs-lookup"><span data-stu-id="d0fce-191">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="d0fce-192">subscription</span><span class="sxs-lookup"><span data-stu-id="d0fce-192">subscription</span></span>](subscription.md) | <span data-ttu-id="d0fce-193">Listen aktiver Abonnements.</span><span class="sxs-lookup"><span data-stu-id="d0fce-193">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="d0fce-194">Get subscription</span><span class="sxs-lookup"><span data-stu-id="d0fce-194">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="d0fce-195">Abonnement</span><span class="sxs-lookup"><span data-stu-id="d0fce-195">subscription</span></span>](subscription.md) | <span data-ttu-id="d0fce-196">Lesen Sie Eigenschaften und Beziehungen Abonnement-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d0fce-196">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="d0fce-197">Delete subscription</span><span class="sxs-lookup"><span data-stu-id="d0fce-197">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="d0fce-198">Keine</span><span class="sxs-lookup"><span data-stu-id="d0fce-198">None</span></span> | <span data-ttu-id="d0fce-199">Löscht ein Abonnementobjekt.</span><span class="sxs-lookup"><span data-stu-id="d0fce-199">Delete a subscription object.</span></span> |

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
