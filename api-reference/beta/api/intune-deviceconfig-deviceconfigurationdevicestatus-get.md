---
title: deviceConfigurationDeviceStatus abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceConfigurationDeviceStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb74ad2d5d765b7e15d8e928a2e8117d39ae3d5c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143099"
---
# <a name="get-deviceconfigurationdevicestatus"></a><span data-ttu-id="8899b-103">deviceConfigurationDeviceStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="8899b-103">Get deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="8899b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8899b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8899b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8899b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8899b-106">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8899b-106">Read properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8899b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8899b-107">Prerequisites</span></span>
<span data-ttu-id="8899b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8899b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8899b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8899b-110">Permission type</span></span>|<span data-ttu-id="8899b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8899b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8899b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8899b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8899b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8899b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8899b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8899b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8899b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8899b-115">Not supported.</span></span>|
|<span data-ttu-id="8899b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8899b-116">Application</span></span>|<span data-ttu-id="8899b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8899b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8899b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8899b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8899b-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8899b-119">Optional query parameters</span></span>
<span data-ttu-id="8899b-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8899b-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8899b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8899b-121">Request headers</span></span>
|<span data-ttu-id="8899b-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8899b-122">Header</span></span>|<span data-ttu-id="8899b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="8899b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8899b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8899b-124">Authorization</span></span>|<span data-ttu-id="8899b-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8899b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8899b-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8899b-126">Accept</span></span>|<span data-ttu-id="8899b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8899b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8899b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8899b-128">Request body</span></span>
<span data-ttu-id="8899b-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8899b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8899b-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="8899b-130">Response</span></span>
<span data-ttu-id="8899b-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8899b-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8899b-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8899b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8899b-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8899b-133">Request</span></span>
<span data-ttu-id="8899b-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8899b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="8899b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="8899b-135">Response</span></span>
<span data-ttu-id="8899b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8899b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 535

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
    "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
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




