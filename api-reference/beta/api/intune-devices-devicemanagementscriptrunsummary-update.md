---
title: DeviceManagementScriptRunSummary aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DeviceManagementScriptRunSummary-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55582147aff81bc8d566634a5fb9fdc1ff4ff2fd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413990"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="e7f0f-103">DeviceManagementScriptRunSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e7f0f-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="e7f0f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e7f0f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e7f0f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e7f0f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7f0f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e7f0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7f0f-107">Aktualisieren Sie die Eigenschaften eines [DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e7f0f-107">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7f0f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e7f0f-108">Prerequisites</span></span>
<span data-ttu-id="e7f0f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e7f0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e7f0f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e7f0f-111">Permission type</span></span>|<span data-ttu-id="e7f0f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e7f0f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7f0f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e7f0f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7f0f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7f0f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e7f0f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e7f0f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7f0f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7f0f-116">Not supported.</span></span>|
|<span data-ttu-id="e7f0f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e7f0f-117">Application</span></span>|<span data-ttu-id="e7f0f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7f0f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7f0f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7f0f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="e7f0f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e7f0f-120">Request headers</span></span>
|<span data-ttu-id="e7f0f-121">Header</span><span class="sxs-lookup"><span data-stu-id="e7f0f-121">Header</span></span>|<span data-ttu-id="e7f0f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e7f0f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7f0f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e7f0f-123">Authorization</span></span>|<span data-ttu-id="e7f0f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e7f0f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7f0f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e7f0f-125">Accept</span></span>|<span data-ttu-id="e7f0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7f0f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7f0f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e7f0f-127">Request body</span></span>
<span data-ttu-id="e7f0f-128">Geben Sie im Textkörper Anforderung für das Objekt [DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="e7f0f-128">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="e7f0f-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="e7f0f-129">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="e7f0f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e7f0f-130">Property</span></span>|<span data-ttu-id="e7f0f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e7f0f-131">Type</span></span>|<span data-ttu-id="e7f0f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e7f0f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7f0f-133">id</span><span class="sxs-lookup"><span data-stu-id="e7f0f-133">id</span></span>|<span data-ttu-id="e7f0f-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7f0f-134">String</span></span>|<span data-ttu-id="e7f0f-135">Das Gerät Management-Skript ausführen Zusammenfassung Entität-Taste.</span><span class="sxs-lookup"><span data-stu-id="e7f0f-135">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="e7f0f-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e7f0f-136">successDeviceCount</span></span>|<span data-ttu-id="e7f0f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e7f0f-137">Int32</span></span>|<span data-ttu-id="e7f0f-138">Anzahl der Geräte Erfolg.</span><span class="sxs-lookup"><span data-stu-id="e7f0f-138">Success device count.</span></span>|
|<span data-ttu-id="e7f0f-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e7f0f-139">errorDeviceCount</span></span>|<span data-ttu-id="e7f0f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e7f0f-140">Int32</span></span>|<span data-ttu-id="e7f0f-141">Anzahl der Fehler Geräte.</span><span class="sxs-lookup"><span data-stu-id="e7f0f-141">Error device count.</span></span>|
|<span data-ttu-id="e7f0f-142">successUserCount</span><span class="sxs-lookup"><span data-stu-id="e7f0f-142">successUserCount</span></span>|<span data-ttu-id="e7f0f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e7f0f-143">Int32</span></span>|<span data-ttu-id="e7f0f-144">Benutzeranzahl Erfolg.</span><span class="sxs-lookup"><span data-stu-id="e7f0f-144">Success user count.</span></span>|
|<span data-ttu-id="e7f0f-145">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="e7f0f-145">errorUserCount</span></span>|<span data-ttu-id="e7f0f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e7f0f-146">Int32</span></span>|<span data-ttu-id="e7f0f-147">Anzahl der Fehler Benutzer.</span><span class="sxs-lookup"><span data-stu-id="e7f0f-147">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="e7f0f-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7f0f-148">Response</span></span>
<span data-ttu-id="e7f0f-149">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e7f0f-149">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7f0f-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e7f0f-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7f0f-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7f0f-151">Request</span></span>
<span data-ttu-id="e7f0f-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e7f0f-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e7f0f-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7f0f-153">Response</span></span>
<span data-ttu-id="e7f0f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e7f0f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




