---
title: EmbeddedSIMActivationCodePoolAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines embeddedSIMActivationCodePoolAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4fa2030d6b2b8fb260c28d94caff031ec2db0ae1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164449"
---
# <a name="update-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="13bfe-103">EmbeddedSIMActivationCodePoolAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="13bfe-103">Update embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="13bfe-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13bfe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13bfe-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="13bfe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13bfe-106">Aktualisieren der Eigenschaften eines [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="13bfe-106">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13bfe-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="13bfe-107">Prerequisites</span></span>
<span data-ttu-id="13bfe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="13bfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="13bfe-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="13bfe-110">Permission type</span></span>|<span data-ttu-id="13bfe-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="13bfe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13bfe-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="13bfe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13bfe-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13bfe-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13bfe-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="13bfe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13bfe-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13bfe-115">Not supported.</span></span>|
|<span data-ttu-id="13bfe-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="13bfe-116">Application</span></span>|<span data-ttu-id="13bfe-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13bfe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13bfe-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13bfe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="13bfe-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="13bfe-119">Request headers</span></span>
|<span data-ttu-id="13bfe-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="13bfe-120">Header</span></span>|<span data-ttu-id="13bfe-121">Wert</span><span class="sxs-lookup"><span data-stu-id="13bfe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13bfe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="13bfe-122">Authorization</span></span>|<span data-ttu-id="13bfe-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="13bfe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13bfe-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="13bfe-124">Accept</span></span>|<span data-ttu-id="13bfe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13bfe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13bfe-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="13bfe-126">Request body</span></span>
<span data-ttu-id="13bfe-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="13bfe-127">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

<span data-ttu-id="13bfe-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="13bfe-128">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

|<span data-ttu-id="13bfe-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13bfe-129">Property</span></span>|<span data-ttu-id="13bfe-130">Typ</span><span class="sxs-lookup"><span data-stu-id="13bfe-130">Type</span></span>|<span data-ttu-id="13bfe-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13bfe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13bfe-132">id</span><span class="sxs-lookup"><span data-stu-id="13bfe-132">id</span></span>|<span data-ttu-id="13bfe-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13bfe-133">String</span></span>|<span data-ttu-id="13bfe-134">Eindeutige ID für den eingebetteten SIM-Aktivierungscode-Pool-Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="13bfe-134">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="13bfe-135">Vom System generierter Wert, der bei der Erstellung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="13bfe-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="13bfe-136">target</span><span class="sxs-lookup"><span data-stu-id="13bfe-136">target</span></span>|[<span data-ttu-id="13bfe-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="13bfe-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="13bfe-138">Der Typ der Gruppen, die vom eingebetteten SIM-Aktivierungscode Pool abzielen.</span><span class="sxs-lookup"><span data-stu-id="13bfe-138">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="13bfe-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="13bfe-139">Response</span></span>
<span data-ttu-id="13bfe-140">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="13bfe-140">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13bfe-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="13bfe-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="13bfe-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="13bfe-142">Request</span></span>
<span data-ttu-id="13bfe-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="13bfe-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="13bfe-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="13bfe-144">Response</span></span>
<span data-ttu-id="13bfe-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="13bfe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




