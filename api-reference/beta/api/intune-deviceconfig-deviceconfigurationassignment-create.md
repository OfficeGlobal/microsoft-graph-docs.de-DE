---
title: Erstellen von „deviceConfigurationAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e555254f473b119b5a1e27cb2c5823e7863060fc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979173"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="ffd46-103">Erstellen von „deviceConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="ffd46-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="ffd46-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ffd46-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffd46-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ffd46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ffd46-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ffd46-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffd46-107">Diese Methode erstellt ein neues Objekt des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ffd46-107">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ffd46-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ffd46-108">Prerequisites</span></span>
<span data-ttu-id="ffd46-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffd46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffd46-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ffd46-111">Permission type</span></span>|<span data-ttu-id="ffd46-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ffd46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffd46-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ffd46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ffd46-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffd46-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ffd46-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ffd46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffd46-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ffd46-116">Not supported.</span></span>|
|<span data-ttu-id="ffd46-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ffd46-117">Application</span></span>|<span data-ttu-id="ffd46-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ffd46-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffd46-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ffd46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ffd46-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ffd46-120">Request headers</span></span>
|<span data-ttu-id="ffd46-121">Header</span><span class="sxs-lookup"><span data-stu-id="ffd46-121">Header</span></span>|<span data-ttu-id="ffd46-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ffd46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffd46-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffd46-123">Authorization</span></span>|<span data-ttu-id="ffd46-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ffd46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffd46-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ffd46-125">Accept</span></span>|<span data-ttu-id="ffd46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffd46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffd46-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ffd46-127">Request body</span></span>
<span data-ttu-id="ffd46-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceConfigurationAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="ffd46-128">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="ffd46-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceConfigurationAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="ffd46-129">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="ffd46-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ffd46-130">Property</span></span>|<span data-ttu-id="ffd46-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ffd46-131">Type</span></span>|<span data-ttu-id="ffd46-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ffd46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffd46-133">id</span><span class="sxs-lookup"><span data-stu-id="ffd46-133">id</span></span>|<span data-ttu-id="ffd46-134">String</span><span class="sxs-lookup"><span data-stu-id="ffd46-134">String</span></span>|<span data-ttu-id="ffd46-135">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="ffd46-135">The key of the assignment.</span></span>|
|<span data-ttu-id="ffd46-136">target</span><span class="sxs-lookup"><span data-stu-id="ffd46-136">target</span></span>|[<span data-ttu-id="ffd46-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ffd46-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ffd46-138">Zuweisungsziel für die Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="ffd46-138">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="ffd46-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="ffd46-139">Response</span></span>
<span data-ttu-id="ffd46-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ffd46-140">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffd46-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ffd46-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="ffd46-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ffd46-142">Request</span></span>
<span data-ttu-id="ffd46-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ffd46-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ffd46-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="ffd46-144">Response</span></span>
<span data-ttu-id="ffd46-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ffd46-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





