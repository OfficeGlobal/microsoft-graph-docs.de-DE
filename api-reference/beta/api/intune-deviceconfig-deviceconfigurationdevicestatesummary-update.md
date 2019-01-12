---
title: Aktualisieren von „deviceConfigurationDeviceStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 599411d60bc723e95297926c600359bda3c70fc1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924594"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="6b69e-103">Aktualisieren von „deviceConfigurationDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="6b69e-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="6b69e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6b69e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b69e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b69e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b69e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6b69e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b69e-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6b69e-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6b69e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6b69e-108">Prerequisites</span></span>
<span data-ttu-id="6b69e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b69e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b69e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6b69e-111">Permission type</span></span>|<span data-ttu-id="6b69e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6b69e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b69e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6b69e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b69e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b69e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b69e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6b69e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b69e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b69e-116">Not supported.</span></span>|
|<span data-ttu-id="6b69e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6b69e-117">Application</span></span>|<span data-ttu-id="6b69e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b69e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b69e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b69e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="6b69e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6b69e-120">Request headers</span></span>
|<span data-ttu-id="6b69e-121">Header</span><span class="sxs-lookup"><span data-stu-id="6b69e-121">Header</span></span>|<span data-ttu-id="6b69e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6b69e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b69e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b69e-123">Authorization</span></span>|<span data-ttu-id="6b69e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6b69e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b69e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6b69e-125">Accept</span></span>|<span data-ttu-id="6b69e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b69e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b69e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6b69e-127">Request body</span></span>
<span data-ttu-id="6b69e-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="6b69e-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="6b69e-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="6b69e-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="6b69e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6b69e-130">Property</span></span>|<span data-ttu-id="6b69e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6b69e-131">Type</span></span>|<span data-ttu-id="6b69e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b69e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b69e-133">id</span><span class="sxs-lookup"><span data-stu-id="6b69e-133">id</span></span>|<span data-ttu-id="6b69e-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6b69e-134">String</span></span>|<span data-ttu-id="6b69e-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6b69e-135">Key of the entity.</span></span>|
|<span data-ttu-id="6b69e-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b69e-136">unknownDeviceCount</span></span>|<span data-ttu-id="6b69e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6b69e-137">Int32</span></span>|<span data-ttu-id="6b69e-138">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="6b69e-138">Number of unknown devices</span></span>|
|<span data-ttu-id="6b69e-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b69e-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="6b69e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6b69e-140">Int32</span></span>|<span data-ttu-id="6b69e-141">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="6b69e-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="6b69e-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b69e-142">compliantDeviceCount</span></span>|<span data-ttu-id="6b69e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6b69e-143">Int32</span></span>|<span data-ttu-id="6b69e-144">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="6b69e-144">Number of compliant devices</span></span>|
|<span data-ttu-id="6b69e-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b69e-145">remediatedDeviceCount</span></span>|<span data-ttu-id="6b69e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="6b69e-146">Int32</span></span>|<span data-ttu-id="6b69e-147">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="6b69e-147">Number of remediated devices</span></span>|
|<span data-ttu-id="6b69e-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b69e-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="6b69e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6b69e-149">Int32</span></span>|<span data-ttu-id="6b69e-150">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="6b69e-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="6b69e-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b69e-151">errorDeviceCount</span></span>|<span data-ttu-id="6b69e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6b69e-152">Int32</span></span>|<span data-ttu-id="6b69e-153">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="6b69e-153">Number of error devices</span></span>|
|<span data-ttu-id="6b69e-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b69e-154">conflictDeviceCount</span></span>|<span data-ttu-id="6b69e-155">Int32</span><span class="sxs-lookup"><span data-stu-id="6b69e-155">Int32</span></span>|<span data-ttu-id="6b69e-156">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="6b69e-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="6b69e-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b69e-157">Response</span></span>
<span data-ttu-id="6b69e-158">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6b69e-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b69e-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6b69e-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="6b69e-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b69e-160">Request</span></span>
<span data-ttu-id="6b69e-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6b69e-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 214

{
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="6b69e-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b69e-162">Response</span></span>
<span data-ttu-id="6b69e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6b69e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





