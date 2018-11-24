# <a name="list-subscriptions"></a><span data-ttu-id="355ef-101">Liste von Abonnements</span><span class="sxs-lookup"><span data-stu-id="355ef-101">List subscriptions</span></span>

<span data-ttu-id="355ef-102">Abrufen der Eigenschaften und Beziehungen zwischen Webhook Abonnements, basierend auf der app-ID, die Benutzer und die Rolle des Benutzers mit einem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="355ef-102">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="355ef-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="355ef-103">Permissions</span></span>

<span data-ttu-id="355ef-104">Diese API unterstützt die folgenden berechtigungsbereiche. Weitere, einschließlich auswählen von Berechtigungen finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="355ef-104">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="355ef-105">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="355ef-105">Permission type</span></span>  | <span data-ttu-id="355ef-106">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="355ef-106">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="355ef-107">[Delegierte Berechtigung](../../../concepts/auth_v2_user.md) (Arbeit oder Schule Konto)</span><span class="sxs-lookup"><span data-stu-id="355ef-107">[Delegated permission](../../../concepts/auth_v2_user.md) (work or school account)</span></span> | <span data-ttu-id="355ef-108">Rolle, die zum [Erstellen von Abonnement](subscription_post_subscriptions.md) oder Subscription.Read.All (siehe unten) erforderlich.</span><span class="sxs-lookup"><span data-stu-id="355ef-108">Role required to [create subscription](subscription_post_subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="355ef-109">[Delegierte Berechtigung](../../../concepts/auth_v2_user.md) (Persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="355ef-109">[Delegated permission](../../../concepts/auth_v2_user.md) (personal Microsoft account)</span></span> | <span data-ttu-id="355ef-110">Rolle, die zum [Erstellen von Abonnement](subscription_post_subscriptions.md) oder Subscription.Read.All (siehe unten) erforderlich.</span><span class="sxs-lookup"><span data-stu-id="355ef-110">Role required to [create subscription](subscription_post_subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="355ef-111">Anwendung die Berechtigung</span><span class="sxs-lookup"><span data-stu-id="355ef-111">Application permission</span></span>](../../../concepts/auth_v2_service.md) | <span data-ttu-id="355ef-112">Rolle erforderlich, um das [Abonnement zu erstellen](subscription_post_subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="355ef-112">Role required to [create subscription](subscription_post_subscriptions.md).</span></span> |

<span data-ttu-id="355ef-113">Antwort Ergebnisse basieren auf dem Kontext der aufrufenden app.</span><span class="sxs-lookup"><span data-stu-id="355ef-113">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="355ef-114">Es folgt eine Zusammenfassung der gängigen Szenarien:</span><span class="sxs-lookup"><span data-stu-id="355ef-114">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="355ef-115">Grundlegende Szenarios</span><span class="sxs-lookup"><span data-stu-id="355ef-115">Basic scenarios</span></span>

<span data-ttu-id="355ef-116">In den meisten Fällen eine Anwendung Abonnements abrufen möchte, die ursprünglich für den aktuell angemeldeten Benutzer oder für alle Benutzer in das Verzeichnis (Arbeit/Schule Konten) erstellt.</span><span class="sxs-lookup"><span data-stu-id="355ef-116">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="355ef-117">Diese Szenarien ist keine speziellen Berechtigungen als die die app ursprünglich verwendet, um dessen Abonnements erstellen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="355ef-117">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="355ef-118">Kontext der aufrufenden app</span><span class="sxs-lookup"><span data-stu-id="355ef-118">Context of the calling app</span></span> | <span data-ttu-id="355ef-119">Antwort enthält</span><span class="sxs-lookup"><span data-stu-id="355ef-119">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="355ef-120">App ist im Namen des angemeldeten Benutzers (Delegierte Berechtigung) aufrufen.</span><span class="sxs-lookup"><span data-stu-id="355ef-120">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="355ef-121">- und -</span><span class="sxs-lookup"><span data-stu-id="355ef-121">-and-</span></span><br/><span data-ttu-id="355ef-122">App besitzt die ursprüngliche Berechtigung erforderlich, um [das Abonnement zu erstellen](subscription_post_subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="355ef-122">App has the original permission required to [create the subscription](subscription_post_subscriptions.md).</span></span><br/><br/><span data-ttu-id="355ef-123">Hinweis: Dies gilt für persönliche Microsoft-Konten und Arbeit/Schule Konten.</span><span class="sxs-lookup"><span data-stu-id="355ef-123">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="355ef-124">Abonnements durch **diese app** für den angemeldeten Benutzer nur erstellt.</span><span class="sxs-lookup"><span data-stu-id="355ef-124">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="355ef-125">App ist im Namen selbst (Anwendung die Berechtigung) aufrufen.</span><span class="sxs-lookup"><span data-stu-id="355ef-125">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="355ef-126">- und -</span><span class="sxs-lookup"><span data-stu-id="355ef-126">-and-</span></span><br/><span data-ttu-id="355ef-127">App besitzt die ursprüngliche Berechtigung erforderlich, um [das Abonnement zu erstellen](subscription_post_subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="355ef-127">App has the original permission required to [create the subscription](subscription_post_subscriptions.md).</span></span><br/><br/><span data-ttu-id="355ef-128">Hinweis: Dies gilt Arbeit/nur Konten Schule.</span><span class="sxs-lookup"><span data-stu-id="355ef-128">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="355ef-129">Abonnements, die **diese** App für sich selbst oder für jeden Benutzer in das Verzeichnis erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="355ef-129">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="355ef-130">Erweiterte Szenarien</span><span class="sxs-lookup"><span data-stu-id="355ef-130">Advanced scenarios</span></span>

<span data-ttu-id="355ef-131">In einigen Fällen eine app von anderen apps erstellt Abonnements abrufen möchte.</span><span class="sxs-lookup"><span data-stu-id="355ef-131">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="355ef-132">Beispielsweise möchte ein Benutzer alle Abonnements, die von einer beliebigen app in ihrem Auftrag erstellt.</span><span class="sxs-lookup"><span data-stu-id="355ef-132">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="355ef-133">Oder ein Administrator alle Abonnements aus allen apps in ihrem Verzeichnis finden Sie unter möchten.</span><span class="sxs-lookup"><span data-stu-id="355ef-133">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="355ef-134">Für solche Szenarien ist eine delegierte Berechtigung Subscription.Read.All erforderlich.</span><span class="sxs-lookup"><span data-stu-id="355ef-134">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="355ef-135">Kontext der aufrufenden app</span><span class="sxs-lookup"><span data-stu-id="355ef-135">Context of the calling app</span></span> | <span data-ttu-id="355ef-136">Antwort enthält</span><span class="sxs-lookup"><span data-stu-id="355ef-136">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="355ef-137">App ist im Namen des angemeldeten Benutzers (Delegierte Berechtigung) aufrufen.</span><span class="sxs-lookup"><span data-stu-id="355ef-137">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="355ef-138">*Der Benutzer ist ein nicht-Administrator*.</span><span class="sxs-lookup"><span data-stu-id="355ef-138">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="355ef-139">- und -</span><span class="sxs-lookup"><span data-stu-id="355ef-139">-and-</span></span><br/><span data-ttu-id="355ef-140">App verfügt über die Berechtigung Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="355ef-140">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="355ef-141">Hinweis: Dies gilt für persönliche Microsoft-Konten und Arbeit/Schule Konten.</span><span class="sxs-lookup"><span data-stu-id="355ef-141">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="355ef-142">Abonnements, die von **einer beliebigen app** nur für den angemeldeten Benutzer erstellt.</span><span class="sxs-lookup"><span data-stu-id="355ef-142">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="355ef-143">App ist im Namen des angemeldeten Benutzers (Delegierte Berechtigung) aufrufen.</span><span class="sxs-lookup"><span data-stu-id="355ef-143">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="355ef-144">*Der Benutzer ist ein Administrator*.</span><span class="sxs-lookup"><span data-stu-id="355ef-144">*The user is an admin*.</span></span><br/><span data-ttu-id="355ef-145">- und -</span><span class="sxs-lookup"><span data-stu-id="355ef-145">-and-</span></span><br/><span data-ttu-id="355ef-146">App verfügt über die Berechtigung Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="355ef-146">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="355ef-147">Hinweis: Dies gilt Arbeit/nur Konten Schule.</span><span class="sxs-lookup"><span data-stu-id="355ef-147">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="355ef-148">Abonnements, die von **einer beliebigen app** für **alle Benutzer** im Verzeichnis erstellt.</span><span class="sxs-lookup"><span data-stu-id="355ef-148">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="355ef-149">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="355ef-149">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="355ef-150">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="355ef-150">Optional query parameters</span></span>

<span data-ttu-id="355ef-151">Diese Methode unterstützt nicht die [OData-Abfrage-Parameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="355ef-151">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="355ef-152">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="355ef-152">Request headers</span></span>

| <span data-ttu-id="355ef-153">Name</span><span class="sxs-lookup"><span data-stu-id="355ef-153">Name</span></span>       | <span data-ttu-id="355ef-154">Typ</span><span class="sxs-lookup"><span data-stu-id="355ef-154">Type</span></span> | <span data-ttu-id="355ef-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="355ef-155">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="355ef-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="355ef-156">Authorization</span></span>  | <span data-ttu-id="355ef-157">string</span><span class="sxs-lookup"><span data-stu-id="355ef-157">string</span></span>  | <span data-ttu-id="355ef-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="355ef-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="355ef-160">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="355ef-160">Request body</span></span>

<span data-ttu-id="355ef-161">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="355ef-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="355ef-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="355ef-162">Response</span></span>

<span data-ttu-id="355ef-163">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste von Objekten im Antworttext [Abonnement](../resources/subscription.md) .</span><span class="sxs-lookup"><span data-stu-id="355ef-163">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="355ef-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="355ef-164">Example</span></span>

##### <a name="request"></a><span data-ttu-id="355ef-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="355ef-165">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="355ef-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="355ef-166">Response</span></span>

<span data-ttu-id="355ef-167">Es folgt eine ein Beispiel für die Antwort.</span><span class="sxs-lookup"><span data-stu-id="355ef-167">Here's an an example of the response.</span></span>  <span data-ttu-id="355ef-168">Beachten Sie, dass der Kürze halber abgeschnitten sein können.</span><span class="sxs-lookup"><span data-stu-id="355ef-168">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="355ef-169">Alle unterstützten Eigenschaften für die Anforderung und der aufrufende Kontext aus einem tatsächlichen Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="355ef-169">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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

<span data-ttu-id="355ef-170">Wenn eine Anforderung mehrere Seiten mit Daten zurückgegeben, die Antwort enthält eine `@odata.nextLink` Eigenschaft zur einfacheren Verwaltung der Ergebnisse.</span><span class="sxs-lookup"><span data-stu-id="355ef-170">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="355ef-171">Finden Sie weitere Informationen finden Sie unter [Microsoft Graph Paging von Daten in Ihrer app](../../../concepts/paging.md).</span><span class="sxs-lookup"><span data-stu-id="355ef-171">To learn more, see [Paging Microsoft Graph data in your app](../../../concepts/paging.md).</span></span>
