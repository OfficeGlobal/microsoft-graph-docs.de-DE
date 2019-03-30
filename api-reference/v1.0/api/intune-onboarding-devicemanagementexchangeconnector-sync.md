---
title: Aktion „sync“
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 98e2c1671b7fde9450b18ca3bd12537450d02416
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988476"
---
# <a name="sync-action"></a><span data-ttu-id="51ed0-103">sync-Aktion</span><span class="sxs-lookup"><span data-stu-id="51ed0-103">sync action</span></span>

> <span data-ttu-id="51ed0-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="51ed0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51ed0-105">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="51ed0-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51ed0-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="51ed0-106">Prerequisites</span></span>
<span data-ttu-id="51ed0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51ed0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51ed0-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="51ed0-109">Permission type</span></span>|<span data-ttu-id="51ed0-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="51ed0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51ed0-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="51ed0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51ed0-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51ed0-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="51ed0-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="51ed0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51ed0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51ed0-114">Not supported.</span></span>|
|<span data-ttu-id="51ed0-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="51ed0-115">Application</span></span>|<span data-ttu-id="51ed0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51ed0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51ed0-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="51ed0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="51ed0-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="51ed0-118">Request headers</span></span>
|<span data-ttu-id="51ed0-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="51ed0-119">Header</span></span>|<span data-ttu-id="51ed0-120">Wert</span><span class="sxs-lookup"><span data-stu-id="51ed0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51ed0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="51ed0-121">Authorization</span></span>|<span data-ttu-id="51ed0-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="51ed0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51ed0-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="51ed0-123">Accept</span></span>|<span data-ttu-id="51ed0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="51ed0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51ed0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="51ed0-125">Request body</span></span>
<span data-ttu-id="51ed0-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="51ed0-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="51ed0-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="51ed0-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="51ed0-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="51ed0-128">Property</span></span>|<span data-ttu-id="51ed0-129">Typ</span><span class="sxs-lookup"><span data-stu-id="51ed0-129">Type</span></span>|<span data-ttu-id="51ed0-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51ed0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51ed0-131">syncType</span><span class="sxs-lookup"><span data-stu-id="51ed0-131">syncType</span></span>|[<span data-ttu-id="51ed0-132">deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="51ed0-132">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="51ed0-133">Typ der auszuführenden Synchronisierung (vollständige Synchronisierung oder Deltasynchronisierung)</span><span class="sxs-lookup"><span data-stu-id="51ed0-133">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="51ed0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="51ed0-134">Response</span></span>
<span data-ttu-id="51ed0-135">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51ed0-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="51ed0-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="51ed0-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="51ed0-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="51ed0-137">Request</span></span>
<span data-ttu-id="51ed0-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="51ed0-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="51ed0-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="51ed0-139">Response</span></span>
<span data-ttu-id="51ed0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51ed0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



