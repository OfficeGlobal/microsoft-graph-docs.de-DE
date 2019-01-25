---
title: 'user: delta'
description: Get neu erstellt, aktualisiert oder Benutzer ohne Durchführung ein alles Lesen der gesamten Benutzer-Auflistung gelöscht. Finden Sie unter Nachverfolgen von Änderungen für Details.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6fd8eb71c1b647550219ae6686a0bc814420b2fa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508902"
---
# <a name="user-delta"></a><span data-ttu-id="45881-104">user: delta</span><span class="sxs-lookup"><span data-stu-id="45881-104">user: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45881-105">Get neu erstellt, aktualisiert oder Benutzer ohne Durchführung ein alles Lesen der gesamten Benutzer-Auflistung gelöscht.</span><span class="sxs-lookup"><span data-stu-id="45881-105">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="45881-106">Einzelheiten finden Sie unter [Nachverfolgen von Änderungen](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="45881-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="45881-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="45881-107">Permissions</span></span>

<span data-ttu-id="45881-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45881-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="45881-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="45881-110">Permission type</span></span>      | <span data-ttu-id="45881-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="45881-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45881-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="45881-112">Delegated (work or school account)</span></span> | <span data-ttu-id="45881-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="45881-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="45881-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="45881-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45881-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45881-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="45881-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="45881-116">Application</span></span> | <span data-ttu-id="45881-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45881-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45881-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="45881-118">HTTP request</span></span>

<span data-ttu-id="45881-119">Um Änderungen nachzuverfolgen, führen Sie zunächst eine Anforderung einschließlich der delta-Funktion für die Benutzerressource aus.</span><span class="sxs-lookup"><span data-stu-id="45881-119">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="45881-120">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="45881-120">Query parameters</span></span>

<span data-ttu-id="45881-121">Nachverfolgen von Änderungen in Benutzer verursacht eine Rundung eine oder mehrere **Delta** Funktionsaufrufe.</span><span class="sxs-lookup"><span data-stu-id="45881-121">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="45881-122">Wenn Sie eine beliebige Abfragezeichenfolgen-Parameter verwenden (außer `$deltatoken` und `$skiptoken`), müssen Sie es in die erste **Delta** -Anforderung angeben.</span><span class="sxs-lookup"><span data-stu-id="45881-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="45881-123">Microsoft Graph codiert angegebenen Parameter automatisch in den token Teil der `nextLink` oder `deltaLink` URL auf, die in der Antwort.</span><span class="sxs-lookup"><span data-stu-id="45881-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="45881-124">Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben.</span><span class="sxs-lookup"><span data-stu-id="45881-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="45881-125">In nachfolgenden Anforderungen können Sie die  `nextLink`- oder `deltaLink`-URL aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="45881-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="45881-126">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="45881-126">Query parameter</span></span>      | <span data-ttu-id="45881-127">Typ</span><span class="sxs-lookup"><span data-stu-id="45881-127">Type</span></span>   |<span data-ttu-id="45881-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45881-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="45881-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="45881-129">$deltatoken</span></span> | <span data-ttu-id="45881-130">string</span><span class="sxs-lookup"><span data-stu-id="45881-130">string</span></span> | <span data-ttu-id="45881-p105">Ein [Statustoken](/graph/delta-query-overview), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Benutzersammlung zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.</span><span class="sxs-lookup"><span data-stu-id="45881-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="45881-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="45881-133">$skiptoken</span></span> | <span data-ttu-id="45881-134">string</span><span class="sxs-lookup"><span data-stu-id="45881-134">string</span></span> | <span data-ttu-id="45881-135">Ein [Statustoken](/graph/delta-query-overview), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Benutzersammlung weitere Änderungen zum Nachverfolgen vorliegen.</span><span class="sxs-lookup"><span data-stu-id="45881-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="45881-136">OData-Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="45881-136">OData query parameters</span></span>

<span data-ttu-id="45881-137">Diese Methode unterstützt optionale Parameter der OData-Abfrage, mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="45881-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="45881-p106">Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft *id* wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="45881-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="45881-140">Es ist eingeschränkte Unterstützung für `$filter`:</span><span class="sxs-lookup"><span data-stu-id="45881-140">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="45881-141">Der einzige unterstützte `$filter`-Ausdruck dient zum Nachverfolgen von Änderungen an einem bestimmten Objekt: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="45881-141">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="45881-142">Sie können mehrere Objekte filtern.</span><span class="sxs-lookup"><span data-stu-id="45881-142">You can filter multiple objects.</span></span> <span data-ttu-id="45881-143">Beispiel: `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="45881-143">For example, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="45881-144">Es gilt ein Grenzwert von 50 gefilterten Objekten.</span><span class="sxs-lookup"><span data-stu-id="45881-144">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45881-145">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="45881-145">Request headers</span></span>
| <span data-ttu-id="45881-146">Name</span><span class="sxs-lookup"><span data-stu-id="45881-146">Name</span></span>       | <span data-ttu-id="45881-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45881-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="45881-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="45881-148">Authorization</span></span>  | <span data-ttu-id="45881-149">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="45881-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="45881-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="45881-150">Content-Type</span></span>  | <span data-ttu-id="45881-151">application/json</span><span class="sxs-lookup"><span data-stu-id="45881-151">application/json</span></span> |
| <span data-ttu-id="45881-152">Prefer</span><span class="sxs-lookup"><span data-stu-id="45881-152">Prefer</span></span> | <span data-ttu-id="45881-153">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="45881-153">return=minimal</span></span> <br><br><span data-ttu-id="45881-154">Angabe dieser Header mit einer Anforderung, die verwendet eine `deltaLink` würde zurückgeben nur die Eigenschaften des Objekts, die seit der letzten Round geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="45881-154">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="45881-155">Optional.</span><span class="sxs-lookup"><span data-stu-id="45881-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45881-156">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="45881-156">Request body</span></span>
<span data-ttu-id="45881-157">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="45881-157">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="45881-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="45881-158">Response</span></span>

<span data-ttu-id="45881-159">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwort Code und [Benutzer](../resources/user.md) -Auflistungsobjekt in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="45881-159">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="45881-160">Die Antwort enthält außerdem eine `nextLink` URL oder eine `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="45881-160">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="45881-161">Wenn ein `nextLink` URL zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="45881-161">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="45881-162">Dies gibt an, dass es sind zusätzliche Seiten mit Daten aus der Sitzung abgerufen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="45881-162">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="45881-163">Die Anwendung weiterhin tätigen Anforderungen mithilfe der `nextLink` URL bis eine `deltaLink` URL in der Antwort enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="45881-163">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="45881-164">Die Antwort enthält den gleichen Satz an Eigenschaften wie in der ersten Delta abfrageanforderung.</span><span class="sxs-lookup"><span data-stu-id="45881-164">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="45881-165">Dadurch können Sie den vollständigen aktuellen Status der Objekte erfasst werden, wenn den Delta-Zyklus zu initiieren.</span><span class="sxs-lookup"><span data-stu-id="45881-165">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="45881-166">Wenn ein `deltaLink` URL zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="45881-166">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="45881-167">Dies gibt an, dass es sind keine weiteren Daten zum vorhandenen Status der Ressource zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="45881-167">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="45881-168">Speichern und verwenden Sie die `deltaLink` URL, um zu lernen in die Ressource in der nächsten Runde geändert.</span><span class="sxs-lookup"><span data-stu-id="45881-168">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="45881-169">Sie haben die Wahl zum Angeben der `Prefer:return=minimal` -Header in der Antwort nur Werte für die Eigenschaften enthalten, die seit der Ausführung geändert wurden die `deltaLink` ausgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="45881-169">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="45881-170">Standard: zurückzugeben Sie, die gleichen Eigenschaften als erste Delta-Anforderung</span><span class="sxs-lookup"><span data-stu-id="45881-170">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="45881-171">Standardmäßig fordert mithilfe einer `deltaLink` oder `nextLink` dieselben Eigenschaften wie in der ersten Delta-Abfrage ausgewählten folgendermaßen zurückgeben:</span><span class="sxs-lookup"><span data-stu-id="45881-171">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="45881-172">Wenn die Eigenschaft geändert wurde, ist der neue Wert in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="45881-172">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="45881-173">Dies schließt Eigenschaften auf null-Wert festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="45881-173">This includes properties being set to null value.</span></span>
- <span data-ttu-id="45881-174">Wenn die Eigenschaft nicht geändert wurde, wird der alte Wert in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="45881-174">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="45881-175">Wenn die Eigenschaft nicht festgelegt wurde, bevor es nicht in der Antwort überhaupt eingeschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="45881-175">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="45881-176">**Hinweis:** Mit diesem Verhalten ist die Antwort verfolgen es nicht möglich, sagen, ob eine Eigenschaft oder nicht geändert wird.</span><span class="sxs-lookup"><span data-stu-id="45881-176">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="45881-177">Darüber hinaus meist die Antworten Delta groß sein, da sie alle Eigenschaftswerte - enthalten wie im [zweiten Beispiel](#request-2) unten dargestellt.</span><span class="sxs-lookup"><span data-stu-id="45881-177">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="45881-178">Alternative: nur die geänderten Eigenschaften zurückgeben</span><span class="sxs-lookup"><span data-stu-id="45881-178">Alternative: return only the changed properties</span></span>

<span data-ttu-id="45881-179">Hinzufügen einer optionalen Anforderungsheader - `prefer:return=minimal` -führt das folgende Verhalten:</span><span class="sxs-lookup"><span data-stu-id="45881-179">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="45881-180">Wenn die Eigenschaft geändert wurde, ist der neue Wert in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="45881-180">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="45881-181">Dies schließt Eigenschaften auf null-Wert festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="45881-181">This includes properties being set to null value.</span></span>
- <span data-ttu-id="45881-182">Wenn die Eigenschaft nicht geändert wurde, ist die Eigenschaft nicht in allen in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="45881-182">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="45881-183">(Andere als das Standardverhalten).</span><span class="sxs-lookup"><span data-stu-id="45881-183">(Different from the default behavior.)</span></span>

> <span data-ttu-id="45881-184">**Hinweis:** Die Kopfzeile hinzugefügt werden kann einen `deltaLink` Anforderung an einer beliebigen Stelle in Zeit im Zyklus Delta.</span><span class="sxs-lookup"><span data-stu-id="45881-184">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="45881-185">Die Kopfzeile wirkt sich nur auf die Gruppe von Eigenschaften, die in der Antwort enthalten, und er hat keinen Einfluss auf wie die Delta-Abfrage ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="45881-185">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="45881-186">Finden Sie im [dritten Beispiel](#request-3) unten.</span><span class="sxs-lookup"><span data-stu-id="45881-186">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="45881-187">Beispiel</span><span class="sxs-lookup"><span data-stu-id="45881-187">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="45881-188">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="45881-188">Request 1</span></span>

<span data-ttu-id="45881-189">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="45881-189">The following is an example of the request.</span></span> <span data-ttu-id="45881-190">Es ist keine `$select` Parameter, damit ein Standardsatz Eigenschaften nachverfolgt und zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="45881-190">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="45881-191">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="45881-191">Response 1</span></span>

<span data-ttu-id="45881-192">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="45881-192">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="45881-p119">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="45881-p119">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="45881-195">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="45881-195">Request 2</span></span>

<span data-ttu-id="45881-196">Das nächste Beispiel veranschaulicht die erste Anforderung 3 Eigenschaften für nachverfolgen Antwort Standardverhalten auswählen:</span><span class="sxs-lookup"><span data-stu-id="45881-196">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="45881-197">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="45881-197">Response 2</span></span>

<span data-ttu-id="45881-198">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="45881-198">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="45881-199">Beachten Sie, dass alle 3 Eigenschaften sind in der Antwort enthalten, und es nicht bekannt ist, welche geändert wurden, seit die `deltaLink` abgerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="45881-199">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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

#### <a name="request-3"></a><span data-ttu-id="45881-200">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="45881-200">Request 3</span></span>

<span data-ttu-id="45881-201">Das nächste Beispiel veranschaulicht die erste Anforderung 3 Eigenschaften für nachverfolgen mit alternativen minimale Antwort Verhalten auswählen:</span><span class="sxs-lookup"><span data-stu-id="45881-201">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="45881-202">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="45881-202">Response 3</span></span>

<span data-ttu-id="45881-203">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="45881-203">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="45881-204">Beachten Sie, dass die `mobilePhone` -Eigenschaft ist nicht enthalten, was bedeutet, dass wurde nicht geändert seit der letzten Delta-Abfrage; `displayName` und `jobTitle` sind enthalten, d. h., deren Werte geändert haben.</span><span class="sxs-lookup"><span data-stu-id="45881-204">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

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

- <span data-ttu-id="45881-205">[Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="45881-205">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="45881-206">[Abrufen inkrementeller Änderungen für Benutzer](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="45881-206">[Get incremental changes for users](/graph/delta-query-users).</span></span>

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
    "Error: /api-reference/beta/api/user-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
