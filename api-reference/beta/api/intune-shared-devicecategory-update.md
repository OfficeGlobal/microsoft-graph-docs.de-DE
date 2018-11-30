---
title: Aktualisieren von „deviceCategory“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceCategory.
ms.openlocfilehash: bd01264d6e7e07a71c683c948fe6b01fd3822f5b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066178"
---
# <a name="update-devicecategory"></a><span data-ttu-id="97fda-103">Aktualisieren von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="97fda-103">Update deviceCategory</span></span>

> <span data-ttu-id="97fda-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="97fda-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97fda-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="97fda-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97fda-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="97fda-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97fda-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="97fda-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97fda-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="97fda-108">Prerequisites</span></span>

<span data-ttu-id="97fda-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97fda-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97fda-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97fda-111">Permission type</span></span>|<span data-ttu-id="97fda-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97fda-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97fda-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97fda-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="97fda-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="97fda-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="97fda-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97fda-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="97fda-116">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="97fda-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="97fda-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97fda-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="97fda-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97fda-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97fda-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97fda-119">Not supported.</span></span>|
|<span data-ttu-id="97fda-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97fda-120">Application</span></span>|<span data-ttu-id="97fda-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97fda-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97fda-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97fda-122">HTTP Request</span></span>

<span data-ttu-id="97fda-123">**deviceManagement**</span><span class="sxs-lookup"><span data-stu-id="97fda-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="97fda-124">**Klicken Sie auf mittels Fingereingabe**</span><span class="sxs-lookup"><span data-stu-id="97fda-124">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="97fda-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97fda-125">Request headers</span></span>

|<span data-ttu-id="97fda-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="97fda-126">Header</span></span>|<span data-ttu-id="97fda-127">Wert</span><span class="sxs-lookup"><span data-stu-id="97fda-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97fda-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="97fda-128">Authorization</span></span>|<span data-ttu-id="97fda-129">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="97fda-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97fda-130">Accept</span><span class="sxs-lookup"><span data-stu-id="97fda-130">Accept</span></span>|<span data-ttu-id="97fda-131">application/json</span><span class="sxs-lookup"><span data-stu-id="97fda-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97fda-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97fda-132">Request body</span></span>

<span data-ttu-id="97fda-133">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) an.</span><span class="sxs-lookup"><span data-stu-id="97fda-133">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="97fda-134">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="97fda-134">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="97fda-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="97fda-135">Property</span></span>|<span data-ttu-id="97fda-136">Typ</span><span class="sxs-lookup"><span data-stu-id="97fda-136">Type</span></span>|<span data-ttu-id="97fda-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97fda-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97fda-138">id</span><span class="sxs-lookup"><span data-stu-id="97fda-138">id</span></span>|<span data-ttu-id="97fda-139">String</span><span class="sxs-lookup"><span data-stu-id="97fda-139">String</span></span>|<span data-ttu-id="97fda-140">Eindeutiger Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="97fda-140">Unique identifier for the device category.</span></span> <span data-ttu-id="97fda-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="97fda-141">Read-only.</span></span>|
|<span data-ttu-id="97fda-142">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="97fda-142">**Onboarding**</span></span>|
|<span data-ttu-id="97fda-143">description</span><span class="sxs-lookup"><span data-stu-id="97fda-143">description</span></span>|<span data-ttu-id="97fda-144">String</span><span class="sxs-lookup"><span data-stu-id="97fda-144">String</span></span>|<span data-ttu-id="97fda-145">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="97fda-145">Optional description for the device category.</span></span>|
|<span data-ttu-id="97fda-146">displayName</span><span class="sxs-lookup"><span data-stu-id="97fda-146">displayName</span></span>|<span data-ttu-id="97fda-147">String</span><span class="sxs-lookup"><span data-stu-id="97fda-147">String</span></span>|<span data-ttu-id="97fda-148">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="97fda-148">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="97fda-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="97fda-149">Response</span></span>

<span data-ttu-id="97fda-150">Bei erfolgreicher Ausführung, gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="97fda-150">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97fda-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97fda-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="97fda-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97fda-152">Request</span></span>

<span data-ttu-id="97fda-153">Es folgen Beispiele für die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97fda-153">Here are examples of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="97fda-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="97fda-154">Response</span></span>

<span data-ttu-id="97fda-155">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="97fda-155">Here is an example of the response.</span></span> <span data-ttu-id="97fda-156">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="97fda-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="97fda-157">Response-Eigenschaften variiert entsprechend Kontext.</span><span class="sxs-lookup"><span data-stu-id="97fda-157">Response properties will vary according to context.</span></span>

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



