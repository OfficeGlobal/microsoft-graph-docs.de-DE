---
title: syncMicrosoftStoreForBusinessApps-Aktion
description: Synchronisiert Intune-Konten mit dem Microsoft Store für Unternehmen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bba25378dae6f74104cb3ecc3a336404181b9a79
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821644"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="a0aa9-103">syncMicrosoftStoreForBusinessApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="a0aa9-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="a0aa9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a0aa9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0aa9-105">Synchronisiert Intune-Konten mit dem Microsoft Store für Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="a0aa9-105">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a0aa9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a0aa9-106">Prerequisites</span></span>
<span data-ttu-id="a0aa9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0aa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0aa9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a0aa9-109">Permission type</span></span>|<span data-ttu-id="a0aa9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a0aa9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0aa9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a0aa9-111">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="a0aa9-112">&nbsp;&nbsp; _Onboarding_</span><span class="sxs-lookup"><span data-stu-id="a0aa9-112">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="a0aa9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0aa9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a0aa9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a0aa9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0aa9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0aa9-115">Not supported.</span></span>|
|<span data-ttu-id="a0aa9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a0aa9-116">Application</span></span>|<span data-ttu-id="a0aa9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0aa9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0aa9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0aa9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="a0aa9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a0aa9-119">Request headers</span></span>
|<span data-ttu-id="a0aa9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a0aa9-120">Header</span></span>|<span data-ttu-id="a0aa9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a0aa9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0aa9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0aa9-122">Authorization</span></span>|<span data-ttu-id="a0aa9-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a0aa9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0aa9-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a0aa9-124">Accept</span></span>|<span data-ttu-id="a0aa9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0aa9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0aa9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a0aa9-126">Request body</span></span>
<span data-ttu-id="a0aa9-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a0aa9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0aa9-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0aa9-128">Response</span></span>
<span data-ttu-id="a0aa9-129">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="a0aa9-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="a0aa9-130">Beispielanforderung</span><span class="sxs-lookup"><span data-stu-id="a0aa9-130">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="a0aa9-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0aa9-131">Response</span></span>

<span data-ttu-id="a0aa9-132">Der Kürze halber werden möglicherweise im Response-Objekt dargestellten abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="a0aa9-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a0aa9-133">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a0aa9-133">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



