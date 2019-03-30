---
title: WindowsInformationProtectionDeviceRegistration erstellen
description: Erstellen eines neuen windowsInformationProtectionDeviceRegistration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f07481326f3766e8a9b1173fc07914bb301d6588
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985991"
---
# <a name="create-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="dec62-103">WindowsInformationProtectionDeviceRegistration erstellen</span><span class="sxs-lookup"><span data-stu-id="dec62-103">Create windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="dec62-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dec62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dec62-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="dec62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dec62-106">Erstellen eines neuen [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="dec62-106">Create a new [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dec62-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dec62-107">Prerequisites</span></span>
<span data-ttu-id="dec62-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dec62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dec62-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dec62-110">Permission type</span></span>|<span data-ttu-id="dec62-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dec62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dec62-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dec62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dec62-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dec62-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dec62-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dec62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dec62-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dec62-115">Not supported.</span></span>|
|<span data-ttu-id="dec62-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dec62-116">Application</span></span>|<span data-ttu-id="dec62-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dec62-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dec62-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dec62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="dec62-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dec62-119">Request headers</span></span>
|<span data-ttu-id="dec62-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dec62-120">Header</span></span>|<span data-ttu-id="dec62-121">Wert</span><span class="sxs-lookup"><span data-stu-id="dec62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dec62-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dec62-122">Authorization</span></span>|<span data-ttu-id="dec62-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dec62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dec62-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dec62-124">Accept</span></span>|<span data-ttu-id="dec62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dec62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dec62-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dec62-126">Request body</span></span>
<span data-ttu-id="dec62-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsInformationProtectionDeviceRegistration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="dec62-127">In the request body, supply a JSON representation for the windowsInformationProtectionDeviceRegistration object.</span></span>

<span data-ttu-id="dec62-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionDeviceRegistration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="dec62-128">The following table shows the properties that are required when you create the windowsInformationProtectionDeviceRegistration.</span></span>

|<span data-ttu-id="dec62-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dec62-129">Property</span></span>|<span data-ttu-id="dec62-130">Typ</span><span class="sxs-lookup"><span data-stu-id="dec62-130">Type</span></span>|<span data-ttu-id="dec62-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dec62-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dec62-132">id</span><span class="sxs-lookup"><span data-stu-id="dec62-132">id</span></span>|<span data-ttu-id="dec62-133">String</span><span class="sxs-lookup"><span data-stu-id="dec62-133">String</span></span>|<span data-ttu-id="dec62-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="dec62-134">Key of the entity.</span></span>|
|<span data-ttu-id="dec62-135">userId</span><span class="sxs-lookup"><span data-stu-id="dec62-135">userId</span></span>|<span data-ttu-id="dec62-136">String</span><span class="sxs-lookup"><span data-stu-id="dec62-136">String</span></span>|<span data-ttu-id="dec62-137">ID, die diesem Geräte Registrierungseintrag zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="dec62-137">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="dec62-138">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="dec62-138">deviceRegistrationId</span></span>|<span data-ttu-id="dec62-139">String</span><span class="sxs-lookup"><span data-stu-id="dec62-139">String</span></span>|<span data-ttu-id="dec62-140">Gerätebezeichner für diesen Geräte Registrierungseintrag.</span><span class="sxs-lookup"><span data-stu-id="dec62-140">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="dec62-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="dec62-141">deviceName</span></span>|<span data-ttu-id="dec62-142">String</span><span class="sxs-lookup"><span data-stu-id="dec62-142">String</span></span>|<span data-ttu-id="dec62-143">Name des Geräts</span><span class="sxs-lookup"><span data-stu-id="dec62-143">Device name.</span></span>|
|<span data-ttu-id="dec62-144">deviceType</span><span class="sxs-lookup"><span data-stu-id="dec62-144">deviceType</span></span>|<span data-ttu-id="dec62-145">String</span><span class="sxs-lookup"><span data-stu-id="dec62-145">String</span></span>|<span data-ttu-id="dec62-146">Gerätetyp, beispielsweise Windows Laptop und Windows phone.</span><span class="sxs-lookup"><span data-stu-id="dec62-146">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="dec62-147">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="dec62-147">deviceMacAddress</span></span>|<span data-ttu-id="dec62-148">String</span><span class="sxs-lookup"><span data-stu-id="dec62-148">String</span></span>|<span data-ttu-id="dec62-149">Mac-Adresse des Geräts.</span><span class="sxs-lookup"><span data-stu-id="dec62-149">Device Mac address.</span></span>|
|<span data-ttu-id="dec62-150">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="dec62-150">lastCheckInDateTime</span></span>|<span data-ttu-id="dec62-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dec62-151">DateTimeOffset</span></span>|<span data-ttu-id="dec62-152">Zeitpunkt des letzten Eincheckens des Geräts.</span><span class="sxs-lookup"><span data-stu-id="dec62-152">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="dec62-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="dec62-153">Response</span></span>
<span data-ttu-id="dec62-154">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dec62-154">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dec62-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dec62-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="dec62-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dec62-156">Request</span></span>
<span data-ttu-id="dec62-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dec62-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations
Content-type: application/json
Content-length: 366

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "userId": "User Id value",
  "deviceRegistrationId": "Device Registration Id value",
  "deviceName": "Device Name value",
  "deviceType": "Device Type value",
  "deviceMacAddress": "Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```

### <a name="response"></a><span data-ttu-id="dec62-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="dec62-158">Response</span></span>
<span data-ttu-id="dec62-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dec62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 415

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "id": "dd72e2c8-e2c8-dd72-c8e2-72ddc8e272dd",
  "userId": "User Id value",
  "deviceRegistrationId": "Device Registration Id value",
  "deviceName": "Device Name value",
  "deviceType": "Device Type value",
  "deviceMacAddress": "Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```




