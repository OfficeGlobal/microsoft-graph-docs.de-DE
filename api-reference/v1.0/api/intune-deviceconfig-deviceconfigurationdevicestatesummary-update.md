---
title: Aktualisieren von „deviceConfigurationDeviceStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 440d1a647b11bbda80e42f0daa4176457da437a5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961448"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="34bbc-103">Aktualisieren von „deviceConfigurationDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="34bbc-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="34bbc-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="34bbc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34bbc-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="34bbc-105">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34bbc-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="34bbc-106">Prerequisites</span></span>
<span data-ttu-id="34bbc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34bbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34bbc-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="34bbc-109">Permission type</span></span>|<span data-ttu-id="34bbc-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="34bbc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34bbc-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="34bbc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="34bbc-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34bbc-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34bbc-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="34bbc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34bbc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34bbc-114">Not supported.</span></span>|
|<span data-ttu-id="34bbc-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="34bbc-115">Application</span></span>|<span data-ttu-id="34bbc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34bbc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34bbc-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="34bbc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="34bbc-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="34bbc-118">Request headers</span></span>
|<span data-ttu-id="34bbc-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="34bbc-119">Header</span></span>|<span data-ttu-id="34bbc-120">Wert</span><span class="sxs-lookup"><span data-stu-id="34bbc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34bbc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="34bbc-121">Authorization</span></span>|<span data-ttu-id="34bbc-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="34bbc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34bbc-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="34bbc-123">Accept</span></span>|<span data-ttu-id="34bbc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="34bbc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34bbc-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="34bbc-125">Request body</span></span>
<span data-ttu-id="34bbc-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="34bbc-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="34bbc-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="34bbc-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="34bbc-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="34bbc-128">Property</span></span>|<span data-ttu-id="34bbc-129">Typ</span><span class="sxs-lookup"><span data-stu-id="34bbc-129">Type</span></span>|<span data-ttu-id="34bbc-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34bbc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34bbc-131">id</span><span class="sxs-lookup"><span data-stu-id="34bbc-131">id</span></span>|<span data-ttu-id="34bbc-132">String</span><span class="sxs-lookup"><span data-stu-id="34bbc-132">String</span></span>|<span data-ttu-id="34bbc-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="34bbc-133">Key of the entity.</span></span>|
|<span data-ttu-id="34bbc-134">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="34bbc-134">unknownDeviceCount</span></span>|<span data-ttu-id="34bbc-135">Int32</span><span class="sxs-lookup"><span data-stu-id="34bbc-135">Int32</span></span>|<span data-ttu-id="34bbc-136">Anzahl der unbekannten Geräte</span><span class="sxs-lookup"><span data-stu-id="34bbc-136">Number of unknown devices</span></span>|
|<span data-ttu-id="34bbc-137">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="34bbc-137">notApplicableDeviceCount</span></span>|<span data-ttu-id="34bbc-138">Int32</span><span class="sxs-lookup"><span data-stu-id="34bbc-138">Int32</span></span>|<span data-ttu-id="34bbc-139">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="34bbc-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="34bbc-140">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="34bbc-140">compliantDeviceCount</span></span>|<span data-ttu-id="34bbc-141">Int32</span><span class="sxs-lookup"><span data-stu-id="34bbc-141">Int32</span></span>|<span data-ttu-id="34bbc-142">Anzahl der konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="34bbc-142">Number of compliant devices</span></span>|
|<span data-ttu-id="34bbc-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="34bbc-143">remediatedDeviceCount</span></span>|<span data-ttu-id="34bbc-144">Int32</span><span class="sxs-lookup"><span data-stu-id="34bbc-144">Int32</span></span>|<span data-ttu-id="34bbc-145">Anzahl der korrigierten Geräte</span><span class="sxs-lookup"><span data-stu-id="34bbc-145">Number of remediated devices</span></span>|
|<span data-ttu-id="34bbc-146">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="34bbc-146">nonCompliantDeviceCount</span></span>|<span data-ttu-id="34bbc-147">Int32</span><span class="sxs-lookup"><span data-stu-id="34bbc-147">Int32</span></span>|<span data-ttu-id="34bbc-148">Anzahl der nicht konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="34bbc-148">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="34bbc-149">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="34bbc-149">errorDeviceCount</span></span>|<span data-ttu-id="34bbc-150">Int32</span><span class="sxs-lookup"><span data-stu-id="34bbc-150">Int32</span></span>|<span data-ttu-id="34bbc-151">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="34bbc-151">Number of error devices</span></span>|
|<span data-ttu-id="34bbc-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="34bbc-152">conflictDeviceCount</span></span>|<span data-ttu-id="34bbc-153">Int32</span><span class="sxs-lookup"><span data-stu-id="34bbc-153">Int32</span></span>|<span data-ttu-id="34bbc-154">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="34bbc-154">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="34bbc-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="34bbc-155">Response</span></span>
<span data-ttu-id="34bbc-156">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="34bbc-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34bbc-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="34bbc-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="34bbc-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="34bbc-158">Request</span></span>
<span data-ttu-id="34bbc-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="34bbc-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
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

### <a name="response"></a><span data-ttu-id="34bbc-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="34bbc-160">Response</span></span>
<span data-ttu-id="34bbc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="34bbc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



