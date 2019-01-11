---
title: Aktualisieren von „managedDeviceMobileAppConfigurationAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 58d28cb3e80f127f164e65861a15c230ef2d45fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864232"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="838a4-103">Aktualisieren von „managedDeviceMobileAppConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="838a4-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="838a4-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="838a4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="838a4-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="838a4-105">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="838a4-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="838a4-106">Prerequisites</span></span>
<span data-ttu-id="838a4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="838a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="838a4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="838a4-109">Permission type</span></span>|<span data-ttu-id="838a4-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="838a4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="838a4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="838a4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="838a4-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="838a4-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="838a4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="838a4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="838a4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="838a4-114">Not supported.</span></span>|
|<span data-ttu-id="838a4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="838a4-115">Application</span></span>|<span data-ttu-id="838a4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="838a4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="838a4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="838a4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="838a4-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="838a4-118">Request headers</span></span>
|<span data-ttu-id="838a4-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="838a4-119">Header</span></span>|<span data-ttu-id="838a4-120">Wert</span><span class="sxs-lookup"><span data-stu-id="838a4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="838a4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="838a4-121">Authorization</span></span>|<span data-ttu-id="838a4-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="838a4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="838a4-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="838a4-123">Accept</span></span>|<span data-ttu-id="838a4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="838a4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="838a4-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="838a4-125">Request body</span></span>
<span data-ttu-id="838a4-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="838a4-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="838a4-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="838a4-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="838a4-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="838a4-128">Property</span></span>|<span data-ttu-id="838a4-129">Typ</span><span class="sxs-lookup"><span data-stu-id="838a4-129">Type</span></span>|<span data-ttu-id="838a4-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="838a4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="838a4-131">id</span><span class="sxs-lookup"><span data-stu-id="838a4-131">id</span></span>|<span data-ttu-id="838a4-132">String</span><span class="sxs-lookup"><span data-stu-id="838a4-132">String</span></span>|<span data-ttu-id="838a4-133">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="838a4-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="838a4-134">target</span><span class="sxs-lookup"><span data-stu-id="838a4-134">target</span></span>|[<span data-ttu-id="838a4-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="838a4-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="838a4-136">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="838a4-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="838a4-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="838a4-137">Response</span></span>
<span data-ttu-id="838a4-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="838a4-138">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="838a4-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="838a4-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="838a4-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="838a4-140">Request</span></span>
<span data-ttu-id="838a4-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="838a4-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="838a4-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="838a4-142">Response</span></span>
<span data-ttu-id="838a4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="838a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



