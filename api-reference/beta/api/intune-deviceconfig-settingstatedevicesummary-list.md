---
title: Auflisten von „settingStateDeviceSummary“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs settingStateDeviceSummary auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30e27fd4320cb89720c89034b9131b6b429c7e2e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959397"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="650c5-103">Auflisten von „settingStateDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="650c5-103">List settingStateDeviceSummaries</span></span>

> <span data-ttu-id="650c5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="650c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="650c5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="650c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="650c5-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) auf.</span><span class="sxs-lookup"><span data-stu-id="650c5-106">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="650c5-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="650c5-107">Prerequisites</span></span>
<span data-ttu-id="650c5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="650c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="650c5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="650c5-110">Permission type</span></span>|<span data-ttu-id="650c5-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="650c5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="650c5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="650c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="650c5-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="650c5-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="650c5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="650c5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="650c5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="650c5-115">Not supported.</span></span>|
|<span data-ttu-id="650c5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="650c5-116">Application</span></span>|<span data-ttu-id="650c5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="650c5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="650c5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="650c5-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="650c5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="650c5-119">Request headers</span></span>
|<span data-ttu-id="650c5-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="650c5-120">Header</span></span>|<span data-ttu-id="650c5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="650c5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="650c5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="650c5-122">Authorization</span></span>|<span data-ttu-id="650c5-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="650c5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="650c5-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="650c5-124">Accept</span></span>|<span data-ttu-id="650c5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="650c5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="650c5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="650c5-126">Request body</span></span>
<span data-ttu-id="650c5-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="650c5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="650c5-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="650c5-128">Response</span></span>
<span data-ttu-id="650c5-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="650c5-129">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="650c5-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="650c5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="650c5-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="650c5-131">Request</span></span>
<span data-ttu-id="650c5-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="650c5-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="650c5-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="650c5-133">Response</span></span>
<span data-ttu-id="650c5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="650c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




