---
title: deviceConfigurationDeviceOverview abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceConfigurationDeviceOverview-Objekts.
ms.openlocfilehash: 9c195553b6bb8beefe54d16181918f13656acbad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062575"
---
# <a name="get-deviceconfigurationdeviceoverview"></a><span data-ttu-id="c9bd8-103">deviceConfigurationDeviceOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="c9bd8-103">Get deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="c9bd8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c9bd8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9bd8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9bd8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9bd8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c9bd8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9bd8-107">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c9bd8-107">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9bd8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c9bd8-108">Prerequisites</span></span>
<span data-ttu-id="c9bd8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9bd8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9bd8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c9bd8-111">Permission type</span></span>|<span data-ttu-id="c9bd8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c9bd8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9bd8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c9bd8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9bd8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9bd8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c9bd8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c9bd8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9bd8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9bd8-116">Not supported.</span></span>|
|<span data-ttu-id="c9bd8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c9bd8-117">Application</span></span>|<span data-ttu-id="c9bd8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9bd8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9bd8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9bd8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9bd8-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c9bd8-120">Optional query parameters</span></span>
<span data-ttu-id="c9bd8-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c9bd8-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c9bd8-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c9bd8-122">Request headers</span></span>
|<span data-ttu-id="c9bd8-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c9bd8-123">Header</span></span>|<span data-ttu-id="c9bd8-124">Wert</span><span class="sxs-lookup"><span data-stu-id="c9bd8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9bd8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9bd8-125">Authorization</span></span>|<span data-ttu-id="c9bd8-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c9bd8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9bd8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c9bd8-127">Accept</span></span>|<span data-ttu-id="c9bd8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c9bd8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9bd8-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c9bd8-129">Request body</span></span>
<span data-ttu-id="c9bd8-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c9bd8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9bd8-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9bd8-131">Response</span></span>
<span data-ttu-id="c9bd8-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9bd8-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9bd8-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c9bd8-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9bd8-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9bd8-134">Request</span></span>
<span data-ttu-id="c9bd8-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c9bd8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="c9bd8-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9bd8-136">Response</span></span>
<span data-ttu-id="c9bd8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9bd8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 435

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
    "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```





