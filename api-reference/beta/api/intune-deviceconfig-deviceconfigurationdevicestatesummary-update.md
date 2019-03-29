---
title: Aktualisieren von „deviceConfigurationDeviceStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d61e2c52fa2644d4a33ffe5f28a5b79f982d87e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977541"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="44ed4-103">Aktualisieren von „deviceConfigurationDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="44ed4-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="44ed4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="44ed4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44ed4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="44ed4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44ed4-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="44ed4-106">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44ed4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="44ed4-107">Prerequisites</span></span>
<span data-ttu-id="44ed4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44ed4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44ed4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="44ed4-110">Permission type</span></span>|<span data-ttu-id="44ed4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="44ed4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44ed4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="44ed4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44ed4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44ed4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44ed4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="44ed4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44ed4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44ed4-115">Not supported.</span></span>|
|<span data-ttu-id="44ed4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="44ed4-116">Application</span></span>|<span data-ttu-id="44ed4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44ed4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44ed4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="44ed4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="44ed4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="44ed4-119">Request headers</span></span>
|<span data-ttu-id="44ed4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="44ed4-120">Header</span></span>|<span data-ttu-id="44ed4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="44ed4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44ed4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="44ed4-122">Authorization</span></span>|<span data-ttu-id="44ed4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="44ed4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44ed4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="44ed4-124">Accept</span></span>|<span data-ttu-id="44ed4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44ed4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44ed4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="44ed4-126">Request body</span></span>
<span data-ttu-id="44ed4-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="44ed4-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="44ed4-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="44ed4-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="44ed4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="44ed4-129">Property</span></span>|<span data-ttu-id="44ed4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="44ed4-130">Type</span></span>|<span data-ttu-id="44ed4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44ed4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44ed4-132">id</span><span class="sxs-lookup"><span data-stu-id="44ed4-132">id</span></span>|<span data-ttu-id="44ed4-133">String</span><span class="sxs-lookup"><span data-stu-id="44ed4-133">String</span></span>|<span data-ttu-id="44ed4-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="44ed4-134">Key of the entity.</span></span>|
|<span data-ttu-id="44ed4-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44ed4-135">unknownDeviceCount</span></span>|<span data-ttu-id="44ed4-136">Int32</span><span class="sxs-lookup"><span data-stu-id="44ed4-136">Int32</span></span>|<span data-ttu-id="44ed4-137">Anzahl der unbekannten Geräte</span><span class="sxs-lookup"><span data-stu-id="44ed4-137">Number of unknown devices</span></span>|
|<span data-ttu-id="44ed4-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44ed4-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="44ed4-139">Int32</span><span class="sxs-lookup"><span data-stu-id="44ed4-139">Int32</span></span>|<span data-ttu-id="44ed4-140">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="44ed4-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="44ed4-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44ed4-141">compliantDeviceCount</span></span>|<span data-ttu-id="44ed4-142">Int32</span><span class="sxs-lookup"><span data-stu-id="44ed4-142">Int32</span></span>|<span data-ttu-id="44ed4-143">Anzahl der konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="44ed4-143">Number of compliant devices</span></span>|
|<span data-ttu-id="44ed4-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44ed4-144">remediatedDeviceCount</span></span>|<span data-ttu-id="44ed4-145">Int32</span><span class="sxs-lookup"><span data-stu-id="44ed4-145">Int32</span></span>|<span data-ttu-id="44ed4-146">Anzahl der korrigierten Geräte</span><span class="sxs-lookup"><span data-stu-id="44ed4-146">Number of remediated devices</span></span>|
|<span data-ttu-id="44ed4-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44ed4-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="44ed4-148">Int32</span><span class="sxs-lookup"><span data-stu-id="44ed4-148">Int32</span></span>|<span data-ttu-id="44ed4-149">Anzahl der nicht konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="44ed4-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="44ed4-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44ed4-150">errorDeviceCount</span></span>|<span data-ttu-id="44ed4-151">Int32</span><span class="sxs-lookup"><span data-stu-id="44ed4-151">Int32</span></span>|<span data-ttu-id="44ed4-152">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="44ed4-152">Number of error devices</span></span>|
|<span data-ttu-id="44ed4-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44ed4-153">conflictDeviceCount</span></span>|<span data-ttu-id="44ed4-154">Int32</span><span class="sxs-lookup"><span data-stu-id="44ed4-154">Int32</span></span>|<span data-ttu-id="44ed4-155">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="44ed4-155">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="44ed4-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="44ed4-156">Response</span></span>
<span data-ttu-id="44ed4-157">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="44ed4-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44ed4-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="44ed4-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="44ed4-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44ed4-159">Request</span></span>
<span data-ttu-id="44ed4-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44ed4-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="44ed4-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="44ed4-161">Response</span></span>
<span data-ttu-id="44ed4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44ed4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```




