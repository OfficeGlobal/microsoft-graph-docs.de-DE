---
title: 'DirectoryRole: Delta'
description: Get neu erstellt, aktualisiert oder gelöscht Directory Rollen ohne ein alles Lesen der gesamte Ressource Auflistung ausführen. Einzelheiten finden Sie unter Delta-Abfrage verwenden.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6da3e8c4cf92edbf79df1b082675c36d54e81292
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923839"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="4848a-104">DirectoryRole: Delta</span><span class="sxs-lookup"><span data-stu-id="4848a-104">directoryRole: delta</span></span>

<span data-ttu-id="4848a-105">Get neu erstellt, aktualisiert oder gelöscht Directory Rollen ohne ein alles Lesen der gesamte Ressource Auflistung ausführen.</span><span class="sxs-lookup"><span data-stu-id="4848a-105">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="4848a-106">Einzelheiten finden Sie unter [Delta-Abfrage verwenden](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="4848a-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="4848a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4848a-107">Permissions</span></span>

<span data-ttu-id="4848a-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4848a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4848a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4848a-110">Permission type</span></span>      | <span data-ttu-id="4848a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4848a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4848a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4848a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4848a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4848a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4848a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4848a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4848a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4848a-115">Not supported.</span></span>    |
|<span data-ttu-id="4848a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4848a-116">Application</span></span> | <span data-ttu-id="4848a-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4848a-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4848a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4848a-118">HTTP request</span></span>

<span data-ttu-id="4848a-119">Zum Nachverfolgen von Änderungen beginnen, stellen Sie eine Anforderung, einschließlich der **Delta** -Funktion für die Ressource [DirectoryRole](../resources/directoryrole.md) .</span><span class="sxs-lookup"><span data-stu-id="4848a-119">To begin tracking changes, you make a request including the **delta** function on the [directoryRole](../resources/directoryrole.md) resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

## <a name="query-parameters"></a><span data-ttu-id="4848a-120">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4848a-120">Query parameters</span></span>

<span data-ttu-id="4848a-121">Nachverfolgen von Änderungen verursacht eine Rundung eine oder mehrere **Delta** Funktionsaufrufe.</span><span class="sxs-lookup"><span data-stu-id="4848a-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="4848a-122">Wenn Sie eine beliebige Abfragezeichenfolgen-Parameter verwenden (außer `$deltatoken` und `$skiptoken`), müssen Sie es in die erste **Delta** -Anforderung angeben.</span><span class="sxs-lookup"><span data-stu-id="4848a-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="4848a-123">Microsoft Graph codiert angegebenen Parameter automatisch in den token Teil der `nextLink` oder `deltaLink` URL auf, die in der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4848a-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="4848a-124">Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben.</span><span class="sxs-lookup"><span data-stu-id="4848a-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="4848a-125">In nachfolgenden Anforderungen können Sie die  `nextLink`- oder `deltaLink`-URL aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="4848a-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="4848a-126">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4848a-126">Query parameter</span></span>      | <span data-ttu-id="4848a-127">Typ</span><span class="sxs-lookup"><span data-stu-id="4848a-127">Type</span></span>   |<span data-ttu-id="4848a-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4848a-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4848a-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="4848a-129">$deltatoken</span></span> | <span data-ttu-id="4848a-130">string</span><span class="sxs-lookup"><span data-stu-id="4848a-130">string</span></span> | <span data-ttu-id="4848a-131">Ein [Token Zustand](/graph/delta-query-overview) zurückgegeben, die der `deltaLink` URL des vorherigen **Delta** Funktionsaufrufs für dieselbe Ressource-Auflistung zurück, der angibt, Rundung des Änderungsprotokolls nach Abschluss.</span><span class="sxs-lookup"><span data-stu-id="4848a-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="4848a-132">Speichern und übernehmen Sie die gesamte `deltaLink` URL einschließlich dieses Token in die erste Anforderung der nächsten der Versionsvergleich für diese Auflistung.</span><span class="sxs-lookup"><span data-stu-id="4848a-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="4848a-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="4848a-133">$skiptoken</span></span> | <span data-ttu-id="4848a-134">string</span><span class="sxs-lookup"><span data-stu-id="4848a-134">string</span></span> | <span data-ttu-id="4848a-135">Ein [Token Zustand](/graph/delta-query-overview) zurückgegeben, die der `nextLink` URL von der vorherigen **Delta** -Funktionsaufruf, der angibt, es sind weitere Änderungen in der gleichen Auflistung Ressource überwacht werden müssen.</span><span class="sxs-lookup"><span data-stu-id="4848a-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="4848a-136">OData-Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4848a-136">OData query parameters</span></span>

<span data-ttu-id="4848a-137">Diese Methode unterstützt OData-Abfrage-Parameter, mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="4848a-137">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="4848a-p106">Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft _id_ wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4848a-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span>

- <span data-ttu-id="4848a-140">Es ist eingeschränkte Unterstützung für `$filter`:</span><span class="sxs-lookup"><span data-stu-id="4848a-140">There is limited support for `$filter`:</span></span>

  - <span data-ttu-id="4848a-141">Der einzige unterstützte `$filter` Ausdruck ist für das Nachverfolgen von Änderungen für bestimmte Ressourcen anhand ihrer Id: `$filter=id+eq+{value}` oder `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="4848a-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="4848a-142">Die Anzahl der Ids, die Sie angeben können, wird durch die maximale Länge des URL begrenzt.</span><span class="sxs-lookup"><span data-stu-id="4848a-142">The number of ids you can specify is limited by the maximum URL length.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4848a-143">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4848a-143">Request headers</span></span>

| <span data-ttu-id="4848a-144">Name</span><span class="sxs-lookup"><span data-stu-id="4848a-144">Name</span></span>       | <span data-ttu-id="4848a-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4848a-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4848a-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="4848a-146">Authorization</span></span>  | <span data-ttu-id="4848a-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="4848a-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="4848a-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4848a-148">Content-Type</span></span>  | <span data-ttu-id="4848a-149">application/json</span><span class="sxs-lookup"><span data-stu-id="4848a-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4848a-150">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4848a-150">Request body</span></span>

<span data-ttu-id="4848a-151">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4848a-151">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="4848a-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="4848a-152">Response</span></span>

<span data-ttu-id="4848a-153">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwort Code und [DirectoryRole](../resources/directoryrole.md) -Auflistungsobjekt in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4848a-153">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="4848a-154">Die Antwort enthält außerdem eine `nextLink` URL oder eine `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="4848a-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="4848a-155">Wenn ein `nextLink` URL zurückgegeben wird, stehen Ihnen zusätzliche Seiten mit Daten aus der Sitzung abgerufen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="4848a-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="4848a-156">Die Anwendung weiterhin tätigen Anforderungen mithilfe der `nextLink` URL bis eine `deltaLink` URL in der Antwort enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="4848a-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="4848a-157">Wenn ein `deltaLink` URL wird zurückgegeben, es sind keine weiteren Daten zum vorhandenen Status der Ressource zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="4848a-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="4848a-158">Speichern Sie `deltaLink` URL, und wenden Sie es im nächsten **Delta** Aufruf über Änderungen an der Ressource in der Zukunft zu informieren.</span><span class="sxs-lookup"><span data-stu-id="4848a-158">Save `deltaLink` URL and apply it in the next **delta** call to learn about changes to the resource in the future.</span></span>

### <a name="example"></a><span data-ttu-id="4848a-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4848a-159">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4848a-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4848a-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/directoryRoles/delta
```

##### <a name="response"></a><span data-ttu-id="4848a-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="4848a-161">Response</span></span>

<span data-ttu-id="4848a-p111">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4848a-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryRoles",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/directoryRoles/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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

### <a name="see-also"></a><span data-ttu-id="4848a-164">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="4848a-164">See also</span></span>

- <span data-ttu-id="4848a-165">[Verwendung Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten](/graph/delta-query-overview) für weitere details</span><span class="sxs-lookup"><span data-stu-id="4848a-165">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview) for more details</span></span>
- <span data-ttu-id="4848a-166">Beispielanforderungen finden Sie unter [Inkrementelle Änderungen für Benutzer abrufen](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="4848a-166">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
