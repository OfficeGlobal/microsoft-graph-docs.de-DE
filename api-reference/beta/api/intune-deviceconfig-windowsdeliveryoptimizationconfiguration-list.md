---
title: WindowsDeliveryOptimizationConfigurations aufListen
description: AufListen von Eigenschaften und Beziehungen der windowsDeliveryOptimizationConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8652ff72647740ebcaf8b62ccdd5c1fa91d86762
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168075"
---
# <a name="list-windowsdeliveryoptimizationconfigurations"></a><span data-ttu-id="2da75-103">WindowsDeliveryOptimizationConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="2da75-103">List windowsDeliveryOptimizationConfigurations</span></span>

> <span data-ttu-id="2da75-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2da75-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2da75-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2da75-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2da75-106">AufListen von Eigenschaften und Beziehungen der [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="2da75-106">List properties and relationships of the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2da75-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2da75-107">Prerequisites</span></span>
<span data-ttu-id="2da75-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2da75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2da75-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2da75-110">Permission type</span></span>|<span data-ttu-id="2da75-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2da75-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2da75-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2da75-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2da75-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2da75-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2da75-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2da75-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2da75-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2da75-115">Not supported.</span></span>|
|<span data-ttu-id="2da75-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2da75-116">Application</span></span>|<span data-ttu-id="2da75-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2da75-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2da75-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2da75-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2da75-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2da75-119">Request headers</span></span>
|<span data-ttu-id="2da75-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2da75-120">Header</span></span>|<span data-ttu-id="2da75-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2da75-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2da75-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2da75-122">Authorization</span></span>|<span data-ttu-id="2da75-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2da75-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2da75-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2da75-124">Accept</span></span>|<span data-ttu-id="2da75-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2da75-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2da75-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2da75-126">Request body</span></span>
<span data-ttu-id="2da75-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2da75-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2da75-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="2da75-128">Response</span></span>
<span data-ttu-id="2da75-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2da75-129">If successful, this method returns a `200 OK` response code and a collection of [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2da75-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2da75-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2da75-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2da75-131">Request</span></span>
<span data-ttu-id="2da75-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2da75-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="2da75-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="2da75-133">Response</span></span>
<span data-ttu-id="2da75-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2da75-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1389

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
      "id": "5954ee9b-ee9b-5954-9bee-54599bee5459",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "deliveryOptimizationMode": "httpOnly",
      "restrictPeerSelectionBy": "subnetMask",
      "groupIdSource": {
        "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
      },
      "bandwidthMode": {
        "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
      },
      "backgroundDownloadFromHttpDelayInSeconds": 8,
      "foregroundDownloadFromHttpDelayInSeconds": 8,
      "minimumRamAllowedToPeerInGigabytes": 2,
      "minimumDiskSizeAllowedToPeerInGigabytes": 7,
      "minimumFileSizeToCacheInMegabytes": 1,
      "minimumBatteryPercentageAllowedToUpload": 7,
      "modifyCacheLocation": "Modify Cache Location value",
      "maximumCacheAgeInDays": 5,
      "maximumCacheSize": {
        "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
      },
      "vpnPeerCaching": "enabled"
    }
  ]
}
```




