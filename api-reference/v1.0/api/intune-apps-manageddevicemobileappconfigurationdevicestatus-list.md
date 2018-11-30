---
title: Liste managedDeviceMobileAppConfigurationDeviceStatuses
description: Listeneigenschaften und Beziehungen der ManagedDeviceMobileAppConfigurationDeviceStatus-Objekte.
ms.openlocfilehash: 0bdbc59ce4aaa32054a8ee8e25535e6dfc03d5eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018164"
---
# <a name="list-manageddevicemobileappconfigurationdevicestatuses"></a><span data-ttu-id="073bc-103">Liste managedDeviceMobileAppConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="073bc-103">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="073bc-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="073bc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="073bc-105">Listeneigenschaften und Beziehungen der [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="073bc-105">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="073bc-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="073bc-106">Prerequisites</span></span>
<span data-ttu-id="073bc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="073bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="073bc-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="073bc-109">Permission type</span></span>|<span data-ttu-id="073bc-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="073bc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="073bc-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="073bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="073bc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="073bc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="073bc-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="073bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="073bc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="073bc-114">Not supported.</span></span>|
|<span data-ttu-id="073bc-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="073bc-115">Application</span></span>|<span data-ttu-id="073bc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="073bc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="073bc-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="073bc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="073bc-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="073bc-118">Request headers</span></span>
|<span data-ttu-id="073bc-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="073bc-119">Header</span></span>|<span data-ttu-id="073bc-120">Wert</span><span class="sxs-lookup"><span data-stu-id="073bc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="073bc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="073bc-121">Authorization</span></span>|<span data-ttu-id="073bc-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="073bc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="073bc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="073bc-123">Accept</span></span>|<span data-ttu-id="073bc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="073bc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="073bc-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="073bc-125">Request body</span></span>
<span data-ttu-id="073bc-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="073bc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="073bc-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="073bc-127">Response</span></span>
<span data-ttu-id="073bc-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="073bc-128">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="073bc-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="073bc-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="073bc-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="073bc-130">Request</span></span>
<span data-ttu-id="073bc-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="073bc-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="073bc-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="073bc-132">Response</span></span>
<span data-ttu-id="073bc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="073bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 563

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
      "id": "477d3651-3651-477d-5136-7d4751367d47",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



