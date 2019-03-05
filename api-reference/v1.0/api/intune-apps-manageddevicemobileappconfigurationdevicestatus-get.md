---
title: ManagedDeviceMobileAppConfigurationDeviceStatus abrufen
description: Lesen von Eigenschaften und Beziehungen des managedDeviceMobileAppConfigurationDeviceStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b5493635a66d29cadd3fc1d8f32fcbb94b7482bb
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256567"
---
# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="7da3c-103">ManagedDeviceMobileAppConfigurationDeviceStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="7da3c-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="7da3c-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7da3c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7da3c-105">Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7da3c-105">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7da3c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7da3c-106">Prerequisites</span></span>
<span data-ttu-id="7da3c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7da3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7da3c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7da3c-109">Permission type</span></span>|<span data-ttu-id="7da3c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7da3c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7da3c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7da3c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7da3c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7da3c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7da3c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7da3c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7da3c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7da3c-114">Not supported.</span></span>|
|<span data-ttu-id="7da3c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7da3c-115">Application</span></span>|<span data-ttu-id="7da3c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7da3c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7da3c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7da3c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7da3c-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7da3c-118">Optional query parameters</span></span>
<span data-ttu-id="7da3c-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7da3c-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7da3c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7da3c-120">Request headers</span></span>
|<span data-ttu-id="7da3c-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7da3c-121">Header</span></span>|<span data-ttu-id="7da3c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7da3c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7da3c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7da3c-123">Authorization</span></span>|<span data-ttu-id="7da3c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7da3c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7da3c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7da3c-125">Accept</span></span>|<span data-ttu-id="7da3c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7da3c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7da3c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7da3c-127">Request body</span></span>
<span data-ttu-id="7da3c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7da3c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7da3c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7da3c-129">Response</span></span>
<span data-ttu-id="7da3c-130">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7da3c-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7da3c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7da3c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7da3c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7da3c-132">Request</span></span>
<span data-ttu-id="7da3c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7da3c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="7da3c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="7da3c-134">Response</span></span>
<span data-ttu-id="7da3c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7da3c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



