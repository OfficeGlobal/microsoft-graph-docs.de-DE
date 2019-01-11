---
title: Aktualisieren von „deviceCategory“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 38377c7b92983f10ad42284b7790782cde2264fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832977"
---
# <a name="update-devicecategory"></a><span data-ttu-id="2fb7b-103">Aktualisieren von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="2fb7b-103">Update deviceCategory</span></span>

> <span data-ttu-id="2fb7b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2fb7b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fb7b-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="2fb7b-105">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2fb7b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2fb7b-106">Prerequisites</span></span>
<span data-ttu-id="2fb7b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fb7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fb7b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2fb7b-109">Permission type</span></span>|<span data-ttu-id="2fb7b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2fb7b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fb7b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2fb7b-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2fb7b-112">&nbsp;&nbsp; **Onboarding** und</span><span class="sxs-lookup"><span data-stu-id="2fb7b-112">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="2fb7b-113">&nbsp;&nbsp; **Gerätemanagement**</span><span class="sxs-lookup"><span data-stu-id="2fb7b-113">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="2fb7b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fb7b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2fb7b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2fb7b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fb7b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2fb7b-116">Not supported.</span></span>|
|<span data-ttu-id="2fb7b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2fb7b-117">Application</span></span>|<span data-ttu-id="2fb7b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2fb7b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fb7b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2fb7b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="2fb7b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2fb7b-120">Request headers</span></span>
|<span data-ttu-id="2fb7b-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2fb7b-121">Header</span></span>|<span data-ttu-id="2fb7b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2fb7b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fb7b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fb7b-123">Authorization</span></span>|<span data-ttu-id="2fb7b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2fb7b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fb7b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2fb7b-125">Accept</span></span>|<span data-ttu-id="2fb7b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2fb7b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fb7b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2fb7b-127">Request body</span></span>
<span data-ttu-id="2fb7b-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) an.</span><span class="sxs-lookup"><span data-stu-id="2fb7b-128">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="2fb7b-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2fb7b-129">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="2fb7b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2fb7b-130">Property</span></span>|<span data-ttu-id="2fb7b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2fb7b-131">Type</span></span>|<span data-ttu-id="2fb7b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2fb7b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fb7b-133">id</span><span class="sxs-lookup"><span data-stu-id="2fb7b-133">id</span></span>|<span data-ttu-id="2fb7b-134">String</span><span class="sxs-lookup"><span data-stu-id="2fb7b-134">String</span></span>|<span data-ttu-id="2fb7b-135">Eindeutiger Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="2fb7b-135">Unique identifier for the device category.</span></span> <span data-ttu-id="2fb7b-136">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2fb7b-136">Read-only.</span></span>|
|<span data-ttu-id="2fb7b-137">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="2fb7b-137">**Onboarding**</span></span>|
|<span data-ttu-id="2fb7b-138">displayName</span><span class="sxs-lookup"><span data-stu-id="2fb7b-138">displayName</span></span>|<span data-ttu-id="2fb7b-139">String</span><span class="sxs-lookup"><span data-stu-id="2fb7b-139">String</span></span>|<span data-ttu-id="2fb7b-140">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="2fb7b-140">Display name for the device category.</span></span>|
|<span data-ttu-id="2fb7b-141">description</span><span class="sxs-lookup"><span data-stu-id="2fb7b-141">description</span></span>|<span data-ttu-id="2fb7b-142">String</span><span class="sxs-lookup"><span data-stu-id="2fb7b-142">String</span></span>|<span data-ttu-id="2fb7b-143">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="2fb7b-143">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="2fb7b-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="2fb7b-144">Response</span></span>
<span data-ttu-id="2fb7b-145">Bei erfolgreicher Ausführung, gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2fb7b-145">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fb7b-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2fb7b-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="2fb7b-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2fb7b-147">Request</span></span>
<span data-ttu-id="2fb7b-148">Es folgen Beispiele für die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2fb7b-148">Here are examples of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2fb7b-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="2fb7b-149">Response</span></span>
<span data-ttu-id="2fb7b-150">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2fb7b-150">Here is an example of the response.</span></span> <span data-ttu-id="2fb7b-151">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="2fb7b-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2fb7b-152">Response-Eigenschaften variiert entsprechend Kontext.</span><span class="sxs-lookup"><span data-stu-id="2fb7b-152">Response properties will vary according to context.</span></span>
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



