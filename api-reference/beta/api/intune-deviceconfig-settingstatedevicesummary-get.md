---
title: Abrufen von „settingStateDeviceSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs settingStateDeviceSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ab2d1b1d23b740290105d67fc591d20ceaa6b322
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423013"
---
# <a name="get-settingstatedevicesummary"></a><span data-ttu-id="90500-103">Abrufen von „settingStateDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="90500-103">Get settingStateDeviceSummary</span></span>

> <span data-ttu-id="90500-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="90500-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="90500-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="90500-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="90500-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="90500-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90500-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="90500-107">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90500-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="90500-108">Prerequisites</span></span>
<span data-ttu-id="90500-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="90500-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="90500-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="90500-111">Permission type</span></span>|<span data-ttu-id="90500-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="90500-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90500-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="90500-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90500-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="90500-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="90500-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="90500-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90500-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="90500-116">Not supported.</span></span>|
|<span data-ttu-id="90500-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="90500-117">Application</span></span>|<span data-ttu-id="90500-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="90500-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90500-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="90500-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="90500-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="90500-120">Optional query parameters</span></span>
<span data-ttu-id="90500-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="90500-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90500-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="90500-122">Request headers</span></span>
|<span data-ttu-id="90500-123">Header</span><span class="sxs-lookup"><span data-stu-id="90500-123">Header</span></span>|<span data-ttu-id="90500-124">Wert</span><span class="sxs-lookup"><span data-stu-id="90500-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90500-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="90500-125">Authorization</span></span>|<span data-ttu-id="90500-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="90500-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90500-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="90500-127">Accept</span></span>|<span data-ttu-id="90500-128">application/json</span><span class="sxs-lookup"><span data-stu-id="90500-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90500-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="90500-129">Request body</span></span>
<span data-ttu-id="90500-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="90500-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90500-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="90500-131">Response</span></span>
<span data-ttu-id="90500-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="90500-132">If successful, this method returns a `200 OK` response code and [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90500-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="90500-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="90500-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="90500-134">Request</span></span>
<span data-ttu-id="90500-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="90500-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="90500-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="90500-136">Response</span></span>
<span data-ttu-id="90500-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="90500-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




