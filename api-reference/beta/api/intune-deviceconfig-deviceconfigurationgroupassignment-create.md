---
title: DeviceConfigurationGroupAssignment erstellen
description: Erstellen eines neuen deviceConfigurationGroupAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9dc2a7895e33c8d9ecf0b5bc0a47e202dfed0b69
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981741"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="4f2d9-103">DeviceConfigurationGroupAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="4f2d9-103">Create deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="4f2d9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4f2d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f2d9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4f2d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f2d9-106">Erstellen eines neuen [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4f2d9-106">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f2d9-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4f2d9-107">Prerequisites</span></span>
<span data-ttu-id="4f2d9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f2d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f2d9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4f2d9-110">Permission type</span></span>|<span data-ttu-id="4f2d9-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4f2d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f2d9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4f2d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f2d9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f2d9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f2d9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4f2d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f2d9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4f2d9-115">Not supported.</span></span>|
|<span data-ttu-id="4f2d9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4f2d9-116">Application</span></span>|<span data-ttu-id="4f2d9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4f2d9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f2d9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f2d9-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4f2d9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4f2d9-119">Request headers</span></span>
|<span data-ttu-id="4f2d9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4f2d9-120">Header</span></span>|<span data-ttu-id="4f2d9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4f2d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f2d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f2d9-122">Authorization</span></span>|<span data-ttu-id="4f2d9-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4f2d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f2d9-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4f2d9-124">Accept</span></span>|<span data-ttu-id="4f2d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f2d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f2d9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4f2d9-126">Request body</span></span>
<span data-ttu-id="4f2d9-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceConfigurationGroupAssignment-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="4f2d9-127">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="4f2d9-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceConfigurationGroupAssignment erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4f2d9-128">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="4f2d9-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4f2d9-129">Property</span></span>|<span data-ttu-id="4f2d9-130">Typ</span><span class="sxs-lookup"><span data-stu-id="4f2d9-130">Type</span></span>|<span data-ttu-id="4f2d9-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f2d9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f2d9-132">id</span><span class="sxs-lookup"><span data-stu-id="4f2d9-132">id</span></span>|<span data-ttu-id="4f2d9-133">String</span><span class="sxs-lookup"><span data-stu-id="4f2d9-133">String</span></span>|<span data-ttu-id="4f2d9-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4f2d9-134">Key of the entity.</span></span>|
|<span data-ttu-id="4f2d9-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="4f2d9-135">targetGroupId</span></span>|<span data-ttu-id="4f2d9-136">String</span><span class="sxs-lookup"><span data-stu-id="4f2d9-136">String</span></span>|<span data-ttu-id="4f2d9-137">Die ID der AAD-Gruppe, auf die die Gerätekonfiguration zielt.</span><span class="sxs-lookup"><span data-stu-id="4f2d9-137">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="4f2d9-138">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="4f2d9-138">excludeGroup</span></span>|<span data-ttu-id="4f2d9-139">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4f2d9-139">Boolean</span></span>|<span data-ttu-id="4f2d9-140">Gibt an, ob diese Gruppe ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="4f2d9-140">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="4f2d9-141">Standardwerte, die die Gruppe enthalten soll</span><span class="sxs-lookup"><span data-stu-id="4f2d9-141">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="4f2d9-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f2d9-142">Response</span></span>
<span data-ttu-id="4f2d9-143">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4f2d9-143">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f2d9-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4f2d9-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f2d9-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f2d9-145">Request</span></span>
<span data-ttu-id="4f2d9-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4f2d9-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4f2d9-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f2d9-147">Response</span></span>
<span data-ttu-id="4f2d9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4f2d9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




