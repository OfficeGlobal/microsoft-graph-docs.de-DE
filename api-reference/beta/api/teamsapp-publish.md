---
title: Berechtigungen
description: 'Veröffentlichen einer app mit dem Microsoft-Teams, apps Katalog. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 656b4a148f1d53cb44e303265af5624ccd1e423b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932924"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="975b3-103">Veröffentlichen von apps in Ihrer Organisation app-Katalog</span><span class="sxs-lookup"><span data-stu-id="975b3-103">Publish apps to your organization's app catalog</span></span>

> <span data-ttu-id="975b3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="975b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="975b3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="975b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="975b3-106">Veröffentlichen einer [app](../resources/teamsapp.md) mit dem Microsoft-Teams, apps Katalog.</span><span class="sxs-lookup"><span data-stu-id="975b3-106">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span> <span data-ttu-id="975b3-107">Diese API veröffentlicht insbesondere die app in Ihrer Organisation-Katalog (die Mandanten-app-Katalog); die erstellte Ressource müssen `distributionMethod`  =  `organization`.</span><span class="sxs-lookup"><span data-stu-id="975b3-107">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="975b3-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="975b3-108">Permissions</span></span>

<span data-ttu-id="975b3-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="975b3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="975b3-111">**Hinweis:** Nur globale Administratoren können diese API aufrufen.</span><span class="sxs-lookup"><span data-stu-id="975b3-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="975b3-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="975b3-112">Permission Type</span></span>                        | <span data-ttu-id="975b3-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="975b3-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="975b3-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="975b3-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="975b3-115">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="975b3-115">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="975b3-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="975b3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="975b3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="975b3-117">Not supported</span></span>|
| <span data-ttu-id="975b3-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="975b3-118">Application</span></span>                            | <span data-ttu-id="975b3-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="975b3-119">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="975b3-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="975b3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="975b3-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="975b3-121">Request headers</span></span>

| <span data-ttu-id="975b3-122">Header</span><span class="sxs-lookup"><span data-stu-id="975b3-122">Header</span></span>        | <span data-ttu-id="975b3-123">Wert</span><span class="sxs-lookup"><span data-stu-id="975b3-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="975b3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="975b3-124">Authorization</span></span> | <span data-ttu-id="975b3-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="975b3-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="975b3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="975b3-127">Content-Type</span></span>  | <span data-ttu-id="975b3-128">Anwendung/zip</span><span class="sxs-lookup"><span data-stu-id="975b3-128">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="975b3-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="975b3-129">Request body</span></span>

<span data-ttu-id="975b3-130">Manifest Teams Zip-Nutzlast.</span><span class="sxs-lookup"><span data-stu-id="975b3-130">Teams Zip Manifest Payload.</span></span> <span data-ttu-id="975b3-131">Zip-Datei [finden Sie unter Erstellen eines app-Pakets](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)für Teams fest.</span><span class="sxs-lookup"><span data-stu-id="975b3-131">For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> <span data-ttu-id="975b3-132">Sie können keine app für eine Organisation erstellen, die die gleiche manifest-ID als einer anderen Anwendung in der Organisation hat.</span><span class="sxs-lookup"><span data-stu-id="975b3-132">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="975b3-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="975b3-133">Response</span></span>

<span data-ttu-id="975b3-134">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein [TeamsCatalogApp](../resources/teamsapp.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="975b3-134">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="975b3-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="975b3-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="975b3-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="975b3-136">Request</span></span>

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="975b3-137">Informationen dazu, wie Sie eine Microsoft-Teams Anwendung Zip-Datei erstellen finden Sie unter [Erstellen eines app-Pakets](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="975b3-137">For information about how to create a Microsoft Teams application zip file, see [Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> 

### <a name="response"></a><span data-ttu-id="975b3-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="975b3-138">Response</span></span>

```
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```
