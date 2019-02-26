---
title: Einrichten von Benachrichtigungen für Änderungen der Benutzerdaten
description: Die Microsoft Graph-API verwendet einen Webhook-Mechanismus zum Übermitteln von Benachrichtigungen an Clients. Ein Client ist ein Webdienst, der eine eigene URL zum Empfangen von Benachrichtigungen konfiguriert. Client-Apps verwenden Benachrichtigungen, um bei Änderungen ihren Status zu aktualisieren.
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 48f9d16374219868418107201ef13a1bf14fb7da
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263377"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="d45d1-105">Einrichten von Benachrichtigungen für Änderungen der Benutzerdaten</span><span class="sxs-lookup"><span data-stu-id="d45d1-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="d45d1-p102">Die Microsoft Graph-API verwendet einen Webhook-Mechanismus zum Übermitteln von Benachrichtigungen an Clients. Ein Client ist ein Webdienst, der eine eigene URL zum Empfangen von Benachrichtigungen konfiguriert. Client-Apps verwenden Benachrichtigungen, um bei Änderungen ihren Status zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="d45d1-p102">The Microsoft Graph API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="d45d1-109">Nachdem Microsoft Graph die Abonnementsanfrage akzeptiert hat, werden Pushbenachrichtigungen an die im Abonnement angegebene URL gesendet.</span><span class="sxs-lookup"><span data-stu-id="d45d1-109">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="d45d1-110">Die App führt dann Aktionen gemäß der Geschäftslogik aus.</span><span class="sxs-lookup"><span data-stu-id="d45d1-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="d45d1-111">Sie ruft z. B. weitere Daten ab, aktualisiert Zwischenspeicher für Dokumente und Ansichten usw.</span><span class="sxs-lookup"><span data-stu-id="d45d1-111">For example, it fetches more data, updates its cache and views, etc.</span></span>

## <a name="supported-resources"></a><span data-ttu-id="d45d1-112">Unterstützte Ressourcen</span><span class="sxs-lookup"><span data-stu-id="d45d1-112">Supported resources</span></span>

<span data-ttu-id="d45d1-113">Mit der Microsoft Graph-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:</span><span class="sxs-lookup"><span data-stu-id="d45d1-113">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="d45d1-114">Outlook-[Nachricht][]</span><span class="sxs-lookup"><span data-stu-id="d45d1-114">Outlook [message][]</span></span>
- <span data-ttu-id="d45d1-115">Outlook-[Ereignis][]</span><span class="sxs-lookup"><span data-stu-id="d45d1-115">Outlook [event][]</span></span>
- <span data-ttu-id="d45d1-116">Persönlicher Outlook-[Kontakt][]</span><span class="sxs-lookup"><span data-stu-id="d45d1-116">Outlook personal [contact][]</span></span>
- <span data-ttu-id="d45d1-117">[Benutzer][]</span><span class="sxs-lookup"><span data-stu-id="d45d1-117">[user][]</span></span>
- <span data-ttu-id="d45d1-118">[Gruppe][]</span><span class="sxs-lookup"><span data-stu-id="d45d1-118">[group][]</span></span>
- <span data-ttu-id="d45d1-119">Office 365-[Gruppenunterhaltung][]</span><span class="sxs-lookup"><span data-stu-id="d45d1-119">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="d45d1-120">Inhalt in der Hierarchie des [driveItem][]-Objekts eines _beliebigen Ordners_ auf dem persönlichen OneDrive eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="d45d1-120">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="d45d1-121">Inhalt in der Hierarchie des [driveItem][]-Objekts eines _Stammordners_ auf OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="d45d1-121">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="d45d1-122">[Sicherheitswarnung][]</span><span class="sxs-lookup"><span data-stu-id="d45d1-122">Security [alert][]</span></span>

<span data-ttu-id="d45d1-123">Sie können ein Abonnement für einen bestimmten Outlook-Ordner erstellen, z.B. den Posteingang: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="d45d1-123">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="d45d1-124">Oder für eine Ressource der obersten Ebene: `me/messages`, `me/contacts`, `me/events`, `users`, oder `groups`</span><span class="sxs-lookup"><span data-stu-id="d45d1-124">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="d45d1-125">Oder für eine bestimmte Ressourceninstanz: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="d45d1-125">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="d45d1-126">Oder für einen beliebigen Ordner in der persönlichen OneDrive-Umgebung eines Benutzers: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="d45d1-126">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="d45d1-127">Oder für den Stammorder eines Sharepoint-/OneDrive for Business-Laufwerks: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="d45d1-127">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="d45d1-128">Oder für eine neue [Sicherheits-API-Warnung](security-concept-overview.md): `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span><span class="sxs-lookup"><span data-stu-id="d45d1-128">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="d45d1-129">Azure AD-Ressourceneinschränkungen</span><span class="sxs-lookup"><span data-stu-id="d45d1-129">Azure AD resource limitations</span></span>

<span data-ttu-id="d45d1-130">Bestimmte Einschränkungen gelten für Azure AD-basierte Ressourcen (Benutzer, Gruppen) und können bei Überschreitung Fehler hervorrufen:</span><span class="sxs-lookup"><span data-stu-id="d45d1-130">Certain limits apply to Azure AD based resources (users, groups) and may generate errors when exceeded:</span></span>

- <span data-ttu-id="d45d1-131">Maximale Abonnementkontingente:</span><span class="sxs-lookup"><span data-stu-id="d45d1-131">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="d45d1-132">Pro App: 50 000 Abonnements insgesamt</span><span class="sxs-lookup"><span data-stu-id="d45d1-132">Per app: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="d45d1-133">Pro Mandant: 1000 Abonnements insgesamt in allen Apps</span><span class="sxs-lookup"><span data-stu-id="d45d1-133">Per tenant: 35 total subscriptions across all apps</span></span>
  - <span data-ttu-id="d45d1-134">Pro App und Mandanten kombiniert: 100 Abonnements insgesamt</span><span class="sxs-lookup"><span data-stu-id="d45d1-134">Per app and tenant combination: 7 total subscriptions</span></span>

- <span data-ttu-id="d45d1-135">Azure AD B2C-Mandanten werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d45d1-135">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="d45d1-136">Benachrichtigungen für Benutzerentitäten werden für persönliche Microsoft-Konten nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d45d1-136">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="d45d1-137">Gültigkeitsdauer von Abonnements</span><span class="sxs-lookup"><span data-stu-id="d45d1-137">Subscription lifetime</span></span>

<span data-ttu-id="d45d1-138">Abonnements haben eine eingeschränkte Gültigkeit.</span><span class="sxs-lookup"><span data-stu-id="d45d1-138">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="d45d1-139">Apps müssen ihre Abonnements vor dem Ablaufzeitpunkt verlängern.</span><span class="sxs-lookup"><span data-stu-id="d45d1-139">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="d45d1-140">Andernfalls müssen sie ein neues Abonnement erstellen.</span><span class="sxs-lookup"><span data-stu-id="d45d1-140">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="d45d1-141">Eine Liste maximaler Ablaufzeiten finden Sie unter [Maximale Abonnementdauer pro Ressourcentyp](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="d45d1-141">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="d45d1-142">Apps können auch jederzeit gekündigt werden, um keine weiteren Benachrichtigungen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="d45d1-142">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="d45d1-143">Verwalten von Abonnements</span><span class="sxs-lookup"><span data-stu-id="d45d1-143">Managing subscriptions</span></span>

<span data-ttu-id="d45d1-144">Clients können Abonnements erstellen, verlängern und löschen.</span><span class="sxs-lookup"><span data-stu-id="d45d1-144">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="d45d1-145">Erstellen eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="d45d1-145">Creating a subscription</span></span>

<span data-ttu-id="d45d1-p105">Um Benachrichtigungen für eine Ressource zu erhalten, muss in einem ersten Schritt ein Abonnement erstellt werden. Der Abonnementprozess läuft wie folgt ab:</span><span class="sxs-lookup"><span data-stu-id="d45d1-p105">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="d45d1-148">Der Client sendet eine Abonnementanforderung (POST) für eine bestimmte Ressource.</span><span class="sxs-lookup"><span data-stu-id="d45d1-148">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="d45d1-149">Microsoft Graph überprüft die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d45d1-149">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="d45d1-150">Wenn die Anforderung gültig ist, sendet Microsoft Graph ein Überprüfungsstoken an die Benachrichtigungs-URL.</span><span class="sxs-lookup"><span data-stu-id="d45d1-150">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="d45d1-151">Wenn die Anfrage ungültig ist, sendet Microsoft Graph eine Fehlermeldung mit Code und Details.</span><span class="sxs-lookup"><span data-stu-id="d45d1-151">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="d45d1-152">Der Client sendet das Überprüfungstoken zurück an Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d45d1-152">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="d45d1-153">Microsoft Graph sendet eine Antwort an den Client zurück.</span><span class="sxs-lookup"><span data-stu-id="d45d1-153">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="d45d1-154">Der Client muss die Abonnement-ID speichern, um Benachrichtigungen mit dem Abonnement korrelieren zu können.</span><span class="sxs-lookup"><span data-stu-id="d45d1-154">The client must store the subscription ID to correlate notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="d45d1-155">Beispiel für eine Abonnementanfrage</span><span class="sxs-lookup"><span data-stu-id="d45d1-155">Subscription request example</span></span>

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/notificationClient",
  "resource": "/me/mailfolders('inbox')/messages",
  "expirationDateTime": "2016-03-20T11:00:00.0000000Z",
  "clientState": "SecretClientState"
}
```

<span data-ttu-id="d45d1-156">Die Eigenschaften `changeType`, `notificationUrl`, `resource` und `expirationDateTime` sind erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d45d1-156">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="d45d1-157">Unter [subscription-Ressourcentyp](/graph/api/resources/subscription?view=graph-rest-1.0) finden Sie die Eigenschaftsdefinitionen und Werte.</span><span class="sxs-lookup"><span data-stu-id="d45d1-157">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="d45d1-158">Die Eigenschaft `resource` gibt die Ressource an, deren Änderungen überwacht werden.</span><span class="sxs-lookup"><span data-stu-id="d45d1-158">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="d45d1-159">Sie können z. B. ein Abonnement für einen bestimmten E-Mail-Ordner erstellen: `me/mailFolders('inbox')/messages` oder im Auftrag eines Benutzers mit der Zustimmung eines Administrators: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span><span class="sxs-lookup"><span data-stu-id="d45d1-159">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="d45d1-160">`clientState` ist zwar nicht erforderlich, muss aber eingeschlossen werden, um unserem empfohlenen Prozess zum Umgang mit Benachrichtigungen zu entsprechen.</span><span class="sxs-lookup"><span data-stu-id="d45d1-160">Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="d45d1-161">Durch das Festlegen dieser Eigenschaft können Sie bestätigen, dass die empfangenen Benachrichtigungen vom Microsoft Graph-Dienst stammen.</span><span class="sxs-lookup"><span data-stu-id="d45d1-161">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="d45d1-162">Aus diesem Grund muss der Wert der Eigenschaft geheim bleiben und darf nur der Anwendung und dem Microsoft Graph-Dienst bekannt sein.</span><span class="sxs-lookup"><span data-stu-id="d45d1-162">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="d45d1-163">Wenn der Vorgang erfolgreich war, gibt Microsoft Graph einen `201 Created`-Code und ein [subscription](/graph/api/resources/subscription?view=graph-rest-1.0)-Objekt im Textkörper zurück.</span><span class="sxs-lookup"><span data-stu-id="d45d1-163">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="d45d1-164">Endpunktprüfung für Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="d45d1-164">Notification endpoint validation</span></span>

<span data-ttu-id="d45d1-165">Microsoft Graph überprüft den Benachrichtigungsendpunkt, der in der Eigenschaft `notificationUrl` der Abonnementanfrage angegeben ist, bevor das Abonnement erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="d45d1-165">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="d45d1-166">Der Überprüfungsprozess läuft wie folgt ab:</span><span class="sxs-lookup"><span data-stu-id="d45d1-166">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="d45d1-167">Microsoft Graph sendet eine POST-Anforderung an die Benachrichtigungs-URL:</span><span class="sxs-lookup"><span data-stu-id="d45d1-167">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="d45d1-168">**Wichtig:** Da `validationToken` ein Abfrageparameter ist, muss er gemäß den HTTP-Codierungspraktiken ordnungsgemäß vom Client decodiert werden.</span><span class="sxs-lookup"><span data-stu-id="d45d1-168">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="d45d1-169">Wenn der Client das Token nicht decodiert und stattdessen im nächsten Schritt (Antwort) den codierten Wert verwendet, tritt bei der Überprüfung ein Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="d45d1-169">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="d45d1-170">Der Client sollte den Tokenwert außerdem als nicht transparent behandeln, da sich das Tokenformat in der Zukunft möglicherweise ohne vorherige Ankündigung ändern kann.</span><span class="sxs-lookup"><span data-stu-id="d45d1-170">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="d45d1-171">Der Client muss innerhalb von 10 Sekunden eine Antwort mit folgenden Merkmalen bereitstellen:</span><span class="sxs-lookup"><span data-stu-id="d45d1-171">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="d45d1-172">Statuscode 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="d45d1-172">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="d45d1-173">Der Inhaltstyp muss `text/plain` sein.</span><span class="sxs-lookup"><span data-stu-id="d45d1-173">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="d45d1-174">Der Textkörper muss das von Microsoft Graph bereitgestellte Überprüfungstoken enthalten.</span><span class="sxs-lookup"><span data-stu-id="d45d1-174">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="d45d1-175">Der Client muss den Überprüfungstoken verwerfen, nachdem er in der Antwort bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="d45d1-175">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="d45d1-176">Verlängern eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="d45d1-176">Renewing a subscription</span></span>

<span data-ttu-id="d45d1-177">Der Kunde kann ein Abonnement mit einem bestimmten Ablaufdatum von bis zu drei Tagen ab dem Zeitpunkt der Anforderung verlängern.</span><span class="sxs-lookup"><span data-stu-id="d45d1-177">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="d45d1-178">Die Eigenschaft `expirationDateTime` muss angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="d45d1-178">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="d45d1-179">Beispiel für eine Abonnementverlängerung</span><span class="sxs-lookup"><span data-stu-id="d45d1-179">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="d45d1-180">Wenn der Vorgang erfolgreich war, gibt Microsoft Graph einen `200 OK`-Code und ein [subscription](/graph/api/resources/subscription?view=graph-rest-1.0)-Objekt im Textkörper zurück.</span><span class="sxs-lookup"><span data-stu-id="d45d1-180">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="d45d1-181">Das Abonnementobjekt enthält den neuen Wert für `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="d45d1-181">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="d45d1-182">Löschen eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="d45d1-182">Deleting a subscription</span></span>

<span data-ttu-id="d45d1-183">Der Client kann den Erhalt von Benachrichtigungen stoppen, indem er das Abonnement anhand seiner ID löscht.</span><span class="sxs-lookup"><span data-stu-id="d45d1-183">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="d45d1-184">Wenn der Vorgang erfolgreich verläuft, gibt Microsoft Graph einen `204 No Content`-Code zurück.</span><span class="sxs-lookup"><span data-stu-id="d45d1-184">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="d45d1-185">Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="d45d1-185">Notifications</span></span>

<span data-ttu-id="d45d1-186">Der Client beginnt, Benachrichtigungen zu erhalten, nachdem das Abonnement erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="d45d1-186">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="d45d1-187">Microsoft Graph sendet eine POST-Anforderung an die Benachrichtigungs-URL, wenn sich die Ressource ändert.</span><span class="sxs-lookup"><span data-stu-id="d45d1-187">Microsoft Graph sends a POST request to the notification URL when the resource changes.</span></span> <span data-ttu-id="d45d1-188">Benachrichtigungen werden nur für die Änderungen des Typs gesendet, der im Abonnement angegeben ist, z. B. `created`.</span><span class="sxs-lookup"><span data-stu-id="d45d1-188">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="d45d1-189">**Hinweis:** Wenn Sie mehrere Abonnements verwenden, die den gleichen Ressourcentyp überwachen und die gleiche Benachrichtigungs-URL verwenden, kann ein POST gesendet werden, der mehrere Benachrichtigungen mit verschiedenen Abonnement-IDs enthalten kann.</span><span class="sxs-lookup"><span data-stu-id="d45d1-189">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="d45d1-190">Es kann nicht garantiert werden, dass alle Benachrichtigungen in einem POST zu einem einzelnen Abonnement gehören.</span><span class="sxs-lookup"><span data-stu-id="d45d1-190">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="d45d1-191">Benachrichtigungseigenschaften</span><span class="sxs-lookup"><span data-stu-id="d45d1-191">Notification properties</span></span>

<span data-ttu-id="d45d1-192">Das Benachrichtigungsobjekt verfügt über die folgenden Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="d45d1-192">The notification object has the following properties:</span></span>

| <span data-ttu-id="d45d1-193">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d45d1-193">Property</span></span> | <span data-ttu-id="d45d1-194">Typ</span><span class="sxs-lookup"><span data-stu-id="d45d1-194">Type</span></span> | <span data-ttu-id="d45d1-195">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d45d1-195">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="d45d1-196">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="d45d1-196">subscriptionId</span></span> | <span data-ttu-id="d45d1-197">string</span><span class="sxs-lookup"><span data-stu-id="d45d1-197">string</span></span> | <span data-ttu-id="d45d1-198">Die ID des Abonnements, das die Benachrichtigung generiert hat.</span><span class="sxs-lookup"><span data-stu-id="d45d1-198">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="d45d1-199">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d45d1-199">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="d45d1-200">dateTime</span><span class="sxs-lookup"><span data-stu-id="d45d1-200">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="d45d1-201">Die Ablaufzeit für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="d45d1-201">The expiration time for the subscription.</span></span> |
| <span data-ttu-id="d45d1-202">clientState</span><span class="sxs-lookup"><span data-stu-id="d45d1-202">clientState</span></span> | <span data-ttu-id="d45d1-203">string</span><span class="sxs-lookup"><span data-stu-id="d45d1-203">string</span></span> | <span data-ttu-id="d45d1-204">Die `clientState`-Eigenschaft in der Abonnementanforderung (falls vorhanden).</span><span class="sxs-lookup"><span data-stu-id="d45d1-204">The `clientState` property specified in the subscription request (if any).</span></span> |
| <span data-ttu-id="d45d1-205">changeType</span><span class="sxs-lookup"><span data-stu-id="d45d1-205">changeType</span></span> | <span data-ttu-id="d45d1-206">string</span><span class="sxs-lookup"><span data-stu-id="d45d1-206">string</span></span> | <span data-ttu-id="d45d1-207">Der Ereignistyp, der die Benachrichtigung ausgelöst hat.</span><span class="sxs-lookup"><span data-stu-id="d45d1-207">The event type that caused the notification.</span></span> <span data-ttu-id="d45d1-208">Beispiel: `created` bei Erhalt einer E-Mail oder `updated`, wenn eine Nachricht als gelesen markiert wird.</span><span class="sxs-lookup"><span data-stu-id="d45d1-208">For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="d45d1-209">resource</span><span class="sxs-lookup"><span data-stu-id="d45d1-209">resource</span></span> | <span data-ttu-id="d45d1-210">string</span><span class="sxs-lookup"><span data-stu-id="d45d1-210">string</span></span> | <span data-ttu-id="d45d1-211">Der URI der Ressource relativ zu `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="d45d1-211">The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="d45d1-212">resourceData</span><span class="sxs-lookup"><span data-stu-id="d45d1-212">resourceData</span></span> | <span data-ttu-id="d45d1-213">object</span><span class="sxs-lookup"><span data-stu-id="d45d1-213">object</span></span> | <span data-ttu-id="d45d1-214">Der Inhalt dieser Eigenschaft hängt vom Typ der Ressource ab, die abonniert wurde.</span><span class="sxs-lookup"><span data-stu-id="d45d1-214">The content of this property depends on the type of resource being subscribed to.</span></span> |

<span data-ttu-id="d45d1-215">Beispiel: Für Outlook-Ressourcen enthält `resourceData` die folgenden Felder:</span><span class="sxs-lookup"><span data-stu-id="d45d1-215">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="d45d1-216">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d45d1-216">Property</span></span> | <span data-ttu-id="d45d1-217">Typ</span><span class="sxs-lookup"><span data-stu-id="d45d1-217">Type</span></span> | <span data-ttu-id="d45d1-218">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d45d1-218">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="d45d1-219">@odata.type</span><span class="sxs-lookup"><span data-stu-id="d45d1-219">@odata.type</span></span> | <span data-ttu-id="d45d1-220">string</span><span class="sxs-lookup"><span data-stu-id="d45d1-220">string</span></span> | <span data-ttu-id="d45d1-221">Der OData-Entitätstyp in Microsoft Graph, der das dargestellte Objekt beschreibt.</span><span class="sxs-lookup"><span data-stu-id="d45d1-221">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="d45d1-222">@odata.id</span><span class="sxs-lookup"><span data-stu-id="d45d1-222">@odata.id</span></span> | <span data-ttu-id="d45d1-223">string</span><span class="sxs-lookup"><span data-stu-id="d45d1-223">string</span></span> | <span data-ttu-id="d45d1-224">Der OData-Bezeichner des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d45d1-224">The OData identifier of the object.</span></span> |
| <span data-ttu-id="d45d1-225">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="d45d1-225">@odata.etag</span></span> | <span data-ttu-id="d45d1-226">string</span><span class="sxs-lookup"><span data-stu-id="d45d1-226">string</span></span> | <span data-ttu-id="d45d1-227">Das HTTP-Entitäts-Tag, das eine Version des Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="d45d1-227">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="d45d1-228">id</span><span class="sxs-lookup"><span data-stu-id="d45d1-228">id</span></span> | <span data-ttu-id="d45d1-229">string</span><span class="sxs-lookup"><span data-stu-id="d45d1-229">string</span></span> | <span data-ttu-id="d45d1-230">Der Bezeichner des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d45d1-230">The identifier of the object.</span></span> |

> <span data-ttu-id="d45d1-231">**Hinweis:** Der Wert `id`, der in `resourceData` bereitgestellt wird, ist zu dem Zeitpunkt gültig, zu dem die Benachrichtigung generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="d45d1-231">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="d45d1-232">Einige Aktionen, z. B. das Verschieben einer Nachricht in einen anderen Ordner, können dazu führen, dass die `id` nicht mehr gültig ist, wenn die Benachrichtigung verarbeitet wird.</span><span class="sxs-lookup"><span data-stu-id="d45d1-232">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="d45d1-233">Benachrichtigungsbeispiel</span><span class="sxs-lookup"><span data-stu-id="d45d1-233">Notification example</span></span>

<span data-ttu-id="d45d1-234">Wenn der Benutzer eine E-Mail empfängt, sendet Microsoft Graph eine Benachrichtigung wie die folgende:</span><span class="sxs-lookup"><span data-stu-id="d45d1-234">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@<tenant_guid>/messages/{long_id_string}",
      "resourceData":
      {
        "@odata.type":"#Microsoft.Graph.Message",
        "@odata.id":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
        "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
        "id":"<long_id_string>"
      }
    }
  ]
}
```

<span data-ttu-id="d45d1-235">Beachten Sie, dass das Feld `value` ein Array von Objekten ist.</span><span class="sxs-lookup"><span data-stu-id="d45d1-235">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="d45d1-236">Wenn viele Benachrichtigungen in der Warteschlange stehen, sendet Microsoft Graph möglicherweise mehrere Objekte in einer einzigen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d45d1-236">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="d45d1-237">Benachrichtigungen aus anderen Abonnements können in dieselbe Benachrichtigungsanforderung aufgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="d45d1-237">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="d45d1-238">Verarbeiten der Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="d45d1-238">Processing the notification</span></span>

<span data-ttu-id="d45d1-239">Jede Benachrichtigung, die Ihre App erhält, sollte verarbeitet werden.</span><span class="sxs-lookup"><span data-stu-id="d45d1-239">Each notification received by your app should be processed.</span></span> <span data-ttu-id="d45d1-240">Die folgenden Aufgaben müssen von der App mindestens durchgeführt werden, um eine Benachrichtigung zu verarbeiten:</span><span class="sxs-lookup"><span data-stu-id="d45d1-240">The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="d45d1-241">Überprüfen der `clientState`-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="d45d1-241">Validate the `clientState` property.</span></span> <span data-ttu-id="d45d1-242">Sie muss dem Wert entsprechen, der ursprünglich mit der Anforderung zum Erstellen eines Abonnement übermittelt wurde.</span><span class="sxs-lookup"><span data-stu-id="d45d1-242">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="d45d1-243">**Hinweis:** Ist dies nicht der Fall, kann die Benachrichtigung nicht als gültig betrachtet werden.</span><span class="sxs-lookup"><span data-stu-id="d45d1-243">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="d45d1-244">Es ist möglich, dass die Benachrichtigung nicht von Microsoft Graph stammt und möglicherweise von einem gefälschten Akteur gesendet wurde.</span><span class="sxs-lookup"><span data-stu-id="d45d1-244">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="d45d1-245">Prüfen Sie auch, woher die Benachrichtigung stammt, und ergreifen Sie die entsprechenden Maßnahmen.</span><span class="sxs-lookup"><span data-stu-id="d45d1-245">You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="d45d1-246">Aktualisieren Sie die Anwendung basierend auf Ihrer Geschäftslogik.</span><span class="sxs-lookup"><span data-stu-id="d45d1-246">Update your application based on your business logic.</span></span>

1. <span data-ttu-id="d45d1-247">Senden Sie in Ihrer Antwort an Microsoft Graph einen `202 - Accepted` -Statuscode.</span><span class="sxs-lookup"><span data-stu-id="d45d1-247">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="d45d1-248">Wenn Microsoft Graph keinen Code der Klasse 2xx erhält, wird versucht, die Benachrichtigung mehrmals erneut zu senden.</span><span class="sxs-lookup"><span data-stu-id="d45d1-248">If Microsoft Graph doesn't receive a 2xx class code, it will retry the notification a number of times.</span></span>

    > <span data-ttu-id="d45d1-249">**Hinweis:** Senden Sie auch dann einen `202 - Accepted`-Statuscode, wenn die Eigenschaft `clientState` nicht mit derjenigen übereinstimmt, die in der Abonnementanfrage übermittelt wurde.</span><span class="sxs-lookup"><span data-stu-id="d45d1-249">**Note:** You should send a `202 - Accepted` status code even if the `clientState` property doesn't match the one submitted with the subscription request.</span></span> <span data-ttu-id="d45d1-250">Dies ist eine empfohlene Vorgehensweise, da sie verhindert, dass ein potenziell gefälschte Akteur die Tatsache erkennt, dass Sie seinen Benachrichtigungen nicht vertrauen. Anhand dieser Informationen versucht er dann möglicherweise, den Wert der `clientState`-Eigenschaft zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="d45d1-250">This is a good practice as it prevents a potential rogue actor from discovering the fact that you may not trust their notifications, and perhaps using that information to guess the value of the `clientState` property.</span></span>

<span data-ttu-id="d45d1-251">Wiederholen Sie den Vorgang für weitere Benachrichtigungen in der Anfrage.</span><span class="sxs-lookup"><span data-stu-id="d45d1-251">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="d45d1-252">Codebeispiele</span><span class="sxs-lookup"><span data-stu-id="d45d1-252">Code samples</span></span>

<span data-ttu-id="d45d1-253">Es folgen einige Codebeispiele in GitHub.</span><span class="sxs-lookup"><span data-stu-id="d45d1-253">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="d45d1-254">Microsoft Graph Webhooks-Beispiel für Node.js</span><span class="sxs-lookup"><span data-stu-id="d45d1-254">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="d45d1-255">Microsoft Graph Webhooks-Beispiel für ASP.NET</span><span class="sxs-lookup"><span data-stu-id="d45d1-255">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="d45d1-256">Microsoft Graph-Benutzer-Webhooks-Beispiel mit dem WebJobs-SDK</span><span class="sxs-lookup"><span data-stu-id="d45d1-256">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="d45d1-257">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="d45d1-257">See also</span></span>

- [<span data-ttu-id="d45d1-258">Abonnementressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d45d1-258">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="d45d1-259">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="d45d1-259">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="d45d1-260">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="d45d1-260">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)

[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[conversation]: /graph/api/resources/conversation?view=graph-rest-1.0
[driveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[group]: /graph/api/resources/group?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
[user]: /graph/api/resources/user?view=graph-rest-1.0
[alert]: /graph/api/resources/alert?view=graph-rest-1.0
