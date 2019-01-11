---
title: Liste der veröffentlichten apps aus dem Microsoft-Teams, app-Katalog
description: 'Liste apps aus dem Microsoft-Teams, app-Katalog. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 4cd3d8d66caa384a064711987f4fcd7473083089
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863455"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="53bf3-103">Liste der veröffentlichten apps aus dem Microsoft-Teams, app-Katalog</span><span class="sxs-lookup"><span data-stu-id="53bf3-103">List the published apps from the Microsoft Teams app catalog</span></span>

> <span data-ttu-id="53bf3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="53bf3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53bf3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="53bf3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="53bf3-106">Liste der [apps](../resources/teamsapp.md) aus dem Microsoft-Teams, app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="53bf3-106">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span> <span data-ttu-id="53bf3-107">Dazu gehören apps aus dem Microsoft-Teams Store als auch apps aus Ihrer Organisation app-Katalog (die Mandanten-app-Katalog).</span><span class="sxs-lookup"><span data-stu-id="53bf3-107">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="53bf3-108">Wenn Sie apps aus app-Katalog nur Ihrer Organisation erhalten möchten, geben Sie `Organization` als die **DistributionMethod** in der [TeamsCatalogApp](../resources/teamsapp.md) -Ressource.</span><span class="sxs-lookup"><span data-stu-id="53bf3-108">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="53bf3-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53bf3-109">Permissions</span></span>

<span data-ttu-id="53bf3-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="53bf3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="53bf3-112">**Hinweis:** Nur globale Administratoren können diese API aufrufen.</span><span class="sxs-lookup"><span data-stu-id="53bf3-112">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="53bf3-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53bf3-113">Permission Type</span></span>                        | <span data-ttu-id="53bf3-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53bf3-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="53bf3-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53bf3-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="53bf3-116">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53bf3-116">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="53bf3-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53bf3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53bf3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53bf3-118">Not supported</span></span>|
| <span data-ttu-id="53bf3-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53bf3-119">Application</span></span>                            | <span data-ttu-id="53bf3-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53bf3-120">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="53bf3-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53bf3-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53bf3-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="53bf3-122">Optional query parameters</span></span>
<span data-ttu-id="53bf3-123">Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="53bf3-123">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53bf3-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53bf3-124">Request headers</span></span>

| <span data-ttu-id="53bf3-125">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="53bf3-125">Header</span></span>        | <span data-ttu-id="53bf3-126">Wert</span><span class="sxs-lookup"><span data-stu-id="53bf3-126">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="53bf3-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="53bf3-127">Authorization</span></span> | <span data-ttu-id="53bf3-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="53bf3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="53bf3-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53bf3-130">Request body</span></span>
<span data-ttu-id="53bf3-131">Keine.</span><span class="sxs-lookup"><span data-stu-id="53bf3-131">None.</span></span>

><span data-ttu-id="53bf3-132">**Hinweis:** Sie können die Felder des [TeamsCatalogApp](../resources/teamsapp.md) -Objekts in der Ergebnisliste verkürzte filtern.</span><span class="sxs-lookup"><span data-stu-id="53bf3-132">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="53bf3-133">Sie können eine der folgenden Filter Vorgänge verwenden: gleich, nicht gleich, und, oder, und nicht.</span><span class="sxs-lookup"><span data-stu-id="53bf3-133">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="53bf3-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="53bf3-134">Response</span></span>
<span data-ttu-id="53bf3-135">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste von Objekten im Antworttext [TeamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="53bf3-135">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53bf3-136">Beispiele</span><span class="sxs-lookup"><span data-stu-id="53bf3-136">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="53bf3-137">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="53bf3-137">Example 1</span></span>
<span data-ttu-id="53bf3-138">Das folgende Beispiel listet alle Anwendungen, die für Ihre Mandanten spezifisch sind.</span><span class="sxs-lookup"><span data-stu-id="53bf3-138">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="53bf3-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53bf3-139">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a><span data-ttu-id="53bf3-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="53bf3-140">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

### <a name="example-2"></a><span data-ttu-id="53bf3-141">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="53bf3-141">Example 2</span></span>

<span data-ttu-id="53bf3-142">Das folgende Beispiel listet Applikationen mit einer bestimmten ID.</span><span class="sxs-lookup"><span data-stu-id="53bf3-142">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="53bf3-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53bf3-143">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="53bf3-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="53bf3-144">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

