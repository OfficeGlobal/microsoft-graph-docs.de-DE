---
title: Berechtigungen
description: 'Entfernen Sie die app aus Ihrer Organisation app-Katalog (die Mandanten-app-Katalog). '
localization_priority: Normal
ms.openlocfilehash: ba932f8d87691cd57e26e5c26904936ce39ba55f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830212"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="668a2-103">Entfernen einer app aus Ihrer Organisation app-Katalog</span><span class="sxs-lookup"><span data-stu-id="668a2-103">Remove an app from your organization's app catalog</span></span>

> <span data-ttu-id="668a2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="668a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="668a2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="668a2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="668a2-106">Entfernen Sie die [app](../resources/teamsapp.md) aus Ihrer Organisation app-Katalog (die Mandanten-app-Katalog).</span><span class="sxs-lookup"><span data-stu-id="668a2-106">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="668a2-107">Wenn Ihre app aus Ihrer Organisation app-Katalog entfernen möchten, geben Sie `organization` als die **DistributionMethod** in der [TeamsCatalogApp](../resources/teamsapp.md) -Ressource.</span><span class="sxs-lookup"><span data-stu-id="668a2-107">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="668a2-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="668a2-108">Permissions</span></span>

<span data-ttu-id="668a2-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="668a2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="668a2-111">**Hinweis:** Nur globale Administratoren können diese API aufrufen.</span><span class="sxs-lookup"><span data-stu-id="668a2-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="668a2-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="668a2-112">Permission Type</span></span>                        | <span data-ttu-id="668a2-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="668a2-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="668a2-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="668a2-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="668a2-115">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="668a2-115">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="668a2-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="668a2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="668a2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="668a2-117">Not supported</span></span>|
| <span data-ttu-id="668a2-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="668a2-118">Application</span></span>                            | <span data-ttu-id="668a2-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="668a2-119">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="668a2-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="668a2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="668a2-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="668a2-121">Request headers</span></span>

| <span data-ttu-id="668a2-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="668a2-122">Header</span></span>        | <span data-ttu-id="668a2-123">Wert</span><span class="sxs-lookup"><span data-stu-id="668a2-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="668a2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="668a2-124">Authorization</span></span> | <span data-ttu-id="668a2-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="668a2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="668a2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="668a2-127">Request body</span></span>

<span data-ttu-id="668a2-128">Keine.</span><span class="sxs-lookup"><span data-stu-id="668a2-128">None.</span></span>

><span data-ttu-id="668a2-129">**Hinweis:** Verwenden Sie die ID aus der [Liste apps veröffentlicht](./teamsapp-list.md) Aufruf für zurückgegeben, auf um die app zu verweisen, die Sie aktualisieren möchten.</span><span class="sxs-lookup"><span data-stu-id="668a2-129">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="668a2-130">Verwenden Sie nicht die in der Manifestdatei der app Zip-Paket-ID ein.</span><span class="sxs-lookup"><span data-stu-id="668a2-130">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="668a2-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="668a2-131">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="668a2-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="668a2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="668a2-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="668a2-133">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="668a2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="668a2-134">Response</span></span>

```http
HTTP/1.1 204 No Content
```
