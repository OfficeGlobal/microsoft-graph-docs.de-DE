---
title: Aktualisieren von „deviceConfigurationAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38818cedc150f380cc803fd52194dadca63e35a4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978473"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="eaa95-103">Aktualisieren von „deviceConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="eaa95-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="eaa95-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="eaa95-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eaa95-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eaa95-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eaa95-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eaa95-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eaa95-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="eaa95-107">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eaa95-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eaa95-108">Prerequisites</span></span>
<span data-ttu-id="eaa95-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaa95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaa95-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eaa95-111">Permission type</span></span>|<span data-ttu-id="eaa95-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eaa95-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eaa95-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eaa95-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eaa95-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaa95-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eaa95-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eaa95-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eaa95-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eaa95-116">Not supported.</span></span>|
|<span data-ttu-id="eaa95-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eaa95-117">Application</span></span>|<span data-ttu-id="eaa95-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eaa95-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaa95-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eaa95-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="eaa95-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eaa95-120">Request headers</span></span>
|<span data-ttu-id="eaa95-121">Header</span><span class="sxs-lookup"><span data-stu-id="eaa95-121">Header</span></span>|<span data-ttu-id="eaa95-122">Wert</span><span class="sxs-lookup"><span data-stu-id="eaa95-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eaa95-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eaa95-123">Authorization</span></span>|<span data-ttu-id="eaa95-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eaa95-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eaa95-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eaa95-125">Accept</span></span>|<span data-ttu-id="eaa95-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eaa95-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaa95-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eaa95-127">Request body</span></span>
<span data-ttu-id="eaa95-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="eaa95-128">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="eaa95-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="eaa95-129">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="eaa95-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eaa95-130">Property</span></span>|<span data-ttu-id="eaa95-131">Typ</span><span class="sxs-lookup"><span data-stu-id="eaa95-131">Type</span></span>|<span data-ttu-id="eaa95-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eaa95-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaa95-133">id</span><span class="sxs-lookup"><span data-stu-id="eaa95-133">id</span></span>|<span data-ttu-id="eaa95-134">String</span><span class="sxs-lookup"><span data-stu-id="eaa95-134">String</span></span>|<span data-ttu-id="eaa95-135">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="eaa95-135">The key of the assignment.</span></span>|
|<span data-ttu-id="eaa95-136">target</span><span class="sxs-lookup"><span data-stu-id="eaa95-136">target</span></span>|[<span data-ttu-id="eaa95-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="eaa95-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="eaa95-138">Zuweisungsziel für die Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="eaa95-138">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="eaa95-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="eaa95-139">Response</span></span>
<span data-ttu-id="eaa95-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="eaa95-140">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaa95-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eaa95-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="eaa95-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eaa95-142">Request</span></span>
<span data-ttu-id="eaa95-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eaa95-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="eaa95-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="eaa95-144">Response</span></span>
<span data-ttu-id="eaa95-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eaa95-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





