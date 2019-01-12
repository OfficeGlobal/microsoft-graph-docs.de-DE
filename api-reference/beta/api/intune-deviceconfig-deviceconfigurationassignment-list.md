---
title: Auflisten von „deviceConfigurationAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceConfigurationAssignment auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9506e692a46cd1b09916621da3f4190869a40a13
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964921"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="85d32-103">Auflisten von „deviceConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="85d32-103">List deviceConfigurationAssignments</span></span>

> <span data-ttu-id="85d32-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="85d32-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85d32-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="85d32-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85d32-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="85d32-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85d32-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="85d32-107">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85d32-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="85d32-108">Prerequisites</span></span>
<span data-ttu-id="85d32-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85d32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85d32-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="85d32-111">Permission type</span></span>|<span data-ttu-id="85d32-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="85d32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85d32-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="85d32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85d32-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="85d32-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="85d32-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="85d32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85d32-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85d32-116">Not supported.</span></span>|
|<span data-ttu-id="85d32-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="85d32-117">Application</span></span>|<span data-ttu-id="85d32-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85d32-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85d32-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="85d32-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="85d32-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="85d32-120">Request headers</span></span>
|<span data-ttu-id="85d32-121">Header</span><span class="sxs-lookup"><span data-stu-id="85d32-121">Header</span></span>|<span data-ttu-id="85d32-122">Wert</span><span class="sxs-lookup"><span data-stu-id="85d32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85d32-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85d32-123">Authorization</span></span>|<span data-ttu-id="85d32-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="85d32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85d32-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="85d32-125">Accept</span></span>|<span data-ttu-id="85d32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85d32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85d32-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="85d32-127">Request body</span></span>
<span data-ttu-id="85d32-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="85d32-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85d32-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="85d32-129">Response</span></span>
<span data-ttu-id="85d32-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="85d32-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85d32-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="85d32-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="85d32-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="85d32-132">Request</span></span>
<span data-ttu-id="85d32-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="85d32-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="85d32-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="85d32-134">Response</span></span>
<span data-ttu-id="85d32-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85d32-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





