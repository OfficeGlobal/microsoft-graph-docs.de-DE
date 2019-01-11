---
title: deviceConfigurationUserStatus abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceConfigurationUserStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b4bfe02f9d3ba04fd52328402c677189498233f1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852857"
---
# <a name="get-deviceconfigurationuserstatus"></a><span data-ttu-id="ee2b1-103">deviceConfigurationUserStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="ee2b1-103">Get deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="ee2b1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ee2b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee2b1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ee2b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee2b1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ee2b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee2b1-107">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ee2b1-107">Read properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ee2b1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ee2b1-108">Prerequisites</span></span>
<span data-ttu-id="ee2b1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee2b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee2b1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ee2b1-111">Permission type</span></span>|<span data-ttu-id="ee2b1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ee2b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee2b1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ee2b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee2b1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee2b1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ee2b1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ee2b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee2b1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ee2b1-116">Not supported.</span></span>|
|<span data-ttu-id="ee2b1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ee2b1-117">Application</span></span>|<span data-ttu-id="ee2b1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ee2b1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee2b1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee2b1-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="ee2b1-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ee2b1-120">Optional query parameters</span></span>
<span data-ttu-id="ee2b1-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ee2b1-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ee2b1-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ee2b1-122">Request headers</span></span>
|<span data-ttu-id="ee2b1-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ee2b1-123">Header</span></span>|<span data-ttu-id="ee2b1-124">Wert</span><span class="sxs-lookup"><span data-stu-id="ee2b1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee2b1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee2b1-125">Authorization</span></span>|<span data-ttu-id="ee2b1-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ee2b1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee2b1-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ee2b1-127">Accept</span></span>|<span data-ttu-id="ee2b1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ee2b1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee2b1-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ee2b1-129">Request body</span></span>
<span data-ttu-id="ee2b1-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ee2b1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee2b1-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee2b1-131">Response</span></span>
<span data-ttu-id="ee2b1-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ee2b1-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee2b1-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ee2b1-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ee2b1-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee2b1-134">Request</span></span>
<span data-ttu-id="ee2b1-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ee2b1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="ee2b1-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee2b1-136">Response</span></span>
<span data-ttu-id="ee2b1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ee2b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





