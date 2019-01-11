---
title: Erstellen von deviceConfigurationGroupAssignment
description: Erstellen eines neuen DeviceConfigurationGroupAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f4193470483918a2b690962ae3e190a08ac2f4c0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869531"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="49832-103">Erstellen von deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="49832-103">Create deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="49832-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="49832-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49832-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="49832-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49832-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="49832-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49832-107">Erstellen eines neuen [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="49832-107">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="49832-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="49832-108">Prerequisites</span></span>
<span data-ttu-id="49832-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49832-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49832-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="49832-111">Permission type</span></span>|<span data-ttu-id="49832-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="49832-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49832-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="49832-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49832-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49832-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49832-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="49832-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49832-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49832-116">Not supported.</span></span>|
|<span data-ttu-id="49832-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="49832-117">Application</span></span>|<span data-ttu-id="49832-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49832-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49832-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="49832-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="49832-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="49832-120">Request headers</span></span>
|<span data-ttu-id="49832-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="49832-121">Header</span></span>|<span data-ttu-id="49832-122">Wert</span><span class="sxs-lookup"><span data-stu-id="49832-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49832-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="49832-123">Authorization</span></span>|<span data-ttu-id="49832-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="49832-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49832-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="49832-125">Accept</span></span>|<span data-ttu-id="49832-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49832-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49832-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="49832-127">Request body</span></span>
<span data-ttu-id="49832-128">Geben Sie im Textkörper Anforderung für das Objekt DeviceConfigurationGroupAssignment eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="49832-128">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="49832-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DeviceConfigurationGroupAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="49832-129">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="49832-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="49832-130">Property</span></span>|<span data-ttu-id="49832-131">Typ</span><span class="sxs-lookup"><span data-stu-id="49832-131">Type</span></span>|<span data-ttu-id="49832-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49832-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49832-133">id</span><span class="sxs-lookup"><span data-stu-id="49832-133">id</span></span>|<span data-ttu-id="49832-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49832-134">String</span></span>|<span data-ttu-id="49832-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="49832-135">Key of the entity.</span></span>|
|<span data-ttu-id="49832-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="49832-136">targetGroupId</span></span>|<span data-ttu-id="49832-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49832-137">String</span></span>|<span data-ttu-id="49832-138">Die Id der Gruppe AAD sind wir Gerätekonfiguration zu adressieren.</span><span class="sxs-lookup"><span data-stu-id="49832-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="49832-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="49832-139">excludeGroup</span></span>|<span data-ttu-id="49832-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="49832-140">Boolean</span></span>|<span data-ttu-id="49832-141">Gibt an, ob diese Gruppe ist ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="49832-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="49832-142">Die Standardeinstellungen, dass die Gruppe eingeschlossen werden sollen</span><span class="sxs-lookup"><span data-stu-id="49832-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="49832-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="49832-143">Response</span></span>
<span data-ttu-id="49832-144">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="49832-144">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49832-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="49832-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="49832-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="49832-146">Request</span></span>
<span data-ttu-id="49832-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="49832-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="49832-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="49832-148">Response</span></span>
<span data-ttu-id="49832-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49832-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 195

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```





