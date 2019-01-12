---
title: Warnungen auflisten
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 507ad72b8d50e2343bfd99446e178e09ea65ac8f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927842"
---
# <a name="list-alerts"></a><span data-ttu-id="02157-104">Warnungen auflisten</span><span class="sxs-lookup"><span data-stu-id="02157-104">List alerts</span></span>

 > <span data-ttu-id="02157-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="02157-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02157-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02157-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="02157-107">Abrufen einer Liste von [Warnung](../resources/alert.md) -Objekten.</span><span class="sxs-lookup"><span data-stu-id="02157-107">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="02157-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="02157-108">Permissions</span></span>

<span data-ttu-id="02157-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02157-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02157-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="02157-111">Permission type</span></span>      | <span data-ttu-id="02157-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="02157-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02157-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="02157-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="02157-114">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02157-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="02157-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="02157-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="02157-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02157-116">Not supported.</span></span>  |
|<span data-ttu-id="02157-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="02157-117">Application</span></span> | <span data-ttu-id="02157-118">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02157-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02157-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="02157-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02157-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="02157-120">Optional query parameters</span></span>

<span data-ttu-id="02157-121">Diese Methode unterstützt die folgenden [Parameter für OData-Abfrage](/graph/query-parameters) , mit denen die Antwort anpassen:</span><span class="sxs-lookup"><span data-stu-id="02157-121">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="02157-122">`$top`Gibt die aggregierten Top-Ergebnisse aus jeder API Sicherheitsanbieter zurück.</span><span class="sxs-lookup"><span data-stu-id="02157-122">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="02157-123">Um eine alternative Eigenschaftensatz zurückzugeben, verwenden Sie die OData `$select` Abfragen Parameter, um die Gruppe von Eigenschaften der **Benachrichtigung** an, Sie werden soll.</span><span class="sxs-lookup"><span data-stu-id="02157-123">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="02157-124">Wenn **AssignedTo**, **Kategorie**und **Schweregrad** Eigenschaften zurückgeben möchten, fügen Sie beispielsweise die folgenden für Ihre Abfrage: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="02157-124">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="02157-125">**Hinweis:** `$top` darf maximal 1000 Warnungen und eine Kombination von `$top`  +  `$skip` 6000 Benachrichtigungen nicht überschreiten.</span><span class="sxs-lookup"><span data-stu-id="02157-125">**Note:** `$top` has a limit of 1000 alerts, and a combination of `$top` + `$skip` cannot exceed 6000 alerts.</span></span> <span data-ttu-id="02157-126">Beispielsweise `/security/alerts?$top=10&$skip=5990` zurückgegebenen eine `200 OK` Antwortcode, aber `/security/alerts?$top=10&$skip=5991` zurückgegebenen eine `400 Bad Request` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="02157-126">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>  <span data-ttu-id="02157-127">Weitere Informationen finden Sie unter [Microsoft Graph Security-API-Fehlerantworten](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="02157-127">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="02157-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="02157-128">Request headers</span></span>

| <span data-ttu-id="02157-129">Name</span><span class="sxs-lookup"><span data-stu-id="02157-129">Name</span></span>      |<span data-ttu-id="02157-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02157-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02157-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="02157-131">Authorization</span></span>  | <span data-ttu-id="02157-p106">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="02157-p106">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02157-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="02157-134">Request body</span></span>

<span data-ttu-id="02157-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="02157-135">Do not supply a request body for this method.</span></span> <span data-ttu-id="02157-136">Textkörper der Anforderung wird ignoriert.</span><span class="sxs-lookup"><span data-stu-id="02157-136">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="02157-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="02157-137">Response</span></span>

<span data-ttu-id="02157-138">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext **Benachrichtigung** .</span><span class="sxs-lookup"><span data-stu-id="02157-138">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="02157-139">Wenn ein Statuscode als 2xx oder 404 von einem Anbieter zurückgegeben wird, oder wenn von ein Anbieter Zeitlimit überschritten, die Antwort werden eine `206 Partial Content` Statuscode mit der Anbieter Antwort in der Kopfzeile einer Warnung.</span><span class="sxs-lookup"><span data-stu-id="02157-139">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="02157-140">Weitere Informationen finden Sie unter [Microsoft Graph Security-API-Fehlerantworten](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="02157-140">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="02157-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="02157-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="02157-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="02157-142">Request</span></span>

<span data-ttu-id="02157-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="02157-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts
```

### <a name="response"></a><span data-ttu-id="02157-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="02157-144">Response</span></span>

<span data-ttu-id="02157-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="02157-145">The following is an example of the response.</span></span>

><span data-ttu-id="02157-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="02157-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
