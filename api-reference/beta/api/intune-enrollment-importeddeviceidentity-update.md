---
title: ImportedDeviceIdentity aktualisieren
description: Aktualisieren der Eigenschaften eines importedDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4bf9585dca2df364d20a9bdbf26dd78a2e1e01d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173710"
---
# <a name="update-importeddeviceidentity"></a><span data-ttu-id="aac87-103">ImportedDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="aac87-103">Update importedDeviceIdentity</span></span>

> <span data-ttu-id="aac87-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aac87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aac87-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="aac87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aac87-106">Aktualisieren der Eigenschaften eines [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="aac87-106">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aac87-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="aac87-107">Prerequisites</span></span>
<span data-ttu-id="aac87-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="aac87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aac87-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aac87-110">Permission type</span></span>|<span data-ttu-id="aac87-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aac87-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aac87-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aac87-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aac87-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac87-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="aac87-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aac87-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aac87-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aac87-115">Not supported.</span></span>|
|<span data-ttu-id="aac87-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aac87-116">Application</span></span>|<span data-ttu-id="aac87-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aac87-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aac87-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aac87-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="aac87-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aac87-119">Request headers</span></span>
|<span data-ttu-id="aac87-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="aac87-120">Header</span></span>|<span data-ttu-id="aac87-121">Wert</span><span class="sxs-lookup"><span data-stu-id="aac87-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aac87-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aac87-122">Authorization</span></span>|<span data-ttu-id="aac87-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="aac87-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aac87-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="aac87-124">Accept</span></span>|<span data-ttu-id="aac87-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aac87-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aac87-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aac87-126">Request body</span></span>
<span data-ttu-id="aac87-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="aac87-127">In the request body, supply a JSON representation for the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

<span data-ttu-id="aac87-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="aac87-128">The following table shows the properties that are required when you create the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>

|<span data-ttu-id="aac87-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aac87-129">Property</span></span>|<span data-ttu-id="aac87-130">Typ</span><span class="sxs-lookup"><span data-stu-id="aac87-130">Type</span></span>|<span data-ttu-id="aac87-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aac87-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aac87-132">id</span><span class="sxs-lookup"><span data-stu-id="aac87-132">id</span></span>|<span data-ttu-id="aac87-133">string</span><span class="sxs-lookup"><span data-stu-id="aac87-133">String</span></span>|<span data-ttu-id="aac87-134">ID der importierten Geräte Identität</span><span class="sxs-lookup"><span data-stu-id="aac87-134">Id of the imported device identity</span></span>|
|<span data-ttu-id="aac87-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="aac87-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="aac87-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aac87-136">String</span></span>|<span data-ttu-id="aac87-137">Importierter Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="aac87-137">Imported Device Identifier</span></span>|
|<span data-ttu-id="aac87-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="aac87-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="aac87-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="aac87-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="aac87-140">Typ der importierten Geräte Identität.</span><span class="sxs-lookup"><span data-stu-id="aac87-140">Type of Imported Device Identity.</span></span> <span data-ttu-id="aac87-141">Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="aac87-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="aac87-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aac87-142">lastModifiedDateTime</span></span>|<span data-ttu-id="aac87-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aac87-143">DateTimeOffset</span></span>|<span data-ttu-id="aac87-144">Datum der letzten Änderung der Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aac87-144">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="aac87-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aac87-145">createdDateTime</span></span>|<span data-ttu-id="aac87-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aac87-146">DateTimeOffset</span></span>|<span data-ttu-id="aac87-147">ErstellungsDatum des Geräts</span><span class="sxs-lookup"><span data-stu-id="aac87-147">Created Date Time of the device</span></span>|
|<span data-ttu-id="aac87-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="aac87-148">lastContactedDateTime</span></span>|<span data-ttu-id="aac87-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aac87-149">DateTimeOffset</span></span>|<span data-ttu-id="aac87-150">Datum der letzten Kontaktaufnahme des Geräts</span><span class="sxs-lookup"><span data-stu-id="aac87-150">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="aac87-151">description</span><span class="sxs-lookup"><span data-stu-id="aac87-151">description</span></span>|<span data-ttu-id="aac87-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aac87-152">String</span></span>|<span data-ttu-id="aac87-153">Die Beschreibung des Geräts</span><span class="sxs-lookup"><span data-stu-id="aac87-153">The description of the device</span></span>|
|<span data-ttu-id="aac87-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="aac87-154">enrollmentState</span></span>|[<span data-ttu-id="aac87-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="aac87-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="aac87-156">Der Status des Geräts in InTune.</span><span class="sxs-lookup"><span data-stu-id="aac87-156">The state of the device in Intune.</span></span> <span data-ttu-id="aac87-157">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="aac87-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="aac87-158">Plattform</span><span class="sxs-lookup"><span data-stu-id="aac87-158">platform</span></span>|[<span data-ttu-id="aac87-159">Plattform</span><span class="sxs-lookup"><span data-stu-id="aac87-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="aac87-160">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="aac87-160">The platform of the Device.</span></span> <span data-ttu-id="aac87-161">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="aac87-161">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="aac87-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="aac87-162">Response</span></span>
<span data-ttu-id="aac87-163">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="aac87-163">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aac87-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aac87-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="aac87-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aac87-165">Request</span></span>
<span data-ttu-id="aac87-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aac87-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 332

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="aac87-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="aac87-167">Response</span></span>
<span data-ttu-id="aac87-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aac87-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```




