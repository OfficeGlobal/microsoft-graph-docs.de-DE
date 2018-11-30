---
title: 'DirectoryRole: Delta'
description: Get neu erstellt, aktualisiert oder gelöscht Directory Rollen ohne ein alles Lesen der gesamte Ressource Auflistung ausführen. Einzelheiten finden Sie unter Delta-Abfrage verwenden.
ms.openlocfilehash: b426dd10ead2d1fc34c1d64aa235c343e8e71c3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058357"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="b8993-104">DirectoryRole: Delta</span><span class="sxs-lookup"><span data-stu-id="b8993-104">directoryRole: delta</span></span>

> <span data-ttu-id="b8993-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b8993-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8993-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8993-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8993-107">Get neu erstellt, aktualisiert oder gelöscht Directory Rollen ohne ein alles Lesen der gesamte Ressource Auflistung ausführen.</span><span class="sxs-lookup"><span data-stu-id="b8993-107">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="b8993-108">Einzelheiten finden Sie unter [Delta-Abfrage verwenden](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="b8993-108">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8993-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b8993-109">Permissions</span></span>

<span data-ttu-id="b8993-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8993-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b8993-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8993-112">Permission type</span></span>      | <span data-ttu-id="b8993-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8993-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8993-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8993-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b8993-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b8993-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b8993-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8993-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8993-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8993-117">Not supported.</span></span>    |
|<span data-ttu-id="b8993-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8993-118">Application</span></span> | <span data-ttu-id="b8993-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8993-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8993-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8993-120">HTTP request</span></span>

<span data-ttu-id="b8993-121">Zum Nachverfolgen von Änderungen beginnen, stellen Sie eine Anforderung, einschließlich der Delta-Funktion für die Ressource DirectoryRole.</span><span class="sxs-lookup"><span data-stu-id="b8993-121">To begin tracking changes, you make a request including the delta function on the directoryRole resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

### <a name="query-parameters"></a><span data-ttu-id="b8993-122">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b8993-122">Query parameters</span></span>

<span data-ttu-id="b8993-123">Nachverfolgen von Änderungen verursacht eine Rundung eine oder mehrere **Delta** Funktionsaufrufe.</span><span class="sxs-lookup"><span data-stu-id="b8993-123">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="b8993-124">Wenn Sie eine beliebige Abfragezeichenfolgen-Parameter verwenden (außer `$deltatoken` und `$skiptoken`), müssen Sie es in die erste **Delta** -Anforderung angeben.</span><span class="sxs-lookup"><span data-stu-id="b8993-124">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="b8993-125">Microsoft Graph codiert angegebenen Parameter automatisch in den token Teil der `nextLink` oder `deltaLink` URL auf, die in der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b8993-125">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="b8993-126">Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben.</span><span class="sxs-lookup"><span data-stu-id="b8993-126">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="b8993-127">In nachfolgenden Anforderungen können Sie die  `nextLink`- oder `deltaLink`-URL aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="b8993-127">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="b8993-128">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b8993-128">Query parameter</span></span>      | <span data-ttu-id="b8993-129">Typ</span><span class="sxs-lookup"><span data-stu-id="b8993-129">Type</span></span>   |<span data-ttu-id="b8993-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8993-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b8993-131">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="b8993-131">$deltatoken</span></span> | <span data-ttu-id="b8993-132">string</span><span class="sxs-lookup"><span data-stu-id="b8993-132">string</span></span> | <span data-ttu-id="b8993-133">Ein [Token Zustand](/graph/delta-query-overview) zurückgegeben, die der `deltaLink` URL des vorherigen **Delta** Funktionsaufrufs für dieselbe Ressource-Auflistung zurück, der angibt, Rundung des Änderungsprotokolls nach Abschluss.</span><span class="sxs-lookup"><span data-stu-id="b8993-133">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="b8993-134">Speichern und übernehmen Sie die gesamte `deltaLink` URL einschließlich dieses Token in die erste Anforderung der nächsten der Versionsvergleich für diese Auflistung.</span><span class="sxs-lookup"><span data-stu-id="b8993-134">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="b8993-135">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="b8993-135">$skiptoken</span></span> | <span data-ttu-id="b8993-136">string</span><span class="sxs-lookup"><span data-stu-id="b8993-136">string</span></span> | <span data-ttu-id="b8993-137">Ein [Token Zustand](/graph/delta-query-overview) zurückgegeben, die der `nextLink` URL von der vorherigen **Delta** -Funktionsaufruf, der angibt, es sind weitere Änderungen in der gleichen Auflistung Ressource überwacht werden müssen.</span><span class="sxs-lookup"><span data-stu-id="b8993-137">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="b8993-138">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b8993-138">Optional query parameters</span></span>

<span data-ttu-id="b8993-139">Diese Methode unterstützt OData-Abfrageparameter zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b8993-139">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="b8993-p107">Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft _id_ wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8993-p107">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="b8993-142">Es ist eingeschränkte Unterstützung für `$filter`:</span><span class="sxs-lookup"><span data-stu-id="b8993-142">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="b8993-143">Der einzige unterstützte `$filter` Ausdruck ist für das Nachverfolgen von Änderungen für bestimmte Ressourcen anhand ihrer Id: `$filter=id+eq+{value}` oder `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="b8993-143">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="b8993-144">Die Anzahl der Ids, die Sie angeben können, wird durch die maximale Länge des URL begrenzt.</span><span class="sxs-lookup"><span data-stu-id="b8993-144">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="b8993-145">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8993-145">Request headers</span></span>
| <span data-ttu-id="b8993-146">Name</span><span class="sxs-lookup"><span data-stu-id="b8993-146">Name</span></span>       | <span data-ttu-id="b8993-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8993-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b8993-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8993-148">Authorization</span></span>  | <span data-ttu-id="b8993-149">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="b8993-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="b8993-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8993-150">Content-Type</span></span>  | <span data-ttu-id="b8993-151">application/json</span><span class="sxs-lookup"><span data-stu-id="b8993-151">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8993-152">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8993-152">Request body</span></span>
<span data-ttu-id="b8993-153">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b8993-153">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="b8993-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8993-154">Response</span></span>

<span data-ttu-id="b8993-155">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwort Code und [DirectoryRole](../resources/directoryrole.md) -Auflistungsobjekt in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b8993-155">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="b8993-156">Die Antwort enthält auch ein NextLink oder eine DeltaLink-URL.</span><span class="sxs-lookup"><span data-stu-id="b8993-156">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="b8993-157">Wenn ein `nextLink` URL zurückgegeben wird, stehen Ihnen zusätzliche Seiten mit Daten aus der Sitzung abgerufen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b8993-157">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="b8993-158">Die Anwendung weiterhin tätigen Anforderungen mithilfe der `nextLink` URL bis eine `deltaLink` URL in der Antwort enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="b8993-158">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="b8993-159">Wenn ein `deltaLink` URL wird zurückgegeben, es sind keine weiteren Daten zum vorhandenen Status der Ressource zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="b8993-159">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="b8993-160">Speichern und verwenden Sie die `deltaLink` URL, um Informationen zu Änderungen an der Ressource in der Zukunft zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="b8993-160">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="b8993-161">Siehe:</span><span class="sxs-lookup"><span data-stu-id="b8993-161">See:</span></span></br>
- <span data-ttu-id="b8993-162">Weitere Informationen finden Sie unter [Verwenden einer Delta-Abfrage](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="b8993-162">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="b8993-163">Beispielanforderungen finden Sie unter [Inkrementelle Änderungen für Benutzer abrufen](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="b8993-163">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="b8993-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8993-164">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8993-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8993-165">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/delta
```

##### <a name="response"></a><span data-ttu-id="b8993-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8993-166">Response</span></span>
<span data-ttu-id="b8993-p112">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8993-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryRoles",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryRoles/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
      {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->