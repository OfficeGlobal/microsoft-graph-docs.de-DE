---
title: deviceConfigurationUserOverview abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceConfigurationUserOverview-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c6a7a2926c8139c19521b1ae52ee39b402aaceb6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411995"
---
# <a name="get-deviceconfigurationuseroverview"></a><span data-ttu-id="6e8ba-103">deviceConfigurationUserOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="6e8ba-103">Get deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="6e8ba-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6e8ba-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6e8ba-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6e8ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e8ba-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6e8ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e8ba-107">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6e8ba-107">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e8ba-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6e8ba-108">Prerequisites</span></span>
<span data-ttu-id="6e8ba-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6e8ba-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6e8ba-111">Permission type</span></span>|<span data-ttu-id="6e8ba-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6e8ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e8ba-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6e8ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e8ba-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e8ba-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6e8ba-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6e8ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e8ba-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6e8ba-116">Not supported.</span></span>|
|<span data-ttu-id="6e8ba-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6e8ba-117">Application</span></span>|<span data-ttu-id="6e8ba-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6e8ba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e8ba-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e8ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e8ba-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6e8ba-120">Optional query parameters</span></span>
<span data-ttu-id="6e8ba-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6e8ba-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e8ba-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6e8ba-122">Request headers</span></span>
|<span data-ttu-id="6e8ba-123">Header</span><span class="sxs-lookup"><span data-stu-id="6e8ba-123">Header</span></span>|<span data-ttu-id="6e8ba-124">Wert</span><span class="sxs-lookup"><span data-stu-id="6e8ba-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e8ba-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6e8ba-125">Authorization</span></span>|<span data-ttu-id="6e8ba-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6e8ba-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e8ba-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6e8ba-127">Accept</span></span>|<span data-ttu-id="6e8ba-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6e8ba-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e8ba-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6e8ba-129">Request body</span></span>
<span data-ttu-id="6e8ba-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6e8ba-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e8ba-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e8ba-131">Response</span></span>
<span data-ttu-id="6e8ba-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6e8ba-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e8ba-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6e8ba-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e8ba-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e8ba-134">Request</span></span>
<span data-ttu-id="6e8ba-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6e8ba-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="6e8ba-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e8ba-136">Response</span></span>
<span data-ttu-id="6e8ba-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6e8ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
    "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```




