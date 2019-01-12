---
title: Liste von Abonnements
description: Abrufen der Eigenschaften und Beziehungen zwischen Webhook Abonnements, basierend auf der app-ID, die Benutzer und die Rolle des Benutzers mit einem Mandanten.
localization_priority: Priority
author: piotrci
ms.openlocfilehash: c2e9446721f4390341c33f8b976893e4b1ab14be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972936"
---
# <a name="list-subscriptions"></a><span data-ttu-id="38ada-103">Liste von Abonnements</span><span class="sxs-lookup"><span data-stu-id="38ada-103">List subscriptions</span></span>

<span data-ttu-id="38ada-104">Abrufen der Eigenschaften und Beziehungen zwischen Webhook Abonnements, basierend auf der app-ID, die Benutzer und die Rolle des Benutzers mit einem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="38ada-104">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="38ada-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="38ada-105">Permissions</span></span>

<span data-ttu-id="38ada-106">Diese API unterstützt die folgenden berechtigungsbereiche. Weitere, einschließlich auswählen von Berechtigungen finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38ada-106">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38ada-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38ada-107">Permission type</span></span>  | <span data-ttu-id="38ada-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38ada-108">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="38ada-109">[Delegierte Berechtigung](/graph/auth-v2-user) (Arbeit oder Schule Konto)</span><span class="sxs-lookup"><span data-stu-id="38ada-109">[Delegated permission](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="38ada-110">Rolle, die zum [Erstellen von Abonnement](subscription-post-subscriptions.md) oder Subscription.Read.All (siehe unten) erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38ada-110">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="38ada-111">[Delegierte Berechtigung](/graph/auth-v2-user) (Persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38ada-111">[Delegated permission](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="38ada-112">Rolle, die zum [Erstellen von Abonnement](subscription-post-subscriptions.md) oder Subscription.Read.All (siehe unten) erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38ada-112">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="38ada-113">Anwendung die Berechtigung</span><span class="sxs-lookup"><span data-stu-id="38ada-113">Application permission</span></span>](/graph/auth-v2-service) | <span data-ttu-id="38ada-114">Rolle erforderlich, um das [Abonnement zu erstellen](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="38ada-114">Role required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="38ada-115">Antwort Ergebnisse basieren auf dem Kontext der aufrufenden app.</span><span class="sxs-lookup"><span data-stu-id="38ada-115">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="38ada-116">Es folgt eine Zusammenfassung der gängigen Szenarien:</span><span class="sxs-lookup"><span data-stu-id="38ada-116">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="38ada-117">Grundlegende Szenarios</span><span class="sxs-lookup"><span data-stu-id="38ada-117">Basic scenarios</span></span>

<span data-ttu-id="38ada-118">In den meisten Fällen eine Anwendung Abonnements abrufen möchte, die ursprünglich für den aktuell angemeldeten Benutzer oder für alle Benutzer in das Verzeichnis (Arbeit/Schule Konten) erstellt.</span><span class="sxs-lookup"><span data-stu-id="38ada-118">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="38ada-119">Diese Szenarien ist keine speziellen Berechtigungen als die die app ursprünglich verwendet, um dessen Abonnements erstellen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38ada-119">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="38ada-120">Kontext der aufrufenden app</span><span class="sxs-lookup"><span data-stu-id="38ada-120">Context of the calling app</span></span> | <span data-ttu-id="38ada-121">Antwort enthält</span><span class="sxs-lookup"><span data-stu-id="38ada-121">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="38ada-122">App ist im Namen des angemeldeten Benutzers (Delegierte Berechtigung) aufrufen.</span><span class="sxs-lookup"><span data-stu-id="38ada-122">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="38ada-123">- und -</span><span class="sxs-lookup"><span data-stu-id="38ada-123">-and-</span></span><br/><span data-ttu-id="38ada-124">App besitzt die ursprüngliche Berechtigung erforderlich, um [das Abonnement zu erstellen](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="38ada-124">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="38ada-125">Hinweis: Dies gilt für persönliche Microsoft-Konten und Arbeit/Schule Konten.</span><span class="sxs-lookup"><span data-stu-id="38ada-125">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="38ada-126">Abonnements durch **diese app** für den angemeldeten Benutzer nur erstellt.</span><span class="sxs-lookup"><span data-stu-id="38ada-126">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="38ada-127">App ist im Namen selbst (Anwendung die Berechtigung) aufrufen.</span><span class="sxs-lookup"><span data-stu-id="38ada-127">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="38ada-128">- und -</span><span class="sxs-lookup"><span data-stu-id="38ada-128">-and-</span></span><br/><span data-ttu-id="38ada-129">App besitzt die ursprüngliche Berechtigung erforderlich, um [das Abonnement zu erstellen](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="38ada-129">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="38ada-130">Hinweis: Dies gilt Arbeit/nur Konten Schule.</span><span class="sxs-lookup"><span data-stu-id="38ada-130">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="38ada-131">Abonnements, die **diese** App für sich selbst oder für jeden Benutzer in das Verzeichnis erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="38ada-131">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="38ada-132">Erweiterte Szenarien</span><span class="sxs-lookup"><span data-stu-id="38ada-132">Advanced scenarios</span></span>

<span data-ttu-id="38ada-133">In einigen Fällen eine app von anderen apps erstellt Abonnements abrufen möchte.</span><span class="sxs-lookup"><span data-stu-id="38ada-133">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="38ada-134">Beispielsweise möchte ein Benutzer alle Abonnements, die von einer beliebigen app in ihrem Auftrag erstellt.</span><span class="sxs-lookup"><span data-stu-id="38ada-134">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="38ada-135">Oder ein Administrator alle Abonnements aus allen apps in ihrem Verzeichnis finden Sie unter möchten.</span><span class="sxs-lookup"><span data-stu-id="38ada-135">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="38ada-136">Für solche Szenarien ist eine delegierte Berechtigung Subscription.Read.All erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38ada-136">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="38ada-137">Kontext der aufrufenden app</span><span class="sxs-lookup"><span data-stu-id="38ada-137">Context of the calling app</span></span> | <span data-ttu-id="38ada-138">Antwort enthält</span><span class="sxs-lookup"><span data-stu-id="38ada-138">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="38ada-139">App ist im Namen des angemeldeten Benutzers (Delegierte Berechtigung) aufrufen.</span><span class="sxs-lookup"><span data-stu-id="38ada-139">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="38ada-140">*Der Benutzer ist ein nicht-Administrator*.</span><span class="sxs-lookup"><span data-stu-id="38ada-140">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="38ada-141">- und -</span><span class="sxs-lookup"><span data-stu-id="38ada-141">-and-</span></span><br/><span data-ttu-id="38ada-142">App verfügt über die Berechtigung Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="38ada-142">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="38ada-143">Hinweis: Dies gilt für persönliche Microsoft-Konten und Arbeit/Schule Konten.</span><span class="sxs-lookup"><span data-stu-id="38ada-143">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="38ada-144">Abonnements, die von **einer beliebigen app** nur für den angemeldeten Benutzer erstellt.</span><span class="sxs-lookup"><span data-stu-id="38ada-144">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="38ada-145">App ist im Namen des angemeldeten Benutzers (Delegierte Berechtigung) aufrufen.</span><span class="sxs-lookup"><span data-stu-id="38ada-145">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="38ada-146">*Der Benutzer ist ein Administrator*.</span><span class="sxs-lookup"><span data-stu-id="38ada-146">*The user is an admin*.</span></span><br/><span data-ttu-id="38ada-147">- und -</span><span class="sxs-lookup"><span data-stu-id="38ada-147">-and-</span></span><br/><span data-ttu-id="38ada-148">App verfügt über die Berechtigung Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="38ada-148">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="38ada-149">Hinweis: Dies gilt Arbeit/nur Konten Schule.</span><span class="sxs-lookup"><span data-stu-id="38ada-149">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="38ada-150">Abonnements, die von **einer beliebigen app** für **alle Benutzer** im Verzeichnis erstellt.</span><span class="sxs-lookup"><span data-stu-id="38ada-150">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38ada-151">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38ada-151">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38ada-152">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="38ada-152">Optional query parameters</span></span>

<span data-ttu-id="38ada-153">Diese Methode unterstützt nicht die [OData-Abfrage-Parameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="38ada-153">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38ada-154">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38ada-154">Request headers</span></span>

| <span data-ttu-id="38ada-155">Name</span><span class="sxs-lookup"><span data-stu-id="38ada-155">Name</span></span>       | <span data-ttu-id="38ada-156">Typ</span><span class="sxs-lookup"><span data-stu-id="38ada-156">Type</span></span> | <span data-ttu-id="38ada-157">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38ada-157">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="38ada-158">Authorization</span><span class="sxs-lookup"><span data-stu-id="38ada-158">Authorization</span></span>  | <span data-ttu-id="38ada-159">string</span><span class="sxs-lookup"><span data-stu-id="38ada-159">string</span></span>  | <span data-ttu-id="38ada-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38ada-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38ada-162">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38ada-162">Request body</span></span>

<span data-ttu-id="38ada-163">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="38ada-163">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38ada-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="38ada-164">Response</span></span>

<span data-ttu-id="38ada-165">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste von Objekten im Antworttext [Abonnement](../resources/subscription.md) .</span><span class="sxs-lookup"><span data-stu-id="38ada-165">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38ada-166">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38ada-166">Example</span></span>

##### <a name="request"></a><span data-ttu-id="38ada-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38ada-167">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="38ada-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="38ada-168">Response</span></span>

<span data-ttu-id="38ada-169">Es folgt eine ein Beispiel für die Antwort.</span><span class="sxs-lookup"><span data-stu-id="38ada-169">Here's an an example of the response.</span></span>  <span data-ttu-id="38ada-170">Beachten Sie, dass der Kürze halber abgeschnitten sein können.</span><span class="sxs-lookup"><span data-stu-id="38ada-170">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="38ada-171">Alle unterstützten Eigenschaften für die Anforderung und der aufrufende Kontext aus einem tatsächlichen Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38ada-171">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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

<span data-ttu-id="38ada-172">Wenn eine Anforderung mehrere Seiten mit Daten zurückgegeben, die Antwort enthält eine `@odata.nextLink` Eigenschaft zur einfacheren Verwaltung der Ergebnisse.</span><span class="sxs-lookup"><span data-stu-id="38ada-172">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="38ada-173">Finden Sie weitere Informationen finden Sie unter [Microsoft Graph Paging von Daten in Ihrer app](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="38ada-173">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
