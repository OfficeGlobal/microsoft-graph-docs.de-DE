---
title: WindowsInformationProtectionDeviceRegistration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsInformationProtectionDeviceRegistration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0c84f81dd8d9df54c6f05b1435ee4644a1a75342
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430072"
---
# <a name="update-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="f017f-103">WindowsInformationProtectionDeviceRegistration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f017f-103">Update windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="f017f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f017f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f017f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f017f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f017f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f017f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f017f-107">Aktualisieren Sie die Eigenschaften eines [WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f017f-107">Update the properties of a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f017f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f017f-108">Prerequisites</span></span>
<span data-ttu-id="f017f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f017f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f017f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f017f-111">Permission type</span></span>|<span data-ttu-id="f017f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f017f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f017f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f017f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f017f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f017f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f017f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f017f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f017f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f017f-116">Not supported.</span></span>|
|<span data-ttu-id="f017f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f017f-117">Application</span></span>|<span data-ttu-id="f017f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f017f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f017f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f017f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="f017f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f017f-120">Request headers</span></span>
|<span data-ttu-id="f017f-121">Header</span><span class="sxs-lookup"><span data-stu-id="f017f-121">Header</span></span>|<span data-ttu-id="f017f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f017f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f017f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f017f-123">Authorization</span></span>|<span data-ttu-id="f017f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f017f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f017f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f017f-125">Accept</span></span>|<span data-ttu-id="f017f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f017f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f017f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f017f-127">Request body</span></span>
<span data-ttu-id="f017f-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f017f-128">In the request body, supply a JSON representation for the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

<span data-ttu-id="f017f-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="f017f-129">The following table shows the properties that are required when you create the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span></span>

|<span data-ttu-id="f017f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f017f-130">Property</span></span>|<span data-ttu-id="f017f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f017f-131">Type</span></span>|<span data-ttu-id="f017f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f017f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f017f-133">id</span><span class="sxs-lookup"><span data-stu-id="f017f-133">id</span></span>|<span data-ttu-id="f017f-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f017f-134">String</span></span>|<span data-ttu-id="f017f-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f017f-135">Key of the entity.</span></span>|
|<span data-ttu-id="f017f-136">userId</span><span class="sxs-lookup"><span data-stu-id="f017f-136">userId</span></span>|<span data-ttu-id="f017f-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f017f-137">String</span></span>|<span data-ttu-id="f017f-138">Benutzer-ID dieses Gerät registrierungsdatensatzes zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="f017f-138">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="f017f-139">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="f017f-139">deviceRegistrationId</span></span>|<span data-ttu-id="f017f-140">String</span><span class="sxs-lookup"><span data-stu-id="f017f-140">String</span></span>|<span data-ttu-id="f017f-141">Geräte-ID für dieses Gerät registrierungsdatensatzes.</span><span class="sxs-lookup"><span data-stu-id="f017f-141">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="f017f-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="f017f-142">deviceName</span></span>|<span data-ttu-id="f017f-143">String</span><span class="sxs-lookup"><span data-stu-id="f017f-143">String</span></span>|<span data-ttu-id="f017f-144">Name des Geräts</span><span class="sxs-lookup"><span data-stu-id="f017f-144">Device name.</span></span>|
|<span data-ttu-id="f017f-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="f017f-145">deviceType</span></span>|<span data-ttu-id="f017f-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f017f-146">String</span></span>|<span data-ttu-id="f017f-147">Gerätetyp, beispielsweise Windows Laptop VS Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f017f-147">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="f017f-148">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="f017f-148">deviceMacAddress</span></span>|<span data-ttu-id="f017f-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f017f-149">String</span></span>|<span data-ttu-id="f017f-150">Mac-Adresse des Geräts.</span><span class="sxs-lookup"><span data-stu-id="f017f-150">Device Mac address.</span></span>|
|<span data-ttu-id="f017f-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="f017f-151">lastCheckInDateTime</span></span>|<span data-ttu-id="f017f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f017f-152">DateTimeOffset</span></span>|<span data-ttu-id="f017f-153">Zeitpunkt der letzten Einchecken des Geräts.</span><span class="sxs-lookup"><span data-stu-id="f017f-153">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="f017f-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="f017f-154">Response</span></span>
<span data-ttu-id="f017f-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f017f-155">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f017f-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f017f-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="f017f-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f017f-157">Request</span></span>
<span data-ttu-id="f017f-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f017f-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
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

### <a name="response"></a><span data-ttu-id="f017f-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="f017f-159">Response</span></span>
<span data-ttu-id="f017f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f017f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




