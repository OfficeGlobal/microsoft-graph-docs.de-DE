---
title: Aktualisieren von „managedDeviceMobileAppConfigurationAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceMobileAppConfigurationAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f27d1e7272e5d90dc59194b2fbc0cfd1e9e72eb0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420227"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="1c408-103">Aktualisieren von „managedDeviceMobileAppConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="1c408-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="1c408-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1c408-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1c408-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1c408-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c408-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1c408-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c408-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1c408-107">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c408-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1c408-108">Prerequisites</span></span>
<span data-ttu-id="1c408-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1c408-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1c408-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1c408-111">Permission type</span></span>|<span data-ttu-id="1c408-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1c408-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c408-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1c408-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c408-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c408-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1c408-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1c408-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c408-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c408-116">Not supported.</span></span>|
|<span data-ttu-id="1c408-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1c408-117">Application</span></span>|<span data-ttu-id="1c408-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c408-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c408-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c408-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1c408-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1c408-120">Request headers</span></span>
|<span data-ttu-id="1c408-121">Header</span><span class="sxs-lookup"><span data-stu-id="1c408-121">Header</span></span>|<span data-ttu-id="1c408-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1c408-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c408-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1c408-123">Authorization</span></span>|<span data-ttu-id="1c408-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1c408-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c408-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1c408-125">Accept</span></span>|<span data-ttu-id="1c408-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c408-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c408-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1c408-127">Request body</span></span>
<span data-ttu-id="1c408-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="1c408-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="1c408-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="1c408-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="1c408-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1c408-130">Property</span></span>|<span data-ttu-id="1c408-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1c408-131">Type</span></span>|<span data-ttu-id="1c408-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c408-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c408-133">id</span><span class="sxs-lookup"><span data-stu-id="1c408-133">id</span></span>|<span data-ttu-id="1c408-134">String</span><span class="sxs-lookup"><span data-stu-id="1c408-134">String</span></span>|<span data-ttu-id="1c408-135">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="1c408-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="1c408-136">target</span><span class="sxs-lookup"><span data-stu-id="1c408-136">target</span></span>|[<span data-ttu-id="1c408-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1c408-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1c408-138">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="1c408-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="1c408-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c408-139">Response</span></span>
<span data-ttu-id="1c408-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1c408-140">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c408-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1c408-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c408-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c408-142">Request</span></span>
<span data-ttu-id="1c408-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1c408-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="1c408-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c408-144">Response</span></span>
<span data-ttu-id="1c408-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c408-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




