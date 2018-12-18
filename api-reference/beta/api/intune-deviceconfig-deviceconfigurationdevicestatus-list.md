---
title: Auflisten von „deviceConfigurationDeviceStatus“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceConfigurationDeviceStatus auf.
author: tfitzmac
ms.openlocfilehash: 2ec7116917891e29798a71b2cb36a75a7468fe1b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336568"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="abf92-103">Auflisten von „deviceConfigurationDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="abf92-103">List deviceConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="abf92-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="abf92-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abf92-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="abf92-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abf92-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="abf92-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abf92-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) auf.</span><span class="sxs-lookup"><span data-stu-id="abf92-107">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="abf92-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="abf92-108">Prerequisites</span></span>
<span data-ttu-id="abf92-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abf92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abf92-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="abf92-111">Permission type</span></span>|<span data-ttu-id="abf92-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="abf92-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abf92-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="abf92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abf92-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="abf92-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="abf92-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="abf92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abf92-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abf92-116">Not supported.</span></span>|
|<span data-ttu-id="abf92-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="abf92-117">Application</span></span>|<span data-ttu-id="abf92-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abf92-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abf92-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="abf92-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="abf92-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="abf92-120">Request headers</span></span>
|<span data-ttu-id="abf92-121">Header</span><span class="sxs-lookup"><span data-stu-id="abf92-121">Header</span></span>|<span data-ttu-id="abf92-122">Wert</span><span class="sxs-lookup"><span data-stu-id="abf92-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abf92-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="abf92-123">Authorization</span></span>|<span data-ttu-id="abf92-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="abf92-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abf92-125">Accept</span><span class="sxs-lookup"><span data-stu-id="abf92-125">Accept</span></span>|<span data-ttu-id="abf92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abf92-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abf92-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="abf92-127">Request body</span></span>
<span data-ttu-id="abf92-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="abf92-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abf92-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="abf92-129">Response</span></span>
<span data-ttu-id="abf92-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="abf92-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abf92-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="abf92-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="abf92-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="abf92-132">Request</span></span>
<span data-ttu-id="abf92-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="abf92-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="abf92-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="abf92-134">Response</span></span>
<span data-ttu-id="abf92-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="abf92-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





