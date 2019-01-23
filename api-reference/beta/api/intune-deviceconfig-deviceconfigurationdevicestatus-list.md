---
title: Auflisten von „deviceConfigurationDeviceStatus“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceConfigurationDeviceStatus auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b470403c3e7581e353326a0557ea78f4feb63e25
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393865"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="ebccb-103">Auflisten von „deviceConfigurationDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="ebccb-103">List deviceConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="ebccb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ebccb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ebccb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ebccb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebccb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ebccb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebccb-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) auf.</span><span class="sxs-lookup"><span data-stu-id="ebccb-107">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebccb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ebccb-108">Prerequisites</span></span>
<span data-ttu-id="ebccb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ebccb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ebccb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ebccb-111">Permission type</span></span>|<span data-ttu-id="ebccb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ebccb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebccb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ebccb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ebccb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebccb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ebccb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ebccb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebccb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ebccb-116">Not supported.</span></span>|
|<span data-ttu-id="ebccb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ebccb-117">Application</span></span>|<span data-ttu-id="ebccb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ebccb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebccb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebccb-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="ebccb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ebccb-120">Request headers</span></span>
|<span data-ttu-id="ebccb-121">Header</span><span class="sxs-lookup"><span data-stu-id="ebccb-121">Header</span></span>|<span data-ttu-id="ebccb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ebccb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebccb-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ebccb-123">Authorization</span></span>|<span data-ttu-id="ebccb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ebccb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebccb-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ebccb-125">Accept</span></span>|<span data-ttu-id="ebccb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ebccb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebccb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ebccb-127">Request body</span></span>
<span data-ttu-id="ebccb-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ebccb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebccb-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebccb-129">Response</span></span>
<span data-ttu-id="ebccb-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ebccb-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebccb-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ebccb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebccb-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebccb-132">Request</span></span>
<span data-ttu-id="ebccb-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ebccb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="ebccb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebccb-134">Response</span></span>
<span data-ttu-id="ebccb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ebccb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




