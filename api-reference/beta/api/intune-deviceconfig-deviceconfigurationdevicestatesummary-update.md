---
title: Aktualisieren von „deviceConfigurationDeviceStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationDeviceStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 41b092aa651d8526618f8287c7a90ff9673c7508
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408551"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="7619a-103">Aktualisieren von „deviceConfigurationDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="7619a-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="7619a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="7619a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7619a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7619a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7619a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7619a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7619a-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7619a-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7619a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7619a-108">Prerequisites</span></span>
<span data-ttu-id="7619a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7619a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7619a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7619a-111">Permission type</span></span>|<span data-ttu-id="7619a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7619a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7619a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7619a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7619a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7619a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7619a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7619a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7619a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7619a-116">Not supported.</span></span>|
|<span data-ttu-id="7619a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7619a-117">Application</span></span>|<span data-ttu-id="7619a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7619a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7619a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7619a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="7619a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7619a-120">Request headers</span></span>
|<span data-ttu-id="7619a-121">Header</span><span class="sxs-lookup"><span data-stu-id="7619a-121">Header</span></span>|<span data-ttu-id="7619a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7619a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7619a-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7619a-123">Authorization</span></span>|<span data-ttu-id="7619a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7619a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7619a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7619a-125">Accept</span></span>|<span data-ttu-id="7619a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7619a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7619a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7619a-127">Request body</span></span>
<span data-ttu-id="7619a-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="7619a-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="7619a-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7619a-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="7619a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7619a-130">Property</span></span>|<span data-ttu-id="7619a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7619a-131">Type</span></span>|<span data-ttu-id="7619a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7619a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7619a-133">id</span><span class="sxs-lookup"><span data-stu-id="7619a-133">id</span></span>|<span data-ttu-id="7619a-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7619a-134">String</span></span>|<span data-ttu-id="7619a-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7619a-135">Key of the entity.</span></span>|
|<span data-ttu-id="7619a-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7619a-136">unknownDeviceCount</span></span>|<span data-ttu-id="7619a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7619a-137">Int32</span></span>|<span data-ttu-id="7619a-138">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="7619a-138">Number of unknown devices</span></span>|
|<span data-ttu-id="7619a-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7619a-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="7619a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7619a-140">Int32</span></span>|<span data-ttu-id="7619a-141">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="7619a-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="7619a-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7619a-142">compliantDeviceCount</span></span>|<span data-ttu-id="7619a-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7619a-143">Int32</span></span>|<span data-ttu-id="7619a-144">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="7619a-144">Number of compliant devices</span></span>|
|<span data-ttu-id="7619a-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7619a-145">remediatedDeviceCount</span></span>|<span data-ttu-id="7619a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="7619a-146">Int32</span></span>|<span data-ttu-id="7619a-147">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="7619a-147">Number of remediated devices</span></span>|
|<span data-ttu-id="7619a-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7619a-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="7619a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="7619a-149">Int32</span></span>|<span data-ttu-id="7619a-150">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="7619a-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="7619a-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7619a-151">errorDeviceCount</span></span>|<span data-ttu-id="7619a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7619a-152">Int32</span></span>|<span data-ttu-id="7619a-153">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="7619a-153">Number of error devices</span></span>|
|<span data-ttu-id="7619a-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7619a-154">conflictDeviceCount</span></span>|<span data-ttu-id="7619a-155">Int32</span><span class="sxs-lookup"><span data-stu-id="7619a-155">Int32</span></span>|<span data-ttu-id="7619a-156">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="7619a-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="7619a-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="7619a-157">Response</span></span>
<span data-ttu-id="7619a-158">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7619a-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7619a-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7619a-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="7619a-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7619a-160">Request</span></span>
<span data-ttu-id="7619a-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7619a-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7619a-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="7619a-162">Response</span></span>
<span data-ttu-id="7619a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7619a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




