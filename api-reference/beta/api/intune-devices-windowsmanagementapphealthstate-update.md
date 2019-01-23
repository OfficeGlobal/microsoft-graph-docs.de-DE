---
title: WindowsManagementAppHealthState aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsManagementAppHealthState-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: de395bdeba104ea3c5c30b8f33e8670a5f2e5480
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423153"
---
# <a name="update-windowsmanagementapphealthstate"></a><span data-ttu-id="97d7a-103">WindowsManagementAppHealthState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="97d7a-103">Update windowsManagementAppHealthState</span></span>

> <span data-ttu-id="97d7a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="97d7a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="97d7a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="97d7a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97d7a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="97d7a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97d7a-107">Aktualisieren Sie die Eigenschaften eines [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="97d7a-107">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97d7a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="97d7a-108">Prerequisites</span></span>
<span data-ttu-id="97d7a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="97d7a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="97d7a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97d7a-111">Permission type</span></span>|<span data-ttu-id="97d7a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97d7a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97d7a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97d7a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97d7a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97d7a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="97d7a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97d7a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97d7a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97d7a-116">Not supported.</span></span>|
|<span data-ttu-id="97d7a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97d7a-117">Application</span></span>|<span data-ttu-id="97d7a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97d7a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97d7a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97d7a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a><span data-ttu-id="97d7a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97d7a-120">Request headers</span></span>
|<span data-ttu-id="97d7a-121">Header</span><span class="sxs-lookup"><span data-stu-id="97d7a-121">Header</span></span>|<span data-ttu-id="97d7a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="97d7a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97d7a-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="97d7a-123">Authorization</span></span>|<span data-ttu-id="97d7a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="97d7a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97d7a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="97d7a-125">Accept</span></span>|<span data-ttu-id="97d7a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97d7a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97d7a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97d7a-127">Request body</span></span>
<span data-ttu-id="97d7a-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="97d7a-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

<span data-ttu-id="97d7a-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="97d7a-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>

|<span data-ttu-id="97d7a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="97d7a-130">Property</span></span>|<span data-ttu-id="97d7a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="97d7a-131">Type</span></span>|<span data-ttu-id="97d7a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97d7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97d7a-133">id</span><span class="sxs-lookup"><span data-stu-id="97d7a-133">id</span></span>|<span data-ttu-id="97d7a-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97d7a-134">String</span></span>|<span data-ttu-id="97d7a-135">Eindeutiger Bezeichner für den Zustand des Windows Management-app</span><span class="sxs-lookup"><span data-stu-id="97d7a-135">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="97d7a-136">healthState</span><span class="sxs-lookup"><span data-stu-id="97d7a-136">healthState</span></span>|[<span data-ttu-id="97d7a-137">healthState</span><span class="sxs-lookup"><span data-stu-id="97d7a-137">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="97d7a-138">Windows Management app Zustand.</span><span class="sxs-lookup"><span data-stu-id="97d7a-138">Windows management app health state.</span></span> <span data-ttu-id="97d7a-139">Mögliche Werte sind: `unknown`, `healthy` und `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="97d7a-139">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="97d7a-140">installedVersion</span><span class="sxs-lookup"><span data-stu-id="97d7a-140">installedVersion</span></span>|<span data-ttu-id="97d7a-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97d7a-141">String</span></span>|<span data-ttu-id="97d7a-142">Windows Management-app-Version installiert.</span><span class="sxs-lookup"><span data-stu-id="97d7a-142">Windows management app installed version.</span></span>|
|<span data-ttu-id="97d7a-143">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="97d7a-143">lastCheckInDateTime</span></span>|<span data-ttu-id="97d7a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97d7a-144">DateTimeOffset</span></span>|<span data-ttu-id="97d7a-145">Windows Management app Einchecken zuletzt.</span><span class="sxs-lookup"><span data-stu-id="97d7a-145">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="97d7a-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="97d7a-146">deviceName</span></span>|<span data-ttu-id="97d7a-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97d7a-147">String</span></span>|<span data-ttu-id="97d7a-148">Name des Geräts, auf dem Windows Management-app installiert ist.</span><span class="sxs-lookup"><span data-stu-id="97d7a-148">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="97d7a-149">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="97d7a-149">deviceOSVersion</span></span>|<span data-ttu-id="97d7a-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97d7a-150">String</span></span>|<span data-ttu-id="97d7a-151">Windows 10 Betriebssystemversion des Geräts, auf dem Windows Management-app installiert ist.</span><span class="sxs-lookup"><span data-stu-id="97d7a-151">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="97d7a-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="97d7a-152">Response</span></span>
<span data-ttu-id="97d7a-153">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="97d7a-153">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97d7a-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97d7a-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="97d7a-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97d7a-155">Request</span></span>
<span data-ttu-id="97d7a-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97d7a-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
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

### <a name="response"></a><span data-ttu-id="97d7a-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="97d7a-157">Response</span></span>
<span data-ttu-id="97d7a-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97d7a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




