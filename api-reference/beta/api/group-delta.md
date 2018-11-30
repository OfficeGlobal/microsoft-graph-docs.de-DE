---
title: 'group: delta'
description: Get neu erstellt, aktualisiert oder Gruppen, einschließlich der Gruppenmitgliedschaft ändert, ohne zum Ausführen eines alles Lesen der ganzen Gruppe-Auflistung gelöscht. Einzelheiten finden Sie unter Delta-Abfrage verwenden.
ms.openlocfilehash: 562321ddff9e5c9d2840c1c1178aa8e4f2fd4114
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064435"
---
# <a name="group-delta"></a><span data-ttu-id="d119b-104">group: delta</span><span class="sxs-lookup"><span data-stu-id="d119b-104">group: delta</span></span>

> <span data-ttu-id="d119b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d119b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d119b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d119b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d119b-107">Get neu erstellt, aktualisiert oder Gruppen, einschließlich der Gruppenmitgliedschaft ändert, ohne zum Ausführen eines alles Lesen der ganzen Gruppe-Auflistung gelöscht.</span><span class="sxs-lookup"><span data-stu-id="d119b-107">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="d119b-108">Einzelheiten finden Sie unter [Delta-Abfrage verwenden](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="d119b-108">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="d119b-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d119b-109">Permissions</span></span>

<span data-ttu-id="d119b-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d119b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d119b-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d119b-112">Permission type</span></span>      | <span data-ttu-id="d119b-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d119b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d119b-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d119b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d119b-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d119b-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d119b-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d119b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d119b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d119b-117">Not supported.</span></span>    |
|<span data-ttu-id="d119b-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d119b-118">Application</span></span> | <span data-ttu-id="d119b-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d119b-119">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d119b-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d119b-120">HTTP request</span></span>

<span data-ttu-id="d119b-121">Um Änderungen nachzuverfolgen, führe Sie zunächst eine Anforderung einschließlich der delta-Funktion für die Gruppenressource aus.</span><span class="sxs-lookup"><span data-stu-id="d119b-121">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="d119b-122">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d119b-122">Query parameters</span></span>

<span data-ttu-id="d119b-p105">Beim Nachverfolgen von Änderungen in Gruppen wird eine Runde von einem oder mehreren **delta**-Funktionsaufrufen ausgeführt. Wenn Sie Abfrageparameter (außer `$deltatoken` und `$skiptoken`) verwenden, müssen Sie sie in der ursprünglichen **delta**-Anforderung angeben. Microsoft Graph codiert automatisch alle angegebenen Parameter in den Tokenteil der in der Antwort enthaltenen `nextLink`- oder `deltaLink`-URL.</span><span class="sxs-lookup"><span data-stu-id="d119b-p105">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="d119b-126">Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben.</span><span class="sxs-lookup"><span data-stu-id="d119b-126">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="d119b-127">In nachfolgenden Anforderungen können Sie die  `nextLink`- oder `deltaLink`-URL aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="d119b-127">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="d119b-128">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d119b-128">Query parameter</span></span> | <span data-ttu-id="d119b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d119b-129">Type</span></span>  |<span data-ttu-id="d119b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d119b-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d119b-131">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="d119b-131">$deltatoken</span></span> | <span data-ttu-id="d119b-132">string</span><span class="sxs-lookup"><span data-stu-id="d119b-132">string</span></span> | <span data-ttu-id="d119b-p106">Ein [Statustoken](/graph/delta-query-overview), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Gruppensammlung zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.</span><span class="sxs-lookup"><span data-stu-id="d119b-p106">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="d119b-135">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="d119b-135">$skiptoken</span></span> | <span data-ttu-id="d119b-136">string</span><span class="sxs-lookup"><span data-stu-id="d119b-136">string</span></span> | <span data-ttu-id="d119b-137">Ein [Statustoken](/graph/delta-query-overview), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Gruppensammlung weitere Änderungen zum Nachverfolgen vorliegen.</span><span class="sxs-lookup"><span data-stu-id="d119b-137">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="d119b-138">OData-Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d119b-138">OData query parameters</span></span>

<span data-ttu-id="d119b-139">Diese Methode unterstützt optionale Parameter der OData-Abfrage, mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="d119b-139">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="d119b-p107">Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft *id* wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d119b-p107">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="d119b-142">Sie können `$expand=members` mitgliedschaftsänderungen abgerufen.</span><span class="sxs-lookup"><span data-stu-id="d119b-142">You can use `$expand=members` to get membership changes.</span></span>
- <span data-ttu-id="d119b-143">Es ist eingeschränkte Unterstützung für `$filter`:</span><span class="sxs-lookup"><span data-stu-id="d119b-143">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="d119b-144">Der einzige unterstützte `$filter`-Ausdruck dient zum Nachverfolgen von Änderungen an einem bestimmten Objekt: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="d119b-144">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="d119b-145">Sie können mehrere Objekte filtern.</span><span class="sxs-lookup"><span data-stu-id="d119b-145">You can filter multiple objects.</span></span> <span data-ttu-id="d119b-146">Beispiel: `https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="d119b-146">For example, `https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="d119b-147">Es gilt ein Grenzwert von 50 gefilterten Objekten.</span><span class="sxs-lookup"><span data-stu-id="d119b-147">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d119b-148">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d119b-148">Request headers</span></span>

| <span data-ttu-id="d119b-149">Name</span><span class="sxs-lookup"><span data-stu-id="d119b-149">Name</span></span>       | <span data-ttu-id="d119b-150">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d119b-150">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d119b-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="d119b-151">Authorization</span></span>  | <span data-ttu-id="d119b-152">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="d119b-152">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="d119b-153">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d119b-153">Content-Type</span></span>  | <span data-ttu-id="d119b-154">application/json</span><span class="sxs-lookup"><span data-stu-id="d119b-154">application/json</span></span> |
| <span data-ttu-id="d119b-155">Prefer</span><span class="sxs-lookup"><span data-stu-id="d119b-155">Prefer</span></span> | <span data-ttu-id="d119b-156">zurückgeben = minimal</span><span class="sxs-lookup"><span data-stu-id="d119b-156">return=minimal</span></span> <br><br><span data-ttu-id="d119b-157">Angabe dieser Header mit einer Anforderung, die verwendet eine `deltaLink` würde zurückgeben nur die Eigenschaften des Objekts, die seit der letzten Round geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="d119b-157">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="d119b-158">Optional.</span><span class="sxs-lookup"><span data-stu-id="d119b-158">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d119b-159">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d119b-159">Request body</span></span>

<span data-ttu-id="d119b-160">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d119b-160">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="d119b-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="d119b-161">Response</span></span>

<span data-ttu-id="d119b-162">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [group](../resources/group.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d119b-162">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="d119b-163">Die Antwort enthält auch ein Status-Token der entweder ein `nextLink` URL oder eine `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="d119b-163">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="d119b-164">Wenn ein `nextLink` URL zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="d119b-164">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="d119b-165">Dies gibt an, dass es sind zusätzliche Seiten mit Daten aus der Sitzung abgerufen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d119b-165">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="d119b-166">Die Anwendung weiterhin tätigen Anforderungen mithilfe der `nextLink` URL bis eine `deltaLink` URL in der Antwort enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="d119b-166">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="d119b-167">Die Antwort enthält den gleichen Satz an Eigenschaften wie in der ersten Delta abfrageanforderung.</span><span class="sxs-lookup"><span data-stu-id="d119b-167">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="d119b-168">Dadurch können Sie den vollständigen aktuellen Status der Objekte erfasst werden, wenn den Delta-Zyklus zu initiieren.</span><span class="sxs-lookup"><span data-stu-id="d119b-168">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="d119b-169">Wenn ein `deltaLink` URL zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="d119b-169">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="d119b-170">Dies gibt an, dass es sind keine weiteren Daten zum vorhandenen Status der Ressource zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="d119b-170">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="d119b-171">Speichern und verwenden Sie die `deltaLink` URL, um zu lernen in die Ressource in der nächsten Runde geändert.</span><span class="sxs-lookup"><span data-stu-id="d119b-171">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="d119b-172">Sie haben die Wahl zum Angeben der `Prefer:return=minimal` -Header in der Antwort nur Werte für die Eigenschaften enthalten, die seit der Ausführung geändert wurden die `deltaLink` ausgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="d119b-172">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="d119b-173">Standard: zurückzugeben Sie, die gleichen Eigenschaften als erste Delta-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d119b-173">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="d119b-174">Standardmäßig fordert mithilfe einer `deltaLink` oder `nextLink` dieselben Eigenschaften wie in der ersten Delta-Abfrage ausgewählten folgendermaßen zurückgeben:</span><span class="sxs-lookup"><span data-stu-id="d119b-174">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="d119b-175">Wenn die Eigenschaft geändert wurde, ist der neue Wert in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="d119b-175">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="d119b-176">Dies schließt Eigenschaften auf null-Wert festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="d119b-176">This includes properties being set to null value.</span></span>
- <span data-ttu-id="d119b-177">Wenn die Eigenschaft nicht geändert wurde, wird der alte Wert in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="d119b-177">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="d119b-178">Wenn die Eigenschaft nicht festgelegt wurde, bevor es nicht in der Antwort überhaupt eingeschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d119b-178">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="d119b-179">**Hinweis:** Mit diesem Verhalten ist die Antwort verfolgen es nicht möglich, sagen, ob eine Eigenschaft oder nicht geändert wird.</span><span class="sxs-lookup"><span data-stu-id="d119b-179">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="d119b-180">Darüber hinaus meist die Antworten Delta groß sein, da sie alle Eigenschaftswerte - enthalten wie im [zweiten Beispiel](#request-2) unten dargestellt.</span><span class="sxs-lookup"><span data-stu-id="d119b-180">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="d119b-181">Alternative: nur die geänderten Eigenschaften zurückgeben</span><span class="sxs-lookup"><span data-stu-id="d119b-181">Alternative: return only the changed properties</span></span>

<span data-ttu-id="d119b-182">Hinzufügen einer optionalen Anforderungsheader - `prefer:return=minimal` -führt das folgende Verhalten:</span><span class="sxs-lookup"><span data-stu-id="d119b-182">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="d119b-183">Wenn die Eigenschaft geändert wurde, ist der neue Wert in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="d119b-183">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="d119b-184">Dies schließt Eigenschaften auf null-Wert festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="d119b-184">This includes properties being set to null value.</span></span>
- <span data-ttu-id="d119b-185">Wenn die Eigenschaft nicht geändert wurde, ist die Eigenschaft nicht in allen in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="d119b-185">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="d119b-186">(Andere als das Standardverhalten).</span><span class="sxs-lookup"><span data-stu-id="d119b-186">(Different from the default behavior.)</span></span>

> <span data-ttu-id="d119b-187">**Hinweis:** Die Kopfzeile hinzugefügt werden kann einen `deltaLink` Anforderung an einer beliebigen Stelle in Zeit im Zyklus Delta.</span><span class="sxs-lookup"><span data-stu-id="d119b-187">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="d119b-188">Die Kopfzeile wirkt sich nur auf die Gruppe von Eigenschaften, die in der Antwort enthalten, und er hat keinen Einfluss auf wie die Delta-Abfrage ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="d119b-188">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="d119b-189">Finden Sie im [dritten Beispiel](#request-3) unten.</span><span class="sxs-lookup"><span data-stu-id="d119b-189">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="d119b-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d119b-190">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="d119b-191">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="d119b-191">Request 1</span></span>

<span data-ttu-id="d119b-192">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d119b-192">The following is an example of the request.</span></span> <span data-ttu-id="d119b-193">Es ist keine `$select` Parameter, damit ein Standardsatz Eigenschaften nachverfolgt und zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="d119b-193">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta
```

#### <a name="response-1"></a><span data-ttu-id="d119b-194">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="d119b-194">Response 1</span></span>

<span data-ttu-id="d119b-195">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="d119b-195">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="d119b-196">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="d119b-196">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d119b-197">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d119b-197">All the properties will be returned from an actual call.</span></span>
>
> <span data-ttu-id="d119b-198">Das Anwesenheitssymbol der *members@delta* -Eigenschaft umfasst die Ids der Member-Objekte in der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="d119b-198">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
  "value":[
    {
      "classification": "classification-value",
      "createdDateTime":"datetime-value",
      "description":"Test group 1",
      "displayName":"TestGroup1",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

#### <a name="request-2"></a><span data-ttu-id="d119b-199">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="d119b-199">Request 2</span></span>

<span data-ttu-id="d119b-200">Das nächste Beispiel veranschaulicht die erste Anforderung 3 Eigenschaften für nachverfolgen Antwort Standardverhalten auswählen:</span><span class="sxs-lookup"><span data-stu-id="d119b-200">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a><span data-ttu-id="d119b-201">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="d119b-201">Response 2</span></span>

<span data-ttu-id="d119b-202">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="d119b-202">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="d119b-203">Beachten Sie, dass alle 3 Eigenschaften sind in der Antwort enthalten, und es nicht bekannt ist, welche geändert wurden, seit die `deltaLink` abgerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="d119b-203">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null,
      "mailNickname": "mailNickname-value"
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="d119b-204">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="d119b-204">Request 3</span></span>

<span data-ttu-id="d119b-205">Das nächste Beispiel veranschaulicht die erste Anforderung 3 Eigenschaften für nachverfolgen mit alternativen minimale Antwort Verhalten auswählen:</span><span class="sxs-lookup"><span data-stu-id="d119b-205">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="d119b-206">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="d119b-206">Response 3</span></span>

<span data-ttu-id="d119b-207">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="d119b-207">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="d119b-208">Beachten Sie, dass die `mailNickname` -Eigenschaft ist nicht enthalten, was bedeutet, dass wurde nicht geändert seit der letzten Delta-Abfrage; `displayName` und `description` sind enthalten, d. h., deren Werte geändert haben.</span><span class="sxs-lookup"><span data-stu-id="d119b-208">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="d119b-209">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="d119b-209">See also</span></span>

- <span data-ttu-id="d119b-210">[Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten verwenden](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="d119b-210">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="d119b-211">[Inkrementelle Änderungen für Gruppen erhalten möchten](/graph/delta-query-groups).</span><span class="sxs-lookup"><span data-stu-id="d119b-211">[Get incremental changes for groups](/graph/delta-query-groups).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
