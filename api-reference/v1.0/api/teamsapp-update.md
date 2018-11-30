---
title: Berechtigungen
description: 'Aktualisieren einer app zuvor in der Microsoft-Teams, app-Katalog veröffentlicht. '
ms.openlocfilehash: 38dd5cdbdb64c31d47c6d7e5b0c4bb27da8ad6e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016662"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="6d26c-103">Aktualisieren von apps in Ihrer Organisation app-Katalog veröffentlicht</span><span class="sxs-lookup"><span data-stu-id="6d26c-103">Update apps published to your organization's app catalog</span></span>



<span data-ttu-id="6d26c-104">Aktualisieren einer [app](../resources/teamsapp.md) veröffentlicht zuvor in der Microsoft-Teams, app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="6d26c-104">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="6d26c-105">Diese API aktualisiert speziell eine app in Ihrer Organisation app-Katalog (die Mandanten-app-Katalog) veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="6d26c-105">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="6d26c-106">Geben Sie zum Veröffentlichen in Ihrer Organisation app-Katalog `organization` als die **DistributionMethod** in der [TeamsCatalogApp](../resources/teamsapp.md) -Ressource.</span><span class="sxs-lookup"><span data-stu-id="6d26c-106">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d26c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6d26c-107">Permissions</span></span>

<span data-ttu-id="6d26c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="6d26c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="6d26c-110">**Hinweis:** Nur globale Administratoren können diese API aufrufen.</span><span class="sxs-lookup"><span data-stu-id="6d26c-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="6d26c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6d26c-111">Permission Type</span></span>                        | <span data-ttu-id="6d26c-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6d26c-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="6d26c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6d26c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d26c-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d26c-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="6d26c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6d26c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d26c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d26c-116">Not supported</span></span>|
| <span data-ttu-id="6d26c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6d26c-117">Application</span></span>                            | <span data-ttu-id="6d26c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d26c-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d26c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d26c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6d26c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6d26c-120">Request headers</span></span>

| <span data-ttu-id="6d26c-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6d26c-121">Header</span></span>        | <span data-ttu-id="6d26c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6d26c-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="6d26c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d26c-123">Authorization</span></span> | <span data-ttu-id="6d26c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6d26c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6d26c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d26c-126">Content-Type</span></span>  | <span data-ttu-id="6d26c-127">Anwendung/zip</span><span class="sxs-lookup"><span data-stu-id="6d26c-127">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d26c-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6d26c-128">Request body</span></span>

<span data-ttu-id="6d26c-129">Manifest Teams Zip-Nutzlast: Für Teams Anwendung zip-Datei [Erstellen eines app-Pakets finden Sie unter](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="6d26c-129">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="6d26c-130">**Hinweis:** Verwenden Sie die ID aus der [Liste apps veröffentlicht](./teamsapp-list.md) Aufruf für zurückgegeben, auf um die app zu verweisen, die Sie aktualisieren möchten.</span><span class="sxs-lookup"><span data-stu-id="6d26c-130">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="6d26c-131">Verwenden Sie nicht die in der Manifestdatei der app Zip-Paket-ID ein.</span><span class="sxs-lookup"><span data-stu-id="6d26c-131">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="6d26c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d26c-132">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="6d26c-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6d26c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d26c-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d26c-134">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="6d26c-135">Für Teams Anwendung zip-Datei [finden Sie unter Erstellen von app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="6d26c-135">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="6d26c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d26c-136">Response</span></span>

```
HTTP/1.1 204 No Content
```
