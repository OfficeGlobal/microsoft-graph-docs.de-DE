---
title: deviceManagementExchangeConnectors auflisten
description: Auflisten von Eigenschaften und Beziehungen der deviceManagementExchangeConnector-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 580c2ce40c0f22b7183092cadaa4c36afac89dc7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153116"
---
# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="79440-103">deviceManagementExchangeConnectors auflisten</span><span class="sxs-lookup"><span data-stu-id="79440-103">List deviceManagementExchangeConnectors</span></span>

> <span data-ttu-id="79440-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="79440-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79440-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="79440-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79440-106">Auflisten von Eigenschaften und Beziehungen der [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="79440-106">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79440-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="79440-107">Prerequisites</span></span>
<span data-ttu-id="79440-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="79440-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="79440-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="79440-110">Permission type</span></span>|<span data-ttu-id="79440-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="79440-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79440-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="79440-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79440-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="79440-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="79440-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="79440-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79440-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79440-115">Not supported.</span></span>|
|<span data-ttu-id="79440-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="79440-116">Application</span></span>|<span data-ttu-id="79440-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79440-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79440-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="79440-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="79440-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="79440-119">Request headers</span></span>
|<span data-ttu-id="79440-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="79440-120">Header</span></span>|<span data-ttu-id="79440-121">Wert</span><span class="sxs-lookup"><span data-stu-id="79440-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79440-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="79440-122">Authorization</span></span>|<span data-ttu-id="79440-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="79440-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79440-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="79440-124">Accept</span></span>|<span data-ttu-id="79440-125">application/json</span><span class="sxs-lookup"><span data-stu-id="79440-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79440-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="79440-126">Request body</span></span>
<span data-ttu-id="79440-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="79440-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79440-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="79440-128">Response</span></span>
<span data-ttu-id="79440-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von Objekten des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="79440-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79440-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="79440-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="79440-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="79440-131">Request</span></span>
<span data-ttu-id="79440-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="79440-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="79440-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="79440-133">Response</span></span>
<span data-ttu-id="79440-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79440-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 616

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
      "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "status": "connectionPending",
      "primarySmtpAddress": "Primary Smtp Address value",
      "serverName": "Server Name value",
      "connectorServerName": "Connector Server Name value",
      "exchangeConnectorType": "hosted",
      "version": "Version value",
      "exchangeAlias": "Exchange Alias value",
      "exchangeOrganization": "Exchange Organization value"
    }
  ]
}
```




