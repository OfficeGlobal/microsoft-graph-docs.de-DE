---
title: Dient zum Abrufen inkrementeller Änderungen für Benutzer.
description: Mit der Delta-Abfrage können Sie Ergänzungen, Löschungen oder Aktualisierungen an Benutzern anhand einer Serie von Delta-Funktionsaufrufen abfragen. Mit der Delta-Abfrage können Sie Änderungen an Benutzern ermitteln, ohne den gesamten Satz von Benutzern von Microsoft Graph abrufen und Änderungen vergleichen zu müssen.
ms.openlocfilehash: 4b0237d01ad806a72c80c55522b06d4b37dc3a44
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092189"
---
# <a name="get-incremental-changes-for-users"></a><span data-ttu-id="964d4-104">Dient zum Abrufen inkrementeller Änderungen für Benutzer.</span><span class="sxs-lookup"><span data-stu-id="964d4-104">Get incremental changes for users</span></span>

<span data-ttu-id="964d4-p102">Mit der [Delta-Abfrage](./delta-query-overview.md) können Sie Ergänzungen, Löschungen oder Aktualisierungen an Benutzern anhand einer Serie von [Delta](/graph/api/user-delta?view=graph-rest-1.0)-Funktionsaufrufen abfragen. Mit der Delta-Abfrage können Sie Änderungen an Benutzern ermitteln, ohne den gesamten Satz von Benutzern von Microsoft Graph abrufen und Änderungen vergleichen zu müssen.</span><span class="sxs-lookup"><span data-stu-id="964d4-p102">[Delta query](./delta-query-overview.md) lets you query for additions, deletions, or updates to users, by way of a series of [delta](/graph/api/user-delta?view=graph-rest-1.0) function calls. Delta query enables you discover changes to users without having to fetch the entire set of users from Microsoft Graph and compare changes.</span></span>

<span data-ttu-id="964d4-p103">Clients, die Benutzer mit einem lokalen Profilspeicher synchronisieren, können Delta Abfragen für die anfängliche vollständige Synchronisierung und für inkrementelle Synchronisierungen in der Zukunft verwenden. In der Regel führt ein Client eine anfängliche vollständige Synchronisierung aller Benutzer in einem Mandanten durch und ruft anschließend regelmäßig inkrementelle Änderungen an Benutzern ab.</span><span class="sxs-lookup"><span data-stu-id="964d4-p103">Clients using synchronizing users with a local profile store can use Delta Query for both their initial full synchronization along with incremental synchronizations in the future. Typically, a client would do an initial full synchronization of all the users in a tenant, and subsequently, get incremental changes to users periodically.</span></span>

## <a name="tracking-user-changes"></a><span data-ttu-id="964d4-109">Nachverfolgen von Benutzeränderungen</span><span class="sxs-lookup"><span data-stu-id="964d4-109">Tracking user changes</span></span>

<span data-ttu-id="964d4-p104">Das Nachverfolgen von Benutzeränderungen ist eine Runde aus einer oder mehreren GET-Anforderungen mit der **Delta**-Funktion. Eine GET-Anforderung wird ähnlich wie das [Auflisten von Benutzern](/graph/api/user-list?view=graph-rest-1.0) durchgeführt, außer dass Folgendes eingeschlossen wird:</span><span class="sxs-lookup"><span data-stu-id="964d4-p104">Tracking user changes is a round of one or more GET requests with the **delta** function. You make a GET request much like the way you [list users](/graph/api/user-list?view=graph-rest-1.0), except that you include the following:</span></span>

- <span data-ttu-id="964d4-112">Die **Delta**-Funktion.</span><span class="sxs-lookup"><span data-stu-id="964d4-112">The **delta** function.</span></span>
- <span data-ttu-id="964d4-113">Ein [Statustoken](./delta-query-overview.md) (_deltaToken_ oder _skipToken_) aus dem vorherigen GET-**Delta**-Funktionsaufruf.</span><span class="sxs-lookup"><span data-stu-id="964d4-113">A [state token](./delta-query-overview.md) (_deltaToken_ or _skipToken_) from the previous GET **delta** function call.</span></span>

## <a name="example"></a><span data-ttu-id="964d4-114">Beispiel</span><span class="sxs-lookup"><span data-stu-id="964d4-114">Example</span></span>

<span data-ttu-id="964d4-115">Das folgende Beispiel zeigt eine Serienanforderung zum Nachverfolgen von Änderungen an Benutzern:</span><span class="sxs-lookup"><span data-stu-id="964d4-115">The following example shows a series  requests to track changes to users:</span></span>

1. <span data-ttu-id="964d4-116">[Ursprüngliche Anforderung](#initial-request) und [Antwort](#initial-response)</span><span class="sxs-lookup"><span data-stu-id="964d4-116">[Initial request](#initial-request) and [response](#initial-response)</span></span>
2. <span data-ttu-id="964d4-117">[nextLink-Anforderung](#nextlink-request) und [Antwort](#nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="964d4-117">[nextLink request](#nextlink-request) and [response](#nextlink-response)</span></span>
3. <span data-ttu-id="964d4-118">[Letzte nextLink-Anforderung](#final-nextlink-request) und [Antwort](#final-nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="964d4-118">[Final nextLink request](#final-nextlink-request) and [response](#final-nextlink-response)</span></span>
4. <span data-ttu-id="964d4-119">[deltaLink-Anforderung](#deltalink-request) und [deltaLink-Antwort](#deltalink-response)</span><span class="sxs-lookup"><span data-stu-id="964d4-119">[deltaLink request](#deltalink-request) and [deltaLink response](#deltalink-response)</span></span>

## <a name="initial-request"></a><span data-ttu-id="964d4-120">Ursprüngliche Anforderung</span><span class="sxs-lookup"><span data-stu-id="964d4-120">Initial request</span></span>

<span data-ttu-id="964d4-121">Um Änderungen an der Benutzerressource nachzuverfolgen, nehmen Sie zunächst eine Anforderung einschließlich der Delta-Funktion für die Benutzerressource vor.</span><span class="sxs-lookup"><span data-stu-id="964d4-121">To begin tracking changes in the user resource, you make a request including the delta function on the user resource.</span></span>

<span data-ttu-id="964d4-122">Beachten Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="964d4-122">Note the following:</span></span>

- <span data-ttu-id="964d4-123">Der optionale Abfrageparameter „$select“ wird in die Anforderung eingeschlossen, um zu veranschaulichen, wie Abfrageparameter automatisch in zukünftige Anforderungen eingeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="964d4-123">The optional $select query parameter is included in the request to demonstrate how query parameters are automatically included in future requests.</span></span>
- <span data-ttu-id="964d4-p105">Die ursprüngliche Anforderung enthält kein Statustoken. Statustoken werden in nachfolgenden Anforderungen verwendet.</span><span class="sxs-lookup"><span data-stu-id="964d4-p105">The initial request does not include a state token. State tokens will be used in subsequent requests.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,givenName,surname
```

## <a name="initial-response"></a><span data-ttu-id="964d4-126">Ursprüngliche Antwort</span><span class="sxs-lookup"><span data-stu-id="964d4-126">Initial response</span></span>

<span data-ttu-id="964d4-p106">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das Sammlungsobjekt [user](/graph/api/resources/user?view=graph-rest-1.0) im Antworttext zurückgegeben. Wenn der ganze Satz von Benutzern zu groß ist, enthält die Antwort zudem ein nextLink-Statustoken.</span><span class="sxs-lookup"><span data-stu-id="964d4-p106">If successful, this method returns `200 OK` response code and [user](/graph/api/resources/user?view=graph-rest-1.0) collection object in the response body. Assuming the entire set of users is too large, the response will also include a nextLink state token.</span></span>

<span data-ttu-id="964d4-p107">In diesem Beispiel wird eine nextLink-URL zurückgegeben, die angibt, dass es zusätzliche Seiten mit Daten gibt, die in der Sitzung abgerufen werden müssen. Der Abfrageparameter „$select“ aus der ursprünglichen Anforderung wird in der nextLink-URL codiert.</span><span class="sxs-lookup"><span data-stu-id="964d4-p107">In this example, a nextLink URL is returned indicating there are additional pages of data to be retrieved in the session. The $select query parameter from the initial request is encoded into the nextLink URL.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users(displayName,givenName,surname)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa",
  "value": [
    {
      "displayName":"Testuser1",
      "givenName":"John",
      "surname":"Doe",
      "id":"ffff7b1a-13b6-477b-8c0c-380905cd99f7"
    },
    {
      "displayName":"Testuser2",
      "givenName":"Jane",
      "surname":"Doe",
      "id":"605d1257-ffff-40b6-8e6f-528a53f5dc55"
    }
  ]
}
```

## <a name="nextlink-request"></a><span data-ttu-id="964d4-131">nextLink-Anforderung</span><span class="sxs-lookup"><span data-stu-id="964d4-131">nextLink request</span></span>

<span data-ttu-id="964d4-p108">Die zweite Anforderung gibt das aus der vorherigen Antwort zurückgegebene `skipToken` an. Beachten Sie, dass der Parameter `$select` nicht erforderlich ist, da das `skipToken` ihn codiert und einschließt.</span><span class="sxs-lookup"><span data-stu-id="964d4-p108">The second request specifies the `skipToken` returned from the previous response. Notice the `$select` parameter is not required, as the `skipToken` encodes and includes it.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa
```

## <a name="nextlink-response"></a><span data-ttu-id="964d4-134">nextLink-Antwort</span><span class="sxs-lookup"><span data-stu-id="964d4-134">nextLink response</span></span>

<span data-ttu-id="964d4-p109">Die Antwort enthält einen `nextLink` und ein weiteres `skipToken`, wodurch angegeben wird, dass weitere Benutzer verfügbar sind. Sie nehmen weiterhin Anforderungen über die nextLink-URL vor, bis eine deltaLink-URL in der Antwort zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="964d4-p109">The response contains a `nextLink` and another `skipToken`, indicating there are more users available. You continue making requests using the nextLink URL until a deltaLink URL is returned in the response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"Testuser3",
      "givenName":"Pat",
      "surname":"Doe",
      "id":"d8c37826-ffff-4cae-b348-e2725b1e814b"
    },
    {
      "displayName":"Testuser4",
      "givenName":"Meghan",
      "surname":"Doe",
      "id":"8b1ee412-cd8f-4d59-ffff-24010edb9f1f"
    }
  ]
}
```

## <a name="final-nextlink-request"></a><span data-ttu-id="964d4-137">Letzte nextLink-Anforderung</span><span class="sxs-lookup"><span data-stu-id="964d4-137">Final nextLink request</span></span>

<span data-ttu-id="964d4-138">Die dritte Anforderung verwendet weiterhin das neueste aus der letzten Synchronisierungsanforderung zurückgegebene `skipToken`.</span><span class="sxs-lookup"><span data-stu-id="964d4-138">The third request continues to use the latest `skipToken` returned from the last sync request.</span></span> 

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhaOYDE2VPA4vxIPA90-P6OzGd6Rvku5fDgBRIGS
```

## <a name="final-nextlink-response"></a><span data-ttu-id="964d4-139">Letzte nextLink-Antwort</span><span class="sxs-lookup"><span data-stu-id="964d4-139">Final nextLink response</span></span>

<span data-ttu-id="964d4-p110">Wenn die deltaLink-URL zurückgegeben wird, gibt es keine weiteren Daten über den derzeitigen Status der zurückzugebenen Ressource. Für zukünftige Anforderungen verwendet die Anwendung die deltaLink-URL, um Informationen zu Änderungen an der Ressource zu erhalten. Speichern Sie das `deltaToken`, und verwenden Sie es in der Anforderungs-URL, um Änderungen an Benutzern zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="964d4-p110">When the deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource. Save the `deltaToken` and use it in the request URL to discover changes to users.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": [
    {
      "displayName":"Testuser5",
      "givenName":"Al",
      "surname":"Doe",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "displayName":"Testuser6",
      "givenName":"Sam",
      "surname":"Doe",
      "id":"f6ede700-27d0-4c42-bfb9-4dffff43c74a"
    }
  ]
}
```

## <a name="deltalink-request"></a><span data-ttu-id="964d4-143">deltaLink-Anforderung</span><span class="sxs-lookup"><span data-stu-id="964d4-143">deltaLink request</span></span>

<span data-ttu-id="964d4-144">Mit dem `deltaToken` aus der [letzten Antwort](#final-nextlink-response) können Sie seit der letzten Anforderung geänderte (hinzugefügte, gelöschte oder aktualisierte) Benutzer abrufen.</span><span class="sxs-lookup"><span data-stu-id="964d4-144">Using the `deltaToken` from the [last response](#final-nextlink-response), you will be able to get changed (by being added, deleted, or updated) users since the last request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460
```

## <a name="deltalink-response"></a><span data-ttu-id="964d4-145">deltaLink-Antwort</span><span class="sxs-lookup"><span data-stu-id="964d4-145">deltaLink response</span></span>

<span data-ttu-id="964d4-146">Falls keine Änderungen vorgenommen wurden, wird dasselbe `deltaToken` ohne Ergebnisse zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="964d4-146">If no changes have occurred, the same `deltaToken` is returned with no results.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": []
}
```

<span data-ttu-id="964d4-147">Wenn Änderungen vorgenommen wurden, wird dasselbe `deltaToken` mit einer Sammlung der geänderten Benutzer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="964d4-147">If changes have occurred, the same `deltaToken` is returned including a collection of changed users.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": [
    {
      "displayName":"Testuser7",
      "givenName":"Joe",
      "surname":"Doe",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "id":"8ffff70c-1c63-4860-b963-e34ec660931d",
      "@removed": {
         "reason": "changed"
      }
    }
  ]
}
```

<span data-ttu-id="964d4-148">Einige Punkte, die Sie bei der oben aufgeführten Beispielantwort beachten sollten:</span><span class="sxs-lookup"><span data-stu-id="964d4-148">Some things to note about the example response above:</span></span>

- <span data-ttu-id="964d4-149">Wenn der Benutzer gelöscht wurde, enthält das Element eine Anmerkung: `@removed` mit einem Wert von `"reason": "changed"`.</span><span class="sxs-lookup"><span data-stu-id="964d4-149">When the user is deleted, the item contains an annotation: `@removed` with value of `"reason": "changed"`.</span></span>

- <span data-ttu-id="964d4-150">Wenn der Benutzer dauerhaft gelöscht wurde, enthält das Element eine Anmerkung: `@removed` mit einem Wert von `"reason": "deleted"`.</span><span class="sxs-lookup"><span data-stu-id="964d4-150">When the user is permanently deleted, the item contains an annotation: `@removed` with value of `"reason": "deleted"`.</span></span>

- <span data-ttu-id="964d4-151">Wenn der Benutzer erstellt oder wiederhergestellt wird, gibt es keine Anmerkung.</span><span class="sxs-lookup"><span data-stu-id="964d4-151">When the user is created, or restored, there is no annotation.</span></span>

## <a name="see-also"></a><span data-ttu-id="964d4-152">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="964d4-152">See also</span></span>
<span data-ttu-id="964d4-153">[Microsoft Graph-Delta-Abfrage](delta-query-overview.md) – Übersicht.</span><span class="sxs-lookup"><span data-stu-id="964d4-153">[Microsoft Graph delta query](delta-query-overview.md) overview.</span></span>