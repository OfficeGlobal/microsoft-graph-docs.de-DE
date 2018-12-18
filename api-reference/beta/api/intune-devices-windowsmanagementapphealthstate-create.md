---
title: Erstellen von windowsManagementAppHealthState
description: Erstellen eines neuen WindowsManagementAppHealthState-Objekts.
author: tfitzmac
ms.openlocfilehash: 5fec23dec7510c0b7b1a53b0be7d2dfe507959f3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359080"
---
# <a name="create-windowsmanagementapphealthstate"></a><span data-ttu-id="1730f-103">Erstellen von windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="1730f-103">Create windowsManagementAppHealthState</span></span>

> <span data-ttu-id="1730f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1730f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1730f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1730f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1730f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1730f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1730f-107">Erstellen eines neuen [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1730f-107">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1730f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1730f-108">Prerequisites</span></span>
<span data-ttu-id="1730f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1730f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1730f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1730f-111">Permission type</span></span>|<span data-ttu-id="1730f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1730f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1730f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1730f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1730f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1730f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1730f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1730f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1730f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1730f-116">Not supported.</span></span>|
|<span data-ttu-id="1730f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1730f-117">Application</span></span>|<span data-ttu-id="1730f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1730f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1730f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1730f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="1730f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1730f-120">Request headers</span></span>
|<span data-ttu-id="1730f-121">Header</span><span class="sxs-lookup"><span data-stu-id="1730f-121">Header</span></span>|<span data-ttu-id="1730f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1730f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1730f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1730f-123">Authorization</span></span>|<span data-ttu-id="1730f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1730f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1730f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1730f-125">Accept</span></span>|<span data-ttu-id="1730f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1730f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1730f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1730f-127">Request body</span></span>
<span data-ttu-id="1730f-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsManagementAppHealthState eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="1730f-128">In the request body, supply a JSON representation for the windowsManagementAppHealthState object.</span></span>

<span data-ttu-id="1730f-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsManagementAppHealthState erstellen.</span><span class="sxs-lookup"><span data-stu-id="1730f-129">The following table shows the properties that are required when you create the windowsManagementAppHealthState.</span></span>

|<span data-ttu-id="1730f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1730f-130">Property</span></span>|<span data-ttu-id="1730f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1730f-131">Type</span></span>|<span data-ttu-id="1730f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1730f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1730f-133">id</span><span class="sxs-lookup"><span data-stu-id="1730f-133">id</span></span>|<span data-ttu-id="1730f-134">String</span><span class="sxs-lookup"><span data-stu-id="1730f-134">String</span></span>|<span data-ttu-id="1730f-135">Eindeutiger Bezeichner für den Zustand des Windows Management-app</span><span class="sxs-lookup"><span data-stu-id="1730f-135">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="1730f-136">healthState</span><span class="sxs-lookup"><span data-stu-id="1730f-136">healthState</span></span>|[<span data-ttu-id="1730f-137">healthState</span><span class="sxs-lookup"><span data-stu-id="1730f-137">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="1730f-138">Windows Management app Zustand.</span><span class="sxs-lookup"><span data-stu-id="1730f-138">Windows management app health state.</span></span> <span data-ttu-id="1730f-139">Mögliche Werte sind: `unknown`, `healthy` und `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="1730f-139">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="1730f-140">installedVersion</span><span class="sxs-lookup"><span data-stu-id="1730f-140">installedVersion</span></span>|<span data-ttu-id="1730f-141">String</span><span class="sxs-lookup"><span data-stu-id="1730f-141">String</span></span>|<span data-ttu-id="1730f-142">Windows Management-app-Version installiert.</span><span class="sxs-lookup"><span data-stu-id="1730f-142">Windows management app installed version.</span></span>|
|<span data-ttu-id="1730f-143">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="1730f-143">lastCheckInDateTime</span></span>|<span data-ttu-id="1730f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1730f-144">DateTimeOffset</span></span>|<span data-ttu-id="1730f-145">Windows Management app Einchecken zuletzt.</span><span class="sxs-lookup"><span data-stu-id="1730f-145">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="1730f-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="1730f-146">deviceName</span></span>|<span data-ttu-id="1730f-147">String</span><span class="sxs-lookup"><span data-stu-id="1730f-147">String</span></span>|<span data-ttu-id="1730f-148">Name des Geräts, auf dem Windows Management-app installiert ist.</span><span class="sxs-lookup"><span data-stu-id="1730f-148">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="1730f-149">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="1730f-149">deviceOSVersion</span></span>|<span data-ttu-id="1730f-150">String</span><span class="sxs-lookup"><span data-stu-id="1730f-150">String</span></span>|<span data-ttu-id="1730f-151">Windows 10 Betriebssystemversion des Geräts, auf dem Windows Management-app installiert ist.</span><span class="sxs-lookup"><span data-stu-id="1730f-151">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="1730f-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="1730f-152">Response</span></span>
<span data-ttu-id="1730f-153">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1730f-153">If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1730f-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1730f-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="1730f-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1730f-155">Request</span></span>
<span data-ttu-id="1730f-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1730f-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "healthState": "healthy",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```

### <a name="response"></a><span data-ttu-id="1730f-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="1730f-157">Response</span></span>
<span data-ttu-id="1730f-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1730f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "5c7e50fb-50fb-5c7e-fb50-7e5cfb507e5c",
  "healthState": "healthy",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```





