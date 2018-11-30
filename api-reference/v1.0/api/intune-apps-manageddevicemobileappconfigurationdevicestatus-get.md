---
title: Abrufen von managedDeviceMobileAppConfigurationDeviceStatus
description: Lesen Sie Eigenschaften und Beziehungen des ManagedDeviceMobileAppConfigurationDeviceStatus-Objekts.
ms.openlocfilehash: f9e55112a29abc89adfdef2172d86aa9914e3d1f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017415"
---
# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="9a517-103">Abrufen von managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="9a517-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="9a517-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9a517-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a517-105">Lesen Sie Eigenschaften und Beziehungen des [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9a517-105">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9a517-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9a517-106">Prerequisites</span></span>
<span data-ttu-id="9a517-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a517-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a517-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9a517-109">Permission type</span></span>|<span data-ttu-id="9a517-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9a517-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a517-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9a517-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9a517-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a517-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9a517-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9a517-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a517-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a517-114">Not supported.</span></span>|
|<span data-ttu-id="9a517-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9a517-115">Application</span></span>|<span data-ttu-id="9a517-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a517-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a517-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a517-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9a517-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9a517-118">Optional query parameters</span></span>
<span data-ttu-id="9a517-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9a517-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9a517-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9a517-120">Request headers</span></span>
|<span data-ttu-id="9a517-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9a517-121">Header</span></span>|<span data-ttu-id="9a517-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9a517-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a517-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a517-123">Authorization</span></span>|<span data-ttu-id="9a517-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9a517-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a517-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9a517-125">Accept</span></span>|<span data-ttu-id="9a517-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a517-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a517-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9a517-127">Request body</span></span>
<span data-ttu-id="9a517-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9a517-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a517-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a517-129">Response</span></span>
<span data-ttu-id="9a517-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9a517-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a517-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9a517-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9a517-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a517-132">Request</span></span>
<span data-ttu-id="9a517-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9a517-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="9a517-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a517-134">Response</span></span>
<span data-ttu-id="9a517-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a517-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 531

{
  "value": {
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
}
```



