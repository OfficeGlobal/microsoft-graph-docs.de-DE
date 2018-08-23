# <a name="list-subscriptions"></a><span data-ttu-id="708de-101">Liste von Abonnements</span><span class="sxs-lookup"><span data-stu-id="708de-101">List subscriptions</span></span>

<span data-ttu-id="708de-102">Rufen Sie die Eigenschaften und Beziehungen von Webhook-Abonnements basierend auf der App-ID, dem Benutzer und der Rolle des Benutzers mit einem Mandanten ab.</span><span class="sxs-lookup"><span data-stu-id="708de-102">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="708de-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="708de-103">Permissions</span></span>

<span data-ttu-id="708de-104">Diese API unterstützt die folgenden Berechtigungsbereiche. Weitere Informationen, unter anderem dazu, wie Sie Berechtigungen auswählen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="708de-104">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="708de-105">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="708de-105">Permission type</span></span>  | <span data-ttu-id="708de-106">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="708de-106">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="708de-107">[Delegiert](../../../concepts/auth_v2_user.md)(Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="708de-107">Delegated (work or school account)</span></span> | <span data-ttu-id="708de-108">Rolle, die zum [Abonnement erstellen](subscription_get.md) oder für Subscriptions.Read.All  (siehe unten) erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="708de-108">Role required to [create subscription](subscription_get.md) or Subscriptions.Read.All (see below).</span></span> |
| <span data-ttu-id="708de-109">[Delegiert](../../../concepts/auth_v2_user.md) (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="708de-109">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="708de-110">Rolle, die zum [Abonnement erstellen](./subscription_get.md) oder für Subscriptions.Read.All  (siehe unten) erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="708de-110">Role required to [create subscription](./subscription_get.md) or Subscriptions.Read.All (see below).</span></span> |
| [<span data-ttu-id="708de-111">Anwendung</span><span class="sxs-lookup"><span data-stu-id="708de-111">Application</span></span>](../../../concepts/auth_v2_service.md) | <span data-ttu-id="708de-112">Rolle, die zum [Abonnement erstellen](./subscription_get.md) erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="708de-112">Role required to [create subscription](./subscription_get.md).</span></span> |

<span data-ttu-id="708de-113">Response-Ergebnisse basieren auf dem Kontext der aufrufenden App.</span><span class="sxs-lookup"><span data-stu-id="708de-113">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="708de-114">Es folgt eine Zusammenfassung der gängigen Szenarien:</span><span class="sxs-lookup"><span data-stu-id="708de-114">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="708de-115">Grundlegende Szenarios</span><span class="sxs-lookup"><span data-stu-id="708de-115">Basic planning scenarios</span></span>

<span data-ttu-id="708de-116">In der Regel möchte eine Anwendung Abonnements abrufen, die sie ursprünglich für den derzeit angemeldeten Benutzer oder für alle Benutzer im Verzeichnis (Geschäfts-/Schul-/Uni-Konten) erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="708de-116">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="708de-117">Für diese Szenarien sind keine besonderen Berechtigungen erforderlich, die über diejenigen hinausgehen, die ursprünglich von der App zum Erstellen der Abonnements verwendet wurden.</span><span class="sxs-lookup"><span data-stu-id="708de-117">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="708de-118">Kontext der aufrufenden App</span><span class="sxs-lookup"><span data-stu-id="708de-118">Context of the calling app</span></span> | <span data-ttu-id="708de-119">Antwort enthält</span><span class="sxs-lookup"><span data-stu-id="708de-119">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="708de-120">App ruft im Namen des angemeldeten Benutzers auf (delegierte Berechtigung).</span><span class="sxs-lookup"><span data-stu-id="708de-120">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="708de-121">-und-</span><span class="sxs-lookup"><span data-stu-id="708de-121">and</span></span><br/><span data-ttu-id="708de-122">App verfügt über die ursprüngliche Berechtigung, die zum [Abonnement erstellen](subscription_post_subscriptions.md)erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="708de-122">App has the original permission required to [create the subscription](subscription_post_subscriptions.md).</span></span><br/><br/><span data-ttu-id="708de-123">Hinweis: Dies gilt für persönliche Microsoft-Konten und Geschäfts-/Schul-/Uni-Konten.</span><span class="sxs-lookup"><span data-stu-id="708de-123">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="708de-124">Abonnements, die durch **diese App** nur für den angemeldeten Benutzer erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="708de-124">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="708de-125">App ruft eigenständig auf (Anwendungsberechtigung).</span><span class="sxs-lookup"><span data-stu-id="708de-125">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="708de-126">-und-</span><span class="sxs-lookup"><span data-stu-id="708de-126">and</span></span><br/><span data-ttu-id="708de-127">App verfügt über die ursprüngliche Berechtigung, die zum [Abonnement erstellen](subscription_post_subscriptions.md)erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="708de-127">App has the original permission required to [create the subscription](subscription_post_subscriptions.md).</span></span><br/><br/><span data-ttu-id="708de-128">Hinweis: Dies gilt nur für Geschäfts-/Schul-/Uni-Konten.</span><span class="sxs-lookup"><span data-stu-id="708de-128">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="708de-129">Abonnements, die durch **diese App** für sich oder für einen beliebigen Benutzer im Verzeichnis erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="708de-129">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="708de-130">Erweiterte Szenarien</span><span class="sxs-lookup"><span data-stu-id="708de-130">Advanced save scenarios</span></span>

<span data-ttu-id="708de-131">In einigen Fällen möchte eine App Abonnements abrufen, die von anderen Apps erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="708de-131">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="708de-132">Beispielsweise möchte ein Benutzer alle Abonnements anzeigen, die von einer beliebigen App eigenständig erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="708de-132">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="708de-133">Oder ein Administrator möchte möglicherweise alle Abonnements von allen Apps in deren Verzeichnis sehen.</span><span class="sxs-lookup"><span data-stu-id="708de-133">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="708de-134">Für solche Szenarien ist eine delegierte Berechtigung Subscription.Read.All erforderlich.</span><span class="sxs-lookup"><span data-stu-id="708de-134">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="708de-135">Kontext der aufrufenden App</span><span class="sxs-lookup"><span data-stu-id="708de-135">Context of the calling app</span></span> | <span data-ttu-id="708de-136">Antwort enthält</span><span class="sxs-lookup"><span data-stu-id="708de-136">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="708de-137">App ruft im Namen des angemeldeten Benutzers auf (delegierte Berechtigung).</span><span class="sxs-lookup"><span data-stu-id="708de-137">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="708de-138">*Der Benutzer ist ein Nicht-Administrator*.</span><span class="sxs-lookup"><span data-stu-id="708de-138">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="708de-139">-und-</span><span class="sxs-lookup"><span data-stu-id="708de-139">and</span></span><br/><span data-ttu-id="708de-140">App verfügt über die Berechtigung Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="708de-140">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="708de-141">Hinweis: Dies gilt für persönliche Microsoft-Konten und Geschäfts-/Schul-/Uni-Konten.</span><span class="sxs-lookup"><span data-stu-id="708de-141">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="708de-142">Abonnements, die durch **eine beliebige App** nur für den angemeldeten Benutzer erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="708de-142">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="708de-143">App ruft im Namen des angemeldeten Benutzers auf (delegierte Berechtigung).</span><span class="sxs-lookup"><span data-stu-id="708de-143">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="708de-144">*Der Benutzer ist ein Administrator*.</span><span class="sxs-lookup"><span data-stu-id="708de-144">*The user is an admin*.</span></span><br/><span data-ttu-id="708de-145">-und-</span><span class="sxs-lookup"><span data-stu-id="708de-145">and</span></span><br/><span data-ttu-id="708de-146">App verfügt über die Berechtigung Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="708de-146">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="708de-147">Hinweis: Dies gilt nur für Geschäfts-/Schul-/Uni-Konten.</span><span class="sxs-lookup"><span data-stu-id="708de-147">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="708de-148">Abonnements, die durch **eine beliebige App** für **einen beliebigen Benutzer**im Verzeichnis erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="708de-148">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="708de-149">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="708de-149">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="708de-150">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="708de-150">Optional query parameters</span></span>

<span data-ttu-id="708de-151">Diese Methode unterstützt nicht die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="708de-151">This method does not support the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="708de-152">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="708de-152">Request headers</span></span>

| <span data-ttu-id="708de-153">Name</span><span class="sxs-lookup"><span data-stu-id="708de-153">Name</span></span>       | <span data-ttu-id="708de-154">Typ</span><span class="sxs-lookup"><span data-stu-id="708de-154">Type</span></span> | <span data-ttu-id="708de-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="708de-155">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="708de-156">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="708de-156">Authorization</span></span>  | <span data-ttu-id="708de-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="708de-157">string</span></span>  | <span data-ttu-id="708de-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="708de-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="708de-160">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="708de-160">Request body</span></span>

<span data-ttu-id="708de-161">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="708de-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="708de-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="708de-162">Response</span></span>

<span data-ttu-id="708de-163">Bei Erfolg gibt diese Methode im Antworttext einen `200 OK` Antwortcode und eine Liste von [Abonnement](../resources/subscription.md) .-Objekten zurück.</span><span class="sxs-lookup"><span data-stu-id="708de-163">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="708de-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="708de-164">Example</span></span>

##### <a name="request"></a><span data-ttu-id="708de-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="708de-165">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="708de-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="708de-166">Response</span></span>

<span data-ttu-id="708de-167">Es folgt das Beispiel einer Antwort.</span><span class="sxs-lookup"><span data-stu-id="708de-167">Here's an excerpt of the response:</span></span>  <span data-ttu-id="708de-168">Bitte beachten Sie, dass diese aus Platzgründen gekürzt sein kann.</span><span class="sxs-lookup"><span data-stu-id="708de-168">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="708de-169">Alle unterstützten Eigenschaften, die für die Anforderung und den Kontext des Aufrufs geeignet sind, werden von einem tatsächlichen Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="708de-169">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 586

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions",
  "value": [
    {
      "id": "0fc0d6db-0073-42e5-a186-853da75fb308",
      "resource": "Users",
      "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
      "changeType": "updated,deleted",
      "clientState": null,
      "notificationUrl": "https://webhookappexample.azurewebsites.net/api/notifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

<span data-ttu-id="708de-170">Gibt eine Anforderung mehrere Seiten mit Daten zurück, enthält die Antwort eine `@odata.nextLink` -Eigenschaft zur einfacheren Verwaltung der Ergebnisse.</span><span class="sxs-lookup"><span data-stu-id="708de-170">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="708de-171">Weitere Informationen finden Sie unter [Paging der Microsoft Graph-Daten in Ihrer App](../../../concepts/paging.md).</span><span class="sxs-lookup"><span data-stu-id="708de-171">To learn more, see [Paging Microsoft Graph data in your app](../../../concepts/paging.md).</span></span>
