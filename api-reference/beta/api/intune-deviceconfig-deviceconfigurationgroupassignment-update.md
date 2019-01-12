---
title: DeviceConfigurationGroupAssignment aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DeviceConfigurationGroupAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 632ade6d8c2fdb2cfb859c3b480606547d9b0ead
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938517"
---
# <a name="update-deviceconfigurationgroupassignment"></a><span data-ttu-id="3e411-103">DeviceConfigurationGroupAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3e411-103">Update deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="3e411-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3e411-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e411-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3e411-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e411-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3e411-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e411-107">Aktualisieren Sie die Eigenschaften eines [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3e411-107">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e411-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3e411-108">Prerequisites</span></span>
<span data-ttu-id="3e411-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e411-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e411-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3e411-111">Permission type</span></span>|<span data-ttu-id="3e411-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3e411-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e411-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3e411-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e411-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e411-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e411-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3e411-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e411-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e411-116">Not supported.</span></span>|
|<span data-ttu-id="3e411-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3e411-117">Application</span></span>|<span data-ttu-id="3e411-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e411-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e411-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e411-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="3e411-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e411-120">Request headers</span></span>
|<span data-ttu-id="3e411-121">Header</span><span class="sxs-lookup"><span data-stu-id="3e411-121">Header</span></span>|<span data-ttu-id="3e411-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3e411-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e411-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e411-123">Authorization</span></span>|<span data-ttu-id="3e411-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3e411-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e411-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3e411-125">Accept</span></span>|<span data-ttu-id="3e411-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e411-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e411-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e411-127">Request body</span></span>
<span data-ttu-id="3e411-128">Geben Sie im Textkörper Anforderung für das Objekt [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="3e411-128">In the request body, supply a JSON representation for the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

<span data-ttu-id="3e411-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="3e411-129">The following table shows the properties that are required when you create the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

|<span data-ttu-id="3e411-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3e411-130">Property</span></span>|<span data-ttu-id="3e411-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3e411-131">Type</span></span>|<span data-ttu-id="3e411-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e411-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e411-133">id</span><span class="sxs-lookup"><span data-stu-id="3e411-133">id</span></span>|<span data-ttu-id="3e411-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3e411-134">String</span></span>|<span data-ttu-id="3e411-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3e411-135">Key of the entity.</span></span>|
|<span data-ttu-id="3e411-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="3e411-136">targetGroupId</span></span>|<span data-ttu-id="3e411-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3e411-137">String</span></span>|<span data-ttu-id="3e411-138">Die Id der Gruppe AAD sind wir Gerätekonfiguration zu adressieren.</span><span class="sxs-lookup"><span data-stu-id="3e411-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="3e411-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="3e411-139">excludeGroup</span></span>|<span data-ttu-id="3e411-140">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3e411-140">Boolean</span></span>|<span data-ttu-id="3e411-141">Gibt an, ob diese Gruppe ist ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="3e411-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="3e411-142">Die Standardeinstellungen, dass die Gruppe eingeschlossen werden sollen</span><span class="sxs-lookup"><span data-stu-id="3e411-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="3e411-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e411-143">Response</span></span>
<span data-ttu-id="3e411-144">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3e411-144">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e411-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e411-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e411-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e411-146">Request</span></span>
<span data-ttu-id="3e411-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3e411-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
Content-type: application/json
Content-length: 73

{
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="3e411-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e411-148">Response</span></span>
<span data-ttu-id="3e411-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e411-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





