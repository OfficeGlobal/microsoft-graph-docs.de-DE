---
title: Abrufen von „settingStateDeviceSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1e1dbe0276d7b2e66e499609e929a3c7995773da
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976603"
---
# <a name="get-settingstatedevicesummary"></a><span data-ttu-id="35fc9-103">Abrufen von „settingStateDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="35fc9-103">Get settingStateDeviceSummary</span></span>

> <span data-ttu-id="35fc9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="35fc9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35fc9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="35fc9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35fc9-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="35fc9-106">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35fc9-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="35fc9-107">Prerequisites</span></span>
<span data-ttu-id="35fc9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35fc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35fc9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="35fc9-110">Permission type</span></span>|<span data-ttu-id="35fc9-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="35fc9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35fc9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="35fc9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35fc9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="35fc9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="35fc9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="35fc9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35fc9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35fc9-115">Not supported.</span></span>|
|<span data-ttu-id="35fc9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="35fc9-116">Application</span></span>|<span data-ttu-id="35fc9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35fc9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35fc9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="35fc9-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="35fc9-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="35fc9-119">Optional query parameters</span></span>
<span data-ttu-id="35fc9-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="35fc9-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35fc9-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="35fc9-121">Request headers</span></span>
|<span data-ttu-id="35fc9-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="35fc9-122">Header</span></span>|<span data-ttu-id="35fc9-123">Wert</span><span class="sxs-lookup"><span data-stu-id="35fc9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35fc9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="35fc9-124">Authorization</span></span>|<span data-ttu-id="35fc9-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="35fc9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35fc9-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="35fc9-126">Accept</span></span>|<span data-ttu-id="35fc9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="35fc9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35fc9-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="35fc9-128">Request body</span></span>
<span data-ttu-id="35fc9-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="35fc9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35fc9-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="35fc9-130">Response</span></span>
<span data-ttu-id="35fc9-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="35fc9-131">If successful, this method returns a `200 OK` response code and [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35fc9-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="35fc9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="35fc9-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="35fc9-133">Request</span></span>
<span data-ttu-id="35fc9-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="35fc9-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="35fc9-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="35fc9-135">Response</span></span>
<span data-ttu-id="35fc9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="35fc9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




