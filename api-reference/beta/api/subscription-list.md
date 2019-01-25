---
title: Liste von Abonnements
description: " finden Sie die Szenarien unter Weitere Informationen."
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 20aad712bc49f91bec58a67c0c66ef76bf4653e2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510981"
---
# <a name="list-subscriptions"></a><span data-ttu-id="0fb1f-103">Liste von Abonnements</span><span class="sxs-lookup"><span data-stu-id="0fb1f-103">List subscriptions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fb1f-104">Abrufen einer Liste der Webhook-Abonnements.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-104">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="0fb1f-105">Der Inhalt der Antwort hängt von den Kontext, in dem die app anruft. finden Sie die Szenarien unter Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-105">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fb1f-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0fb1f-106">Permissions</span></span>

<span data-ttu-id="0fb1f-107">Diese API unterstützt die folgenden berechtigungsbereiche. Weitere, einschließlich auswählen von Berechtigungen finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fb1f-107">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0fb1f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0fb1f-108">Permission type</span></span>  | <span data-ttu-id="0fb1f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0fb1f-109">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="0fb1f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0fb1f-110">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="0fb1f-111">Erforderliche Berechtigung zum [Erstellen von Abonnement](subscription-post-subscriptions.md) oder Subscription.Read.All (siehe unten).</span><span class="sxs-lookup"><span data-stu-id="0fb1f-111">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="0fb1f-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0fb1f-112">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="0fb1f-113">Erforderliche Berechtigung zum [Erstellen von Abonnement](subscription-post-subscriptions.md) oder Subscription.Read.All (siehe unten).</span><span class="sxs-lookup"><span data-stu-id="0fb1f-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="0fb1f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0fb1f-114">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="0fb1f-115">Erforderliche Berechtigung zum [Abonnement zu erstellen](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="0fb1f-115">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="0fb1f-116">Antwort Ergebnisse basieren auf dem Kontext der aufrufenden app.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-116">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="0fb1f-117">Es folgt eine Zusammenfassung der gängigen Szenarien:</span><span class="sxs-lookup"><span data-stu-id="0fb1f-117">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="0fb1f-118">Grundlegende Szenarios</span><span class="sxs-lookup"><span data-stu-id="0fb1f-118">Basic scenarios</span></span>

<span data-ttu-id="0fb1f-119">In den meisten Fällen eine Anwendung Abonnements abrufen möchte, die ursprünglich für den aktuell angemeldeten Benutzer oder für alle Benutzer in das Verzeichnis (Arbeit/Schule Konten) erstellt.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-119">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="0fb1f-120">Diese Szenarien ist keine speziellen Berechtigungen als die die app ursprünglich verwendet, um dessen Abonnements erstellen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-120">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="0fb1f-121">Kontext der aufrufenden app</span><span class="sxs-lookup"><span data-stu-id="0fb1f-121">Context of the calling app</span></span> | <span data-ttu-id="0fb1f-122">Antwort enthält</span><span class="sxs-lookup"><span data-stu-id="0fb1f-122">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="0fb1f-123">App ist im Namen des angemeldeten Benutzers (Delegierte Berechtigung) aufrufen.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-123">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="0fb1f-124">"AND"</span><span class="sxs-lookup"><span data-stu-id="0fb1f-124">-and-</span></span><br/><span data-ttu-id="0fb1f-125">App besitzt die ursprüngliche Berechtigung erforderlich, um [das Abonnement zu erstellen](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="0fb1f-125">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="0fb1f-126">Hinweis: Dies gilt für persönliche Microsoft-Konten und Arbeit/Schule Konten.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-126">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="0fb1f-127">Abonnements durch **diese app** für den angemeldeten Benutzer nur erstellt.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-127">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="0fb1f-128">App ist im Namen selbst (Anwendung die Berechtigung) aufrufen.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-128">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="0fb1f-129">"AND"</span><span class="sxs-lookup"><span data-stu-id="0fb1f-129">-and-</span></span><br/><span data-ttu-id="0fb1f-130">App besitzt die ursprüngliche Berechtigung erforderlich, um [das Abonnement zu erstellen](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="0fb1f-130">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="0fb1f-131">Hinweis: Dies gilt Arbeit/nur Konten Schule.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-131">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="0fb1f-132">Abonnements, die **diese** App für sich selbst oder für jeden Benutzer in das Verzeichnis erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-132">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="0fb1f-133">Erweiterte Szenarien</span><span class="sxs-lookup"><span data-stu-id="0fb1f-133">Advanced scenarios</span></span>

<span data-ttu-id="0fb1f-134">In einigen Fällen eine app von anderen apps erstellt Abonnements abrufen möchte.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-134">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="0fb1f-135">Beispielsweise möchte ein Benutzer alle Abonnements, die von einer beliebigen app in ihrem Auftrag erstellt.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-135">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="0fb1f-136">Oder ein Administrator alle Abonnements aus allen apps in ihrem Verzeichnis finden Sie unter möchten.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-136">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="0fb1f-137">Für solche Szenarien ist eine delegierte Berechtigung Subscription.Read.All erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-137">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="0fb1f-138">Kontext der aufrufenden app</span><span class="sxs-lookup"><span data-stu-id="0fb1f-138">Context of the calling app</span></span> | <span data-ttu-id="0fb1f-139">Antwort enthält</span><span class="sxs-lookup"><span data-stu-id="0fb1f-139">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="0fb1f-140">App ist im Namen des angemeldeten Benutzers (Delegierte Berechtigung) aufrufen.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-140">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="0fb1f-141">*Der Benutzer ist ein nicht-Administrator*.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-141">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="0fb1f-142">"AND"</span><span class="sxs-lookup"><span data-stu-id="0fb1f-142">-and-</span></span><br/><span data-ttu-id="0fb1f-143">App verfügt über die Berechtigung Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fb1f-143">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="0fb1f-144">Hinweis: Dies gilt für persönliche Microsoft-Konten und Arbeit/Schule Konten.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-144">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="0fb1f-145">Abonnements, die von **einer beliebigen app** nur für den angemeldeten Benutzer erstellt.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-145">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="0fb1f-146">App ist im Namen des angemeldeten Benutzers (Delegierte Berechtigung) aufrufen.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-146">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="0fb1f-147">*Der Benutzer ist ein Administrator*.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-147">*The user is an admin*.</span></span><br/><span data-ttu-id="0fb1f-148">"AND"</span><span class="sxs-lookup"><span data-stu-id="0fb1f-148">-and-</span></span><br/><span data-ttu-id="0fb1f-149">App verfügt über die Berechtigung Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fb1f-149">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="0fb1f-150">Hinweis: Dies gilt Arbeit/nur Konten Schule.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-150">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="0fb1f-151">Abonnements, die von **einer beliebigen app** für **alle Benutzer** im Verzeichnis erstellt.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-151">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fb1f-152">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0fb1f-152">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0fb1f-153">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0fb1f-153">Optional query parameters</span></span>

<span data-ttu-id="0fb1f-154">Diese Methode unterstützt nicht die [OData-Abfrage-Parameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-154">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fb1f-155">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0fb1f-155">Request headers</span></span>

| <span data-ttu-id="0fb1f-156">Name</span><span class="sxs-lookup"><span data-stu-id="0fb1f-156">Name</span></span>       | <span data-ttu-id="0fb1f-157">Typ</span><span class="sxs-lookup"><span data-stu-id="0fb1f-157">Type</span></span> | <span data-ttu-id="0fb1f-158">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0fb1f-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0fb1f-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fb1f-159">Authorization</span></span>  | <span data-ttu-id="0fb1f-160">string</span><span class="sxs-lookup"><span data-stu-id="0fb1f-160">string</span></span>  | <span data-ttu-id="0fb1f-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fb1f-163">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0fb1f-163">Request body</span></span>

<span data-ttu-id="0fb1f-164">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fb1f-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="0fb1f-165">Response</span></span>

<span data-ttu-id="0fb1f-166">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste von Objekten im Antworttext [Abonnement](../resources/subscription.md) .</span><span class="sxs-lookup"><span data-stu-id="0fb1f-166">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fb1f-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0fb1f-167">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0fb1f-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0fb1f-168">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a><span data-ttu-id="0fb1f-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="0fb1f-169">Response</span></span>

<span data-ttu-id="0fb1f-170">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-170">Here is an example of the response.</span></span> <span data-ttu-id="0fb1f-171">Hinweis: Die hier gezeigte Antwort der Kürze halber werden möglicherweise abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-171">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="0fb1f-172">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-172">All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

<span data-ttu-id="0fb1f-173">Wenn eine Anforderung mehrere Seiten mit Daten zurückgegeben, die Antwort enthält eine `@odata.nextLink` Eigenschaft zur einfacheren Verwaltung der Ergebnisse.</span><span class="sxs-lookup"><span data-stu-id="0fb1f-173">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="0fb1f-174">Finden Sie weitere Informationen finden Sie unter [Microsoft Graph Paging von Daten in Ihrer app](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="0fb1f-174">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
