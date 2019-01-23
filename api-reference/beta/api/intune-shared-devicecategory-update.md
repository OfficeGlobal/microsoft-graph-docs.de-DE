---
title: Aktualisieren von „deviceCategory“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90f5305e2fb52b5ecd184aad837f2c9d8f6334ef
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395013"
---
# <a name="update-devicecategory"></a><span data-ttu-id="5e86f-103">Aktualisieren von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="5e86f-103">Update deviceCategory</span></span>

> <span data-ttu-id="5e86f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5e86f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5e86f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5e86f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e86f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5e86f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e86f-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="5e86f-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e86f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5e86f-108">Prerequisites</span></span>

<span data-ttu-id="5e86f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e86f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e86f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5e86f-111">Permission type</span></span>|<span data-ttu-id="5e86f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5e86f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e86f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5e86f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5e86f-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="5e86f-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5e86f-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e86f-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="5e86f-116">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="5e86f-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="5e86f-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e86f-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5e86f-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5e86f-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e86f-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5e86f-119">Not supported.</span></span>|
|<span data-ttu-id="5e86f-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5e86f-120">Application</span></span>|<span data-ttu-id="5e86f-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5e86f-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e86f-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e86f-122">HTTP Request</span></span>

<span data-ttu-id="5e86f-123">**deviceManagement**</span><span class="sxs-lookup"><span data-stu-id="5e86f-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="5e86f-124">**Klicken Sie auf mittels Fingereingabe**</span><span class="sxs-lookup"><span data-stu-id="5e86f-124">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="5e86f-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5e86f-125">Request headers</span></span>

|<span data-ttu-id="5e86f-126">Header</span><span class="sxs-lookup"><span data-stu-id="5e86f-126">Header</span></span>|<span data-ttu-id="5e86f-127">Wert</span><span class="sxs-lookup"><span data-stu-id="5e86f-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e86f-128">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5e86f-128">Authorization</span></span>|<span data-ttu-id="5e86f-129">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5e86f-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e86f-130">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5e86f-130">Accept</span></span>|<span data-ttu-id="5e86f-131">application/json</span><span class="sxs-lookup"><span data-stu-id="5e86f-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e86f-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5e86f-132">Request body</span></span>

<span data-ttu-id="5e86f-133">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) an.</span><span class="sxs-lookup"><span data-stu-id="5e86f-133">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="5e86f-134">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="5e86f-134">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="5e86f-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5e86f-135">Property</span></span>|<span data-ttu-id="5e86f-136">Typ</span><span class="sxs-lookup"><span data-stu-id="5e86f-136">Type</span></span>|<span data-ttu-id="5e86f-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e86f-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e86f-138">id</span><span class="sxs-lookup"><span data-stu-id="5e86f-138">id</span></span>|<span data-ttu-id="5e86f-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5e86f-139">String</span></span>|<span data-ttu-id="5e86f-140">Eindeutiger Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="5e86f-140">Unique identifier for the device category.</span></span> <span data-ttu-id="5e86f-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5e86f-141">Read-only.</span></span>|
|<span data-ttu-id="5e86f-142">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="5e86f-142">**Onboarding**</span></span>|
|<span data-ttu-id="5e86f-143">description</span><span class="sxs-lookup"><span data-stu-id="5e86f-143">description</span></span>|<span data-ttu-id="5e86f-144">String</span><span class="sxs-lookup"><span data-stu-id="5e86f-144">String</span></span>|<span data-ttu-id="5e86f-145">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="5e86f-145">Optional description for the device category.</span></span>|
|<span data-ttu-id="5e86f-146">displayName</span><span class="sxs-lookup"><span data-stu-id="5e86f-146">displayName</span></span>|<span data-ttu-id="5e86f-147">String</span><span class="sxs-lookup"><span data-stu-id="5e86f-147">String</span></span>|<span data-ttu-id="5e86f-148">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="5e86f-148">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="5e86f-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e86f-149">Response</span></span>

<span data-ttu-id="5e86f-150">Bei erfolgreicher Ausführung, gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5e86f-150">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e86f-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5e86f-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e86f-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e86f-152">Request</span></span>

<span data-ttu-id="5e86f-153">Es folgen Beispiele für die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5e86f-153">Here are examples of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="5e86f-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e86f-154">Response</span></span>

<span data-ttu-id="5e86f-155">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5e86f-155">Here is an example of the response.</span></span> <span data-ttu-id="5e86f-156">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="5e86f-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5e86f-157">Response-Eigenschaften variiert entsprechend Kontext.</span><span class="sxs-lookup"><span data-stu-id="5e86f-157">Response properties will vary according to context.</span></span>

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



