---
title: Erstellen von deviceConfigurationGroupAssignment
description: Erstellen eines neuen DeviceConfigurationGroupAssignment-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2a74acc7b2be82506195d5d3646e6932533a62ee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413227"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="7c49e-103">Erstellen von deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7c49e-103">Create deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="7c49e-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="7c49e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7c49e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7c49e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c49e-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7c49e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c49e-107">Erstellen eines neuen [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7c49e-107">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c49e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7c49e-108">Prerequisites</span></span>
<span data-ttu-id="7c49e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c49e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7c49e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c49e-111">Permission type</span></span>|<span data-ttu-id="7c49e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c49e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c49e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c49e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c49e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c49e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c49e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c49e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c49e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c49e-116">Not supported.</span></span>|
|<span data-ttu-id="7c49e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c49e-117">Application</span></span>|<span data-ttu-id="7c49e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c49e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c49e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c49e-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="7c49e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c49e-120">Request headers</span></span>
|<span data-ttu-id="7c49e-121">Header</span><span class="sxs-lookup"><span data-stu-id="7c49e-121">Header</span></span>|<span data-ttu-id="7c49e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7c49e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c49e-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7c49e-123">Authorization</span></span>|<span data-ttu-id="7c49e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7c49e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c49e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7c49e-125">Accept</span></span>|<span data-ttu-id="7c49e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c49e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c49e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7c49e-127">Request body</span></span>
<span data-ttu-id="7c49e-128">Geben Sie im Textkörper Anforderung für das Objekt DeviceConfigurationGroupAssignment eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="7c49e-128">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="7c49e-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DeviceConfigurationGroupAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="7c49e-129">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="7c49e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7c49e-130">Property</span></span>|<span data-ttu-id="7c49e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7c49e-131">Type</span></span>|<span data-ttu-id="7c49e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c49e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c49e-133">id</span><span class="sxs-lookup"><span data-stu-id="7c49e-133">id</span></span>|<span data-ttu-id="7c49e-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7c49e-134">String</span></span>|<span data-ttu-id="7c49e-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7c49e-135">Key of the entity.</span></span>|
|<span data-ttu-id="7c49e-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="7c49e-136">targetGroupId</span></span>|<span data-ttu-id="7c49e-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7c49e-137">String</span></span>|<span data-ttu-id="7c49e-138">Die Id der Gruppe AAD sind wir Gerätekonfiguration zu adressieren.</span><span class="sxs-lookup"><span data-stu-id="7c49e-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="7c49e-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="7c49e-139">excludeGroup</span></span>|<span data-ttu-id="7c49e-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c49e-140">Boolean</span></span>|<span data-ttu-id="7c49e-141">Gibt an, ob diese Gruppe ist ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="7c49e-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="7c49e-142">Die Standardeinstellungen, dass die Gruppe eingeschlossen werden sollen</span><span class="sxs-lookup"><span data-stu-id="7c49e-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="7c49e-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c49e-143">Response</span></span>
<span data-ttu-id="7c49e-144">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7c49e-144">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c49e-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c49e-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c49e-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c49e-146">Request</span></span>
<span data-ttu-id="7c49e-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c49e-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c49e-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c49e-148">Response</span></span>
<span data-ttu-id="7c49e-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7c49e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




