---
title: 'Anwendung: Delta'
description: Get neu erstellt, aktualisiert oder gelöscht Applications ohne ein alles Lesen der gesamte Ressource Auflistung ausführen. Einzelheiten finden Sie unter Delta-Abfrage verwenden.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 13b6f7809cf47edcc9de8c9ddfb052645b15f25a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517071"
---
# <a name="application-delta"></a><span data-ttu-id="77035-104">Anwendung: Delta</span><span class="sxs-lookup"><span data-stu-id="77035-104">application: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77035-105">Get neu erstellt, aktualisiert oder gelöscht Applications ohne ein alles Lesen der gesamte Ressource Auflistung ausführen.</span><span class="sxs-lookup"><span data-stu-id="77035-105">Get newly created, updated, or deleted applications without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="77035-106">Einzelheiten finden Sie unter [Delta-Abfrage verwenden](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="77035-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="77035-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="77035-107">Permissions</span></span>

<span data-ttu-id="77035-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77035-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="77035-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77035-110">Permission type</span></span>      | <span data-ttu-id="77035-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77035-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77035-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77035-112">Delegated (work or school account)</span></span> | <span data-ttu-id="77035-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="77035-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="77035-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77035-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77035-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77035-115">Not supported.</span></span>    |
|<span data-ttu-id="77035-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77035-116">Application</span></span> | <span data-ttu-id="77035-117">Application.ReadWrite.All Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="77035-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77035-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77035-118">HTTP request</span></span>

<span data-ttu-id="77035-119">Zum Nachverfolgen von Änderungen beginnen, stellen Sie eine Anforderung, einschließlich der Delta-Funktion für die Anwendungsressource.</span><span class="sxs-lookup"><span data-stu-id="77035-119">To begin tracking changes, you make a request including the delta function on the application resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /applications/delta
```

### <a name="query-parameters"></a><span data-ttu-id="77035-120">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="77035-120">Query parameters</span></span>

<span data-ttu-id="77035-121">Nachverfolgen von Änderungen verursacht eine Rundung eine oder mehrere **Delta** Funktionsaufrufe.</span><span class="sxs-lookup"><span data-stu-id="77035-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="77035-122">Wenn Sie eine beliebige Abfragezeichenfolgen-Parameter verwenden (außer `$deltatoken` und `$skiptoken`), müssen Sie es in die erste **Delta** -Anforderung angeben.</span><span class="sxs-lookup"><span data-stu-id="77035-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="77035-123">Microsoft Graph codiert angegebenen Parameter automatisch in den token Teil der `nextLink` oder `deltaLink` URL auf, die in der Antwort.</span><span class="sxs-lookup"><span data-stu-id="77035-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="77035-124">Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben.</span><span class="sxs-lookup"><span data-stu-id="77035-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="77035-125">In nachfolgenden Anforderungen können Sie die  `nextLink`- oder `deltaLink`-URL aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="77035-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="77035-126">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="77035-126">Query parameter</span></span>      | <span data-ttu-id="77035-127">Typ</span><span class="sxs-lookup"><span data-stu-id="77035-127">Type</span></span>   |<span data-ttu-id="77035-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77035-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="77035-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="77035-129">$deltatoken</span></span> | <span data-ttu-id="77035-130">string</span><span class="sxs-lookup"><span data-stu-id="77035-130">string</span></span> | <span data-ttu-id="77035-131">Ein [Token Zustand](/graph/delta-query-overview) zurückgegeben, die der `deltaLink` URL des vorherigen **Delta** Funktionsaufrufs für dieselbe Ressource-Auflistung zurück, der angibt, Rundung des Änderungsprotokolls nach Abschluss.</span><span class="sxs-lookup"><span data-stu-id="77035-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="77035-132">Speichern und übernehmen Sie die gesamte `deltaLink` URL einschließlich dieses Token in die erste Anforderung der nächsten der Versionsvergleich für diese Auflistung.</span><span class="sxs-lookup"><span data-stu-id="77035-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="77035-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="77035-133">$skiptoken</span></span> | <span data-ttu-id="77035-134">string</span><span class="sxs-lookup"><span data-stu-id="77035-134">string</span></span> | <span data-ttu-id="77035-135">Ein [Token Zustand](/graph/delta-query-overview) zurückgegeben, die der `nextLink` URL von der vorherigen **Delta** -Funktionsaufruf, der angibt, es sind weitere Änderungen in der gleichen Auflistung Ressource überwacht werden müssen.</span><span class="sxs-lookup"><span data-stu-id="77035-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="77035-136">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="77035-136">Optional query parameters</span></span>

<span data-ttu-id="77035-137">Diese Methode unterstützt OData-Abfrageparameter zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="77035-137">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="77035-p106">Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft _id_ wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77035-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="77035-140">Es ist eingeschränkte Unterstützung für `$filter`:</span><span class="sxs-lookup"><span data-stu-id="77035-140">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="77035-141">Der einzige unterstützte `$filter` Ausdruck ist für das Nachverfolgen von Änderungen für bestimmte Ressourcen anhand ihrer Id: `$filter=id+eq+{value}` oder `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="77035-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="77035-142">Die Anzahl der Ids, die Sie angeben können, wird durch die maximale Länge des URL begrenzt.</span><span class="sxs-lookup"><span data-stu-id="77035-142">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="77035-143">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77035-143">Request headers</span></span>
| <span data-ttu-id="77035-144">Name</span><span class="sxs-lookup"><span data-stu-id="77035-144">Name</span></span>       | <span data-ttu-id="77035-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77035-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="77035-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="77035-146">Authorization</span></span>  | <span data-ttu-id="77035-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="77035-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="77035-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="77035-148">Content-Type</span></span>  | <span data-ttu-id="77035-149">application/json</span><span class="sxs-lookup"><span data-stu-id="77035-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="77035-150">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77035-150">Request body</span></span>
<span data-ttu-id="77035-151">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="77035-151">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="77035-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="77035-152">Response</span></span>

<span data-ttu-id="77035-153">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwort Code und [Anwendungen](../resources/application.md) -Auflistungsobjekt in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="77035-153">If successful, this method returns `200 OK` response code and [application](../resources/application.md) collection object in the response body.</span></span> <span data-ttu-id="77035-154">Die Antwort enthält auch ein NextLink oder eine DeltaLink-URL.</span><span class="sxs-lookup"><span data-stu-id="77035-154">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="77035-155">Wenn ein `nextLink` URL zurückgegeben wird, stehen Ihnen zusätzliche Seiten mit Daten aus der Sitzung abgerufen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="77035-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="77035-156">Die Anwendung weiterhin tätigen Anforderungen mithilfe der `nextLink` URL bis eine `deltaLink` URL in der Antwort enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="77035-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="77035-157">Wenn ein `deltaLink` URL wird zurückgegeben, es sind keine weiteren Daten zum vorhandenen Status der Ressource zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="77035-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="77035-158">Speichern und verwenden Sie die `deltaLink` URL, um Informationen zu Änderungen an der Ressource in der Zukunft zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="77035-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="77035-159">Siehe:</span><span class="sxs-lookup"><span data-stu-id="77035-159">See:</span></span></br>
- <span data-ttu-id="77035-160">Weitere Informationen finden Sie unter [Verwenden einer Delta-Abfrage](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="77035-160">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="77035-161">Beispielanforderungen finden Sie unter [Inkrementelle Änderungen für Benutzer abrufen](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="77035-161">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="77035-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77035-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77035-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77035-163">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "application_delta"
}-->
```http
GET https://graph.microsoft.com/beta/applications/delta
```

##### <a name="response"></a><span data-ttu-id="77035-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="77035-164">Response</span></span>
<span data-ttu-id="77035-p111">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77035-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#applications",
  "@odata.nextLink":"https://graph.microsoft.com/beta/applications/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "application: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
