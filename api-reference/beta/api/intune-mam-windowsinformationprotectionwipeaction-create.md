---
title: WindowsInformationProtectionWipeAction erstellen
description: Erstellen eines neuen windowsInformationProtectionWipeAction-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 26a90166c82843ccb0584b8d720f053fe6378844
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158849"
---
# <a name="create-windowsinformationprotectionwipeaction"></a><span data-ttu-id="c9b4e-103">WindowsInformationProtectionWipeAction erstellen</span><span class="sxs-lookup"><span data-stu-id="c9b4e-103">Create windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="c9b4e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9b4e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9b4e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c9b4e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9b4e-106">Erstellen eines neuen [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c9b4e-106">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9b4e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c9b4e-107">Prerequisites</span></span>
<span data-ttu-id="c9b4e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c9b4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c9b4e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c9b4e-110">Permission type</span></span>|<span data-ttu-id="c9b4e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c9b4e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9b4e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c9b4e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9b4e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9b4e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c9b4e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c9b4e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9b4e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9b4e-115">Not supported.</span></span>|
|<span data-ttu-id="c9b4e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c9b4e-116">Application</span></span>|<span data-ttu-id="c9b4e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9b4e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9b4e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9b4e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="c9b4e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c9b4e-119">Request headers</span></span>
|<span data-ttu-id="c9b4e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c9b4e-120">Header</span></span>|<span data-ttu-id="c9b4e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c9b4e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9b4e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9b4e-122">Authorization</span></span>|<span data-ttu-id="c9b4e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c9b4e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9b4e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c9b4e-124">Accept</span></span>|<span data-ttu-id="c9b4e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9b4e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9b4e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c9b4e-126">Request body</span></span>
<span data-ttu-id="c9b4e-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsInformationProtectionWipeAction-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c9b4e-127">In the request body, supply a JSON representation for the windowsInformationProtectionWipeAction object.</span></span>

<span data-ttu-id="c9b4e-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionWipeAction erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c9b4e-128">The following table shows the properties that are required when you create the windowsInformationProtectionWipeAction.</span></span>

|<span data-ttu-id="c9b4e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9b4e-129">Property</span></span>|<span data-ttu-id="c9b4e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c9b4e-130">Type</span></span>|<span data-ttu-id="c9b4e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9b4e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9b4e-132">id</span><span class="sxs-lookup"><span data-stu-id="c9b4e-132">id</span></span>|<span data-ttu-id="c9b4e-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9b4e-133">String</span></span>|<span data-ttu-id="c9b4e-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c9b4e-134">Key of the entity.</span></span>|
|<span data-ttu-id="c9b4e-135">status</span><span class="sxs-lookup"><span data-stu-id="c9b4e-135">status</span></span>|[<span data-ttu-id="c9b4e-136">actionState</span><span class="sxs-lookup"><span data-stu-id="c9b4e-136">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c9b4e-137">Aktionsstatus wischen.</span><span class="sxs-lookup"><span data-stu-id="c9b4e-137">Wipe action status.</span></span> <span data-ttu-id="c9b4e-138">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="c9b4e-138">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c9b4e-139">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="c9b4e-139">targetedUserId</span></span>|<span data-ttu-id="c9b4e-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9b4e-140">String</span></span>|<span data-ttu-id="c9b4e-141">Die UserId, die von dieser Löschaktion bestimmt wird.</span><span class="sxs-lookup"><span data-stu-id="c9b4e-141">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="c9b4e-142">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="c9b4e-142">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="c9b4e-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9b4e-143">String</span></span>|<span data-ttu-id="c9b4e-144">Die DeviceRegistrationId, die von dieser Löschaktion bestimmt wird.</span><span class="sxs-lookup"><span data-stu-id="c9b4e-144">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="c9b4e-145">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="c9b4e-145">targetedDeviceName</span></span>|<span data-ttu-id="c9b4e-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9b4e-146">String</span></span>|<span data-ttu-id="c9b4e-147">Name des Zielgeräts.</span><span class="sxs-lookup"><span data-stu-id="c9b4e-147">Targeted device name.</span></span>|
|<span data-ttu-id="c9b4e-148">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="c9b4e-148">targetedDeviceMacAddress</span></span>|<span data-ttu-id="c9b4e-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9b4e-149">String</span></span>|<span data-ttu-id="c9b4e-150">Mac-Adresse des Zielgeräts.</span><span class="sxs-lookup"><span data-stu-id="c9b4e-150">Targeted device Mac address.</span></span>|
|<span data-ttu-id="c9b4e-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="c9b4e-151">lastCheckInDateTime</span></span>|<span data-ttu-id="c9b4e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9b4e-152">DateTimeOffset</span></span>|<span data-ttu-id="c9b4e-153">Letzter Eincheck Zeitpunkt des Geräts, das von dieser Löschaktion bestimmt wurde.</span><span class="sxs-lookup"><span data-stu-id="c9b4e-153">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="c9b4e-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9b4e-154">Response</span></span>
<span data-ttu-id="c9b4e-155">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c9b4e-155">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9b4e-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c9b4e-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9b4e-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9b4e-157">Request</span></span>
<span data-ttu-id="c9b4e-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c9b4e-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions
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

### <a name="response"></a><span data-ttu-id="c9b4e-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9b4e-159">Response</span></span>
<span data-ttu-id="c9b4e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9b4e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




