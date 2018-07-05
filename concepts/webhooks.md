# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="edaa3-101">Einrichten von Benachrichtigungen für Änderungen der Benutzerdaten</span><span class="sxs-lookup"><span data-stu-id="edaa3-101">Set up notifications for changes in user data</span></span>

<span data-ttu-id="edaa3-p101">Die Microsoft Graph-API verwendet einen Webhook-Mechanismus zum Übermitteln von Benachrichtigungen an Clients. Ein Client ist ein Webdienst, der eine eigene URL zum Empfangen von Benachrichtigungen konfiguriert. Client-Apps verwenden Benachrichtigungen, um bei Änderungen ihren Status zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="edaa3-p101">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="edaa3-105">Nachdem Microsoft Graph die Abonnementsanfrage akzeptiert hat, werden Pushbenachrichtigungen an die im Abonnement angegebene URL gesendet.</span><span class="sxs-lookup"><span data-stu-id="edaa3-105">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription. The app then takes action according to its business logic. For example, it fetches more data, updates cache and views, etc.</span></span> <span data-ttu-id="edaa3-106">Die App führt dann Aktionen gemäß der Geschäftslogik aus.</span><span class="sxs-lookup"><span data-stu-id="edaa3-106">The app then takes action according to its business logic.</span></span> <span data-ttu-id="edaa3-107">Sie ruft z. B. weitere Daten ab, aktualisiert Zwischenspeicher für Dokumente und Ansichten usw.</span><span class="sxs-lookup"><span data-stu-id="edaa3-107">For example, it fetches more data, updates its cache and views, etc.</span></span>

## <a name="supported-resources"></a><span data-ttu-id="edaa3-108">Unterstützte Ressourcen</span><span class="sxs-lookup"><span data-stu-id="edaa3-108">Supported resources</span></span>

<span data-ttu-id="edaa3-109">Mit der Microsoft Graph-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:</span><span class="sxs-lookup"><span data-stu-id="edaa3-109">Using the Microsoft Graph REST API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="edaa3-110">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="edaa3-110">Messages</span></span>
- <span data-ttu-id="edaa3-111">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="edaa3-111">Events</span></span>
- <span data-ttu-id="edaa3-112">Kontakte</span><span class="sxs-lookup"><span data-stu-id="edaa3-112">Contacts</span></span>
- <span data-ttu-id="edaa3-113">Benutzer</span><span class="sxs-lookup"><span data-stu-id="edaa3-113">Users</span></span>
- <span data-ttu-id="edaa3-114">Gruppen</span><span class="sxs-lookup"><span data-stu-id="edaa3-114">Groups</span></span>
- <span data-ttu-id="edaa3-115">Gruppenunterhaltungen</span><span class="sxs-lookup"><span data-stu-id="edaa3-115">Group conversations</span></span>
- <span data-ttu-id="edaa3-116">Inhalten, die in OneDrive freigegeben werden, einschließlich der diesen SharePoint-Websites zugeordneten Laufwerke</span><span class="sxs-lookup"><span data-stu-id="edaa3-116">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="edaa3-117">Persönlichen OneDrive-Ordnern des Benutzers</span><span class="sxs-lookup"><span data-stu-id="edaa3-117">User's personal OneDrive folders</span></span>

<span data-ttu-id="edaa3-118">Sie können zum Beispiel ein Abonnement für einen bestimmten Mailordner erstellen: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="edaa3-118">For instance, you can create a subscription to a specific folder: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="edaa3-119">Oder für eine Ressource der obersten Ebene: `me/messages`, `me/contacts`, `me/events`, `users`, oder `groups`</span><span class="sxs-lookup"><span data-stu-id="edaa3-119">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="edaa3-120">Oder für eine bestimmte Ressourceninstanz: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="edaa3-120">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="edaa3-121">Oder für ein Sharepoint Online/OneDrive for Business-Laufwerk: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="edaa3-121">Or to a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="edaa3-122">Oder für die persönliche OneDrive-Umgebung eines Benutzers:`/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="edaa3-122">Or on a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="edaa3-123">Azure AD-Ressourceneinschränkungen</span><span class="sxs-lookup"><span data-stu-id="edaa3-123">Azure AD Resource Limitations</span></span>

<span data-ttu-id="edaa3-124">Bestimmte Einschränkungen gelten für Azure AD-basierte Ressourcen (Benutzer, Gruppen) und können bei Überschreitung Fehler hervorrufen:</span><span class="sxs-lookup"><span data-stu-id="edaa3-124">Certain limits apply to Azure AD based resources (users, groups) and may generate errors when exceeded:</span></span>

- <span data-ttu-id="edaa3-125">Maximale Abonnementkontingente:</span><span class="sxs-lookup"><span data-stu-id="edaa3-125">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="edaa3-126">Pro App: 50 000 Abonnements insgesamt</span><span class="sxs-lookup"><span data-stu-id="edaa3-126">Per App: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="edaa3-127">Pro Mandant: 35 Abonnements insgesamt in allen Apps</span><span class="sxs-lookup"><span data-stu-id="edaa3-127">Per Tenant: 35 total subscriptions across all apps</span></span>
  - <span data-ttu-id="edaa3-128">Pro App und Mandanten kombiniert: 7 Abonnements insgesamt</span><span class="sxs-lookup"><span data-stu-id="edaa3-128">Per App and Tenant combination: 7 total subscriptions</span></span>

- <span data-ttu-id="edaa3-129">Azure AD B2C-Mandanten werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="edaa3-129">Azure AD B2C tenants are not supported</span></span>

- <span data-ttu-id="edaa3-130">Benachrichtigungen für Benutzerentitäten werden für persönliche Microsoft-Konten nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="edaa3-130">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="edaa3-131">Gültigkeitsdauer von Abonnements</span><span class="sxs-lookup"><span data-stu-id="edaa3-131">Subscription lifetime</span></span>

<span data-ttu-id="edaa3-132">Abonnements haben eine eingeschränkte Gültigkeit.</span><span class="sxs-lookup"><span data-stu-id="edaa3-132">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="edaa3-133">Apps müssen ihre Abonnements vor dem Ablaufzeitpunkt verlängern.</span><span class="sxs-lookup"><span data-stu-id="edaa3-133">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="edaa3-134">Andernfalls müssen sie ein neues Abonnement erstellen.</span><span class="sxs-lookup"><span data-stu-id="edaa3-134">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="edaa3-135">Eine Liste maximaler Ablaufzeiten finden Sie unter [Maximale Abonnementdauer pro Ressourcentyp](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="edaa3-135">For a list of maximum expiration times, see [Maximum length of subscription per resource type](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="edaa3-136">Apps können auch jederzeit gekündigt werden, um keine weiteren Benachrichtigungen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="edaa3-136">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="edaa3-137">Verwalten von Abonnements</span><span class="sxs-lookup"><span data-stu-id="edaa3-137">Managing subscriptions</span></span>

<span data-ttu-id="edaa3-138">Clients können Abonnements erstellen, verlängern und löschen.</span><span class="sxs-lookup"><span data-stu-id="edaa3-138">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="edaa3-139">Erstellen eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="edaa3-139">Creating a subscription</span></span>

<span data-ttu-id="edaa3-p104">Um Benachrichtigungen für eine Ressource zu erhalten, muss in einem ersten Schritt ein Abonnement erstellt werden. Der Abonnementprozess läuft wie folgt ab:</span><span class="sxs-lookup"><span data-stu-id="edaa3-p104">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="edaa3-142">Der Client sendet eine Abonnementanforderung (POST) für eine bestimmte Ressource.</span><span class="sxs-lookup"><span data-stu-id="edaa3-142">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="edaa3-143">Microsoft Graph überprüft die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="edaa3-143">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="edaa3-144">Wenn die Anforderung gültig ist, sendet Microsoft Graph ein Überprüfungsstoken an die Benachrichtigungs-URL.</span><span class="sxs-lookup"><span data-stu-id="edaa3-144">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="edaa3-145">Wenn die Anfrage ungültig ist, sendet Microsoft Graph eine Fehlermeldung mit Code und Details.</span><span class="sxs-lookup"><span data-stu-id="edaa3-145">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="edaa3-146">Der Client sendet das Überprüfungstoken zurück an Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="edaa3-146">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="edaa3-147">Microsoft Graph sendet eine Antwort an den Client zurück.</span><span class="sxs-lookup"><span data-stu-id="edaa3-147">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="edaa3-148">Der Client muss die Abonnement-ID speichern, um Benachrichtigungen mit dem Abonnement korrelieren zu können.</span><span class="sxs-lookup"><span data-stu-id="edaa3-148">Client must store the subscription ID to correlate a notification with the corresponding subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="edaa3-149">Beispiel für eine Abonnementanfrage</span><span class="sxs-lookup"><span data-stu-id="edaa3-149">Subscription request example</span></span>

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

<span data-ttu-id="edaa3-150">Die Eigenschaften `changeType`, `notificationUrl`, `resource` und `expirationDateTime` sind erforderlich.</span><span class="sxs-lookup"><span data-stu-id="edaa3-150">The `changeType`, `notificationUrl`, `resource` and `expirationDateTime` properties are required while the rest are optional.</span></span> <span data-ttu-id="edaa3-151">Unter [subscription-Ressourcentyp](../api-reference/v1.0/resources/subscription.md) finden Sie die Eigenschaftsdefinitionen und Werte.</span><span class="sxs-lookup"><span data-stu-id="edaa3-151">See [subscription resource type](../api-reference/v1.0/resources/subscription.md) for property definitions and values.</span></span>

<span data-ttu-id="edaa3-152">`clientState` ist zwar nicht erforderlich, muss aber eingeschlossen werden, um unserem empfohlenen Prozess zum Umgang mit Benachrichtigungen zu entsprechen.</span><span class="sxs-lookup"><span data-stu-id="edaa3-152">The , , , and  properties are required. See subscription resource type for property definitions and values. Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="edaa3-153">Durch das Festlegen dieser Eigenschaft können Sie bestätigen, dass die empfangenen Benachrichtigungen vom Microsoft Graph-Dienst stammen.</span><span class="sxs-lookup"><span data-stu-id="edaa3-153">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="edaa3-154">Aus diesem Grund muss der Wert der Eigenschaft geheim bleiben und darf nur der Anwendung und dem Microsoft Graph-Dienst bekannt sein.</span><span class="sxs-lookup"><span data-stu-id="edaa3-154">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="edaa3-155">Wenn der Vorgang erfolgreich war, gibt Microsoft Graph einen `201 Created`-Code und ein [subscription](../api-reference/v1.0/resources/subscription.md)-Objekt im Textkörper zurück.</span><span class="sxs-lookup"><span data-stu-id="edaa3-155">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](../api-reference/v1.0/resources/subscription.md) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="edaa3-156">Endpunktprüfung für Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="edaa3-156">Notification endpoint validation</span></span>

<span data-ttu-id="edaa3-157">Microsoft Graph überprüft den Benachrichtigungsendpunkt, der in der Eigenschaft `notificationUrl` der Abonnementanfrage angegeben ist, bevor das Abonnement erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="edaa3-157">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="edaa3-158">Der Überprüfungsprozess läuft wie folgt ab:</span><span class="sxs-lookup"><span data-stu-id="edaa3-158">The filtering process in a dashboard occurs as follows:</span></span>

1. <span data-ttu-id="edaa3-159">Microsoft Graph sendet eine POST-Anforderung an die Benachrichtigungs-URL:</span><span class="sxs-lookup"><span data-stu-id="edaa3-159">Microsoft Graph sends a POST request to the notification URL:</span></span>

  ``` http
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ```

1. <span data-ttu-id="edaa3-160">Der Client muss innerhalb von 10 Sekunden eine Antwort mit folgenden Merkmalen bereitstellen:</span><span class="sxs-lookup"><span data-stu-id="edaa3-160">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="edaa3-161">Statuscode 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="edaa3-161">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="edaa3-162">Der Inhaltstyp muss `text/plain` sein.</span><span class="sxs-lookup"><span data-stu-id="edaa3-162">The content type must be text/plain.</span></span>
    - <span data-ttu-id="edaa3-163">Der Textkörper muss das von Microsoft Graph bereitgestellte Überprüfungstoken enthalten.</span><span class="sxs-lookup"><span data-stu-id="edaa3-163">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="edaa3-164">Der Client muss den Überprüfungstoken verwerfen, nachdem er in der Antwort bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="edaa3-164">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="edaa3-165">Verlängern eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="edaa3-165">Renewing a subscription</span></span>

<span data-ttu-id="edaa3-166">Der Kunde kann ein Abonnement mit einem bestimmten Ablaufdatum von bis zu drei Tagen ab dem Zeitpunkt der Anforderung verlängern.</span><span class="sxs-lookup"><span data-stu-id="edaa3-166">The client can renew a subscription with a specific expiration date of up to three days from the time of request. The expirationDateTime property is required.</span></span> <span data-ttu-id="edaa3-167">Die Eigenschaft `expirationDateTime` muss angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="edaa3-167">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="edaa3-168">Beispiel für eine Abonnementverlängerung</span><span class="sxs-lookup"><span data-stu-id="edaa3-168">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="edaa3-169">Wenn der Vorgang erfolgreich war, gibt Microsoft Graph einen `200 OK`-Code und ein [subscription](../api-reference/v1.0/resources/subscription.md)-Objekt im Textkörper zurück.</span><span class="sxs-lookup"><span data-stu-id="edaa3-169">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](../api-reference/v1.0/resources/subscription.md) object in the body.</span></span> <span data-ttu-id="edaa3-170">Das Abonnementobjekt enthält den neuen Wert für `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="edaa3-170">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="edaa3-171">Löschen eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="edaa3-171">Deleting a subscription</span></span>

<span data-ttu-id="edaa3-172">Der Client kann den Erhalt von Benachrichtigungen stoppen, indem er das Abonnement anhand seiner ID löscht.</span><span class="sxs-lookup"><span data-stu-id="edaa3-172">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="edaa3-173">Wenn der Vorgang erfolgreich verläuft, gibt Microsoft Graph einen `204 No Content`-Code zurück.</span><span class="sxs-lookup"><span data-stu-id="edaa3-173">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="edaa3-174">Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="edaa3-174">Notifications</span></span>

<span data-ttu-id="edaa3-175">Der Client beginnt, Benachrichtigungen zu erhalten, nachdem das Abonnement erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="edaa3-175">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="edaa3-176">Microsoft Graph sendet eine POST-Anforderung an die Benachrichtigungs-URL, wenn sich die Ressource ändert.</span><span class="sxs-lookup"><span data-stu-id="edaa3-176">Microsoft Graph sends a POST request to the notification URL:</span></span> <span data-ttu-id="edaa3-177">Benachrichtigungen werden nur für die Änderungen des Typs gesendet, der im Abonnement angegeben ist, z. B. `created`.</span><span class="sxs-lookup"><span data-stu-id="edaa3-177">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="edaa3-178">**Hinweis:** Wenn Sie mehrere Abonnements verwenden, die den gleichen Ressourcentyp überwachen und die gleiche Benachrichtigungs-URL verwenden, kann ein POST gesendet werden, der mehrere Benachrichtigungen mit verschiedenen Abonnement-IDs enthalten kann.</span><span class="sxs-lookup"><span data-stu-id="edaa3-178">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="edaa3-179">Es kann nicht garantiert werden, dass alle Benachrichtigungen in einem POST zu einem einzelnen Abonnement gehören.</span><span class="sxs-lookup"><span data-stu-id="edaa3-179">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="edaa3-180">Benachrichtigungseigenschaften</span><span class="sxs-lookup"><span data-stu-id="edaa3-180">Notification properties</span></span>

<span data-ttu-id="edaa3-181">Das Benachrichtigungsobjekt verfügt über die folgenden Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="edaa3-181">The notification object has the following properties:</span></span>

| <span data-ttu-id="edaa3-182">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="edaa3-182">Property</span></span> | <span data-ttu-id="edaa3-183">Typ</span><span class="sxs-lookup"><span data-stu-id="edaa3-183">Type</span></span> | <span data-ttu-id="edaa3-184">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="edaa3-184">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="edaa3-185">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="edaa3-185">subscriptionId</span></span> | <span data-ttu-id="edaa3-186">string</span><span class="sxs-lookup"><span data-stu-id="edaa3-186">string</span></span> | <span data-ttu-id="edaa3-187">Die ID des Abonnements, das die Benachrichtigung generiert hat.</span><span class="sxs-lookup"><span data-stu-id="edaa3-187">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="edaa3-188">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="edaa3-188">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="edaa3-189">dateTime</span><span class="sxs-lookup"><span data-stu-id="edaa3-189">dateTime</span></span>](http://tools.ietf.org/html/rfc3339) | <span data-ttu-id="edaa3-190">Die Ablaufzeit für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="edaa3-190">: The expiration time for the subscription.</span></span> |
| <span data-ttu-id="edaa3-191">clientState</span><span class="sxs-lookup"><span data-stu-id="edaa3-191">clientState</span></span> | <span data-ttu-id="edaa3-192">string</span><span class="sxs-lookup"><span data-stu-id="edaa3-192">string</span></span> | <span data-ttu-id="edaa3-193">Die `clientState`-Eigenschaft in der Abonnementanforderung (falls vorhanden).</span><span class="sxs-lookup"><span data-stu-id="edaa3-193">clientState - The clientState property specified in the subscription request.</span></span> |
| <span data-ttu-id="edaa3-194">changeType</span><span class="sxs-lookup"><span data-stu-id="edaa3-194">changeType</span></span> | <span data-ttu-id="edaa3-195">string</span><span class="sxs-lookup"><span data-stu-id="edaa3-195">string</span></span> | <span data-ttu-id="edaa3-196">Der Ereignistyp, der die Benachrichtigung ausgelöst hat.</span><span class="sxs-lookup"><span data-stu-id="edaa3-196">The event type that caused the notification.</span></span> <span data-ttu-id="edaa3-197">Beispiel: `created` bei Erhalt einer E-Mail oder `updated`, wenn eine Nachricht als gelesen markiert wird.</span><span class="sxs-lookup"><span data-stu-id="edaa3-197">changeType - The event type that caused the notification. For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="edaa3-198">resource</span><span class="sxs-lookup"><span data-stu-id="edaa3-198">resource</span></span> | <span data-ttu-id="edaa3-199">string</span><span class="sxs-lookup"><span data-stu-id="edaa3-199">string</span></span> | <span data-ttu-id="edaa3-200">Der URI der Ressource relativ zu `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="edaa3-200">resource - The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="edaa3-201">resourceData</span><span class="sxs-lookup"><span data-stu-id="edaa3-201">ResourceData</span></span> | <span data-ttu-id="edaa3-202">object</span><span class="sxs-lookup"><span data-stu-id="edaa3-202">object</span></span> | <span data-ttu-id="edaa3-203">Der Inhalt dieser Eigenschaft hängt vom Typ der Ressource ab, die abonniert wurde.</span><span class="sxs-lookup"><span data-stu-id="edaa3-203">The content of this property depends on the type of resource being subscribed to.</span></span> |

<span data-ttu-id="edaa3-204">Beispiel: Für Outlook-Ressourcen enthält `resourceData` die folgenden Felder:</span><span class="sxs-lookup"><span data-stu-id="edaa3-204">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="edaa3-205">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="edaa3-205">Property</span></span> | <span data-ttu-id="edaa3-206">Typ</span><span class="sxs-lookup"><span data-stu-id="edaa3-206">Type</span></span> | <span data-ttu-id="edaa3-207">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="edaa3-207">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="edaa3-208">@odata.type</span><span class="sxs-lookup"><span data-stu-id="edaa3-208">@odata.type</span></span> | <span data-ttu-id="edaa3-209">string</span><span class="sxs-lookup"><span data-stu-id="edaa3-209">string</span></span> | <span data-ttu-id="edaa3-210">Der OData-Entitätstyp in Microsoft Graph, der das dargestellte Objekt beschreibt.</span><span class="sxs-lookup"><span data-stu-id="edaa3-210">@odata.type - The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="edaa3-211">@odata.id</span><span class="sxs-lookup"><span data-stu-id="edaa3-211">@odata.id</span></span> | <span data-ttu-id="edaa3-212">string</span><span class="sxs-lookup"><span data-stu-id="edaa3-212">string</span></span> | <span data-ttu-id="edaa3-213">Der OData-Bezeichner des Objekts.</span><span class="sxs-lookup"><span data-stu-id="edaa3-213">@odata.id - The OData identifier of the object.</span></span> |
| <span data-ttu-id="edaa3-214">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="edaa3-214">@odata.etag</span></span> | <span data-ttu-id="edaa3-215">string</span><span class="sxs-lookup"><span data-stu-id="edaa3-215">string</span></span> | <span data-ttu-id="edaa3-216">Das HTTP-Entitäts-Tag, das eine Version des Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="edaa3-216">@odata.etag - The HTTP entity tag that represents a version of the object.</span></span> |
| <span data-ttu-id="edaa3-217">id</span><span class="sxs-lookup"><span data-stu-id="edaa3-217">id</span></span> | <span data-ttu-id="edaa3-218">string</span><span class="sxs-lookup"><span data-stu-id="edaa3-218">string</span></span> | <span data-ttu-id="edaa3-219">Der Bezeichner des Objekts.</span><span class="sxs-lookup"><span data-stu-id="edaa3-219">Id - The identifier of the object.</span></span> |

> <span data-ttu-id="edaa3-220">**Hinweis:** Der Wert `id`, der in `resourceData` bereitgestellt wird, ist zu dem Zeitpunkt gültig, zu dem die Benachrichtigung generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="edaa3-220">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="edaa3-221">Einige Aktionen, z. B. das Verschieben einer Nachricht in einen anderen Ordner, können dazu führen, dass die `id` nicht mehr gültig ist, wenn die Benachrichtigung verarbeitet wird.</span><span class="sxs-lookup"><span data-stu-id="edaa3-221">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="edaa3-222">Benachrichtigungsbeispiel</span><span class="sxs-lookup"><span data-stu-id="edaa3-222">Notification example</span></span>

<span data-ttu-id="edaa3-223">Wenn der Benutzer eine E-Mail empfängt, sendet Microsoft Graph eine Benachrichtigung wie die folgende:</span><span class="sxs-lookup"><span data-stu-id="edaa3-223">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

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

<span data-ttu-id="edaa3-224">Beachten Sie, dass das Feld `value` ein Array von Objekten ist.</span><span class="sxs-lookup"><span data-stu-id="edaa3-224">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="edaa3-225">Wenn viele Benachrichtigungen in der Warteschlange stehen, sendet Microsoft Graph möglicherweise mehrere Objekte in einer einzigen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="edaa3-225">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="edaa3-226">Benachrichtigungen aus anderen Abonnements können in dieselbe Benachrichtigungsanforderung aufgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="edaa3-226">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="edaa3-227">Verarbeiten der Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="edaa3-227">Processing the notification</span></span>

<span data-ttu-id="edaa3-228">Jede Benachrichtigung, die Ihre App erhält, sollte verarbeitet werden.</span><span class="sxs-lookup"><span data-stu-id="edaa3-228">Each notification received by your app should be processed.</span></span> <span data-ttu-id="edaa3-229">Die folgenden Aufgaben müssen von der App mindestens durchgeführt werden, um eine Benachrichtigung zu verarbeiten:</span><span class="sxs-lookup"><span data-stu-id="edaa3-229">After your application starts receiving notifications it must process them. The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="edaa3-230">Überprüfen der `clientState`-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="edaa3-230">Validate the `clientState` property.</span></span> <span data-ttu-id="edaa3-231">Sie muss dem Wert entsprechen, der ursprünglich mit der Anforderung zum Erstellen eines Abonnement übermittelt wurde.</span><span class="sxs-lookup"><span data-stu-id="edaa3-231">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="edaa3-232">**Hinweis:** Ist dies nicht der Fall, kann die Benachrichtigung nicht als gültig betrachtet werden.</span><span class="sxs-lookup"><span data-stu-id="edaa3-232">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="edaa3-233">Es ist möglich, dass die Benachrichtigung nicht von Microsoft Graph stammt und möglicherweise von einem gefälschten Akteur gesendet wurde.</span><span class="sxs-lookup"><span data-stu-id="edaa3-233">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="edaa3-234">Prüfen Sie auch, woher die Benachrichtigung stammt, und ergreifen Sie die entsprechenden Maßnahmen.</span><span class="sxs-lookup"><span data-stu-id="edaa3-234">Note: If this isn't true, you shouldn't consider this a valid notification. You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="edaa3-235">Aktualisieren Sie die Anwendung basierend auf Ihrer Geschäftslogik.</span><span class="sxs-lookup"><span data-stu-id="edaa3-235">Update your application based on your business logic.</span></span>

1. <span data-ttu-id="edaa3-236">Senden Sie in Ihrer Antwort an Microsoft Graph einen `202 - Accepted` -Statuscode.</span><span class="sxs-lookup"><span data-stu-id="edaa3-236">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="edaa3-237">Wenn Microsoft Graph keinen Code der Klasse 2xx erhält, wird versucht, die Benachrichtigung mehrmals erneut zu senden.</span><span class="sxs-lookup"><span data-stu-id="edaa3-237">Send a  status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>

    > <span data-ttu-id="edaa3-238">**Hinweis:** Senden Sie auch dann einen `202 - Accepted`-Statuscode, wenn die Eigenschaft `clientState` nicht mit derjenigen übereinstimmt, die in der Abonnementanfrage übermittelt wurde.</span><span class="sxs-lookup"><span data-stu-id="edaa3-238">You should send a  status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span> <span data-ttu-id="edaa3-239">Dies ist eine empfohlene Vorgehensweise, da sie verhindert, dass ein potenziell gefälschte Akteur die Tatsache erkennt, dass Sie seinen Benachrichtigungen nicht vertrauen. Anhand dieser Informationen versucht er dann möglicherweise, den Wert der `clientState`-Eigenschaft zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="edaa3-239">This is a good practice as it prevents a potential rogue actor from discovering the fact that you may not trust their notifications, and perhaps using that information to guess the value of the `clientState` property.</span></span>

<span data-ttu-id="edaa3-240">Wiederholen Sie den Vorgang für weitere Benachrichtigungen in der Anfrage.</span><span class="sxs-lookup"><span data-stu-id="edaa3-240">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="edaa3-241">Codebeispiele</span><span class="sxs-lookup"><span data-stu-id="edaa3-241">Code samples</span></span>

<span data-ttu-id="edaa3-242">Es folgen einige Codebeispiele in GitHub.</span><span class="sxs-lookup"><span data-stu-id="edaa3-242">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="edaa3-243">Microsoft Graph Webhooks-Beispiel für Node.js</span><span class="sxs-lookup"><span data-stu-id="edaa3-243">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="edaa3-244">Microsoft Graph Webhooks-Beispiel für ASP.NET</span><span class="sxs-lookup"><span data-stu-id="edaa3-244">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="edaa3-245">Microsoft Graph-Benutzer-Webhooks-Beispiel mit dem WebJobs-SDK</span><span class="sxs-lookup"><span data-stu-id="edaa3-245">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="edaa3-246">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="edaa3-246">See also</span></span>

- [<span data-ttu-id="edaa3-247">Abonnementressourcentyp</span><span class="sxs-lookup"><span data-stu-id="edaa3-247">Subscription resource type</span></span>](../api-reference/v1.0/resources/subscription.md)
- [<span data-ttu-id="edaa3-248">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="edaa3-248">Get subscription</span></span>](../api-reference/v1.0/api/subscription_get.md)
- [<span data-ttu-id="edaa3-249">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="edaa3-249">Create subscription</span></span>](../api-reference/v1.0/api/subscription_post_subscriptions.md)

[contact]: ../api-reference/v1.0/resources/contact.md
[conversation]: ../api-reference/v1.0/resources/conversation.md
[drive]: ../api-reference/v1.0/resources/drive.md
[event]: ../api-reference/v1.0/resources/event.md
[message]: ../api-reference/v1.0/resources/message.md
