# <a name="working-with-webhooks-in-microsoft-graph"></a><span data-ttu-id="4b84d-101">Arbeiten mit Webhooks in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4b84d-101">Working with Webhooks in Microsoft Graph</span></span>

<span data-ttu-id="4b84d-p101">Die Microsoft Graph-REST-API verwendet einen Webhook-Mechanismus zum Übermitteln von Benachrichtigungen an Clients. Ein Client ist ein Webdienst, der eine eigene URL zum Empfangen von Benachrichtigungen konfiguriert. Client-Apps verwenden Benachrichtigungen, um bei Änderungen ihren Status zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="4b84d-p101">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="4b84d-105">Mithilfe der Microsoft Graph-REST-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:</span><span class="sxs-lookup"><span data-stu-id="4b84d-105">Using the Microsoft Graph REST API, an app can subscribe to changes on the following resources:</span></span>

* <span data-ttu-id="4b84d-106">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="4b84d-106">Messages</span></span>
* <span data-ttu-id="4b84d-107">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="4b84d-107">Events</span></span>
* <span data-ttu-id="4b84d-108">Kontakte</span><span class="sxs-lookup"><span data-stu-id="4b84d-108">Contacts</span></span>
* <span data-ttu-id="4b84d-109">Benutzer</span><span class="sxs-lookup"><span data-stu-id="4b84d-109">Users</span></span>
* <span data-ttu-id="4b84d-110">Gruppen</span><span class="sxs-lookup"><span data-stu-id="4b84d-110">Groups</span></span>
* <span data-ttu-id="4b84d-111">Gruppenunterhaltungen</span><span class="sxs-lookup"><span data-stu-id="4b84d-111">Group conversations</span></span>
* <span data-ttu-id="4b84d-112">Inhalten, die in OneDrive freigegeben werden, einschließlich der diesen SharePoint-Websites zugeordneten Laufwerke</span><span class="sxs-lookup"><span data-stu-id="4b84d-112">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
* <span data-ttu-id="4b84d-113">Persönlichen OneDrive-Ordnern des Benutzers</span><span class="sxs-lookup"><span data-stu-id="4b84d-113">User's personal OneDrive folders</span></span>

<span data-ttu-id="4b84d-114">Sie können zum Beispiel ein Abonnement für einen bestimmten Ordner erstellen: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="4b84d-114">For instance, you can create a subscription to a specific folder: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="4b84d-115">Oder eine bestimmte ID: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="4b84d-115">Or a specific ID: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="4b84d-116">Oder für eine Ressource der obersten Ebene: `me/messages`, `me/contacts`, `me/events`, `users`, oder `groups`</span><span class="sxs-lookup"><span data-stu-id="4b84d-116">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`</span></span>

<span data-ttu-id="4b84d-117">Oder ein Sharepoint Online/OneDrive for Business-Laufwerk: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="4b84d-117">Or on a Sharepoint / OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="4b84d-118">Oder persönliche OneDrive-Umgebung eines Benutzers:`/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="4b84d-118">Or on a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="4b84d-p102">Nachdem Microsoft Graph die Abonnementsanfrage akzeptiert hat, werden Pushbenachrichtigungen an die im Abonnement angegebene URL gesendet. Die App führt dann Aktionen gemäß der Geschäftslogik aus. Sie ruft z. B. weitere Daten ab, aktualisiert Zwischenspeicher für Dokumente und Ansichten usw.</span><span class="sxs-lookup"><span data-stu-id="4b84d-p102">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription. The app then takes action according to its business logic. For example, it fetches more data, updates cache and views, etc.</span></span>

<span data-ttu-id="4b84d-122">Apps müssen ihre Abonnements vor dem Ablaufzeitpunkt verlängern.</span><span class="sxs-lookup"><span data-stu-id="4b84d-122">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="4b84d-123">Andernfalls müssen sie ein neues Abonnement erstellen.</span><span class="sxs-lookup"><span data-stu-id="4b84d-123">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="4b84d-124">Eine Liste maximaler Ablaufzeiten finden Sie unter [Maximale Abonnementdauer pro Ressourcentyp](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="4b84d-124">For a list of maximum expiration times, see [Maximum length of subscription per resource type](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="4b84d-125">Apps können auch jederzeit gekündigt werden, um keine weiteren Benachrichtigungen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="4b84d-125">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

<span data-ttu-id="4b84d-p104">In der Regel sind für Abonnementvorgänge Leseberechtigungen für die Ressource erforderlich. Beispiel: um Benachrichtigungen zu Nachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. Unter [Abonnement erstellen](../api-reference/v1.0/api/subscription_post_subscriptions.md) werden die Berechtigungen aufgeführt, die für den jeweiligen Ressourcentyp erforderlich sind. Die folgende Tabelle enthält die Typen von Berechtigungen, die Ihre App für die Verwendung von Webhooks für bestimmte Ressourcentypen anfordern kann.</span><span class="sxs-lookup"><span data-stu-id="4b84d-p104">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api-reference/v1.0/api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span> 

| <span data-ttu-id="4b84d-130">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b84d-130">Permission type</span></span>                        | <span data-ttu-id="4b84d-131">Unterstützte Ressourcentypen in v1.0</span><span class="sxs-lookup"><span data-stu-id="4b84d-131">Supported resource types in v1.0</span></span>                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="4b84d-132">Delegiert – Geschäfts-, Schul- oder Unikonto</span><span class="sxs-lookup"><span data-stu-id="4b84d-132">Delegated - work or school account</span></span>     | <span data-ttu-id="4b84d-133">[Kontakt][], [Unterhaltung][], [Laufwerk][], [Ereignis][], [Nachricht][]</span><span class="sxs-lookup"><span data-stu-id="4b84d-133">[contact][], [conversation][], [drive][], [event][], [message][]</span></span> |
| <span data-ttu-id="4b84d-134">Delegiert – persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="4b84d-134">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="4b84d-135">Keine</span><span class="sxs-lookup"><span data-stu-id="4b84d-135">None</span></span>                                                             |
| <span data-ttu-id="4b84d-136">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b84d-136">Application</span></span>                            | <span data-ttu-id="4b84d-137">[Kontakt][], [Unterhaltung][], [Ereignis][], [Nachricht][]</span><span class="sxs-lookup"><span data-stu-id="4b84d-137">[contact][], [conversation][], [event][], [message][]</span></span>            |


## <a name="code-samples"></a><span data-ttu-id="4b84d-138">Codebeispiele</span><span class="sxs-lookup"><span data-stu-id="4b84d-138">Code samples</span></span>

<span data-ttu-id="4b84d-139">Es folgen einige Codebeispiele in GitHub.</span><span class="sxs-lookup"><span data-stu-id="4b84d-139">The following code samples are available on GitHub.</span></span>

* [<span data-ttu-id="4b84d-140">Microsoft Graph Webhooks-Beispiel für Node.js</span><span class="sxs-lookup"><span data-stu-id="4b84d-140">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="4b84d-141">Microsoft Graph Webhooks-Beispiel für ASP.NET</span><span class="sxs-lookup"><span data-stu-id="4b84d-141">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

### <a name="creating-a-subscription"></a><span data-ttu-id="4b84d-142">Erstellen eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="4b84d-142">Creating a subscription</span></span>

<span data-ttu-id="4b84d-p105">Um Benachrichtigungen für eine Ressource zu erhalten, muss in einem ersten Schritt ein Abonnement erstellt werden. Der Abonnementprozess läuft wie folgt ab:</span><span class="sxs-lookup"><span data-stu-id="4b84d-p105">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="4b84d-145">Der Client sendet eine Abonnementanforderung (POST) für eine bestimmte Ressource.</span><span class="sxs-lookup"><span data-stu-id="4b84d-145">The client sends a subscription (POST) request for a specific resource.</span></span>
2. <span data-ttu-id="4b84d-146">Microsoft Graph überprüft die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4b84d-146">Microsoft Graph verifies the request.</span></span>
  * <span data-ttu-id="4b84d-147">Wenn die Anforderung gültig ist, sendet Microsoft Graph ein Überprüfungsstoken an die Benachrichtigungs-URL.</span><span class="sxs-lookup"><span data-stu-id="4b84d-147">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
  * <span data-ttu-id="4b84d-148">Wenn die Anfrage ungültig ist, sendet Microsoft Graph eine Fehlermeldung mit Code und Details.</span><span class="sxs-lookup"><span data-stu-id="4b84d-148">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>
3. <span data-ttu-id="4b84d-149">Der Client sendet das Überprüfungstoken zurück an Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4b84d-149">The client sends the validation token back to Microsoft Graph.</span></span>

<span data-ttu-id="4b84d-150">Der Client muss die Abonnement-ID speichern, um eine Benachrichtigung mit dem entsprechenden Abonnement korrelieren zu können.</span><span class="sxs-lookup"><span data-stu-id="4b84d-150">Client must store the subscription ID to correlate a notification with the corresponding subscription.</span></span>

### <a name="notification-url-validation"></a><span data-ttu-id="4b84d-151">Überprüfung der Benachrichtigungs-URL</span><span class="sxs-lookup"><span data-stu-id="4b84d-151">Notification URL validation</span></span>

<span data-ttu-id="4b84d-p106">Microsoft Graph überprüft die Benachrichtigungs-URL in einer Abonnementanfrage vor dem Erstellen des Abonnements. Der Überprüfungsprozess läuft wie folgt ab:</span><span class="sxs-lookup"><span data-stu-id="4b84d-p106">Microsoft Graph validates the notification URL in a subscription request before creating the subscription. The validation process occurs as follows:</span></span>

1. <span data-ttu-id="4b84d-154">Microsoft Graph sendet eine POST-Anforderung an die Benachrichtigungs-URL:</span><span class="sxs-lookup"><span data-stu-id="4b84d-154">Microsoft Graph sends a POST request to the notification URL:</span></span>

  ``` http
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ClientState: {Data sent in ClientState value in subscription request (if any)}
  ```

2. <span data-ttu-id="4b84d-155">Der Client muss innerhalb von 10 Sekunden eine Antwort mit folgenden Merkmalen bereitstellen:</span><span class="sxs-lookup"><span data-stu-id="4b84d-155">The client must provide a response with the following characteristics within 10 seconds:</span></span>

  * <span data-ttu-id="4b84d-156">Statuscode 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="4b84d-156">A 200 (OK) status code.</span></span>
  * <span data-ttu-id="4b84d-157">Der Inhaltstyp muss „text/plain“ sein.</span><span class="sxs-lookup"><span data-stu-id="4b84d-157">The content type must be text/plain.</span></span> 
  * <span data-ttu-id="4b84d-158">Der Textkörper muss das von Microsoft Graph bereitgestellte Überprüfungstoken enthalten.</span><span class="sxs-lookup"><span data-stu-id="4b84d-158">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="4b84d-159">Der Client muss den Überprüfungstoken verwerfen, nachdem er in der Antwort bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="4b84d-159">The client should discard the validation token after providing it in the response.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="4b84d-160">Beispiel für eine Abonnementanfrage</span><span class="sxs-lookup"><span data-stu-id="4b84d-160">Subscription request example</span></span>

``` http
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

<span data-ttu-id="4b84d-p107">Die Eigenschaften `changeType`, `notificationUrl`, `resource` und `expirationDateTime` sind erforderlich. Unter [subscription-Ressourcentyp](../api-reference/v1.0/resources/subscription.md) finden Sie die Eigenschaftsdefinitionen und Werte. `clientState` ist zwar nicht erforderlich, muss aber eingeschlossen werden, um unserem empfohlenen Prozess zum Umgang mit Benachrichtigungen zu entsprechen.</span><span class="sxs-lookup"><span data-stu-id="4b84d-p107">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required. See [subscription resource type](../api-reference/v1.0/resources/subscription.md) for property definitions and values. Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span>

<span data-ttu-id="4b84d-164">Wenn der Vorgang erfolgreich war, gibt Microsoft Graph einen `201 Created`-Code und ein [subscription](../api-reference/v1.0/resources/subscription.md)-Objekt im Textkörper zurück.</span><span class="sxs-lookup"><span data-stu-id="4b84d-164">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](../api-reference/v1.0/resources/subscription.md) object in the body.</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="4b84d-165">Azure AD-Ressourceneinschränkungen</span><span class="sxs-lookup"><span data-stu-id="4b84d-165">Azure AD Resource Limitations</span></span>

<span data-ttu-id="4b84d-166">Bestimmte Einschränkungen gelten für Azure AD-basierte Ressourcen (Benutzer, Gruppen) und können bei Überschreitung Fehler hervorrufen:</span><span class="sxs-lookup"><span data-stu-id="4b84d-166">Certain limits apply to Azure AD based resources (users, groups) and may generate errors when exceeded:</span></span>

* <span data-ttu-id="4b84d-167">Maximale Abonnementkontingente:</span><span class="sxs-lookup"><span data-stu-id="4b84d-167">Maximum subscription quotas:</span></span>

  * <span data-ttu-id="4b84d-168">Pro App: 50.000 Abonnements insgesamt</span><span class="sxs-lookup"><span data-stu-id="4b84d-168">Per App: 50,000 total subscriptions</span></span>
  * <span data-ttu-id="4b84d-169">Pro Mandant: 35 Abonnements insgesamt in allen Apps</span><span class="sxs-lookup"><span data-stu-id="4b84d-169">Per Tenant: 35 total subscriptions across all apps</span></span>
  * <span data-ttu-id="4b84d-170">Pro App und Mandanten kombiniert: 7 Abonnements insgesamt</span><span class="sxs-lookup"><span data-stu-id="4b84d-170">Per App and Tenant combination: 7 total subscriptions</span></span>

* <span data-ttu-id="4b84d-171">Azure AD B2C-Mandanten werden nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b84d-171">Azure AD B2C tenants are not supported</span></span>

* <span data-ttu-id="4b84d-172">Privatanwender-Konten werden nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b84d-172">Consumer account Users not supported</span></span>

## <a name="renewing-a-subscription"></a><span data-ttu-id="4b84d-173">Verlängern eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="4b84d-173">Renewing a subscription</span></span>

<span data-ttu-id="4b84d-p108">Der Kunde kann ein Abonnement mit einem bestimmten Ablaufdatum von bis zu drei Tagen ab dem Zeitpunkt der Anforderung verlängern. Die Eigenschaft „expirationDateTime“ ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4b84d-p108">The client can renew a subscription with a specific expiration date of up to three days from the time of request. The expirationDateTime property is required.</span></span>

### <a name="subscription-renewal-example"></a><span data-ttu-id="4b84d-176">Beispiel für eine Abonnementverlängerung</span><span class="sxs-lookup"><span data-stu-id="4b84d-176">Subscription renewal example</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id};
Content-Type: application/json
{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="4b84d-p109">Wenn der Vorgang erfolgreich war, gibt Microsoft Graph einen `200 OK`-Code und ein [subscription](../api-reference/v1.0/resources/subscription.md)-Objekt im Textkörper zurück. Das Abonnementobjekt enthält den neuen Wert füe „expirationDateTime“.</span><span class="sxs-lookup"><span data-stu-id="4b84d-p109">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](../api-reference/v1.0/resources/subscription.md) object in the body. The subscription object includes the new expirationDateTime value.</span></span> 

## <a name="deleting-a-subscription"></a><span data-ttu-id="4b84d-179">Löschen eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="4b84d-179">Deleting a subscription</span></span>

<span data-ttu-id="4b84d-180">Der Client kann den Erhalt von Benachrichtigungen stoppen, indem er das Abonnement anhand seiner ID löscht.</span><span class="sxs-lookup"><span data-stu-id="4b84d-180">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="4b84d-181">Wenn der Vorgang erfolgreich verläuft, gibt Microsoft Graph einen `204 No Content`-Code zurück.</span><span class="sxs-lookup"><span data-stu-id="4b84d-181">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="4b84d-182">Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="4b84d-182">Notifications</span></span>

<span data-ttu-id="4b84d-p110">Der Client beginnt, Benachrichtigungen zu erhalten, nachdem das Abonnement erstellt wurde. Microsoft Graph sendet eine POST-Anforderung an die Benachrichtigungs-URL, wenn Änderungen an der Ressource eintreten. Der Kunde erhält nur Benachrichtigungen gemäß dem angegebenen Änderungstyp, z. B. *created*.</span><span class="sxs-lookup"><span data-stu-id="4b84d-p110">The client starts receiving notifications after creating the subscription. Microsoft Graph sends a POST request to the notification URL when changes happen to the resource. The client only gets notifications according to the specified change type, such as *created*.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="4b84d-186">Benachrichtigungseigenschaften</span><span class="sxs-lookup"><span data-stu-id="4b84d-186">Notification properties</span></span>

<span data-ttu-id="4b84d-187">Das Benachrichtigungsobjekt verfügt über die folgenden Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="4b84d-187">The notification object has the following properties:</span></span>

* <span data-ttu-id="4b84d-188">subscriptionId: Die ID für das Abonnement, zu dem diese Benachrichtigung gehört.</span><span class="sxs-lookup"><span data-stu-id="4b84d-188">subscriptionId - The ID for the subscription to which this notification belongs.</span></span>
* <span data-ttu-id="4b84d-189">subscriptionExpirationDateTime: Die Ablaufzeit für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="4b84d-189">subscriptionExpirationDateTime - The expiration time for the subscription.</span></span>
* <span data-ttu-id="4b84d-190">clientState: Die clientState-Eigenschaft, die in der Abonnementanfrage angegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="4b84d-190">clientState - The clientState property specified in the subscription request.</span></span>
* <span data-ttu-id="4b84d-p111">changeType: Der Ereignistyp, der die Benachrichtigung ausgelöst hat. Z. B. *created* bei Erhalt einer E-Mail oder *updated*, wenn eine Nachricht als gelesen markiert wird.</span><span class="sxs-lookup"><span data-stu-id="4b84d-p111">changeType - The event type that caused the notification. For example, *created* on mail receive, or *updated* on marking a message read.</span></span>
* <span data-ttu-id="4b84d-193">resource: Der URI der Ressource relativ zu `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="4b84d-193">resource - The URI of the resource relative to `https://graph.microsoft.com`.</span></span> 
* <span data-ttu-id="4b84d-p112">resourceData: Das Objekt das von der abonnierten Ressource abhängt.  Z. B. für Outlook-Ressourcen:</span><span class="sxs-lookup"><span data-stu-id="4b84d-p112">resourceData - The object dependent on the resource being subscribed to.  For example, for Outlook resources:</span></span>
  * <span data-ttu-id="4b84d-196">@odata.type: Der OData-Entitätstyp in Microsoft Graph, der das dargestellte Objekt beschreibt.</span><span class="sxs-lookup"><span data-stu-id="4b84d-196">@odata.type - The OData entity type in Microsoft Graph that describes the represented object.</span></span>
  * <span data-ttu-id="4b84d-197">@odata.id: Der OData-Bezeichner des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4b84d-197">@odata.id - The OData identifier of the object.</span></span>
  * <span data-ttu-id="4b84d-198">@odata.etag: Das HTTP-Entitäts-Tag, das eine Version des Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="4b84d-198">@odata.etag - The HTTP entity tag that represents a version of the object.</span></span>
  * <span data-ttu-id="4b84d-199">Id: Der Bezeichner des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4b84d-199">id - The identifier of the object.</span></span>

> <span data-ttu-id="4b84d-p113">Hinweis: Der in „resourceData“ bereitgestellte Id-Wert ist zu dem Zeitpunkt gültig, zu dem die Benachrichtigung in die Warteschlange gestellt wurde. Bei einigen Aktionen, wie z. B. de Verschieben einer Nachricht in einen anderen Ordner, kann es zu einer Änderung der Ressourcen-ID kommen.</span><span class="sxs-lookup"><span data-stu-id="4b84d-p113">Note: The Id value provided in resourceData is valid at the time the notification was queued. Some actions, such as moving a message to another folder, may result in a resource's Id being changed.</span></span> 

### <a name="notification-example"></a><span data-ttu-id="4b84d-202">Benachrichtigungsbeispiel</span><span class="sxs-lookup"><span data-stu-id="4b84d-202">Notification example</span></span>

<span data-ttu-id="4b84d-203">Wenn der Benutzer eine E-Mail empfängt, sendet Microsoft Graph eine Benachrichtigung wie die folgende:</span><span class="sxs-lookup"><span data-stu-id="4b84d-203">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

``` json
{
  "value":[
  {
    "subscriptionId":"<subscription_guid>",
    "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
    "clientState":"SecretClientState",
    "changeType":"Created",
    "resource":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
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

<span data-ttu-id="4b84d-p114">Beachten Sie, dass das Wertobjekt eine Liste enthält. Wenn viele Benachrichtigungen in der Warteschlange stehen, sendet Microsoft Graph diese in einer einzigen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4b84d-p114">Note the value object contains a list. If there are many queued notifications, Microsoft Graph sends them in a single request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="4b84d-206">Verarbeiten der Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="4b84d-206">Processing the notification</span></span>

<span data-ttu-id="4b84d-p115">Sobald Ihre Anwendung Benachrichtigungen erhält, muss sie diese verarbeiten. Die folgenden Aufgaben müssen von der App mindestens durchgeführt werden, um eine Benachrichtigung zu verarbeiten:</span><span class="sxs-lookup"><span data-stu-id="4b84d-p115">After your application starts receiving notifications it must process them. The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="4b84d-p116">Überprüfen der `clientState`-Eigenschaft. Die Eigenschaft „clientState“ in der Benachrichtigung muss derjenigen übereinstimmen, die in der Abonnementanfrage übermittelt wurde.</span><span class="sxs-lookup"><span data-stu-id="4b84d-p116">Validate the `clientState` property. The clientState property in the notification must match the one submitted with the subscription request.</span></span>
  > <span data-ttu-id="4b84d-p117">Hinweis: Ist dies nicht der Fall, kann die Benachrichtigung nicht als gültig betrachtet werden. Prüfen Sie auch, woher die Benachrichtigung stammt, und ergreifen Sie die entsprechenden Maßnahmen.</span><span class="sxs-lookup"><span data-stu-id="4b84d-p117">Note: If this isn't true, you shouldn't consider this a valid notification. You should also investigate where the notification comes from and take appropriate action.</span></span>

2. <span data-ttu-id="4b84d-213">Aktualisieren Sie die Anwendung basierend auf Ihrer Geschäftslogik.</span><span class="sxs-lookup"><span data-stu-id="4b84d-213">Update your application based on your business logic.</span></span>

3. <span data-ttu-id="4b84d-p118">Senden Sie in Ihrer Antwort an Microsoft Graph einen `202 - Accepted` -Statuscode. Wenn Microsoft Graph keinen Code der Klasse 2xx erhält, wird versucht, die Benachrichtigung mehrmals erneut zu senden.</span><span class="sxs-lookup"><span data-stu-id="4b84d-p118">Send a `202 - Accepted` status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>
  > <span data-ttu-id="4b84d-216">Senden Sie auch dann einen `202 - Accepted`-Statuscode, wenn die Eigenschaft „clientState“ nicht mit derjenigen übereinstimmt, die in der Abonnementanfrage übermittelt wurde.</span><span class="sxs-lookup"><span data-stu-id="4b84d-216">You should send a `202 - Accepted` status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span>

<span data-ttu-id="4b84d-217">Wiederholen Sie den Vorgang für weitere Benachrichtigungen in der Anfrage.</span><span class="sxs-lookup"><span data-stu-id="4b84d-217">Repeat for other notifications in the request.</span></span>

## <a name="see-also"></a><span data-ttu-id="4b84d-218">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="4b84d-218">See also</span></span>

* [<span data-ttu-id="4b84d-219">Abonnementressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4b84d-219">Subscription resource type</span></span>](../api-reference/v1.0/resources/subscription.md)
* [<span data-ttu-id="4b84d-220">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="4b84d-220">Get subscription</span></span>](../api-reference/v1.0/api/subscription_get.md)
* [<span data-ttu-id="4b84d-221">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="4b84d-221">Create subscription</span></span>](../api-reference/v1.0/api/subscription_post_subscriptions.md)
* [<span data-ttu-id="4b84d-222">Microsoft Graph Webhooks-Beispiel für Node.js</span><span class="sxs-lookup"><span data-stu-id="4b84d-222">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="4b84d-223">Microsoft Graph Webhooks-Beispiel für ASP.NET</span><span class="sxs-lookup"><span data-stu-id="4b84d-223">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

[Kontakt]: ../api-reference/v1.0/resources/contact.md
[contact]: ../api-reference/v1.0/resources/contact.md
[Unterhaltung]: ../api-reference/v1.0/resources/conversation.md
[conversation]: ../api-reference/v1.0/resources/conversation.md
[Laufwerk]: ../api-reference/v1.0/resources/drive.md
[drive]: ../api-reference/v1.0/resources/drive.md
[Ereignis]: ../api-reference/v1.0/resources/event.md
[event]: ../api-reference/v1.0/resources/event.md
[Nachricht]: ../api-reference/v1.0/resources/message.md
[message]: ../api-reference/v1.0/resources/message.md
