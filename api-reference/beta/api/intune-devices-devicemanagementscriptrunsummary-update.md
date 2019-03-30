---
title: DeviceManagementScriptRunSummary aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementScriptRunSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 040214d3236e877b9c7d12b63bda659058028244
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986341"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="b8a76-103">DeviceManagementScriptRunSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b8a76-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="b8a76-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8a76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8a76-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b8a76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8a76-106">Aktualisieren der Eigenschaften eines [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b8a76-106">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8a76-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b8a76-107">Prerequisites</span></span>
<span data-ttu-id="b8a76-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8a76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8a76-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8a76-110">Permission type</span></span>|<span data-ttu-id="b8a76-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8a76-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8a76-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8a76-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b8a76-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8a76-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b8a76-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8a76-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8a76-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8a76-115">Not supported.</span></span>|
|<span data-ttu-id="b8a76-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8a76-116">Application</span></span>|<span data-ttu-id="b8a76-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8a76-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8a76-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8a76-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="b8a76-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8a76-119">Request headers</span></span>
|<span data-ttu-id="b8a76-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b8a76-120">Header</span></span>|<span data-ttu-id="b8a76-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b8a76-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8a76-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8a76-122">Authorization</span></span>|<span data-ttu-id="b8a76-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b8a76-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8a76-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b8a76-124">Accept</span></span>|<span data-ttu-id="b8a76-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b8a76-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8a76-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8a76-126">Request body</span></span>
<span data-ttu-id="b8a76-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b8a76-127">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="b8a76-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b8a76-128">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="b8a76-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8a76-129">Property</span></span>|<span data-ttu-id="b8a76-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b8a76-130">Type</span></span>|<span data-ttu-id="b8a76-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8a76-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8a76-132">id</span><span class="sxs-lookup"><span data-stu-id="b8a76-132">id</span></span>|<span data-ttu-id="b8a76-133">String</span><span class="sxs-lookup"><span data-stu-id="b8a76-133">String</span></span>|<span data-ttu-id="b8a76-134">Der Schlüssel der Device Management-Skript Ausführungs Zusammenfassungs Entität.</span><span class="sxs-lookup"><span data-stu-id="b8a76-134">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="b8a76-135">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b8a76-135">successDeviceCount</span></span>|<span data-ttu-id="b8a76-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b8a76-136">Int32</span></span>|<span data-ttu-id="b8a76-137">Anzahl der erfolgreichen Geräte.</span><span class="sxs-lookup"><span data-stu-id="b8a76-137">Success device count.</span></span>|
|<span data-ttu-id="b8a76-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b8a76-138">errorDeviceCount</span></span>|<span data-ttu-id="b8a76-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b8a76-139">Int32</span></span>|<span data-ttu-id="b8a76-140">Fehlergeräte Anzahl.</span><span class="sxs-lookup"><span data-stu-id="b8a76-140">Error device count.</span></span>|
|<span data-ttu-id="b8a76-141">successUserCount</span><span class="sxs-lookup"><span data-stu-id="b8a76-141">successUserCount</span></span>|<span data-ttu-id="b8a76-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b8a76-142">Int32</span></span>|<span data-ttu-id="b8a76-143">Anzahl der erfolgreichen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="b8a76-143">Success user count.</span></span>|
|<span data-ttu-id="b8a76-144">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="b8a76-144">errorUserCount</span></span>|<span data-ttu-id="b8a76-145">Int32</span><span class="sxs-lookup"><span data-stu-id="b8a76-145">Int32</span></span>|<span data-ttu-id="b8a76-146">Fehler Benutzeranzahl.</span><span class="sxs-lookup"><span data-stu-id="b8a76-146">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="b8a76-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8a76-147">Response</span></span>
<span data-ttu-id="b8a76-148">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b8a76-148">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8a76-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8a76-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8a76-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8a76-150">Request</span></span>
<span data-ttu-id="b8a76-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b8a76-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

### <a name="response"></a><span data-ttu-id="b8a76-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8a76-152">Response</span></span>
<span data-ttu-id="b8a76-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8a76-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "514d5d38-5d38-514d-385d-4d51385d4d51",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```




