---
title: Liste managedDeviceMobileAppConfigurationDeviceStatuses
description: Listeneigenschaften und Beziehungen der ManagedDeviceMobileAppConfigurationDeviceStatus-Objekte.
author: tfitzmac
ms.openlocfilehash: eebe5ec2da36cad972af87600b6d6776debcbbee
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342966"
---
# <a name="list-manageddevicemobileappconfigurationdevicestatuses"></a><span data-ttu-id="3d684-103">Liste managedDeviceMobileAppConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="3d684-103">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="3d684-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3d684-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d684-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3d684-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d684-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3d684-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d684-107">Listeneigenschaften und Beziehungen der [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="3d684-107">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3d684-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3d684-108">Prerequisites</span></span>
<span data-ttu-id="3d684-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d684-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d684-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3d684-111">Permission type</span></span>|<span data-ttu-id="3d684-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3d684-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d684-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3d684-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d684-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d684-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3d684-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3d684-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d684-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d684-116">Not supported.</span></span>|
|<span data-ttu-id="3d684-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3d684-117">Application</span></span>|<span data-ttu-id="3d684-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d684-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d684-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d684-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="3d684-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3d684-120">Request headers</span></span>
|<span data-ttu-id="3d684-121">Header</span><span class="sxs-lookup"><span data-stu-id="3d684-121">Header</span></span>|<span data-ttu-id="3d684-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3d684-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d684-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3d684-123">Authorization</span></span>|<span data-ttu-id="3d684-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3d684-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d684-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3d684-125">Accept</span></span>|<span data-ttu-id="3d684-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d684-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d684-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3d684-127">Request body</span></span>
<span data-ttu-id="3d684-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3d684-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d684-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d684-129">Response</span></span>
<span data-ttu-id="3d684-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="3d684-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d684-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3d684-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3d684-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d684-132">Request</span></span>
<span data-ttu-id="3d684-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3d684-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="3d684-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d684-134">Response</span></span>
<span data-ttu-id="3d684-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3d684-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





