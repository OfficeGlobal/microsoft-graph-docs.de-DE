---
title: Aktualisieren von „deviceConfigurationAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0a09b2ed63d381fd305859919017295987faf78f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155930"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="2b5a5-103">Aktualisieren von „deviceConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="2b5a5-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="2b5a5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2b5a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b5a5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2b5a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b5a5-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2b5a5-106">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b5a5-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2b5a5-107">Prerequisites</span></span>
<span data-ttu-id="2b5a5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2b5a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2b5a5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2b5a5-110">Permission type</span></span>|<span data-ttu-id="2b5a5-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2b5a5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b5a5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2b5a5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2b5a5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b5a5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2b5a5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2b5a5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b5a5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b5a5-115">Not supported.</span></span>|
|<span data-ttu-id="2b5a5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2b5a5-116">Application</span></span>|<span data-ttu-id="2b5a5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b5a5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b5a5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b5a5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2b5a5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2b5a5-119">Request headers</span></span>
|<span data-ttu-id="2b5a5-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2b5a5-120">Header</span></span>|<span data-ttu-id="2b5a5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2b5a5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b5a5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b5a5-122">Authorization</span></span>|<span data-ttu-id="2b5a5-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2b5a5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b5a5-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2b5a5-124">Accept</span></span>|<span data-ttu-id="2b5a5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2b5a5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b5a5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2b5a5-126">Request body</span></span>
<span data-ttu-id="2b5a5-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="2b5a5-127">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="2b5a5-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2b5a5-128">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="2b5a5-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2b5a5-129">Property</span></span>|<span data-ttu-id="2b5a5-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2b5a5-130">Type</span></span>|<span data-ttu-id="2b5a5-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b5a5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b5a5-132">id</span><span class="sxs-lookup"><span data-stu-id="2b5a5-132">id</span></span>|<span data-ttu-id="2b5a5-133">String</span><span class="sxs-lookup"><span data-stu-id="2b5a5-133">String</span></span>|<span data-ttu-id="2b5a5-134">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="2b5a5-134">The key of the assignment.</span></span>|
|<span data-ttu-id="2b5a5-135">target</span><span class="sxs-lookup"><span data-stu-id="2b5a5-135">target</span></span>|[<span data-ttu-id="2b5a5-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2b5a5-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2b5a5-137">Zuweisungsziel für die Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="2b5a5-137">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="2b5a5-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b5a5-138">Response</span></span>
<span data-ttu-id="2b5a5-139">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2b5a5-139">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b5a5-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2b5a5-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b5a5-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b5a5-141">Request</span></span>
<span data-ttu-id="2b5a5-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2b5a5-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="2b5a5-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b5a5-143">Response</span></span>
<span data-ttu-id="2b5a5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b5a5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




