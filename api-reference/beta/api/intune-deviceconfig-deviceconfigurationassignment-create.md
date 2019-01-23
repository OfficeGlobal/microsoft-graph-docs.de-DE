---
title: Erstellen von „deviceConfigurationAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs deviceConfigurationAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6dcac355c72e9326909091293af8759d0e8584c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400382"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="e0145-103">Erstellen von „deviceConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="e0145-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="e0145-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e0145-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e0145-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e0145-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0145-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e0145-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0145-107">Diese Methode erstellt ein neues Objekt des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e0145-107">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0145-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e0145-108">Prerequisites</span></span>
<span data-ttu-id="e0145-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e0145-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e0145-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e0145-111">Permission type</span></span>|<span data-ttu-id="e0145-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e0145-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0145-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e0145-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0145-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0145-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0145-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e0145-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0145-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0145-116">Not supported.</span></span>|
|<span data-ttu-id="e0145-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e0145-117">Application</span></span>|<span data-ttu-id="e0145-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0145-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0145-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0145-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e0145-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e0145-120">Request headers</span></span>
|<span data-ttu-id="e0145-121">Header</span><span class="sxs-lookup"><span data-stu-id="e0145-121">Header</span></span>|<span data-ttu-id="e0145-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e0145-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0145-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e0145-123">Authorization</span></span>|<span data-ttu-id="e0145-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e0145-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0145-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e0145-125">Accept</span></span>|<span data-ttu-id="e0145-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0145-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0145-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e0145-127">Request body</span></span>
<span data-ttu-id="e0145-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceConfigurationAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="e0145-128">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="e0145-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceConfigurationAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="e0145-129">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="e0145-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e0145-130">Property</span></span>|<span data-ttu-id="e0145-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e0145-131">Type</span></span>|<span data-ttu-id="e0145-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0145-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0145-133">id</span><span class="sxs-lookup"><span data-stu-id="e0145-133">id</span></span>|<span data-ttu-id="e0145-134">String</span><span class="sxs-lookup"><span data-stu-id="e0145-134">String</span></span>|<span data-ttu-id="e0145-135">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="e0145-135">The key of the assignment.</span></span>|
|<span data-ttu-id="e0145-136">target</span><span class="sxs-lookup"><span data-stu-id="e0145-136">target</span></span>|[<span data-ttu-id="e0145-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e0145-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e0145-138">Zuweisungsziel für die Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="e0145-138">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="e0145-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0145-139">Response</span></span>
<span data-ttu-id="e0145-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e0145-140">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0145-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e0145-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0145-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0145-142">Request</span></span>
<span data-ttu-id="e0145-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e0145-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e0145-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0145-144">Response</span></span>
<span data-ttu-id="e0145-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0145-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




