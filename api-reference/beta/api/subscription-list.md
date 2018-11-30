---
title: Liste von Abonnements
description: " finden Sie die Szenarien unter Weitere Informationen."
ms.openlocfilehash: ad5e97a9b721a9e557e01dd4743b53a52c6dc8d7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065075"
---
# <a name="list-subscriptions"></a><span data-ttu-id="582be-103">Liste von Abonnements</span><span class="sxs-lookup"><span data-stu-id="582be-103">List subscriptions</span></span>

> <span data-ttu-id="582be-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="582be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="582be-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="582be-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="582be-106">Abrufen einer Liste der Webhook-Abonnements.</span><span class="sxs-lookup"><span data-stu-id="582be-106">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="582be-107">Der Inhalt der Antwort hängt von den Kontext, in dem die app anruft. finden Sie die Szenarien unter Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="582be-107">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="582be-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="582be-108">Permissions</span></span>

<span data-ttu-id="582be-109">Diese API unterstützt die folgenden berechtigungsbereiche. Weitere, einschließlich auswählen von Berechtigungen finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="582be-109">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="582be-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="582be-110">Permission type</span></span>  | <span data-ttu-id="582be-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="582be-111">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="582be-112">[Delegiert](/graph/auth-v2-user) (Arbeit oder Schule Konto)</span><span class="sxs-lookup"><span data-stu-id="582be-112">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="582be-113">Erforderliche Berechtigung zum [Erstellen von Abonnement](subscription-post-subscriptions.md) oder Subscription.Read.All (siehe unten).</span><span class="sxs-lookup"><span data-stu-id="582be-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="582be-114">[Delegiert](/graph/auth-v2-user) (Persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="582be-114">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="582be-115">Erforderliche Berechtigung zum [Erstellen von Abonnement](subscription-post-subscriptions.md) oder Subscription.Read.All (siehe unten).</span><span class="sxs-lookup"><span data-stu-id="582be-115">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="582be-116">Application</span><span class="sxs-lookup"><span data-stu-id="582be-116">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="582be-117">Erforderliche Berechtigung zum [Abonnement zu erstellen](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="582be-117">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="582be-118">Antwort Ergebnisse basieren auf dem Kontext der aufrufenden app.</span><span class="sxs-lookup"><span data-stu-id="582be-118">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="582be-119">Es folgt eine Zusammenfassung der gängigen Szenarien:</span><span class="sxs-lookup"><span data-stu-id="582be-119">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="582be-120">Grundlegende Szenarios</span><span class="sxs-lookup"><span data-stu-id="582be-120">Basic scenarios</span></span>

<span data-ttu-id="582be-121">In den meisten Fällen eine Anwendung Abonnements abrufen möchte, die ursprünglich für den aktuell angemeldeten Benutzer oder für alle Benutzer in das Verzeichnis (Arbeit/Schule Konten) erstellt.</span><span class="sxs-lookup"><span data-stu-id="582be-121">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="582be-122">Diese Szenarien ist keine speziellen Berechtigungen als die die app ursprünglich verwendet, um dessen Abonnements erstellen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="582be-122">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="582be-123">Kontext der aufrufenden app</span><span class="sxs-lookup"><span data-stu-id="582be-123">Context of the calling app</span></span> | <span data-ttu-id="582be-124">Antwort enthält</span><span class="sxs-lookup"><span data-stu-id="582be-124">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="582be-125">App ist im Namen des angemeldeten Benutzers (Delegierte Berechtigung) aufrufen.</span><span class="sxs-lookup"><span data-stu-id="582be-125">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="582be-126">- und -</span><span class="sxs-lookup"><span data-stu-id="582be-126">-and-</span></span><br/><span data-ttu-id="582be-127">App besitzt die ursprüngliche Berechtigung erforderlich, um [das Abonnement zu erstellen](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="582be-127">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="582be-128">Hinweis: Dies gilt für persönliche Microsoft-Konten und Arbeit/Schule Konten.</span><span class="sxs-lookup"><span data-stu-id="582be-128">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="582be-129">Abonnements durch **diese app** für den angemeldeten Benutzer nur erstellt.</span><span class="sxs-lookup"><span data-stu-id="582be-129">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="582be-130">App ist im Namen selbst (Anwendung die Berechtigung) aufrufen.</span><span class="sxs-lookup"><span data-stu-id="582be-130">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="582be-131">- und -</span><span class="sxs-lookup"><span data-stu-id="582be-131">-and-</span></span><br/><span data-ttu-id="582be-132">App besitzt die ursprüngliche Berechtigung erforderlich, um [das Abonnement zu erstellen](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="582be-132">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="582be-133">Hinweis: Dies gilt Arbeit/nur Konten Schule.</span><span class="sxs-lookup"><span data-stu-id="582be-133">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="582be-134">Abonnements, die **diese** App für sich selbst oder für jeden Benutzer in das Verzeichnis erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="582be-134">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="582be-135">Erweiterte Szenarien</span><span class="sxs-lookup"><span data-stu-id="582be-135">Advanced scenarios</span></span>

<span data-ttu-id="582be-136">In einigen Fällen eine app von anderen apps erstellt Abonnements abrufen möchte.</span><span class="sxs-lookup"><span data-stu-id="582be-136">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="582be-137">Beispielsweise möchte ein Benutzer alle Abonnements, die von einer beliebigen app in ihrem Auftrag erstellt.</span><span class="sxs-lookup"><span data-stu-id="582be-137">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="582be-138">Oder ein Administrator alle Abonnements aus allen apps in ihrem Verzeichnis finden Sie unter möchten.</span><span class="sxs-lookup"><span data-stu-id="582be-138">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="582be-139">Für solche Szenarien ist eine delegierte Berechtigung Subscription.Read.All erforderlich.</span><span class="sxs-lookup"><span data-stu-id="582be-139">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="582be-140">Kontext der aufrufenden app</span><span class="sxs-lookup"><span data-stu-id="582be-140">Context of the calling app</span></span> | <span data-ttu-id="582be-141">Antwort enthält</span><span class="sxs-lookup"><span data-stu-id="582be-141">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="582be-142">App ist im Namen des angemeldeten Benutzers (Delegierte Berechtigung) aufrufen.</span><span class="sxs-lookup"><span data-stu-id="582be-142">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="582be-143">*Der Benutzer ist ein nicht-Administrator*.</span><span class="sxs-lookup"><span data-stu-id="582be-143">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="582be-144">- und -</span><span class="sxs-lookup"><span data-stu-id="582be-144">-and-</span></span><br/><span data-ttu-id="582be-145">App verfügt über die Berechtigung Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="582be-145">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="582be-146">Hinweis: Dies gilt für persönliche Microsoft-Konten und Arbeit/Schule Konten.</span><span class="sxs-lookup"><span data-stu-id="582be-146">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="582be-147">Abonnements, die von **einer beliebigen app** nur für den angemeldeten Benutzer erstellt.</span><span class="sxs-lookup"><span data-stu-id="582be-147">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="582be-148">App ist im Namen des angemeldeten Benutzers (Delegierte Berechtigung) aufrufen.</span><span class="sxs-lookup"><span data-stu-id="582be-148">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="582be-149">*Der Benutzer ist ein Administrator*.</span><span class="sxs-lookup"><span data-stu-id="582be-149">*The user is an admin*.</span></span><br/><span data-ttu-id="582be-150">- und -</span><span class="sxs-lookup"><span data-stu-id="582be-150">-and-</span></span><br/><span data-ttu-id="582be-151">App verfügt über die Berechtigung Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="582be-151">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="582be-152">Hinweis: Dies gilt Arbeit/nur Konten Schule.</span><span class="sxs-lookup"><span data-stu-id="582be-152">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="582be-153">Abonnements, die von **einer beliebigen app** für **alle Benutzer** im Verzeichnis erstellt.</span><span class="sxs-lookup"><span data-stu-id="582be-153">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="582be-154">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="582be-154">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="582be-155">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="582be-155">Optional query parameters</span></span>

<span data-ttu-id="582be-156">Diese Methode unterstützt nicht die [OData-Abfrage-Parameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="582be-156">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="582be-157">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="582be-157">Request headers</span></span>

| <span data-ttu-id="582be-158">Name</span><span class="sxs-lookup"><span data-stu-id="582be-158">Name</span></span>       | <span data-ttu-id="582be-159">Typ</span><span class="sxs-lookup"><span data-stu-id="582be-159">Type</span></span> | <span data-ttu-id="582be-160">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="582be-160">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="582be-161">Authorization</span><span class="sxs-lookup"><span data-stu-id="582be-161">Authorization</span></span>  | <span data-ttu-id="582be-162">string</span><span class="sxs-lookup"><span data-stu-id="582be-162">string</span></span>  | <span data-ttu-id="582be-p108">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="582be-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="582be-165">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="582be-165">Request body</span></span>

<span data-ttu-id="582be-166">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="582be-166">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="582be-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="582be-167">Response</span></span>

<span data-ttu-id="582be-168">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste von Objekten im Antworttext [Abonnement](../resources/subscription.md) .</span><span class="sxs-lookup"><span data-stu-id="582be-168">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="582be-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="582be-169">Example</span></span>

##### <a name="request"></a><span data-ttu-id="582be-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="582be-170">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a><span data-ttu-id="582be-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="582be-171">Response</span></span>

<span data-ttu-id="582be-172">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="582be-172">Here is an example of the response.</span></span> <span data-ttu-id="582be-173">Hinweis: Die hier gezeigte Antwort der Kürze halber werden möglicherweise abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="582be-173">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="582be-174">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="582be-174">All of the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions",
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

<span data-ttu-id="582be-175">Wenn eine Anforderung mehrere Seiten mit Daten zurückgegeben, die Antwort enthält eine `@odata.nextLink` Eigenschaft zur einfacheren Verwaltung der Ergebnisse.</span><span class="sxs-lookup"><span data-stu-id="582be-175">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="582be-176">Finden Sie weitere Informationen finden Sie unter [Microsoft Graph Paging von Daten in Ihrer app](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="582be-176">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
