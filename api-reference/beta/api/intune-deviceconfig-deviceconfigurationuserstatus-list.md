---
title: Auflisten von „deviceConfigurationUserStatus“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceConfigurationUserStatus auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c44f984aab21a2155ce2f93fd25f82752f8aa7c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943144"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="43aaf-103">Auflisten von „deviceConfigurationUserStatus“</span><span class="sxs-lookup"><span data-stu-id="43aaf-103">List deviceConfigurationUserStatuses</span></span>

> <span data-ttu-id="43aaf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="43aaf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43aaf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="43aaf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43aaf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="43aaf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43aaf-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) auf.</span><span class="sxs-lookup"><span data-stu-id="43aaf-107">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43aaf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="43aaf-108">Prerequisites</span></span>
<span data-ttu-id="43aaf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43aaf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43aaf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="43aaf-111">Permission type</span></span>|<span data-ttu-id="43aaf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="43aaf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43aaf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="43aaf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43aaf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="43aaf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="43aaf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="43aaf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43aaf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43aaf-116">Not supported.</span></span>|
|<span data-ttu-id="43aaf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="43aaf-117">Application</span></span>|<span data-ttu-id="43aaf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43aaf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43aaf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="43aaf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="43aaf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="43aaf-120">Request headers</span></span>
|<span data-ttu-id="43aaf-121">Header</span><span class="sxs-lookup"><span data-stu-id="43aaf-121">Header</span></span>|<span data-ttu-id="43aaf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="43aaf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43aaf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43aaf-123">Authorization</span></span>|<span data-ttu-id="43aaf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="43aaf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43aaf-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="43aaf-125">Accept</span></span>|<span data-ttu-id="43aaf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43aaf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43aaf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="43aaf-127">Request body</span></span>
<span data-ttu-id="43aaf-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="43aaf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43aaf-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="43aaf-129">Response</span></span>
<span data-ttu-id="43aaf-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="43aaf-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43aaf-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="43aaf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="43aaf-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="43aaf-132">Request</span></span>
<span data-ttu-id="43aaf-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="43aaf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="43aaf-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="43aaf-134">Response</span></span>
<span data-ttu-id="43aaf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43aaf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
      "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





