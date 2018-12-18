---
title: DeviceConfigurationGroupAssignment aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DeviceConfigurationGroupAssignment-Objekts.
author: tfitzmac
ms.openlocfilehash: 7ea879c7d267337a247455235f069206b7b3b2a0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313881"
---
# <a name="update-deviceconfigurationgroupassignment"></a><span data-ttu-id="f24c8-103">DeviceConfigurationGroupAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f24c8-103">Update deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="f24c8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f24c8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f24c8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f24c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f24c8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f24c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f24c8-107">Aktualisieren Sie die Eigenschaften eines [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f24c8-107">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f24c8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f24c8-108">Prerequisites</span></span>
<span data-ttu-id="f24c8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f24c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f24c8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f24c8-111">Permission type</span></span>|<span data-ttu-id="f24c8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f24c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f24c8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f24c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f24c8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f24c8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f24c8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f24c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f24c8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f24c8-116">Not supported.</span></span>|
|<span data-ttu-id="f24c8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f24c8-117">Application</span></span>|<span data-ttu-id="f24c8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f24c8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f24c8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f24c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="f24c8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f24c8-120">Request headers</span></span>
|<span data-ttu-id="f24c8-121">Header</span><span class="sxs-lookup"><span data-stu-id="f24c8-121">Header</span></span>|<span data-ttu-id="f24c8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f24c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f24c8-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f24c8-123">Authorization</span></span>|<span data-ttu-id="f24c8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f24c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f24c8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f24c8-125">Accept</span></span>|<span data-ttu-id="f24c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f24c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f24c8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f24c8-127">Request body</span></span>
<span data-ttu-id="f24c8-128">Geben Sie im Textkörper Anforderung für das Objekt [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f24c8-128">In the request body, supply a JSON representation for the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

<span data-ttu-id="f24c8-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="f24c8-129">The following table shows the properties that are required when you create the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

|<span data-ttu-id="f24c8-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f24c8-130">Property</span></span>|<span data-ttu-id="f24c8-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f24c8-131">Type</span></span>|<span data-ttu-id="f24c8-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f24c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f24c8-133">id</span><span class="sxs-lookup"><span data-stu-id="f24c8-133">id</span></span>|<span data-ttu-id="f24c8-134">String</span><span class="sxs-lookup"><span data-stu-id="f24c8-134">String</span></span>|<span data-ttu-id="f24c8-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f24c8-135">Key of the entity.</span></span>|
|<span data-ttu-id="f24c8-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="f24c8-136">targetGroupId</span></span>|<span data-ttu-id="f24c8-137">String</span><span class="sxs-lookup"><span data-stu-id="f24c8-137">String</span></span>|<span data-ttu-id="f24c8-138">Die Id der Gruppe AAD sind wir Gerätekonfiguration zu adressieren.</span><span class="sxs-lookup"><span data-stu-id="f24c8-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="f24c8-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="f24c8-139">excludeGroup</span></span>|<span data-ttu-id="f24c8-140">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f24c8-140">Boolean</span></span>|<span data-ttu-id="f24c8-141">Gibt an, ob diese Gruppe ist ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="f24c8-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="f24c8-142">Die Standardeinstellungen, dass die Gruppe eingeschlossen werden sollen</span><span class="sxs-lookup"><span data-stu-id="f24c8-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="f24c8-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="f24c8-143">Response</span></span>
<span data-ttu-id="f24c8-144">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f24c8-144">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f24c8-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f24c8-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="f24c8-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f24c8-146">Request</span></span>
<span data-ttu-id="f24c8-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f24c8-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
Content-type: application/json
Content-length: 73

{
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="f24c8-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="f24c8-148">Response</span></span>
<span data-ttu-id="f24c8-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f24c8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 195

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```





