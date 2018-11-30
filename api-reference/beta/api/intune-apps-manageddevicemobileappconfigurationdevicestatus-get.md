---
title: Abrufen von managedDeviceMobileAppConfigurationDeviceStatus
description: Lesen Sie Eigenschaften und Beziehungen des ManagedDeviceMobileAppConfigurationDeviceStatus-Objekts.
ms.openlocfilehash: 2dfa08ae817c2ffbf4fcfdf241eb190942efe904
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060531"
---
# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="be047-103">Abrufen von managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="be047-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="be047-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="be047-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be047-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="be047-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be047-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="be047-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be047-107">Lesen Sie Eigenschaften und Beziehungen des [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="be047-107">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be047-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="be047-108">Prerequisites</span></span>
<span data-ttu-id="be047-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be047-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be047-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="be047-111">Permission type</span></span>|<span data-ttu-id="be047-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="be047-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be047-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="be047-113">Delegated (work or school account)</span></span>|<span data-ttu-id="be047-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="be047-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="be047-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="be047-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be047-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be047-116">Not supported.</span></span>|
|<span data-ttu-id="be047-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="be047-117">Application</span></span>|<span data-ttu-id="be047-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be047-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be047-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="be047-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be047-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="be047-120">Optional query parameters</span></span>
<span data-ttu-id="be047-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="be047-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="be047-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="be047-122">Request headers</span></span>
|<span data-ttu-id="be047-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="be047-123">Header</span></span>|<span data-ttu-id="be047-124">Wert</span><span class="sxs-lookup"><span data-stu-id="be047-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be047-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="be047-125">Authorization</span></span>|<span data-ttu-id="be047-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="be047-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be047-127">Accept</span><span class="sxs-lookup"><span data-stu-id="be047-127">Accept</span></span>|<span data-ttu-id="be047-128">application/json</span><span class="sxs-lookup"><span data-stu-id="be047-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be047-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="be047-129">Request body</span></span>
<span data-ttu-id="be047-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="be047-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be047-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="be047-131">Response</span></span>
<span data-ttu-id="be047-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="be047-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be047-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="be047-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="be047-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="be047-134">Request</span></span>
<span data-ttu-id="be047-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="be047-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="be047-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="be047-136">Response</span></span>
<span data-ttu-id="be047-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be047-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 551

{
  "value": {
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
}
```





