---
title: Auflisten von „settingStateDeviceSummary“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs settingStateDeviceSummary auf.
ms.openlocfilehash: 67439546e66b863ea4a0fbc91dbbab76ef2d66c7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058803"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="ef39f-103">Auflisten von „settingStateDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="ef39f-103">List settingStateDeviceSummaries</span></span>

> <span data-ttu-id="ef39f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ef39f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef39f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ef39f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef39f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ef39f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef39f-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) auf.</span><span class="sxs-lookup"><span data-stu-id="ef39f-107">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef39f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ef39f-108">Prerequisites</span></span>
<span data-ttu-id="ef39f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef39f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef39f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ef39f-111">Permission type</span></span>|<span data-ttu-id="ef39f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ef39f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef39f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ef39f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef39f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef39f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ef39f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ef39f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef39f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef39f-116">Not supported.</span></span>|
|<span data-ttu-id="ef39f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ef39f-117">Application</span></span>|<span data-ttu-id="ef39f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef39f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef39f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef39f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="ef39f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ef39f-120">Request headers</span></span>
|<span data-ttu-id="ef39f-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ef39f-121">Header</span></span>|<span data-ttu-id="ef39f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ef39f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef39f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef39f-123">Authorization</span></span>|<span data-ttu-id="ef39f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ef39f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef39f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef39f-125">Accept</span></span>|<span data-ttu-id="ef39f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef39f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef39f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ef39f-127">Request body</span></span>
<span data-ttu-id="ef39f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ef39f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef39f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef39f-129">Response</span></span>
<span data-ttu-id="ef39f-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ef39f-130">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef39f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ef39f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef39f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef39f-132">Request</span></span>
<span data-ttu-id="ef39f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ef39f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="ef39f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef39f-134">Response</span></span>
<span data-ttu-id="ef39f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef39f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 486

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
      "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
      "settingName": "Setting Name value",
      "instancePath": "Instance Path value",
      "unknownDeviceCount": 2,
      "notApplicableDeviceCount": 8,
      "compliantDeviceCount": 4,
      "remediatedDeviceCount": 5,
      "nonCompliantDeviceCount": 7,
      "errorDeviceCount": 0,
      "conflictDeviceCount": 3
    }
  ]
}
```





