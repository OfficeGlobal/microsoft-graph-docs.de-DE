---
title: Liste der veröffentlichten apps aus dem Microsoft-Teams, app-Katalog
description: 'Liste apps aus dem Microsoft-Teams, app-Katalog. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a19c852b4cca08b7318ef33cdf24929e5f4c3042
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016667"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="63bf1-103">Liste der veröffentlichten apps aus dem Microsoft-Teams, app-Katalog</span><span class="sxs-lookup"><span data-stu-id="63bf1-103">List the published apps from the Microsoft Teams app catalog</span></span>



<span data-ttu-id="63bf1-104">Liste der [apps](../resources/teamsapp.md) aus dem Microsoft-Teams, app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="63bf1-104">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span> <span data-ttu-id="63bf1-105">Dazu gehören apps aus dem Microsoft-Teams Store als auch apps aus Ihrer Organisation app-Katalog (die Mandanten-app-Katalog).</span><span class="sxs-lookup"><span data-stu-id="63bf1-105">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="63bf1-106">Wenn Sie apps aus app-Katalog nur Ihrer Organisation erhalten möchten, geben Sie `Organization` als die **DistributionMethod** in der [TeamsCatalogApp](../resources/teamsapp.md) -Ressource.</span><span class="sxs-lookup"><span data-stu-id="63bf1-106">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="63bf1-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="63bf1-107">Permissions</span></span>

<span data-ttu-id="63bf1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="63bf1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="63bf1-110">**Hinweis:** Nur globale Administratoren können diese API aufrufen.</span><span class="sxs-lookup"><span data-stu-id="63bf1-110">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="63bf1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="63bf1-111">Permission Type</span></span>                        | <span data-ttu-id="63bf1-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="63bf1-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="63bf1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="63bf1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="63bf1-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63bf1-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="63bf1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="63bf1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63bf1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63bf1-116">Not supported</span></span>|
| <span data-ttu-id="63bf1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="63bf1-117">Application</span></span>                            | <span data-ttu-id="63bf1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63bf1-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="63bf1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="63bf1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="63bf1-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="63bf1-120">Optional query parameters</span></span>
<span data-ttu-id="63bf1-121">Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="63bf1-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63bf1-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="63bf1-122">Request headers</span></span>

| <span data-ttu-id="63bf1-123">Header</span><span class="sxs-lookup"><span data-stu-id="63bf1-123">Header</span></span>        | <span data-ttu-id="63bf1-124">Wert</span><span class="sxs-lookup"><span data-stu-id="63bf1-124">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="63bf1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="63bf1-125">Authorization</span></span> | <span data-ttu-id="63bf1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="63bf1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63bf1-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="63bf1-128">Request body</span></span>
<span data-ttu-id="63bf1-129">Keine.</span><span class="sxs-lookup"><span data-stu-id="63bf1-129">None.</span></span>

><span data-ttu-id="63bf1-130">**Hinweis:** Sie können die Felder des [TeamsCatalogApp](../resources/teamsapp.md) -Objekts in der Ergebnisliste verkürzte filtern.</span><span class="sxs-lookup"><span data-stu-id="63bf1-130">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="63bf1-131">Sie können eine der folgenden Filter Vorgänge verwenden: gleich, nicht gleich, und, oder, und nicht.</span><span class="sxs-lookup"><span data-stu-id="63bf1-131">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="63bf1-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="63bf1-132">Response</span></span>
<span data-ttu-id="63bf1-133">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste von Objekten im Antworttext [TeamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="63bf1-133">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63bf1-134">Beispiele</span><span class="sxs-lookup"><span data-stu-id="63bf1-134">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="63bf1-135">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="63bf1-135">Example 1</span></span>
<span data-ttu-id="63bf1-136">Das folgende Beispiel listet alle Anwendungen, die für Ihre Mandanten spezifisch sind.</span><span class="sxs-lookup"><span data-stu-id="63bf1-136">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="63bf1-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="63bf1-137">Request</span></span>
```
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a><span data-ttu-id="63bf1-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="63bf1-138">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="63bf1-139">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="63bf1-139">Example 2</span></span>

<span data-ttu-id="63bf1-140">Das folgende Beispiel listet Applikationen mit einer bestimmten ID.</span><span class="sxs-lookup"><span data-stu-id="63bf1-140">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="63bf1-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="63bf1-141">Request</span></span>
```
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="63bf1-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="63bf1-142">Response</span></span>
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

