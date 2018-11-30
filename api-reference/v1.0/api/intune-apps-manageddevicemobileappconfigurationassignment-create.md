---
title: Erstellen von „managedDeviceMobileAppConfigurationAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs managedDeviceMobileAppConfigurationAssignment.
ms.openlocfilehash: 4b479f7c0f93e41aa8691749925203652d2dcc9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017142"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="89b87-103">Erstellen von „managedDeviceMobileAppConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="89b87-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="89b87-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="89b87-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89b87-105">Diese Methode erstellt ein neues Objekt des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="89b87-105">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89b87-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="89b87-106">Prerequisites</span></span>
<span data-ttu-id="89b87-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89b87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89b87-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="89b87-109">Permission type</span></span>|<span data-ttu-id="89b87-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="89b87-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89b87-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="89b87-111">Delegated (work or school account)</span></span>|<span data-ttu-id="89b87-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89b87-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="89b87-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="89b87-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89b87-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="89b87-114">Not supported.</span></span>|
|<span data-ttu-id="89b87-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="89b87-115">Application</span></span>|<span data-ttu-id="89b87-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="89b87-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89b87-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="89b87-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="89b87-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="89b87-118">Request headers</span></span>
|<span data-ttu-id="89b87-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="89b87-119">Header</span></span>|<span data-ttu-id="89b87-120">Wert</span><span class="sxs-lookup"><span data-stu-id="89b87-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89b87-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="89b87-121">Authorization</span></span>|<span data-ttu-id="89b87-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="89b87-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89b87-123">Accept</span><span class="sxs-lookup"><span data-stu-id="89b87-123">Accept</span></span>|<span data-ttu-id="89b87-124">application/json</span><span class="sxs-lookup"><span data-stu-id="89b87-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89b87-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="89b87-125">Request body</span></span>
<span data-ttu-id="89b87-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „managedDeviceMobileAppConfigurationAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="89b87-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="89b87-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „managedDeviceMobileAppConfigurationAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="89b87-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="89b87-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="89b87-128">Property</span></span>|<span data-ttu-id="89b87-129">Typ</span><span class="sxs-lookup"><span data-stu-id="89b87-129">Type</span></span>|<span data-ttu-id="89b87-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89b87-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89b87-131">id</span><span class="sxs-lookup"><span data-stu-id="89b87-131">id</span></span>|<span data-ttu-id="89b87-132">String</span><span class="sxs-lookup"><span data-stu-id="89b87-132">String</span></span>|<span data-ttu-id="89b87-133">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="89b87-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="89b87-134">target</span><span class="sxs-lookup"><span data-stu-id="89b87-134">target</span></span>|[<span data-ttu-id="89b87-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="89b87-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="89b87-136">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="89b87-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="89b87-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="89b87-137">Response</span></span>
<span data-ttu-id="89b87-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="89b87-138">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89b87-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="89b87-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="89b87-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="89b87-140">Request</span></span>
<span data-ttu-id="89b87-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="89b87-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="89b87-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="89b87-142">Response</span></span>
<span data-ttu-id="89b87-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="89b87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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


