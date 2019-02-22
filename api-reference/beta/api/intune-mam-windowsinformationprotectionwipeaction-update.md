---
title: WindowsInformationProtectionWipeAction aktualisieren
description: Aktualisieren der Eigenschaften eines windowsInformationProtectionWipeAction-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b198f1387cc3f0806cc6b76953948eca08d88cfc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159101"
---
# <a name="update-windowsinformationprotectionwipeaction"></a><span data-ttu-id="044c3-103">WindowsInformationProtectionWipeAction aktualisieren</span><span class="sxs-lookup"><span data-stu-id="044c3-103">Update windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="044c3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="044c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="044c3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="044c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="044c3-106">Aktualisieren der Eigenschaften eines [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="044c3-106">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="044c3-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="044c3-107">Prerequisites</span></span>
<span data-ttu-id="044c3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="044c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="044c3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="044c3-110">Permission type</span></span>|<span data-ttu-id="044c3-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="044c3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="044c3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="044c3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="044c3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="044c3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="044c3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="044c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="044c3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="044c3-115">Not supported.</span></span>|
|<span data-ttu-id="044c3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="044c3-116">Application</span></span>|<span data-ttu-id="044c3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="044c3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="044c3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="044c3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="request-headers"></a><span data-ttu-id="044c3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="044c3-119">Request headers</span></span>
|<span data-ttu-id="044c3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="044c3-120">Header</span></span>|<span data-ttu-id="044c3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="044c3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="044c3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="044c3-122">Authorization</span></span>|<span data-ttu-id="044c3-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="044c3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="044c3-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="044c3-124">Accept</span></span>|<span data-ttu-id="044c3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="044c3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="044c3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="044c3-126">Request body</span></span>
<span data-ttu-id="044c3-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="044c3-127">In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

<span data-ttu-id="044c3-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="044c3-128">The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>

|<span data-ttu-id="044c3-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="044c3-129">Property</span></span>|<span data-ttu-id="044c3-130">Typ</span><span class="sxs-lookup"><span data-stu-id="044c3-130">Type</span></span>|<span data-ttu-id="044c3-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="044c3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="044c3-132">id</span><span class="sxs-lookup"><span data-stu-id="044c3-132">id</span></span>|<span data-ttu-id="044c3-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="044c3-133">String</span></span>|<span data-ttu-id="044c3-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="044c3-134">Key of the entity.</span></span>|
|<span data-ttu-id="044c3-135">status</span><span class="sxs-lookup"><span data-stu-id="044c3-135">status</span></span>|[<span data-ttu-id="044c3-136">actionState</span><span class="sxs-lookup"><span data-stu-id="044c3-136">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="044c3-137">Aktionsstatus wischen.</span><span class="sxs-lookup"><span data-stu-id="044c3-137">Wipe action status.</span></span> <span data-ttu-id="044c3-138">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="044c3-138">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="044c3-139">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="044c3-139">targetedUserId</span></span>|<span data-ttu-id="044c3-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="044c3-140">String</span></span>|<span data-ttu-id="044c3-141">Die UserId, die von dieser Löschaktion bestimmt wird.</span><span class="sxs-lookup"><span data-stu-id="044c3-141">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="044c3-142">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="044c3-142">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="044c3-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="044c3-143">String</span></span>|<span data-ttu-id="044c3-144">Die DeviceRegistrationId, die von dieser Löschaktion bestimmt wird.</span><span class="sxs-lookup"><span data-stu-id="044c3-144">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="044c3-145">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="044c3-145">targetedDeviceName</span></span>|<span data-ttu-id="044c3-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="044c3-146">String</span></span>|<span data-ttu-id="044c3-147">Name des Zielgeräts.</span><span class="sxs-lookup"><span data-stu-id="044c3-147">Targeted device name.</span></span>|
|<span data-ttu-id="044c3-148">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="044c3-148">targetedDeviceMacAddress</span></span>|<span data-ttu-id="044c3-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="044c3-149">String</span></span>|<span data-ttu-id="044c3-150">Mac-Adresse des Zielgeräts.</span><span class="sxs-lookup"><span data-stu-id="044c3-150">Targeted device Mac address.</span></span>|
|<span data-ttu-id="044c3-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="044c3-151">lastCheckInDateTime</span></span>|<span data-ttu-id="044c3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="044c3-152">DateTimeOffset</span></span>|<span data-ttu-id="044c3-153">Letzter Eincheck Zeitpunkt des Geräts, das von dieser Löschaktion bestimmt wurde.</span><span class="sxs-lookup"><span data-stu-id="044c3-153">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="044c3-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="044c3-154">Response</span></span>
<span data-ttu-id="044c3-155">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="044c3-155">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="044c3-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="044c3-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="044c3-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="044c3-157">Request</span></span>
<span data-ttu-id="044c3-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="044c3-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
Content-type: application/json
Content-length: 412

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```

### <a name="response"></a><span data-ttu-id="044c3-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="044c3-159">Response</span></span>
<span data-ttu-id="044c3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="044c3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 461

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "2620a996-a996-2620-96a9-202696a92026",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```




