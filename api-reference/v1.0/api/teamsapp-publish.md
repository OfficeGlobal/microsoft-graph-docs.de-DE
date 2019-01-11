---
title: Berechtigungen
description: 'Veröffentlichen einer app mit dem Microsoft-Teams, apps Katalog. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 7d6ad2d06db89f0f516cfe6a5fa37effe2af4f36
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840033"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="532c5-103">Veröffentlichen von apps in Ihrer Organisation app-Katalog</span><span class="sxs-lookup"><span data-stu-id="532c5-103">Publish apps to your organization's app catalog</span></span>



<span data-ttu-id="532c5-104">Veröffentlichen einer [app](../resources/teamsapp.md) mit dem Microsoft-Teams, apps Katalog.</span><span class="sxs-lookup"><span data-stu-id="532c5-104">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span> <span data-ttu-id="532c5-105">Diese API veröffentlicht insbesondere die app in Ihrer Organisation-Katalog (die Mandanten-app-Katalog); die erstellte Ressource müssen `distributionMethod`  =  `organization`.</span><span class="sxs-lookup"><span data-stu-id="532c5-105">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="532c5-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="532c5-106">Permissions</span></span>

<span data-ttu-id="532c5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="532c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="532c5-109">**Hinweis:** Nur globale Administratoren können diese API aufrufen.</span><span class="sxs-lookup"><span data-stu-id="532c5-109">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="532c5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="532c5-110">Permission Type</span></span>                        | <span data-ttu-id="532c5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="532c5-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="532c5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="532c5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="532c5-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="532c5-113">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="532c5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="532c5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="532c5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="532c5-115">Not supported</span></span>|
| <span data-ttu-id="532c5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="532c5-116">Application</span></span>                            | <span data-ttu-id="532c5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="532c5-117">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="532c5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="532c5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="532c5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="532c5-119">Request headers</span></span>

| <span data-ttu-id="532c5-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="532c5-120">Header</span></span>        | <span data-ttu-id="532c5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="532c5-121">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="532c5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="532c5-122">Authorization</span></span> | <span data-ttu-id="532c5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="532c5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="532c5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="532c5-125">Content-Type</span></span>  | <span data-ttu-id="532c5-126">Anwendung/zip</span><span class="sxs-lookup"><span data-stu-id="532c5-126">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="532c5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="532c5-127">Request body</span></span>

<span data-ttu-id="532c5-128">Manifest Teams Zip-Nutzlast.</span><span class="sxs-lookup"><span data-stu-id="532c5-128">Teams Zip Manifest Payload.</span></span> <span data-ttu-id="532c5-129">Zip-Datei [finden Sie unter Erstellen eines app-Pakets](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)für Teams fest.</span><span class="sxs-lookup"><span data-stu-id="532c5-129">For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> <span data-ttu-id="532c5-130">Sie können keine app für eine Organisation erstellen, die die gleiche manifest-ID als einer anderen Anwendung in der Organisation hat.</span><span class="sxs-lookup"><span data-stu-id="532c5-130">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="532c5-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="532c5-131">Response</span></span>

<span data-ttu-id="532c5-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein [TeamsCatalogApp](../resources/teamsapp.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="532c5-132">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="532c5-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="532c5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="532c5-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="532c5-134">Request</span></span>

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="532c5-135">Informationen dazu, wie Sie eine Microsoft-Teams Anwendung Zip-Datei erstellen finden Sie unter [Erstellen eines app-Pakets](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="532c5-135">For information about how to create a Microsoft Teams application zip file, see [Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> 

### <a name="response"></a><span data-ttu-id="532c5-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="532c5-136">Response</span></span>

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
