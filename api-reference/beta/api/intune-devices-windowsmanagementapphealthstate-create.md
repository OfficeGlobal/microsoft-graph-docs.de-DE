---
title: WindowsManagementAppHealthState erstellen
description: Erstellen eines neuen windowsManagementAppHealthState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f8bead779385d8599bdd91932fbf310767b2e35
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157729"
---
# <a name="create-windowsmanagementapphealthstate"></a><span data-ttu-id="23a1f-103">WindowsManagementAppHealthState erstellen</span><span class="sxs-lookup"><span data-stu-id="23a1f-103">Create windowsManagementAppHealthState</span></span>

> <span data-ttu-id="23a1f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23a1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23a1f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="23a1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23a1f-106">Erstellen eines neuen [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="23a1f-106">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23a1f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="23a1f-107">Prerequisites</span></span>
<span data-ttu-id="23a1f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="23a1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="23a1f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="23a1f-110">Permission type</span></span>|<span data-ttu-id="23a1f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="23a1f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23a1f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="23a1f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="23a1f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23a1f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="23a1f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="23a1f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23a1f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23a1f-115">Not supported.</span></span>|
|<span data-ttu-id="23a1f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="23a1f-116">Application</span></span>|<span data-ttu-id="23a1f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23a1f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23a1f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="23a1f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="23a1f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="23a1f-119">Request headers</span></span>
|<span data-ttu-id="23a1f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="23a1f-120">Header</span></span>|<span data-ttu-id="23a1f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="23a1f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23a1f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="23a1f-122">Authorization</span></span>|<span data-ttu-id="23a1f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="23a1f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23a1f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="23a1f-124">Accept</span></span>|<span data-ttu-id="23a1f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="23a1f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23a1f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="23a1f-126">Request body</span></span>
<span data-ttu-id="23a1f-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsManagementAppHealthState-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="23a1f-127">In the request body, supply a JSON representation for the windowsManagementAppHealthState object.</span></span>

<span data-ttu-id="23a1f-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsManagementAppHealthState erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="23a1f-128">The following table shows the properties that are required when you create the windowsManagementAppHealthState.</span></span>

|<span data-ttu-id="23a1f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23a1f-129">Property</span></span>|<span data-ttu-id="23a1f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="23a1f-130">Type</span></span>|<span data-ttu-id="23a1f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23a1f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23a1f-132">id</span><span class="sxs-lookup"><span data-stu-id="23a1f-132">id</span></span>|<span data-ttu-id="23a1f-133">String</span><span class="sxs-lookup"><span data-stu-id="23a1f-133">String</span></span>|<span data-ttu-id="23a1f-134">Eindeutiger Bezeichner für den Integritätsstatus der Windows-Verwaltungsanwendung</span><span class="sxs-lookup"><span data-stu-id="23a1f-134">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="23a1f-135">healthState</span><span class="sxs-lookup"><span data-stu-id="23a1f-135">healthState</span></span>|[<span data-ttu-id="23a1f-136">healthState</span><span class="sxs-lookup"><span data-stu-id="23a1f-136">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="23a1f-137">Integritätsstatus der Windows-Verwaltungsanwendung</span><span class="sxs-lookup"><span data-stu-id="23a1f-137">Windows management app health state.</span></span> <span data-ttu-id="23a1f-138">Mögliche Werte sind: `unknown`, `healthy` und `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="23a1f-138">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="23a1f-139">installedVersion</span><span class="sxs-lookup"><span data-stu-id="23a1f-139">installedVersion</span></span>|<span data-ttu-id="23a1f-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="23a1f-140">String</span></span>|<span data-ttu-id="23a1f-141">Installierte Version der Windows-Verwaltungs-app.</span><span class="sxs-lookup"><span data-stu-id="23a1f-141">Windows management app installed version.</span></span>|
|<span data-ttu-id="23a1f-142">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="23a1f-142">lastCheckInDateTime</span></span>|<span data-ttu-id="23a1f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23a1f-143">DateTimeOffset</span></span>|<span data-ttu-id="23a1f-144">Windows Management APP – letzter Eincheck Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="23a1f-144">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="23a1f-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="23a1f-145">deviceName</span></span>|<span data-ttu-id="23a1f-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="23a1f-146">String</span></span>|<span data-ttu-id="23a1f-147">Name des Geräts, auf dem die Windows-Verwaltungs-App installiert ist.</span><span class="sxs-lookup"><span data-stu-id="23a1f-147">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="23a1f-148">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="23a1f-148">deviceOSVersion</span></span>|<span data-ttu-id="23a1f-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="23a1f-149">String</span></span>|<span data-ttu-id="23a1f-150">Windows 10-Betriebssystemversion des Geräts, auf dem die Windows-Verwaltungs-App installiert ist.</span><span class="sxs-lookup"><span data-stu-id="23a1f-150">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="23a1f-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="23a1f-151">Response</span></span>
<span data-ttu-id="23a1f-152">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="23a1f-152">If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23a1f-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="23a1f-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="23a1f-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23a1f-154">Request</span></span>
<span data-ttu-id="23a1f-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="23a1f-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="23a1f-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="23a1f-156">Response</span></span>
<span data-ttu-id="23a1f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23a1f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




