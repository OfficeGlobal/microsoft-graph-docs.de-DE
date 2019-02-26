---
title: syncMicrosoftStoreForBusinessApps-Aktion
description: Synchronisiert Intune-Konten mit dem Microsoft Store für Unternehmen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e71bfb1e4ac6d4ce6c31344289eab7fb15b65594
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254268"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="ce473-103">syncMicrosoftStoreForBusinessApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="ce473-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="ce473-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ce473-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce473-105">Synchronisiert Intune-Konten mit dem Microsoft Store für Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="ce473-105">Syncs Intune account with Microsoft Store For Business</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce473-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ce473-106">Prerequisites</span></span>
<span data-ttu-id="ce473-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce473-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce473-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ce473-109">Permission type</span></span>|<span data-ttu-id="ce473-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ce473-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce473-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ce473-111">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="ce473-112">&nbsp; &nbsp; _Onboarding_</span><span class="sxs-lookup"><span data-stu-id="ce473-112">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="ce473-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce473-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ce473-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ce473-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce473-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce473-115">Not supported.</span></span>|
|<span data-ttu-id="ce473-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ce473-116">Application</span></span>|<span data-ttu-id="ce473-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce473-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce473-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce473-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="ce473-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ce473-119">Request headers</span></span>
|<span data-ttu-id="ce473-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ce473-120">Header</span></span>|<span data-ttu-id="ce473-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ce473-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce473-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce473-122">Authorization</span></span>|<span data-ttu-id="ce473-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ce473-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce473-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ce473-124">Accept</span></span>|<span data-ttu-id="ce473-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ce473-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce473-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ce473-126">Request body</span></span>
<span data-ttu-id="ce473-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ce473-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce473-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce473-128">Response</span></span>
<span data-ttu-id="ce473-129">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="ce473-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="ce473-130">Beispielanforderung</span><span class="sxs-lookup"><span data-stu-id="ce473-130">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="ce473-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce473-131">Response</span></span>

<span data-ttu-id="ce473-132">Das hier gezeigte Antwortobjekt kann zur Kürze abgeschnitten werden.</span><span class="sxs-lookup"><span data-stu-id="ce473-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ce473-133">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce473-133">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



