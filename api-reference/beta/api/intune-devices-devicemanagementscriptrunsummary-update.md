---
title: DeviceManagementScriptRunSummary aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DeviceManagementScriptRunSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c7a82b01ccae7e3f5ca1e8c3b3b784791fe08df3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858324"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="767c9-103">DeviceManagementScriptRunSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="767c9-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="767c9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="767c9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="767c9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="767c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="767c9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="767c9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="767c9-107">Aktualisieren Sie die Eigenschaften eines [DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="767c9-107">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="767c9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="767c9-108">Prerequisites</span></span>
<span data-ttu-id="767c9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="767c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="767c9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="767c9-111">Permission type</span></span>|<span data-ttu-id="767c9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="767c9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="767c9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="767c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="767c9-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="767c9-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="767c9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="767c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="767c9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="767c9-116">Not supported.</span></span>|
|<span data-ttu-id="767c9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="767c9-117">Application</span></span>|<span data-ttu-id="767c9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="767c9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="767c9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="767c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="767c9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="767c9-120">Request headers</span></span>
|<span data-ttu-id="767c9-121">Header</span><span class="sxs-lookup"><span data-stu-id="767c9-121">Header</span></span>|<span data-ttu-id="767c9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="767c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="767c9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="767c9-123">Authorization</span></span>|<span data-ttu-id="767c9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="767c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="767c9-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="767c9-125">Accept</span></span>|<span data-ttu-id="767c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="767c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="767c9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="767c9-127">Request body</span></span>
<span data-ttu-id="767c9-128">Geben Sie im Textkörper Anforderung für das Objekt [DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="767c9-128">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="767c9-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="767c9-129">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="767c9-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="767c9-130">Property</span></span>|<span data-ttu-id="767c9-131">Typ</span><span class="sxs-lookup"><span data-stu-id="767c9-131">Type</span></span>|<span data-ttu-id="767c9-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="767c9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="767c9-133">id</span><span class="sxs-lookup"><span data-stu-id="767c9-133">id</span></span>|<span data-ttu-id="767c9-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="767c9-134">String</span></span>|<span data-ttu-id="767c9-135">Das Gerät Management-Skript ausführen Zusammenfassung Entität-Taste.</span><span class="sxs-lookup"><span data-stu-id="767c9-135">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="767c9-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="767c9-136">successDeviceCount</span></span>|<span data-ttu-id="767c9-137">Int32</span><span class="sxs-lookup"><span data-stu-id="767c9-137">Int32</span></span>|<span data-ttu-id="767c9-138">Anzahl der Geräte Erfolg.</span><span class="sxs-lookup"><span data-stu-id="767c9-138">Success device count.</span></span>|
|<span data-ttu-id="767c9-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="767c9-139">errorDeviceCount</span></span>|<span data-ttu-id="767c9-140">Int32</span><span class="sxs-lookup"><span data-stu-id="767c9-140">Int32</span></span>|<span data-ttu-id="767c9-141">Anzahl der Fehler Geräte.</span><span class="sxs-lookup"><span data-stu-id="767c9-141">Error device count.</span></span>|
|<span data-ttu-id="767c9-142">successUserCount</span><span class="sxs-lookup"><span data-stu-id="767c9-142">successUserCount</span></span>|<span data-ttu-id="767c9-143">Int32</span><span class="sxs-lookup"><span data-stu-id="767c9-143">Int32</span></span>|<span data-ttu-id="767c9-144">Benutzeranzahl Erfolg.</span><span class="sxs-lookup"><span data-stu-id="767c9-144">Success user count.</span></span>|
|<span data-ttu-id="767c9-145">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="767c9-145">errorUserCount</span></span>|<span data-ttu-id="767c9-146">Int32</span><span class="sxs-lookup"><span data-stu-id="767c9-146">Int32</span></span>|<span data-ttu-id="767c9-147">Anzahl der Fehler Benutzer.</span><span class="sxs-lookup"><span data-stu-id="767c9-147">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="767c9-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="767c9-148">Response</span></span>
<span data-ttu-id="767c9-149">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="767c9-149">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="767c9-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="767c9-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="767c9-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="767c9-151">Request</span></span>
<span data-ttu-id="767c9-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="767c9-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
Content-type: application/json
Content-length: 108

{
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

### <a name="response"></a><span data-ttu-id="767c9-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="767c9-153">Response</span></span>
<span data-ttu-id="767c9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="767c9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





