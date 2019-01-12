---
title: 'user: delta'
description: Get neu erstellt, aktualisiert oder Benutzer ohne Durchführung ein alles Lesen der gesamten Benutzer-Auflistung gelöscht. Finden Sie unter Nachverfolgen von Änderungen für Details.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f63a426c97aaf695447de9075b91fb2c534309db
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984633"
---
# <a name="user-delta"></a><span data-ttu-id="04369-104">user: delta</span><span class="sxs-lookup"><span data-stu-id="04369-104">user: delta</span></span>

> <span data-ttu-id="04369-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="04369-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04369-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="04369-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="04369-107">Get neu erstellt, aktualisiert oder Benutzer ohne Durchführung ein alles Lesen der gesamten Benutzer-Auflistung gelöscht.</span><span class="sxs-lookup"><span data-stu-id="04369-107">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="04369-108">Einzelheiten finden Sie unter [Nachverfolgen von Änderungen](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="04369-108">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="04369-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="04369-109">Permissions</span></span>

<span data-ttu-id="04369-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04369-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="04369-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04369-112">Permission type</span></span>      | <span data-ttu-id="04369-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04369-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04369-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04369-114">Delegated (work or school account)</span></span> | <span data-ttu-id="04369-115">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="04369-115">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="04369-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04369-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04369-117">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04369-117">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="04369-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04369-118">Application</span></span> | <span data-ttu-id="04369-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04369-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04369-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04369-120">HTTP request</span></span>

<span data-ttu-id="04369-121">Um Änderungen nachzuverfolgen, führen Sie zunächst eine Anforderung einschließlich der delta-Funktion für die Benutzerressource aus.</span><span class="sxs-lookup"><span data-stu-id="04369-121">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="04369-122">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="04369-122">Query parameters</span></span>

<span data-ttu-id="04369-123">Nachverfolgen von Änderungen in Benutzer verursacht eine Rundung eine oder mehrere **Delta** Funktionsaufrufe.</span><span class="sxs-lookup"><span data-stu-id="04369-123">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="04369-124">Wenn Sie eine beliebige Abfragezeichenfolgen-Parameter verwenden (außer `$deltatoken` und `$skiptoken`), müssen Sie es in die erste **Delta** -Anforderung angeben.</span><span class="sxs-lookup"><span data-stu-id="04369-124">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="04369-125">Microsoft Graph codiert angegebenen Parameter automatisch in den token Teil der `nextLink` oder `deltaLink` URL auf, die in der Antwort.</span><span class="sxs-lookup"><span data-stu-id="04369-125">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="04369-126">Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben.</span><span class="sxs-lookup"><span data-stu-id="04369-126">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="04369-127">In nachfolgenden Anforderungen können Sie die  `nextLink`- oder `deltaLink`-URL aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="04369-127">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="04369-128">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="04369-128">Query parameter</span></span>      | <span data-ttu-id="04369-129">Typ</span><span class="sxs-lookup"><span data-stu-id="04369-129">Type</span></span>   |<span data-ttu-id="04369-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04369-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="04369-131">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="04369-131">$deltatoken</span></span> | <span data-ttu-id="04369-132">string</span><span class="sxs-lookup"><span data-stu-id="04369-132">string</span></span> | <span data-ttu-id="04369-p106">Ein [Statustoken](/graph/delta-query-overview), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Benutzersammlung zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.</span><span class="sxs-lookup"><span data-stu-id="04369-p106">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="04369-135">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="04369-135">$skiptoken</span></span> | <span data-ttu-id="04369-136">string</span><span class="sxs-lookup"><span data-stu-id="04369-136">string</span></span> | <span data-ttu-id="04369-137">Ein [Statustoken](/graph/delta-query-overview), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Benutzersammlung weitere Änderungen zum Nachverfolgen vorliegen.</span><span class="sxs-lookup"><span data-stu-id="04369-137">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="04369-138">OData-Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="04369-138">OData query parameters</span></span>

<span data-ttu-id="04369-139">Diese Methode unterstützt optionale Parameter der OData-Abfrage, mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="04369-139">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="04369-p107">Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft *id* wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04369-p107">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="04369-142">Es ist eingeschränkte Unterstützung für `$filter`:</span><span class="sxs-lookup"><span data-stu-id="04369-142">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="04369-143">Der einzige unterstützte `$filter`-Ausdruck dient zum Nachverfolgen von Änderungen an einem bestimmten Objekt: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="04369-143">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="04369-144">Sie können mehrere Objekte filtern.</span><span class="sxs-lookup"><span data-stu-id="04369-144">You can filter multiple objects.</span></span> <span data-ttu-id="04369-145">Beispiel: `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="04369-145">For example, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="04369-146">Es gilt ein Grenzwert von 50 gefilterten Objekten.</span><span class="sxs-lookup"><span data-stu-id="04369-146">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04369-147">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04369-147">Request headers</span></span>
| <span data-ttu-id="04369-148">Name</span><span class="sxs-lookup"><span data-stu-id="04369-148">Name</span></span>       | <span data-ttu-id="04369-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04369-149">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="04369-150">Authorization</span><span class="sxs-lookup"><span data-stu-id="04369-150">Authorization</span></span>  | <span data-ttu-id="04369-151">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="04369-151">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="04369-152">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04369-152">Content-Type</span></span>  | <span data-ttu-id="04369-153">application/json</span><span class="sxs-lookup"><span data-stu-id="04369-153">application/json</span></span> |
| <span data-ttu-id="04369-154">Prefer</span><span class="sxs-lookup"><span data-stu-id="04369-154">Prefer</span></span> | <span data-ttu-id="04369-155">zurückgeben = minimal</span><span class="sxs-lookup"><span data-stu-id="04369-155">return=minimal</span></span> <br><br><span data-ttu-id="04369-156">Angabe dieser Header mit einer Anforderung, die verwendet eine `deltaLink` würde zurückgeben nur die Eigenschaften des Objekts, die seit der letzten Round geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="04369-156">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="04369-157">Optional.</span><span class="sxs-lookup"><span data-stu-id="04369-157">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04369-158">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04369-158">Request body</span></span>
<span data-ttu-id="04369-159">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="04369-159">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="04369-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="04369-160">Response</span></span>

<span data-ttu-id="04369-161">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwort Code und [Benutzer](../resources/user.md) -Auflistungsobjekt in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="04369-161">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="04369-162">Die Antwort enthält außerdem eine `nextLink` URL oder eine `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="04369-162">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="04369-163">Wenn ein `nextLink` URL zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="04369-163">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="04369-164">Dies gibt an, dass es sind zusätzliche Seiten mit Daten aus der Sitzung abgerufen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="04369-164">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="04369-165">Die Anwendung weiterhin tätigen Anforderungen mithilfe der `nextLink` URL bis eine `deltaLink` URL in der Antwort enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="04369-165">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="04369-166">Die Antwort enthält den gleichen Satz an Eigenschaften wie in der ersten Delta abfrageanforderung.</span><span class="sxs-lookup"><span data-stu-id="04369-166">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="04369-167">Dadurch können Sie den vollständigen aktuellen Status der Objekte erfasst werden, wenn den Delta-Zyklus zu initiieren.</span><span class="sxs-lookup"><span data-stu-id="04369-167">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="04369-168">Wenn ein `deltaLink` URL zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="04369-168">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="04369-169">Dies gibt an, dass es sind keine weiteren Daten zum vorhandenen Status der Ressource zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="04369-169">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="04369-170">Speichern und verwenden Sie die `deltaLink` URL, um zu lernen in die Ressource in der nächsten Runde geändert.</span><span class="sxs-lookup"><span data-stu-id="04369-170">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="04369-171">Sie haben die Wahl zum Angeben der `Prefer:return=minimal` -Header in der Antwort nur Werte für die Eigenschaften enthalten, die seit der Ausführung geändert wurden die `deltaLink` ausgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="04369-171">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="04369-172">Standard: zurückzugeben Sie, die gleichen Eigenschaften als erste Delta-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04369-172">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="04369-173">Standardmäßig fordert mithilfe einer `deltaLink` oder `nextLink` dieselben Eigenschaften wie in der ersten Delta-Abfrage ausgewählten folgendermaßen zurückgeben:</span><span class="sxs-lookup"><span data-stu-id="04369-173">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="04369-174">Wenn die Eigenschaft geändert wurde, ist der neue Wert in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="04369-174">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="04369-175">Dies schließt Eigenschaften auf null-Wert festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="04369-175">This includes properties being set to null value.</span></span>
- <span data-ttu-id="04369-176">Wenn die Eigenschaft nicht geändert wurde, wird der alte Wert in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="04369-176">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="04369-177">Wenn die Eigenschaft nicht festgelegt wurde, bevor es nicht in der Antwort überhaupt eingeschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="04369-177">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="04369-178">**Hinweis:** Mit diesem Verhalten ist die Antwort verfolgen es nicht möglich, sagen, ob eine Eigenschaft oder nicht geändert wird.</span><span class="sxs-lookup"><span data-stu-id="04369-178">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="04369-179">Darüber hinaus meist die Antworten Delta groß sein, da sie alle Eigenschaftswerte - enthalten wie im [zweiten Beispiel](#request-2) unten dargestellt.</span><span class="sxs-lookup"><span data-stu-id="04369-179">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="04369-180">Alternative: nur die geänderten Eigenschaften zurückgeben</span><span class="sxs-lookup"><span data-stu-id="04369-180">Alternative: return only the changed properties</span></span>

<span data-ttu-id="04369-181">Hinzufügen einer optionalen Anforderungsheader - `prefer:return=minimal` -führt das folgende Verhalten:</span><span class="sxs-lookup"><span data-stu-id="04369-181">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="04369-182">Wenn die Eigenschaft geändert wurde, ist der neue Wert in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="04369-182">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="04369-183">Dies schließt Eigenschaften auf null-Wert festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="04369-183">This includes properties being set to null value.</span></span>
- <span data-ttu-id="04369-184">Wenn die Eigenschaft nicht geändert wurde, ist die Eigenschaft nicht in allen in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="04369-184">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="04369-185">(Andere als das Standardverhalten).</span><span class="sxs-lookup"><span data-stu-id="04369-185">(Different from the default behavior.)</span></span>

> <span data-ttu-id="04369-186">**Hinweis:** Die Kopfzeile hinzugefügt werden kann einen `deltaLink` Anforderung an einer beliebigen Stelle in Zeit im Zyklus Delta.</span><span class="sxs-lookup"><span data-stu-id="04369-186">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="04369-187">Die Kopfzeile wirkt sich nur auf die Gruppe von Eigenschaften, die in der Antwort enthalten, und er hat keinen Einfluss auf wie die Delta-Abfrage ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="04369-187">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="04369-188">Finden Sie im [dritten Beispiel](#request-3) unten.</span><span class="sxs-lookup"><span data-stu-id="04369-188">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="04369-189">Beispiel</span><span class="sxs-lookup"><span data-stu-id="04369-189">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="04369-190">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="04369-190">Request 1</span></span>

<span data-ttu-id="04369-191">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="04369-191">The following is an example of the request.</span></span> <span data-ttu-id="04369-192">Es ist keine `$select` Parameter, damit ein Standardsatz Eigenschaften nachverfolgt und zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="04369-192">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="04369-193">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="04369-193">Response 1</span></span>

<span data-ttu-id="04369-194">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="04369-194">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="04369-p120">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="04369-p120">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "businessPhones": [
          "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

#### <a name="request-2"></a><span data-ttu-id="04369-197">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="04369-197">Request 2</span></span>

<span data-ttu-id="04369-198">Das nächste Beispiel veranschaulicht die erste Anforderung 3 Eigenschaften für nachverfolgen Antwort Standardverhalten auswählen:</span><span class="sxs-lookup"><span data-stu-id="04369-198">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="04369-199">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="04369-199">Response 2</span></span>

<span data-ttu-id="04369-200">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="04369-200">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="04369-201">Beachten Sie, dass alle 3 Eigenschaften sind in der Antwort enthalten, und es nicht bekannt ist, welche geändert wurden, seit die `deltaLink` abgerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="04369-201">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": "jobTitle-value",
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="04369-202">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="04369-202">Request 3</span></span>

<span data-ttu-id="04369-203">Das nächste Beispiel veranschaulicht die erste Anforderung 3 Eigenschaften für nachverfolgen mit alternativen minimale Antwort Verhalten auswählen:</span><span class="sxs-lookup"><span data-stu-id="04369-203">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="04369-204">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="04369-204">Response 3</span></span>

<span data-ttu-id="04369-205">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="04369-205">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="04369-206">Beachten Sie, dass die `mobilePhone` -Eigenschaft ist nicht enthalten, was bedeutet, dass wurde nicht geändert seit der letzten Delta-Abfrage; `displayName` und `jobTitle` sind enthalten, d. h., deren Werte geändert haben.</span><span class="sxs-lookup"><span data-stu-id="04369-206">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```

- <span data-ttu-id="04369-207">[Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten verwenden](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="04369-207">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="04369-208">[Inkrementelle Änderungen für Benutzer erhalten möchten](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="04369-208">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
