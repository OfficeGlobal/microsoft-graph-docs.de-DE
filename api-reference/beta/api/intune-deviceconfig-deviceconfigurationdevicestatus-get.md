---
title: deviceConfigurationDeviceStatus abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceConfigurationDeviceStatus-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 94e7462406b9310366f9a3c28c4fb25f370697e1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406220"
---
# <a name="get-deviceconfigurationdevicestatus"></a><span data-ttu-id="2f293-103">deviceConfigurationDeviceStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="2f293-103">Get deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="2f293-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2f293-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2f293-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2f293-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f293-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2f293-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f293-107">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2f293-107">Read properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f293-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2f293-108">Prerequisites</span></span>
<span data-ttu-id="2f293-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f293-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2f293-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f293-111">Permission type</span></span>|<span data-ttu-id="2f293-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f293-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f293-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f293-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f293-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f293-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2f293-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f293-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f293-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f293-116">Not supported.</span></span>|
|<span data-ttu-id="2f293-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f293-117">Application</span></span>|<span data-ttu-id="2f293-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f293-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f293-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f293-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="2f293-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2f293-120">Optional query parameters</span></span>
<span data-ttu-id="2f293-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2f293-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f293-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f293-122">Request headers</span></span>
|<span data-ttu-id="2f293-123">Header</span><span class="sxs-lookup"><span data-stu-id="2f293-123">Header</span></span>|<span data-ttu-id="2f293-124">Wert</span><span class="sxs-lookup"><span data-stu-id="2f293-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f293-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2f293-125">Authorization</span></span>|<span data-ttu-id="2f293-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2f293-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f293-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2f293-127">Accept</span></span>|<span data-ttu-id="2f293-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2f293-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f293-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f293-129">Request body</span></span>
<span data-ttu-id="2f293-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2f293-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f293-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f293-131">Response</span></span>
<span data-ttu-id="2f293-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f293-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f293-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f293-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f293-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f293-134">Request</span></span>
<span data-ttu-id="2f293-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f293-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="2f293-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f293-136">Response</span></span>
<span data-ttu-id="2f293-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f293-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




