---
title: deviceCategory aktualisieren
description: Aktualisieren der Eigenschaften eines deviceCategory-Objekts
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90f5305e2fb52b5ecd184aad837f2c9d8f6334ef
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970100"
---
# <a name="update-devicecategory"></a><span data-ttu-id="d3983-103">deviceCategory aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d3983-103">Update deviceCategory</span></span>

> <span data-ttu-id="d3983-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="d3983-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d3983-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d3983-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3983-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d3983-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3983-107">Aktualisieren der Eigenschaften eines [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts</span><span class="sxs-lookup"><span data-stu-id="d3983-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3983-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d3983-108">Prerequisites</span></span>

<span data-ttu-id="d3983-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3983-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3983-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d3983-111">Permission type</span></span>|<span data-ttu-id="d3983-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d3983-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3983-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d3983-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d3983-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="d3983-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d3983-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3983-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="d3983-116">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="d3983-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d3983-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3983-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d3983-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d3983-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3983-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3983-119">Not supported.</span></span>|
|<span data-ttu-id="d3983-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d3983-120">Application</span></span>|<span data-ttu-id="d3983-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3983-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3983-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3983-122">HTTP Request</span></span>

<span data-ttu-id="d3983-123">**deviceManagement**</span><span class="sxs-lookup"><span data-stu-id="d3983-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="d3983-124">**On-Boarding**</span><span class="sxs-lookup"><span data-stu-id="d3983-124">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="d3983-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d3983-125">Request headers</span></span>

|<span data-ttu-id="d3983-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d3983-126">Header</span></span>|<span data-ttu-id="d3983-127">Wert</span><span class="sxs-lookup"><span data-stu-id="d3983-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3983-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3983-128">Authorization</span></span>|<span data-ttu-id="d3983-129">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d3983-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3983-130">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d3983-130">Accept</span></span>|<span data-ttu-id="d3983-131">application/json</span><span class="sxs-lookup"><span data-stu-id="d3983-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3983-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d3983-132">Request body</span></span>

<span data-ttu-id="d3983-133">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekt des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) an.</span><span class="sxs-lookup"><span data-stu-id="d3983-133">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="d3983-134">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="d3983-134">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="d3983-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d3983-135">Property</span></span>|<span data-ttu-id="d3983-136">Typ</span><span class="sxs-lookup"><span data-stu-id="d3983-136">Type</span></span>|<span data-ttu-id="d3983-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3983-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3983-138">id</span><span class="sxs-lookup"><span data-stu-id="d3983-138">id</span></span>|<span data-ttu-id="d3983-139">String</span><span class="sxs-lookup"><span data-stu-id="d3983-139">String</span></span>|<span data-ttu-id="d3983-140">Der eindeutige Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="d3983-140">Unique identifier for the device category.</span></span> <span data-ttu-id="d3983-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d3983-141">Read-only.</span></span>|
|<span data-ttu-id="d3983-142">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="d3983-142">**Onboarding**</span></span>|
|<span data-ttu-id="d3983-143">description</span><span class="sxs-lookup"><span data-stu-id="d3983-143">description</span></span>|<span data-ttu-id="d3983-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d3983-144">String</span></span>|<span data-ttu-id="d3983-145">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="d3983-145">Optional description for the device category.</span></span>|
|<span data-ttu-id="d3983-146">displayName</span><span class="sxs-lookup"><span data-stu-id="d3983-146">displayName</span></span>|<span data-ttu-id="d3983-147">String</span><span class="sxs-lookup"><span data-stu-id="d3983-147">String</span></span>|<span data-ttu-id="d3983-148">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="d3983-148">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="d3983-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3983-149">Response</span></span>

<span data-ttu-id="d3983-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d3983-150">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3983-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d3983-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3983-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3983-152">Request</span></span>

<span data-ttu-id="d3983-153">Hier sind Beispiele für die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d3983-153">Here are examples of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="d3983-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3983-154">Response</span></span>

<span data-ttu-id="d3983-155">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d3983-155">Here is an example of the response.</span></span> <span data-ttu-id="d3983-156">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="d3983-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d3983-157">Antworteigenschaften können je nach Kontext variieren.</span><span class="sxs-lookup"><span data-stu-id="d3983-157">Response properties will vary according to context.</span></span>

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



