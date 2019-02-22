---
title: Auflisten von „deviceConfigurationDeviceStatus“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceConfigurationDeviceStatus auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aae4e87029cb2ce6bdb93581df5599062f3af260
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173304"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="f3874-103">Auflisten von „deviceConfigurationDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="f3874-103">List deviceConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="f3874-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3874-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3874-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f3874-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3874-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) auf.</span><span class="sxs-lookup"><span data-stu-id="f3874-106">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3874-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f3874-107">Prerequisites</span></span>
<span data-ttu-id="f3874-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f3874-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f3874-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f3874-110">Permission type</span></span>|<span data-ttu-id="f3874-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f3874-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3874-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f3874-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3874-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3874-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f3874-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f3874-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3874-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3874-115">Not supported.</span></span>|
|<span data-ttu-id="f3874-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f3874-116">Application</span></span>|<span data-ttu-id="f3874-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3874-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3874-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3874-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="f3874-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f3874-119">Request headers</span></span>
|<span data-ttu-id="f3874-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f3874-120">Header</span></span>|<span data-ttu-id="f3874-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f3874-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3874-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3874-122">Authorization</span></span>|<span data-ttu-id="f3874-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f3874-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3874-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f3874-124">Accept</span></span>|<span data-ttu-id="f3874-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3874-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3874-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f3874-126">Request body</span></span>
<span data-ttu-id="f3874-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f3874-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3874-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3874-128">Response</span></span>
<span data-ttu-id="f3874-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f3874-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3874-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f3874-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3874-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3874-131">Request</span></span>
<span data-ttu-id="f3874-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f3874-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="f3874-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3874-133">Response</span></span>
<span data-ttu-id="f3874-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3874-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 569

{
  "value": [
    {
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
  ]
}
```




