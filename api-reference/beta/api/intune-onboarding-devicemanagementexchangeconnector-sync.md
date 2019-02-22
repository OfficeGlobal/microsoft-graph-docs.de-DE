---
title: Aktion „sync“
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7d524ef97ccd4791361220d1c5d95e15491e473e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153032"
---
# <a name="sync-action"></a><span data-ttu-id="caffa-103">sync-Aktion</span><span class="sxs-lookup"><span data-stu-id="caffa-103">sync action</span></span>

> <span data-ttu-id="caffa-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="caffa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="caffa-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="caffa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="caffa-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="caffa-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="caffa-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="caffa-107">Prerequisites</span></span>
<span data-ttu-id="caffa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="caffa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="caffa-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="caffa-110">Permission type</span></span>|<span data-ttu-id="caffa-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="caffa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="caffa-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="caffa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="caffa-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caffa-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="caffa-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="caffa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="caffa-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="caffa-115">Not supported.</span></span>|
|<span data-ttu-id="caffa-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="caffa-116">Application</span></span>|<span data-ttu-id="caffa-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="caffa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="caffa-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="caffa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="caffa-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="caffa-119">Request headers</span></span>
|<span data-ttu-id="caffa-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="caffa-120">Header</span></span>|<span data-ttu-id="caffa-121">Wert</span><span class="sxs-lookup"><span data-stu-id="caffa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="caffa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="caffa-122">Authorization</span></span>|<span data-ttu-id="caffa-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="caffa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="caffa-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="caffa-124">Accept</span></span>|<span data-ttu-id="caffa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="caffa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="caffa-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="caffa-126">Request body</span></span>
<span data-ttu-id="caffa-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="caffa-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="caffa-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="caffa-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="caffa-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="caffa-129">Property</span></span>|<span data-ttu-id="caffa-130">Typ</span><span class="sxs-lookup"><span data-stu-id="caffa-130">Type</span></span>|<span data-ttu-id="caffa-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="caffa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caffa-132">syncType</span><span class="sxs-lookup"><span data-stu-id="caffa-132">syncType</span></span>|[<span data-ttu-id="caffa-133">deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="caffa-133">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="caffa-134">Typ der auszuführenden Synchronisierung (vollständige Synchronisierung oder Deltasynchronisierung)</span><span class="sxs-lookup"><span data-stu-id="caffa-134">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="caffa-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="caffa-135">Response</span></span>
<span data-ttu-id="caffa-136">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="caffa-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="caffa-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="caffa-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="caffa-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="caffa-138">Request</span></span>
<span data-ttu-id="caffa-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="caffa-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="caffa-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="caffa-140">Response</span></span>
<span data-ttu-id="caffa-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="caffa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




