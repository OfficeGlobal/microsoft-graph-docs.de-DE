---
title: Berechtigungen
description: 'Aktualisieren einer app zuvor in der Microsoft-Teams, app-Katalog veröffentlicht. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2b9a16dc64557776eb6571ba3740249593684ba2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526984"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="8795e-103">Aktualisieren von apps in Ihrer Organisation app-Katalog veröffentlicht</span><span class="sxs-lookup"><span data-stu-id="8795e-103">Update apps published to your organization's app catalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8795e-104">Aktualisieren einer [app](../resources/teamsapp.md) veröffentlicht zuvor in der Microsoft-Teams, app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="8795e-104">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="8795e-105">Diese API aktualisiert speziell eine app in Ihrer Organisation app-Katalog (die Mandanten-app-Katalog) veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="8795e-105">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="8795e-106">Geben Sie zum Veröffentlichen in Ihrer Organisation app-Katalog `organization` als die **DistributionMethod** in der [TeamsCatalogApp](../resources/teamsapp.md) -Ressource.</span><span class="sxs-lookup"><span data-stu-id="8795e-106">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="8795e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8795e-107">Permissions</span></span>

<span data-ttu-id="8795e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="8795e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="8795e-110">**Hinweis:** Nur globale Administratoren können diese API aufrufen.</span><span class="sxs-lookup"><span data-stu-id="8795e-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="8795e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8795e-111">Permission Type</span></span>                        | <span data-ttu-id="8795e-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8795e-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="8795e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8795e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8795e-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8795e-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="8795e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8795e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8795e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8795e-116">Not supported</span></span>|
| <span data-ttu-id="8795e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8795e-117">Application</span></span>                            | <span data-ttu-id="8795e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8795e-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="8795e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8795e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8795e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8795e-120">Request headers</span></span>

| <span data-ttu-id="8795e-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8795e-121">Header</span></span>        | <span data-ttu-id="8795e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8795e-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="8795e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8795e-123">Authorization</span></span> | <span data-ttu-id="8795e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8795e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8795e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8795e-126">Content-Type</span></span>  | <span data-ttu-id="8795e-127">Anwendung/zip</span><span class="sxs-lookup"><span data-stu-id="8795e-127">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="8795e-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8795e-128">Request body</span></span>

<span data-ttu-id="8795e-129">Manifest Teams Zip-Nutzlast: Für Teams Anwendung zip-Datei [Erstellen eines app-Pakets finden Sie unter](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="8795e-129">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="8795e-130">**Hinweis:** Verwenden Sie die ID aus der [Liste apps veröffentlicht](./teamsapp-list.md) Aufruf für zurückgegeben, auf um die app zu verweisen, die Sie aktualisieren möchten.</span><span class="sxs-lookup"><span data-stu-id="8795e-130">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="8795e-131">Verwenden Sie nicht die in der Manifestdatei der app Zip-Paket-ID ein.</span><span class="sxs-lookup"><span data-stu-id="8795e-131">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="8795e-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="8795e-132">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="8795e-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8795e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8795e-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8795e-134">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="8795e-135">Für Teams Anwendung zip-Datei [finden Sie unter Erstellen von app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="8795e-135">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="8795e-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="8795e-136">Response</span></span>

```
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsapp-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
