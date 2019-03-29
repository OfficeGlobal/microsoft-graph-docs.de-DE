---
title: Auflisten von „deviceConfigurationAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceConfigurationAssignment auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b39206581090300fdf8769ef972b3b968b10faaa
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984948"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="09efb-103">Auflisten von „deviceConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="09efb-103">List deviceConfigurationAssignments</span></span>

> <span data-ttu-id="09efb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="09efb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09efb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="09efb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09efb-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="09efb-106">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09efb-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="09efb-107">Prerequisites</span></span>
<span data-ttu-id="09efb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09efb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09efb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="09efb-110">Permission type</span></span>|<span data-ttu-id="09efb-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="09efb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09efb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="09efb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="09efb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="09efb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="09efb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="09efb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09efb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09efb-115">Not supported.</span></span>|
|<span data-ttu-id="09efb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="09efb-116">Application</span></span>|<span data-ttu-id="09efb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09efb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09efb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="09efb-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="09efb-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="09efb-119">Request headers</span></span>
|<span data-ttu-id="09efb-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="09efb-120">Header</span></span>|<span data-ttu-id="09efb-121">Wert</span><span class="sxs-lookup"><span data-stu-id="09efb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09efb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="09efb-122">Authorization</span></span>|<span data-ttu-id="09efb-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="09efb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09efb-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="09efb-124">Accept</span></span>|<span data-ttu-id="09efb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09efb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09efb-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="09efb-126">Request body</span></span>
<span data-ttu-id="09efb-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="09efb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09efb-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="09efb-128">Response</span></span>
<span data-ttu-id="09efb-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="09efb-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09efb-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="09efb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="09efb-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09efb-131">Request</span></span>
<span data-ttu-id="09efb-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="09efb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="09efb-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="09efb-133">Response</span></span>
<span data-ttu-id="09efb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="09efb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




