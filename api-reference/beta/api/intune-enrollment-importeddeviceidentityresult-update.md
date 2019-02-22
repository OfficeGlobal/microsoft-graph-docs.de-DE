---
title: ImportedDeviceIdentityResult aktualisieren
description: Aktualisieren der Eigenschaften eines importedDeviceIdentityResult-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dea1d8309507ae5eb5a969c710308bf2d779be15
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142966"
---
# <a name="update-importeddeviceidentityresult"></a><span data-ttu-id="fda35-103">ImportedDeviceIdentityResult aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fda35-103">Update importedDeviceIdentityResult</span></span>

> <span data-ttu-id="fda35-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fda35-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fda35-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fda35-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fda35-106">Aktualisieren der Eigenschaften eines [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fda35-106">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fda35-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fda35-107">Prerequisites</span></span>
<span data-ttu-id="fda35-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fda35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fda35-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fda35-110">Permission type</span></span>|<span data-ttu-id="fda35-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fda35-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fda35-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fda35-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fda35-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fda35-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fda35-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fda35-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fda35-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fda35-115">Not supported.</span></span>|
|<span data-ttu-id="fda35-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fda35-116">Application</span></span>|<span data-ttu-id="fda35-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fda35-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fda35-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fda35-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="fda35-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fda35-119">Request headers</span></span>
|<span data-ttu-id="fda35-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fda35-120">Header</span></span>|<span data-ttu-id="fda35-121">Wert</span><span class="sxs-lookup"><span data-stu-id="fda35-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fda35-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fda35-122">Authorization</span></span>|<span data-ttu-id="fda35-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fda35-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fda35-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fda35-124">Accept</span></span>|<span data-ttu-id="fda35-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fda35-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fda35-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fda35-126">Request body</span></span>
<span data-ttu-id="fda35-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="fda35-127">In the request body, supply a JSON representation for the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

<span data-ttu-id="fda35-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="fda35-128">The following table shows the properties that are required when you create the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>

|<span data-ttu-id="fda35-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fda35-129">Property</span></span>|<span data-ttu-id="fda35-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fda35-130">Type</span></span>|<span data-ttu-id="fda35-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fda35-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fda35-132">id</span><span class="sxs-lookup"><span data-stu-id="fda35-132">id</span></span>|<span data-ttu-id="fda35-133">string</span><span class="sxs-lookup"><span data-stu-id="fda35-133">String</span></span>|<span data-ttu-id="fda35-134">ID der von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten importierten Geräte Identität</span><span class="sxs-lookup"><span data-stu-id="fda35-134">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="fda35-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="fda35-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="fda35-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fda35-136">String</span></span>|<span data-ttu-id="fda35-137">Von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbte importierte Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="fda35-137">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="fda35-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="fda35-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="fda35-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="fda35-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="fda35-140">Typ der importierten Geräte Identität, die von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="fda35-140">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="fda35-141">Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="fda35-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="fda35-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fda35-142">lastModifiedDateTime</span></span>|<span data-ttu-id="fda35-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fda35-143">DateTimeOffset</span></span>|<span data-ttu-id="fda35-144">Datum der letzten Änderung der von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fda35-144">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="fda35-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fda35-145">createdDateTime</span></span>|<span data-ttu-id="fda35-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fda35-146">DateTimeOffset</span></span>|<span data-ttu-id="fda35-147">ErstellungsDatum des von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten Geräts</span><span class="sxs-lookup"><span data-stu-id="fda35-147">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="fda35-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="fda35-148">lastContactedDateTime</span></span>|<span data-ttu-id="fda35-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fda35-149">DateTimeOffset</span></span>|<span data-ttu-id="fda35-150">Datum der letzten Kontaktaufnahme des von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten Geräts</span><span class="sxs-lookup"><span data-stu-id="fda35-150">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="fda35-151">description</span><span class="sxs-lookup"><span data-stu-id="fda35-151">description</span></span>|<span data-ttu-id="fda35-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fda35-152">String</span></span>|<span data-ttu-id="fda35-153">Die Beschreibung des von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten Geräts</span><span class="sxs-lookup"><span data-stu-id="fda35-153">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="fda35-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="fda35-154">enrollmentState</span></span>|[<span data-ttu-id="fda35-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="fda35-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="fda35-156">Der Status des Geräts in InTune, das von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="fda35-156">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="fda35-157">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="fda35-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="fda35-158">Plattform</span><span class="sxs-lookup"><span data-stu-id="fda35-158">platform</span></span>|[<span data-ttu-id="fda35-159">Plattform</span><span class="sxs-lookup"><span data-stu-id="fda35-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="fda35-160">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="fda35-160">The platform of the Device.</span></span> <span data-ttu-id="fda35-161">Von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="fda35-161">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="fda35-162">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="fda35-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="fda35-163">status</span><span class="sxs-lookup"><span data-stu-id="fda35-163">status</span></span>|<span data-ttu-id="fda35-164">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fda35-164">Boolean</span></span>|<span data-ttu-id="fda35-165">Status der importierten Geräte Identität</span><span class="sxs-lookup"><span data-stu-id="fda35-165">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="fda35-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="fda35-166">Response</span></span>
<span data-ttu-id="fda35-167">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fda35-167">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fda35-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fda35-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="fda35-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fda35-169">Request</span></span>
<span data-ttu-id="fda35-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fda35-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="fda35-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="fda35-171">Response</span></span>
<span data-ttu-id="fda35-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fda35-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```




