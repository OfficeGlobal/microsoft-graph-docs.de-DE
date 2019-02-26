---
title: Erstellen von „deviceConfigurationAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4fc75ded1de59ee691b6b2888f4ecda6ad5c618e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261922"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="af47d-103">Erstellen von „deviceConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="af47d-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="af47d-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="af47d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af47d-105">Diese Methode erstellt ein neues Objekt des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="af47d-105">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af47d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="af47d-106">Prerequisites</span></span>
<span data-ttu-id="af47d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="af47d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="af47d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="af47d-109">Permission type</span></span>|<span data-ttu-id="af47d-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="af47d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af47d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="af47d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="af47d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af47d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af47d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="af47d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af47d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af47d-114">Not supported.</span></span>|
|<span data-ttu-id="af47d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="af47d-115">Application</span></span>|<span data-ttu-id="af47d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af47d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af47d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="af47d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="af47d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="af47d-118">Request headers</span></span>
|<span data-ttu-id="af47d-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="af47d-119">Header</span></span>|<span data-ttu-id="af47d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="af47d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af47d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="af47d-121">Authorization</span></span>|<span data-ttu-id="af47d-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="af47d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af47d-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="af47d-123">Accept</span></span>|<span data-ttu-id="af47d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="af47d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af47d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="af47d-125">Request body</span></span>
<span data-ttu-id="af47d-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceConfigurationAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="af47d-126">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="af47d-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceConfigurationAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="af47d-127">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="af47d-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="af47d-128">Property</span></span>|<span data-ttu-id="af47d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="af47d-129">Type</span></span>|<span data-ttu-id="af47d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af47d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af47d-131">id</span><span class="sxs-lookup"><span data-stu-id="af47d-131">id</span></span>|<span data-ttu-id="af47d-132">String</span><span class="sxs-lookup"><span data-stu-id="af47d-132">String</span></span>|<span data-ttu-id="af47d-133">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="af47d-133">The key of the assignment.</span></span>|
|<span data-ttu-id="af47d-134">target</span><span class="sxs-lookup"><span data-stu-id="af47d-134">target</span></span>|[<span data-ttu-id="af47d-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="af47d-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="af47d-136">Zuweisungsziel für die Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="af47d-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="af47d-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="af47d-137">Response</span></span>
<span data-ttu-id="af47d-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="af47d-138">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af47d-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="af47d-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="af47d-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="af47d-140">Request</span></span>
<span data-ttu-id="af47d-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="af47d-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="af47d-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="af47d-142">Response</span></span>
<span data-ttu-id="af47d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="af47d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



