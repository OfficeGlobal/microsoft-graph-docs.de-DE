---
title: 'DirectoryObject: Delta'
description: 'Get neu erstellt, aktualisiert oder gelöscht Verzeichnisobjekten der folgenden Typen: Benutzer, Gruppe oder Organisation Kontakt in einer einzelnen Delta-Abfrage. Finden Sie unter Nachverfolgen von Änderungen für Details.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4b00f86dcb3789a2117a23ffa20e6392e557910d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573256"
---
# <a name="directoryobject-delta"></a><span data-ttu-id="c0bfa-104">DirectoryObject: Delta</span><span class="sxs-lookup"><span data-stu-id="c0bfa-104">directoryObject: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0bfa-105">Get neu erstellt, aktualisiert oder gelöscht Verzeichnisobjekten der folgenden Typen: [Benutzer](../resources/user.md), [Gruppe](../resources/group.md) und [organisatorische Kontakt](../resources/orgcontact.md)in einer einzelnen Delta-Abfrage.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-105">Get newly created, updated, or deleted directory objects of the following types: [user](../resources/user.md), [group](../resources/group.md) and [organizational contact](../resources/orgcontact.md), in a single delta query.</span></span> <span data-ttu-id="c0bfa-106">Einzelheiten finden Sie unter [Nachverfolgen von Änderungen](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="c0bfa-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0bfa-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c0bfa-107">Permissions</span></span>

<span data-ttu-id="c0bfa-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0bfa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0bfa-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0bfa-110">Permission type</span></span>      | <span data-ttu-id="c0bfa-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0bfa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0bfa-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0bfa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c0bfa-113">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c0bfa-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="c0bfa-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0bfa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0bfa-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0bfa-115">Not supported.</span></span>  |
|<span data-ttu-id="c0bfa-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0bfa-116">Application</span></span> | <span data-ttu-id="c0bfa-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0bfa-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0bfa-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0bfa-118">HTTP request</span></span>

<span data-ttu-id="c0bfa-119">Zum Nachverfolgen von Änderungen beginnen, stellen Sie eine Anforderung, einschließlich der Delta-Funktion für die Ressource DirectoryObjects.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-119">To begin tracking changes, you make a request including the delta function on the directoryObjects resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a><span data-ttu-id="c0bfa-120">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c0bfa-120">Query parameters</span></span>

<span data-ttu-id="c0bfa-121">Nachverfolgen von Änderungen verursacht eine Rundung eine oder mehrere **Delta** Funktionsaufrufe.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="c0bfa-122">Wenn Sie eine beliebige Abfragezeichenfolgen-Parameter verwenden (außer `$deltatoken` und `$skiptoken`), müssen Sie es in die erste **Delta** -Anforderung angeben.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="c0bfa-123">Microsoft Graph codiert angegebenen Parameter automatisch in den token Teil der `nextLink` oder `deltaLink` URL auf, die in der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="c0bfa-124">Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="c0bfa-125">In nachfolgenden Anforderungen können Sie die  `nextLink`- oder `deltaLink`-URL aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="c0bfa-126">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c0bfa-126">Query parameter</span></span> | <span data-ttu-id="c0bfa-127">Typ</span><span class="sxs-lookup"><span data-stu-id="c0bfa-127">Type</span></span> |<span data-ttu-id="c0bfa-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0bfa-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c0bfa-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="c0bfa-129">$deltatoken</span></span> | <span data-ttu-id="c0bfa-130">string</span><span class="sxs-lookup"><span data-stu-id="c0bfa-130">string</span></span> | <span data-ttu-id="c0bfa-p105">Ein [Statustoken](/graph/delta-query-overview), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Benutzersammlung zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="c0bfa-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="c0bfa-133">$skiptoken</span></span> | <span data-ttu-id="c0bfa-134">string</span><span class="sxs-lookup"><span data-stu-id="c0bfa-134">string</span></span> | <span data-ttu-id="c0bfa-135">Ein [Statustoken](/graph/delta-query-overview), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Benutzersammlung weitere Änderungen zum Nachverfolgen vorliegen.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="c0bfa-136">OData-Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c0bfa-136">OData query parameters</span></span>

<span data-ttu-id="c0bfa-137">Diese Methode unterstützt optionale Parameter der OData-Abfrage, mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="c0bfa-138">Sie können `$filter` mit den speziellen `isOf` Operator Filtern eine Teilmenge der Typen von DirectoryObject abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-138">You can use `$filter` with the special `isOf` operator to filter a subset of types derived from directoryObject.</span></span>
  - <span data-ttu-id="c0bfa-139">Sie können mehrere Ausdrücke mit kombinieren ein `or`, ermöglicht eine einzelne Delta-Abfrage mehrere Typen nachverfolgen vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-139">You can combine multiple expressions using an `or`, which allows you to have a single delta query tracking multiple types.</span></span> <span data-ttu-id="c0bfa-140">Finden Sie im [dritten Beispiel](#request-3) für Details.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-140">See the [third example](#request-3) for details.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0bfa-141">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0bfa-141">Request headers</span></span>

| <span data-ttu-id="c0bfa-142">Name</span><span class="sxs-lookup"><span data-stu-id="c0bfa-142">Name</span></span>       | <span data-ttu-id="c0bfa-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0bfa-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c0bfa-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0bfa-144">Authorization</span></span>  | <span data-ttu-id="c0bfa-145">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="c0bfa-145">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="c0bfa-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0bfa-146">Content-Type</span></span>  | <span data-ttu-id="c0bfa-147">application/json</span><span class="sxs-lookup"><span data-stu-id="c0bfa-147">application/json</span></span> |
| <span data-ttu-id="c0bfa-148">Prefer</span><span class="sxs-lookup"><span data-stu-id="c0bfa-148">Prefer</span></span> | <span data-ttu-id="c0bfa-149">zurückgeben = minimal</span><span class="sxs-lookup"><span data-stu-id="c0bfa-149">return=minimal</span></span> <br><br><span data-ttu-id="c0bfa-150">Angabe dieser Header mit einer Anforderung, die verwendet eine `deltaLink` würde zurückgeben nur die Eigenschaften des Objekts, die seit der letzten Round geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-150">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="c0bfa-151">Optional.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0bfa-152">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0bfa-152">Request body</span></span>

<span data-ttu-id="c0bfa-153">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-153">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="c0bfa-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0bfa-154">Response</span></span>

<span data-ttu-id="c0bfa-155">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwort Code und [Benutzer](../resources/directoryobject.md) -Auflistungsobjekt in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-155">If successful, this method returns `200 OK` response code and [user](../resources/directoryobject.md) collection object in the response body.</span></span> <span data-ttu-id="c0bfa-156">Die Antwort enthält außerdem eine `nextLink` URL oder eine `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-156">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="c0bfa-157">Wenn ein `nextLink` URL zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="c0bfa-157">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="c0bfa-158">Dies gibt an, dass es sind zusätzliche Seiten mit Daten aus der Sitzung abgerufen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-158">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="c0bfa-159">Die Anwendung weiterhin tätigen Anforderungen mithilfe der `nextLink` URL bis eine `deltaLink` URL in der Antwort enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-159">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="c0bfa-160">Die Antwort enthält den gleichen Satz an Eigenschaften wie in der ersten Delta abfrageanforderung.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-160">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="c0bfa-161">Dadurch können Sie den vollständigen aktuellen Status der Objekte erfasst werden, wenn den Delta-Zyklus zu initiieren.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-161">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="c0bfa-162">Wenn ein `deltaLink` URL zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="c0bfa-162">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="c0bfa-163">Dies gibt an, dass es sind keine weiteren Daten zum vorhandenen Status der Ressource zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-163">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="c0bfa-164">Speichern und verwenden Sie die `deltaLink` URL, um zu lernen in die Ressource in der nächsten Runde geändert.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-164">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="c0bfa-165">Sie haben die Wahl zum Angeben der `Prefer:return=minimal` -Header in der Antwort nur Werte für die Eigenschaften enthalten, die seit der Ausführung geändert wurden die `deltaLink` ausgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-165">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="c0bfa-166">Standard: zurückzugeben Sie, die gleichen Eigenschaften als erste Delta-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0bfa-166">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="c0bfa-167">Standardmäßig fordert mithilfe einer `deltaLink` oder `nextLink` dieselben Eigenschaften wie in der ersten Delta-Abfrage ausgewählten folgendermaßen zurückgeben:</span><span class="sxs-lookup"><span data-stu-id="c0bfa-167">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="c0bfa-168">Wenn die Eigenschaft geändert wurde, ist der neue Wert in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-168">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="c0bfa-169">Dies schließt Eigenschaften auf null-Wert festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-169">This includes properties being set to null value.</span></span>
- <span data-ttu-id="c0bfa-170">Wenn die Eigenschaft nicht geändert wurde, wird der alte Wert in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-170">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="c0bfa-171">Wenn die Eigenschaft nicht festgelegt wurde, bevor es nicht in der Antwort überhaupt eingeschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-171">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="c0bfa-172">**Hinweis:** Mit diesem Verhalten ist die Antwort verfolgen es nicht möglich, sagen, ob eine Eigenschaft oder nicht geändert wird.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-172">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="c0bfa-173">Darüber hinaus meist die Antworten Delta groß sein, da sie alle Eigenschaftswerte enthalten.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-173">Also, the delta responses tend to be large because they contain all property values.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="c0bfa-174">Alternative: nur die geänderten Eigenschaften zurückgeben</span><span class="sxs-lookup"><span data-stu-id="c0bfa-174">Alternative: return only the changed properties</span></span>

<span data-ttu-id="c0bfa-175">Hinzufügen einer optionalen Anforderungsheader - `prefer:return=minimal` -führt das folgende Verhalten:</span><span class="sxs-lookup"><span data-stu-id="c0bfa-175">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="c0bfa-176">Wenn die Eigenschaft geändert wurde, ist der neue Wert in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-176">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="c0bfa-177">Dies schließt Eigenschaften auf null-Wert festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-177">This includes properties being set to null value.</span></span>
- <span data-ttu-id="c0bfa-178">Wenn die Eigenschaft nicht geändert wurde, ist die Eigenschaft nicht in allen in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-178">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="c0bfa-179">(Andere als das Standardverhalten).</span><span class="sxs-lookup"><span data-stu-id="c0bfa-179">(Different from the default behavior.)</span></span>

> <span data-ttu-id="c0bfa-180">**Hinweis:** Die Kopfzeile hinzugefügt werden kann einen `deltaLink` Anforderung an einer beliebigen Stelle in Zeit im Zyklus Delta.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-180">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="c0bfa-181">Die Kopfzeile wirkt sich nur auf die Gruppe von Eigenschaften, die in der Antwort enthalten, und er hat keinen Einfluss auf wie die Delta-Abfrage ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-181">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span>

## <a name="example"></a><span data-ttu-id="c0bfa-182">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0bfa-182">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="c0bfa-183">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="c0bfa-183">Request 1</span></span>

<span data-ttu-id="c0bfa-184">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-184">The following is an example of the request.</span></span> <span data-ttu-id="c0bfa-185">Es ist keine `$select` Parameter, damit ein Standardsatz Eigenschaften nachverfolgt und zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-185">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta",
  "truncated": true
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
```

### <a name="response-1"></a><span data-ttu-id="c0bfa-186">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="c0bfa-186">Response 1</span></span>

<span data-ttu-id="c0bfa-187">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-187">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="c0bfa-188">Nicht `isOf` Filter verwendet wurde, damit alle Typen von DirectoryObject abgeleitete zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-188">No `isOf` filter has been used, so all types derived from directoryObject are returned.</span></span>

><span data-ttu-id="c0bfa-p119">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-p119">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp"
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": ["string"],
      "city": "string",
      "companyName": "string",
      "country": "string",
      "department": "string",
      "displayName": "string",
      "givenName": "string",
      "jobTitle": "string"
    }    
  ]
}
```

### <a name="request-2"></a><span data-ttu-id="c0bfa-191">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="c0bfa-191">Request 2</span></span>

<span data-ttu-id="c0bfa-192">Im nächste Beispiel wird die Verwendung des Verhaltens alternative minimale Antwort:</span><span class="sxs-lookup"><span data-stu-id="c0bfa-192">The next example shows the use of the alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta",
  "truncated": true
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```

### <a name="response-2"></a><span data-ttu-id="c0bfa-193">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="c0bfa-193">Response 2</span></span>

<span data-ttu-id="c0bfa-194">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-194">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="c0bfa-195">Beachten Sie, dass nur die Eigenschaften, die tatsächlich geändert wurden zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-195">Note only the properties that have actually changed are returned.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "displayName": "John Smith"
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "description": null,
      "displayName": "testgp"
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": "12345"
    }    
  ]
}
```

### <a name="request-3"></a><span data-ttu-id="c0bfa-196">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="c0bfa-196">Request 3</span></span>

<span data-ttu-id="c0bfa-197">Das nächste Beispiel veranschaulicht die erste Anforderung mithilfe der `isOf` Operator herausfiltern nur Benutzer- und Entitäten:</span><span class="sxs-lookup"><span data-stu-id="c0bfa-197">The next example shows the initial request using the `isOf` operator to filter out only user and group entities:</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta",
  "truncated": true
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```

### <a name="response-3"></a><span data-ttu-id="c0bfa-198">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="c0bfa-198">Response 3</span></span>

<span data-ttu-id="c0bfa-199">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="c0bfa-199">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="c0bfa-200">Beachten Sie, dass nur Benutzer und Gruppe Objekte zurückgegeben werden:</span><span class="sxs-lookup"><span data-stu-id="c0bfa-200">Note that only user and group objects are returned:</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp"      
    }    
  ]
}
```

- <span data-ttu-id="c0bfa-201">[Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten verwenden](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="c0bfa-201">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="c0bfa-202">[Inkrementelle Änderungen für Benutzer erhalten möchten](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="c0bfa-202">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
