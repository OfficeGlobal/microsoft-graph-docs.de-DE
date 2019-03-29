---
title: ManagedDeviceMobileAppConfigurationDeviceStatuses aufListen
description: AufListen von Eigenschaften und Beziehungen der managedDeviceMobileAppConfigurationDeviceStatus-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6289173d36419b629c663c182b4b1459a8ec8afb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958907"
---
# <a name="list-manageddevicemobileappconfigurationdevicestatuses"></a><span data-ttu-id="c54ee-103">ManagedDeviceMobileAppConfigurationDeviceStatuses aufListen</span><span class="sxs-lookup"><span data-stu-id="c54ee-103">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="c54ee-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c54ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c54ee-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c54ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c54ee-106">AufListen von Eigenschaften und Beziehungen der [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="c54ee-106">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c54ee-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c54ee-107">Prerequisites</span></span>
<span data-ttu-id="c54ee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c54ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c54ee-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c54ee-110">Permission type</span></span>|<span data-ttu-id="c54ee-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c54ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c54ee-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c54ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c54ee-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c54ee-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c54ee-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c54ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c54ee-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c54ee-115">Not supported.</span></span>|
|<span data-ttu-id="c54ee-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c54ee-116">Application</span></span>|<span data-ttu-id="c54ee-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c54ee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c54ee-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c54ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c54ee-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c54ee-119">Request headers</span></span>
|<span data-ttu-id="c54ee-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c54ee-120">Header</span></span>|<span data-ttu-id="c54ee-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c54ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c54ee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c54ee-122">Authorization</span></span>|<span data-ttu-id="c54ee-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c54ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c54ee-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c54ee-124">Accept</span></span>|<span data-ttu-id="c54ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c54ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c54ee-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c54ee-126">Request body</span></span>
<span data-ttu-id="c54ee-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c54ee-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c54ee-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="c54ee-128">Response</span></span>
<span data-ttu-id="c54ee-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c54ee-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c54ee-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c54ee-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c54ee-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c54ee-131">Request</span></span>
<span data-ttu-id="c54ee-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c54ee-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="c54ee-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c54ee-133">Response</span></span>
<span data-ttu-id="c54ee-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c54ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 585

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
      "id": "477d3651-3651-477d-5136-7d4751367d47",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "platform": 8,
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




