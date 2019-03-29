---
title: Aktualisieren von „deviceConfigurationAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d31914b287707ef62a2d3771ffecac99817ebbee
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971430"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="affc7-103">Aktualisieren von „deviceConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="affc7-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="affc7-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="affc7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="affc7-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="affc7-105">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="affc7-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="affc7-106">Prerequisites</span></span>
<span data-ttu-id="affc7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="affc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="affc7-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="affc7-109">Permission type</span></span>|<span data-ttu-id="affc7-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="affc7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="affc7-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="affc7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="affc7-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="affc7-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="affc7-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="affc7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="affc7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="affc7-114">Not supported.</span></span>|
|<span data-ttu-id="affc7-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="affc7-115">Application</span></span>|<span data-ttu-id="affc7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="affc7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="affc7-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="affc7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="affc7-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="affc7-118">Request headers</span></span>
|<span data-ttu-id="affc7-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="affc7-119">Header</span></span>|<span data-ttu-id="affc7-120">Wert</span><span class="sxs-lookup"><span data-stu-id="affc7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="affc7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="affc7-121">Authorization</span></span>|<span data-ttu-id="affc7-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="affc7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="affc7-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="affc7-123">Accept</span></span>|<span data-ttu-id="affc7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="affc7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="affc7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="affc7-125">Request body</span></span>
<span data-ttu-id="affc7-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="affc7-126">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="affc7-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="affc7-127">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="affc7-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="affc7-128">Property</span></span>|<span data-ttu-id="affc7-129">Typ</span><span class="sxs-lookup"><span data-stu-id="affc7-129">Type</span></span>|<span data-ttu-id="affc7-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="affc7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="affc7-131">id</span><span class="sxs-lookup"><span data-stu-id="affc7-131">id</span></span>|<span data-ttu-id="affc7-132">String</span><span class="sxs-lookup"><span data-stu-id="affc7-132">String</span></span>|<span data-ttu-id="affc7-133">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="affc7-133">The key of the assignment.</span></span>|
|<span data-ttu-id="affc7-134">target</span><span class="sxs-lookup"><span data-stu-id="affc7-134">target</span></span>|[<span data-ttu-id="affc7-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="affc7-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="affc7-136">Zuweisungsziel für die Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="affc7-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="affc7-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="affc7-137">Response</span></span>
<span data-ttu-id="affc7-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="affc7-138">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="affc7-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="affc7-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="affc7-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="affc7-140">Request</span></span>
<span data-ttu-id="affc7-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="affc7-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="affc7-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="affc7-142">Response</span></span>
<span data-ttu-id="affc7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="affc7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



