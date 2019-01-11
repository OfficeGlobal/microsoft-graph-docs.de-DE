---
title: Berechtigungen
description: 'Entfernen Sie die app aus Ihrer Organisation app-Katalog (die Mandanten-app-Katalog). '
localization_priority: Normal
ms.openlocfilehash: e19826407a5f809787beffc8211f77ddce21d043
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804928"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="a1660-103">Entfernen einer app aus Ihrer Organisation app-Katalog</span><span class="sxs-lookup"><span data-stu-id="a1660-103">Remove an app from your organization's app catalog</span></span>



<span data-ttu-id="a1660-104">Entfernen Sie die [app](../resources/teamsapp.md) aus Ihrer Organisation app-Katalog (die Mandanten-app-Katalog).</span><span class="sxs-lookup"><span data-stu-id="a1660-104">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="a1660-105">Wenn Ihre app aus Ihrer Organisation app-Katalog entfernen möchten, geben Sie `organization` als die **DistributionMethod** in der [TeamsCatalogApp](../resources/teamsapp.md) -Ressource.</span><span class="sxs-lookup"><span data-stu-id="a1660-105">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1660-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a1660-106">Permissions</span></span>

<span data-ttu-id="a1660-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="a1660-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="a1660-109">**Hinweis:** Nur globale Administratoren können diese API aufrufen.</span><span class="sxs-lookup"><span data-stu-id="a1660-109">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="a1660-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a1660-110">Permission Type</span></span>                        | <span data-ttu-id="a1660-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a1660-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="a1660-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a1660-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1660-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1660-113">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="a1660-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a1660-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1660-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1660-115">Not supported</span></span>|
| <span data-ttu-id="a1660-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a1660-116">Application</span></span>                            | <span data-ttu-id="a1660-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1660-117">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1660-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1660-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a1660-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a1660-119">Request headers</span></span>

| <span data-ttu-id="a1660-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a1660-120">Header</span></span>        | <span data-ttu-id="a1660-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a1660-121">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="a1660-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1660-122">Authorization</span></span> | <span data-ttu-id="a1660-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a1660-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a1660-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a1660-125">Request body</span></span>

<span data-ttu-id="a1660-126">Keine.</span><span class="sxs-lookup"><span data-stu-id="a1660-126">None.</span></span>

><span data-ttu-id="a1660-127">**Hinweis:** Verwenden Sie die ID aus der [Liste apps veröffentlicht](./teamsapp-list.md) Aufruf für zurückgegeben, auf um die app zu verweisen, die Sie aktualisieren möchten.</span><span class="sxs-lookup"><span data-stu-id="a1660-127">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="a1660-128">Verwenden Sie nicht die in der Manifestdatei der app Zip-Paket-ID ein.</span><span class="sxs-lookup"><span data-stu-id="a1660-128">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="a1660-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1660-129">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="a1660-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a1660-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1660-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1660-131">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="a1660-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1660-132">Response</span></span>

```http
HTTP/1.1 204 No Content
```
