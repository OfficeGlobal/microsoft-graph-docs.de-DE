---
title: Liste der veröffentlichten apps aus dem Microsoft-Teams, app-Katalog
description: 'Liste apps aus dem Microsoft-Teams, app-Katalog. '
ms.openlocfilehash: 5855f34e836e4d2d86261fe7a15232dadeee4ac2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018196"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="5a80b-103">Liste der veröffentlichten apps aus dem Microsoft-Teams, app-Katalog</span><span class="sxs-lookup"><span data-stu-id="5a80b-103">List the published apps from the Microsoft Teams app catalog</span></span>



<span data-ttu-id="5a80b-104">Liste der [apps](../resources/teamsapp.md) aus dem Microsoft-Teams, app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="5a80b-104">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span> <span data-ttu-id="5a80b-105">Dazu gehören apps aus dem Microsoft-Teams Store als auch apps aus Ihrer Organisation app-Katalog (die Mandanten-app-Katalog).</span><span class="sxs-lookup"><span data-stu-id="5a80b-105">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="5a80b-106">Wenn Sie apps aus app-Katalog nur Ihrer Organisation erhalten möchten, geben Sie `Organization` als die **DistributionMethod** in der [TeamsCatalogApp](../resources/teamsapp.md) -Ressource.</span><span class="sxs-lookup"><span data-stu-id="5a80b-106">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a80b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5a80b-107">Permissions</span></span>

<span data-ttu-id="5a80b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="5a80b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="5a80b-110">**Hinweis:** Nur globale Administratoren können diese API aufrufen.</span><span class="sxs-lookup"><span data-stu-id="5a80b-110">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="5a80b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5a80b-111">Permission Type</span></span>                        | <span data-ttu-id="5a80b-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5a80b-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="5a80b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5a80b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a80b-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a80b-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="5a80b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5a80b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a80b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a80b-116">Not supported</span></span>|
| <span data-ttu-id="5a80b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5a80b-117">Application</span></span>                            | <span data-ttu-id="5a80b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a80b-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a80b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a80b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5a80b-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5a80b-120">Optional query parameters</span></span>
<span data-ttu-id="5a80b-121">Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="5a80b-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a80b-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5a80b-122">Request headers</span></span>

| <span data-ttu-id="5a80b-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5a80b-123">Header</span></span>        | <span data-ttu-id="5a80b-124">Wert</span><span class="sxs-lookup"><span data-stu-id="5a80b-124">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="5a80b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a80b-125">Authorization</span></span> | <span data-ttu-id="5a80b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5a80b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5a80b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5a80b-128">Request body</span></span>
<span data-ttu-id="5a80b-129">Keine.</span><span class="sxs-lookup"><span data-stu-id="5a80b-129">None.</span></span>

><span data-ttu-id="5a80b-130">**Hinweis:** Sie können die Felder des [TeamsCatalogApp](../resources/teamsapp.md) -Objekts in der Ergebnisliste verkürzte filtern.</span><span class="sxs-lookup"><span data-stu-id="5a80b-130">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="5a80b-131">Sie können eine der folgenden Filter Vorgänge verwenden: gleich, nicht gleich, und, oder, und nicht.</span><span class="sxs-lookup"><span data-stu-id="5a80b-131">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="5a80b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a80b-132">Response</span></span>
<span data-ttu-id="5a80b-133">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste von Objekten im Antworttext [TeamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="5a80b-133">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5a80b-134">Beispiele</span><span class="sxs-lookup"><span data-stu-id="5a80b-134">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="5a80b-135">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="5a80b-135">Example 1</span></span>
<span data-ttu-id="5a80b-136">Das folgende Beispiel listet alle Anwendungen, die für Ihre Mandanten spezifisch sind.</span><span class="sxs-lookup"><span data-stu-id="5a80b-136">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="5a80b-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a80b-137">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a><span data-ttu-id="5a80b-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a80b-138">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="5a80b-139">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="5a80b-139">Example 2</span></span>

<span data-ttu-id="5a80b-140">Das folgende Beispiel listet Applikationen mit einer bestimmten ID.</span><span class="sxs-lookup"><span data-stu-id="5a80b-140">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="5a80b-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a80b-141">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="5a80b-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a80b-142">Response</span></span>
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

