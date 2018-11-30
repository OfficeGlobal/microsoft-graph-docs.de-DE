---
title: Berechtigungen
description: 'Aktualisieren einer app zuvor in der Microsoft-Teams, app-Katalog veröffentlicht. '
ms.openlocfilehash: f63b75fe3373ad89148b2901b828dcc0ae1f95a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065019"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="d032d-103">Aktualisieren von apps in Ihrer Organisation app-Katalog veröffentlicht</span><span class="sxs-lookup"><span data-stu-id="d032d-103">Update apps published to your organization's app catalog</span></span>

> <span data-ttu-id="d032d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d032d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d032d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d032d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d032d-106">Aktualisieren einer [app](../resources/teamsapp.md) veröffentlicht zuvor in der Microsoft-Teams, app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="d032d-106">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="d032d-107">Diese API aktualisiert speziell eine app in Ihrer Organisation app-Katalog (die Mandanten-app-Katalog) veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="d032d-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="d032d-108">Geben Sie zum Veröffentlichen in Ihrer Organisation app-Katalog `organization` als die **DistributionMethod** in der [TeamsCatalogApp](../resources/teamsapp.md) -Ressource.</span><span class="sxs-lookup"><span data-stu-id="d032d-108">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="d032d-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d032d-109">Permissions</span></span>

<span data-ttu-id="d032d-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="d032d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="d032d-112">**Hinweis:** Nur globale Administratoren können diese API aufrufen.</span><span class="sxs-lookup"><span data-stu-id="d032d-112">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="d032d-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d032d-113">Permission Type</span></span>                        | <span data-ttu-id="d032d-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d032d-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="d032d-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d032d-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="d032d-116">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d032d-116">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="d032d-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d032d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d032d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d032d-118">Not supported</span></span>|
| <span data-ttu-id="d032d-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d032d-119">Application</span></span>                            | <span data-ttu-id="d032d-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d032d-120">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="d032d-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d032d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d032d-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d032d-122">Request headers</span></span>

| <span data-ttu-id="d032d-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d032d-123">Header</span></span>        | <span data-ttu-id="d032d-124">Wert</span><span class="sxs-lookup"><span data-stu-id="d032d-124">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="d032d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d032d-125">Authorization</span></span> | <span data-ttu-id="d032d-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d032d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d032d-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d032d-128">Content-Type</span></span>  | <span data-ttu-id="d032d-129">Anwendung/zip</span><span class="sxs-lookup"><span data-stu-id="d032d-129">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="d032d-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d032d-130">Request body</span></span>

<span data-ttu-id="d032d-131">Manifest Teams Zip-Nutzlast: Für Teams Anwendung zip-Datei [Erstellen eines app-Pakets finden Sie unter](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="d032d-131">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="d032d-132">**Hinweis:** Verwenden Sie die ID aus der [Liste apps veröffentlicht](./teamsapp-list.md) Aufruf für zurückgegeben, auf um die app zu verweisen, die Sie aktualisieren möchten.</span><span class="sxs-lookup"><span data-stu-id="d032d-132">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="d032d-133">Verwenden Sie nicht die in der Manifestdatei der app Zip-Paket-ID ein.</span><span class="sxs-lookup"><span data-stu-id="d032d-133">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="d032d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d032d-134">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="d032d-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d032d-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="d032d-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d032d-136">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="d032d-137">Für Teams Anwendung zip-Datei [finden Sie unter Erstellen von app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="d032d-137">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="d032d-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="d032d-138">Response</span></span>

```
HTTP/1.1 204 No Content
```
