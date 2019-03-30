---
title: ManagedDeviceMobileAppConfigurationDeviceStatus abrufen
description: Lesen von Eigenschaften und Beziehungen des managedDeviceMobileAppConfigurationDeviceStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8fea7554c85f7b47eb5964a2fe12dbe16a22e09c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974244"
---
# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="683cd-103">ManagedDeviceMobileAppConfigurationDeviceStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="683cd-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="683cd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="683cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="683cd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="683cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="683cd-106">Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="683cd-106">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="683cd-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="683cd-107">Prerequisites</span></span>
<span data-ttu-id="683cd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="683cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="683cd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="683cd-110">Permission type</span></span>|<span data-ttu-id="683cd-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="683cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="683cd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="683cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="683cd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="683cd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="683cd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="683cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="683cd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="683cd-115">Not supported.</span></span>|
|<span data-ttu-id="683cd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="683cd-116">Application</span></span>|<span data-ttu-id="683cd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="683cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="683cd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="683cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="683cd-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="683cd-119">Optional query parameters</span></span>
<span data-ttu-id="683cd-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="683cd-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="683cd-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="683cd-121">Request headers</span></span>
|<span data-ttu-id="683cd-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="683cd-122">Header</span></span>|<span data-ttu-id="683cd-123">Wert</span><span class="sxs-lookup"><span data-stu-id="683cd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="683cd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="683cd-124">Authorization</span></span>|<span data-ttu-id="683cd-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="683cd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="683cd-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="683cd-126">Accept</span></span>|<span data-ttu-id="683cd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="683cd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="683cd-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="683cd-128">Request body</span></span>
<span data-ttu-id="683cd-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="683cd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="683cd-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="683cd-130">Response</span></span>
<span data-ttu-id="683cd-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="683cd-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="683cd-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="683cd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="683cd-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="683cd-133">Request</span></span>
<span data-ttu-id="683cd-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="683cd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="683cd-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="683cd-135">Response</span></span>
<span data-ttu-id="683cd-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="683cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




