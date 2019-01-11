---
title: Aktualisieren von „deviceConfigurationAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c39a50f5cfba40cf4b41f654e75cd84e69b7f8cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894355"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="3e4c4-103">Aktualisieren von „deviceConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="3e4c4-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="3e4c4-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3e4c4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e4c4-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3e4c4-105">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e4c4-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3e4c4-106">Prerequisites</span></span>
<span data-ttu-id="3e4c4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e4c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e4c4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3e4c4-109">Permission type</span></span>|<span data-ttu-id="3e4c4-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3e4c4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e4c4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3e4c4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3e4c4-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e4c4-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e4c4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3e4c4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e4c4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e4c4-114">Not supported.</span></span>|
|<span data-ttu-id="3e4c4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3e4c4-115">Application</span></span>|<span data-ttu-id="3e4c4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e4c4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e4c4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e4c4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3e4c4-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e4c4-118">Request headers</span></span>
|<span data-ttu-id="3e4c4-119">Header</span><span class="sxs-lookup"><span data-stu-id="3e4c4-119">Header</span></span>|<span data-ttu-id="3e4c4-120">Wert</span><span class="sxs-lookup"><span data-stu-id="3e4c4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e4c4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e4c4-121">Authorization</span></span>|<span data-ttu-id="3e4c4-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3e4c4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e4c4-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3e4c4-123">Accept</span></span>|<span data-ttu-id="3e4c4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3e4c4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e4c4-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e4c4-125">Request body</span></span>
<span data-ttu-id="3e4c4-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="3e4c4-126">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="3e4c4-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="3e4c4-127">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="3e4c4-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3e4c4-128">Property</span></span>|<span data-ttu-id="3e4c4-129">Typ</span><span class="sxs-lookup"><span data-stu-id="3e4c4-129">Type</span></span>|<span data-ttu-id="3e4c4-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e4c4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e4c4-131">id</span><span class="sxs-lookup"><span data-stu-id="3e4c4-131">id</span></span>|<span data-ttu-id="3e4c4-132">String</span><span class="sxs-lookup"><span data-stu-id="3e4c4-132">String</span></span>|<span data-ttu-id="3e4c4-133">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="3e4c4-133">The key of the assignment.</span></span>|
|<span data-ttu-id="3e4c4-134">target</span><span class="sxs-lookup"><span data-stu-id="3e4c4-134">target</span></span>|[<span data-ttu-id="3e4c4-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3e4c4-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3e4c4-136">Zuweisungsziel für die Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="3e4c4-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="3e4c4-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e4c4-137">Response</span></span>
<span data-ttu-id="3e4c4-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3e4c4-138">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e4c4-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e4c4-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e4c4-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e4c4-140">Request</span></span>
<span data-ttu-id="3e4c4-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3e4c4-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="3e4c4-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e4c4-142">Response</span></span>
<span data-ttu-id="3e4c4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e4c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



