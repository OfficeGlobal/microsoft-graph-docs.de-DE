---
title: Aktualisieren von „deviceCategory“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 831232fc656ad4aa0968e40aca5ae54b1e13ceef
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255178"
---
# <a name="update-devicecategory"></a><span data-ttu-id="b8e97-103">Aktualisieren von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="b8e97-103">Update deviceCategory</span></span>

> <span data-ttu-id="b8e97-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b8e97-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8e97-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b8e97-105">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8e97-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b8e97-106">Prerequisites</span></span>
<span data-ttu-id="b8e97-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8e97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8e97-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8e97-109">Permission type</span></span>|<span data-ttu-id="b8e97-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8e97-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8e97-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8e97-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b8e97-112">&nbsp;&nbsp; \*\*\*\* Onboarding und</span><span class="sxs-lookup"><span data-stu-id="b8e97-112">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="b8e97-113">&nbsp;&nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="b8e97-113">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="b8e97-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8e97-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b8e97-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8e97-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8e97-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8e97-116">Not supported.</span></span>|
|<span data-ttu-id="b8e97-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8e97-117">Application</span></span>|<span data-ttu-id="b8e97-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8e97-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8e97-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8e97-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="b8e97-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8e97-120">Request headers</span></span>
|<span data-ttu-id="b8e97-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b8e97-121">Header</span></span>|<span data-ttu-id="b8e97-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b8e97-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8e97-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8e97-123">Authorization</span></span>|<span data-ttu-id="b8e97-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b8e97-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8e97-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b8e97-125">Accept</span></span>|<span data-ttu-id="b8e97-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8e97-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8e97-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8e97-127">Request body</span></span>
<span data-ttu-id="b8e97-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) an.</span><span class="sxs-lookup"><span data-stu-id="b8e97-128">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="b8e97-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="b8e97-129">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="b8e97-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8e97-130">Property</span></span>|<span data-ttu-id="b8e97-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b8e97-131">Type</span></span>|<span data-ttu-id="b8e97-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8e97-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8e97-133">id</span><span class="sxs-lookup"><span data-stu-id="b8e97-133">id</span></span>|<span data-ttu-id="b8e97-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8e97-134">String</span></span>|<span data-ttu-id="b8e97-135">Eindeutiger Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="b8e97-135">Unique identifier for the device category.</span></span> <span data-ttu-id="b8e97-136">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b8e97-136">Read-only.</span></span>|
|<span data-ttu-id="b8e97-137">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="b8e97-137">**Onboarding**</span></span>|
|<span data-ttu-id="b8e97-138">displayName</span><span class="sxs-lookup"><span data-stu-id="b8e97-138">displayName</span></span>|<span data-ttu-id="b8e97-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8e97-139">String</span></span>|<span data-ttu-id="b8e97-140">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="b8e97-140">Display name for the device category.</span></span>|
|<span data-ttu-id="b8e97-141">description</span><span class="sxs-lookup"><span data-stu-id="b8e97-141">description</span></span>|<span data-ttu-id="b8e97-142">String</span><span class="sxs-lookup"><span data-stu-id="b8e97-142">String</span></span>|<span data-ttu-id="b8e97-143">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="b8e97-143">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="b8e97-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8e97-144">Response</span></span>
<span data-ttu-id="b8e97-145">Bei erfolgreicher Ausführung, gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b8e97-145">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8e97-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8e97-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8e97-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8e97-147">Request</span></span>
<span data-ttu-id="b8e97-148">Hier sind Beispiele für die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b8e97-148">Here are examples of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a><span data-ttu-id="b8e97-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8e97-149">Response</span></span>
<span data-ttu-id="b8e97-150">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b8e97-150">Here is an example of the response.</span></span> <span data-ttu-id="b8e97-151">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="b8e97-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b8e97-152">Antworteigenschaften können je nach Kontext variieren.</span><span class="sxs-lookup"><span data-stu-id="b8e97-152">Response properties will vary according to context.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



