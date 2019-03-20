---
title: deviceCategory aktualisieren
description: Aktualisieren der Eigenschaften eines deviceCategory-Objekts
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: eb2d3bc4f081065f27de1c303f87f9e98700d7b9
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572348"
---
# <a name="update-devicecategory"></a><span data-ttu-id="e3099-103">deviceCategory aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e3099-103">Update deviceCategory</span></span>

> <span data-ttu-id="e3099-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="e3099-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e3099-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3099-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3099-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e3099-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3099-107">Aktualisieren der Eigenschaften eines [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts</span><span class="sxs-lookup"><span data-stu-id="e3099-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3099-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e3099-108">Prerequisites</span></span>

<span data-ttu-id="e3099-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e3099-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e3099-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3099-111">Permission type</span></span>|<span data-ttu-id="e3099-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3099-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3099-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3099-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e3099-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="e3099-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e3099-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3099-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="e3099-116">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="e3099-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e3099-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3099-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e3099-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3099-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3099-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3099-119">Not supported.</span></span>|
|<span data-ttu-id="e3099-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3099-120">Application</span></span>|<span data-ttu-id="e3099-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3099-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3099-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3099-122">HTTP Request</span></span>

<span data-ttu-id="e3099-123">**deviceManagement**</span><span class="sxs-lookup"><span data-stu-id="e3099-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="e3099-124">**On-Boarding**</span><span class="sxs-lookup"><span data-stu-id="e3099-124">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="e3099-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3099-125">Request headers</span></span>

|<span data-ttu-id="e3099-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e3099-126">Header</span></span>|<span data-ttu-id="e3099-127">Wert</span><span class="sxs-lookup"><span data-stu-id="e3099-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3099-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3099-128">Authorization</span></span>|<span data-ttu-id="e3099-129">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e3099-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3099-130">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e3099-130">Accept</span></span>|<span data-ttu-id="e3099-131">application/json</span><span class="sxs-lookup"><span data-stu-id="e3099-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3099-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3099-132">Request body</span></span>

<span data-ttu-id="e3099-133">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekt des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) an.</span><span class="sxs-lookup"><span data-stu-id="e3099-133">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="e3099-134">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="e3099-134">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="e3099-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3099-135">Property</span></span>|<span data-ttu-id="e3099-136">Typ</span><span class="sxs-lookup"><span data-stu-id="e3099-136">Type</span></span>|<span data-ttu-id="e3099-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3099-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3099-138">id</span><span class="sxs-lookup"><span data-stu-id="e3099-138">id</span></span>|<span data-ttu-id="e3099-139">String</span><span class="sxs-lookup"><span data-stu-id="e3099-139">String</span></span>|<span data-ttu-id="e3099-140">Der eindeutige Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="e3099-140">Unique identifier for the device category.</span></span> <span data-ttu-id="e3099-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e3099-141">Read-only.</span></span>|
|<span data-ttu-id="e3099-142">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="e3099-142">**Onboarding**</span></span>|
|<span data-ttu-id="e3099-143">description</span><span class="sxs-lookup"><span data-stu-id="e3099-143">description</span></span>|<span data-ttu-id="e3099-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3099-144">String</span></span>|<span data-ttu-id="e3099-145">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="e3099-145">Optional description for the device category.</span></span>|
|<span data-ttu-id="e3099-146">displayName</span><span class="sxs-lookup"><span data-stu-id="e3099-146">displayName</span></span>|<span data-ttu-id="e3099-147">String</span><span class="sxs-lookup"><span data-stu-id="e3099-147">String</span></span>|<span data-ttu-id="e3099-148">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="e3099-148">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="e3099-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3099-149">Response</span></span>

<span data-ttu-id="e3099-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3099-150">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3099-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3099-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3099-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3099-152">Request</span></span>

<span data-ttu-id="e3099-153">Hier sind Beispiele für die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e3099-153">Here are examples of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a><span data-ttu-id="e3099-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3099-154">Response</span></span>

<span data-ttu-id="e3099-155">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e3099-155">Here is an example of the response.</span></span> <span data-ttu-id="e3099-156">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="e3099-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e3099-157">Antworteigenschaften können je nach Kontext variieren.</span><span class="sxs-lookup"><span data-stu-id="e3099-157">Response properties will vary according to context.</span></span>

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



