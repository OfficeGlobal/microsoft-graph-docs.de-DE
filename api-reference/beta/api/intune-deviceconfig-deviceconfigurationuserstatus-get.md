---
title: deviceConfigurationUserStatus abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceConfigurationUserStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e7873a32db68136c33c040ae141647b75f053f8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174382"
---
# <a name="get-deviceconfigurationuserstatus"></a><span data-ttu-id="7a1e7-103">deviceConfigurationUserStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="7a1e7-103">Get deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="7a1e7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7a1e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a1e7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7a1e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a1e7-106">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7a1e7-106">Read properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a1e7-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7a1e7-107">Prerequisites</span></span>
<span data-ttu-id="7a1e7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7a1e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7a1e7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a1e7-110">Permission type</span></span>|<span data-ttu-id="7a1e7-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a1e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a1e7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a1e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7a1e7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a1e7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7a1e7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a1e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a1e7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a1e7-115">Not supported.</span></span>|
|<span data-ttu-id="7a1e7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a1e7-116">Application</span></span>|<span data-ttu-id="7a1e7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a1e7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a1e7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a1e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a1e7-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7a1e7-119">Optional query parameters</span></span>
<span data-ttu-id="7a1e7-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7a1e7-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a1e7-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a1e7-121">Request headers</span></span>
|<span data-ttu-id="7a1e7-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7a1e7-122">Header</span></span>|<span data-ttu-id="7a1e7-123">Wert</span><span class="sxs-lookup"><span data-stu-id="7a1e7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a1e7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a1e7-124">Authorization</span></span>|<span data-ttu-id="7a1e7-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7a1e7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a1e7-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7a1e7-126">Accept</span></span>|<span data-ttu-id="7a1e7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7a1e7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a1e7-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a1e7-128">Request body</span></span>
<span data-ttu-id="7a1e7-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7a1e7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a1e7-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a1e7-130">Response</span></span>
<span data-ttu-id="7a1e7-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a1e7-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a1e7-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a1e7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a1e7-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a1e7-133">Request</span></span>
<span data-ttu-id="7a1e7-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7a1e7-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="7a1e7-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a1e7-135">Response</span></span>
<span data-ttu-id="7a1e7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a1e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
    "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
    "userDisplayName": "User Display Name value",
    "devicesCount": 12,
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```




