---
title: WindowsManagementAppHealthState aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsManagementAppHealthState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b52762bf13a7ff534c3c76b8b0c94561744b15fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924230"
---
# <a name="update-windowsmanagementapphealthstate"></a><span data-ttu-id="f8100-103">WindowsManagementAppHealthState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f8100-103">Update windowsManagementAppHealthState</span></span>

> <span data-ttu-id="f8100-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f8100-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8100-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8100-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8100-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f8100-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8100-107">Aktualisieren Sie die Eigenschaften eines [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f8100-107">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8100-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f8100-108">Prerequisites</span></span>
<span data-ttu-id="f8100-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8100-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8100-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8100-111">Permission type</span></span>|<span data-ttu-id="f8100-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8100-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8100-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8100-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8100-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8100-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f8100-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8100-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8100-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8100-116">Not supported.</span></span>|
|<span data-ttu-id="f8100-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8100-117">Application</span></span>|<span data-ttu-id="f8100-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8100-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8100-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8100-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a><span data-ttu-id="f8100-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f8100-120">Request headers</span></span>
|<span data-ttu-id="f8100-121">Header</span><span class="sxs-lookup"><span data-stu-id="f8100-121">Header</span></span>|<span data-ttu-id="f8100-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f8100-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8100-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8100-123">Authorization</span></span>|<span data-ttu-id="f8100-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f8100-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8100-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f8100-125">Accept</span></span>|<span data-ttu-id="f8100-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8100-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8100-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f8100-127">Request body</span></span>
<span data-ttu-id="f8100-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f8100-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

<span data-ttu-id="f8100-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="f8100-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>

|<span data-ttu-id="f8100-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8100-130">Property</span></span>|<span data-ttu-id="f8100-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f8100-131">Type</span></span>|<span data-ttu-id="f8100-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8100-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8100-133">id</span><span class="sxs-lookup"><span data-stu-id="f8100-133">id</span></span>|<span data-ttu-id="f8100-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8100-134">String</span></span>|<span data-ttu-id="f8100-135">Eindeutiger Bezeichner für den Zustand des Windows Management-app</span><span class="sxs-lookup"><span data-stu-id="f8100-135">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="f8100-136">healthState</span><span class="sxs-lookup"><span data-stu-id="f8100-136">healthState</span></span>|[<span data-ttu-id="f8100-137">healthState</span><span class="sxs-lookup"><span data-stu-id="f8100-137">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="f8100-138">Windows Management app Zustand.</span><span class="sxs-lookup"><span data-stu-id="f8100-138">Windows management app health state.</span></span> <span data-ttu-id="f8100-139">Mögliche Werte sind: `unknown`, `healthy` und `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="f8100-139">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="f8100-140">installedVersion</span><span class="sxs-lookup"><span data-stu-id="f8100-140">installedVersion</span></span>|<span data-ttu-id="f8100-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8100-141">String</span></span>|<span data-ttu-id="f8100-142">Windows Management-app-Version installiert.</span><span class="sxs-lookup"><span data-stu-id="f8100-142">Windows management app installed version.</span></span>|
|<span data-ttu-id="f8100-143">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="f8100-143">lastCheckInDateTime</span></span>|<span data-ttu-id="f8100-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8100-144">DateTimeOffset</span></span>|<span data-ttu-id="f8100-145">Windows Management app Einchecken zuletzt.</span><span class="sxs-lookup"><span data-stu-id="f8100-145">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="f8100-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="f8100-146">deviceName</span></span>|<span data-ttu-id="f8100-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8100-147">String</span></span>|<span data-ttu-id="f8100-148">Name des Geräts, auf dem Windows Management-app installiert ist.</span><span class="sxs-lookup"><span data-stu-id="f8100-148">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="f8100-149">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="f8100-149">deviceOSVersion</span></span>|<span data-ttu-id="f8100-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8100-150">String</span></span>|<span data-ttu-id="f8100-151">Windows 10 Betriebssystemversion des Geräts, auf dem Windows Management-app installiert ist.</span><span class="sxs-lookup"><span data-stu-id="f8100-151">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="f8100-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8100-152">Response</span></span>
<span data-ttu-id="f8100-153">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f8100-153">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8100-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f8100-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8100-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8100-155">Request</span></span>
<span data-ttu-id="f8100-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f8100-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
Content-type: application/json
Content-length: 230

{
  "healthState": "healthy",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```

### <a name="response"></a><span data-ttu-id="f8100-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8100-157">Response</span></span>
<span data-ttu-id="f8100-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8100-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





