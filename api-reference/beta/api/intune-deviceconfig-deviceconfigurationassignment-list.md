---
title: Auflisten von „deviceConfigurationAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceConfigurationAssignment auf.
author: tfitzmac
ms.openlocfilehash: 605eda7354fc6af240e076427989eec05877e455
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319138"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="cdbac-103">Auflisten von „deviceConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="cdbac-103">List deviceConfigurationAssignments</span></span>

> <span data-ttu-id="cdbac-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cdbac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cdbac-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cdbac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cdbac-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cdbac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cdbac-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="cdbac-107">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cdbac-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cdbac-108">Prerequisites</span></span>
<span data-ttu-id="cdbac-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdbac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdbac-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cdbac-111">Permission type</span></span>|<span data-ttu-id="cdbac-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cdbac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdbac-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cdbac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cdbac-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdbac-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cdbac-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cdbac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdbac-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cdbac-116">Not supported.</span></span>|
|<span data-ttu-id="cdbac-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cdbac-117">Application</span></span>|<span data-ttu-id="cdbac-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cdbac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdbac-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cdbac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="cdbac-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cdbac-120">Request headers</span></span>
|<span data-ttu-id="cdbac-121">Header</span><span class="sxs-lookup"><span data-stu-id="cdbac-121">Header</span></span>|<span data-ttu-id="cdbac-122">Wert</span><span class="sxs-lookup"><span data-stu-id="cdbac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdbac-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cdbac-123">Authorization</span></span>|<span data-ttu-id="cdbac-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cdbac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdbac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cdbac-125">Accept</span></span>|<span data-ttu-id="cdbac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cdbac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdbac-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cdbac-127">Request body</span></span>
<span data-ttu-id="cdbac-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cdbac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdbac-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="cdbac-129">Response</span></span>
<span data-ttu-id="cdbac-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cdbac-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdbac-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cdbac-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="cdbac-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cdbac-132">Request</span></span>
<span data-ttu-id="cdbac-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cdbac-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="cdbac-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="cdbac-134">Response</span></span>
<span data-ttu-id="cdbac-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cdbac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





