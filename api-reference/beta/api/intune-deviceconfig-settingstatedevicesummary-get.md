---
title: Abrufen von „settingStateDeviceSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs settingStateDeviceSummary.
author: tfitzmac
ms.openlocfilehash: 3308a4fff48b6433d7c35303566ddc73f03c23e6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333509"
---
# <a name="get-settingstatedevicesummary"></a><span data-ttu-id="da3de-103">Abrufen von „settingStateDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="da3de-103">Get settingStateDeviceSummary</span></span>

> <span data-ttu-id="da3de-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="da3de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da3de-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da3de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da3de-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="da3de-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da3de-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="da3de-107">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da3de-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="da3de-108">Prerequisites</span></span>
<span data-ttu-id="da3de-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da3de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da3de-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="da3de-111">Permission type</span></span>|<span data-ttu-id="da3de-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="da3de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da3de-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="da3de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da3de-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="da3de-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="da3de-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="da3de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da3de-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da3de-116">Not supported.</span></span>|
|<span data-ttu-id="da3de-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="da3de-117">Application</span></span>|<span data-ttu-id="da3de-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da3de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da3de-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="da3de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da3de-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="da3de-120">Optional query parameters</span></span>
<span data-ttu-id="da3de-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="da3de-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="da3de-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="da3de-122">Request headers</span></span>
|<span data-ttu-id="da3de-123">Header</span><span class="sxs-lookup"><span data-stu-id="da3de-123">Header</span></span>|<span data-ttu-id="da3de-124">Wert</span><span class="sxs-lookup"><span data-stu-id="da3de-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da3de-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="da3de-125">Authorization</span></span>|<span data-ttu-id="da3de-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="da3de-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da3de-127">Accept</span><span class="sxs-lookup"><span data-stu-id="da3de-127">Accept</span></span>|<span data-ttu-id="da3de-128">application/json</span><span class="sxs-lookup"><span data-stu-id="da3de-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da3de-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="da3de-129">Request body</span></span>
<span data-ttu-id="da3de-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="da3de-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da3de-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="da3de-131">Response</span></span>
<span data-ttu-id="da3de-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="da3de-132">If successful, this method returns a `200 OK` response code and [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da3de-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="da3de-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="da3de-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="da3de-134">Request</span></span>
<span data-ttu-id="da3de-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="da3de-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="da3de-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="da3de-136">Response</span></span>
<span data-ttu-id="da3de-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="da3de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": {
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
}
```





