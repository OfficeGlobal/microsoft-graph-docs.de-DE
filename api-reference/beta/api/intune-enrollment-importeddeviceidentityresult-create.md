---
title: ImportedDeviceIdentityResult erstellen
description: Erstellen eines neuen importedDeviceIdentityResult-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa58ab82f0e86b9ad83b0fd1759886ae3ddfda09
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965886"
---
# <a name="create-importeddeviceidentityresult"></a><span data-ttu-id="b0edc-103">ImportedDeviceIdentityResult erstellen</span><span class="sxs-lookup"><span data-stu-id="b0edc-103">Create importedDeviceIdentityResult</span></span>

> <span data-ttu-id="b0edc-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b0edc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0edc-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b0edc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0edc-106">Erstellen eines neuen [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b0edc-106">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0edc-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b0edc-107">Prerequisites</span></span>
<span data-ttu-id="b0edc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0edc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0edc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b0edc-110">Permission type</span></span>|<span data-ttu-id="b0edc-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b0edc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0edc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b0edc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0edc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0edc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b0edc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b0edc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0edc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b0edc-115">Not supported.</span></span>|
|<span data-ttu-id="b0edc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b0edc-116">Application</span></span>|<span data-ttu-id="b0edc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b0edc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0edc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0edc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="b0edc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b0edc-119">Request headers</span></span>
|<span data-ttu-id="b0edc-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b0edc-120">Header</span></span>|<span data-ttu-id="b0edc-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b0edc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0edc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0edc-122">Authorization</span></span>|<span data-ttu-id="b0edc-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b0edc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0edc-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b0edc-124">Accept</span></span>|<span data-ttu-id="b0edc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b0edc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0edc-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b0edc-126">Request body</span></span>
<span data-ttu-id="b0edc-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das importedDeviceIdentityResult-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b0edc-127">In the request body, supply a JSON representation for the importedDeviceIdentityResult object.</span></span>

<span data-ttu-id="b0edc-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der importedDeviceIdentityResult erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b0edc-128">The following table shows the properties that are required when you create the importedDeviceIdentityResult.</span></span>

|<span data-ttu-id="b0edc-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b0edc-129">Property</span></span>|<span data-ttu-id="b0edc-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b0edc-130">Type</span></span>|<span data-ttu-id="b0edc-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0edc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0edc-132">id</span><span class="sxs-lookup"><span data-stu-id="b0edc-132">id</span></span>|<span data-ttu-id="b0edc-133">String</span><span class="sxs-lookup"><span data-stu-id="b0edc-133">String</span></span>|<span data-ttu-id="b0edc-134">ID der von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten importierten Geräte Identität</span><span class="sxs-lookup"><span data-stu-id="b0edc-134">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="b0edc-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b0edc-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="b0edc-136">String</span><span class="sxs-lookup"><span data-stu-id="b0edc-136">String</span></span>|<span data-ttu-id="b0edc-137">Von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbte importierte Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="b0edc-137">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="b0edc-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="b0edc-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="b0edc-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="b0edc-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="b0edc-140">Typ der importierten Geräte Identität, die von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="b0edc-140">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="b0edc-141">Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="b0edc-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="b0edc-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0edc-142">lastModifiedDateTime</span></span>|<span data-ttu-id="b0edc-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0edc-143">DateTimeOffset</span></span>|<span data-ttu-id="b0edc-144">Datum der letzten Änderung der von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0edc-144">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="b0edc-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0edc-145">createdDateTime</span></span>|<span data-ttu-id="b0edc-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0edc-146">DateTimeOffset</span></span>|<span data-ttu-id="b0edc-147">ErstellungsDatum des von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten Geräts</span><span class="sxs-lookup"><span data-stu-id="b0edc-147">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="b0edc-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0edc-148">lastContactedDateTime</span></span>|<span data-ttu-id="b0edc-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0edc-149">DateTimeOffset</span></span>|<span data-ttu-id="b0edc-150">Datum der letzten Kontaktaufnahme des von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten Geräts</span><span class="sxs-lookup"><span data-stu-id="b0edc-150">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="b0edc-151">description</span><span class="sxs-lookup"><span data-stu-id="b0edc-151">description</span></span>|<span data-ttu-id="b0edc-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0edc-152">String</span></span>|<span data-ttu-id="b0edc-153">Die Beschreibung des von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten Geräts</span><span class="sxs-lookup"><span data-stu-id="b0edc-153">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="b0edc-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="b0edc-154">enrollmentState</span></span>|[<span data-ttu-id="b0edc-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="b0edc-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="b0edc-156">Der Status des Geräts in InTune, das von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="b0edc-156">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="b0edc-157">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="b0edc-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="b0edc-158">Plattform</span><span class="sxs-lookup"><span data-stu-id="b0edc-158">platform</span></span>|[<span data-ttu-id="b0edc-159">Plattform</span><span class="sxs-lookup"><span data-stu-id="b0edc-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="b0edc-160">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="b0edc-160">The platform of the Device.</span></span> <span data-ttu-id="b0edc-161">Von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="b0edc-161">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="b0edc-162">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="b0edc-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="b0edc-163">status</span><span class="sxs-lookup"><span data-stu-id="b0edc-163">status</span></span>|<span data-ttu-id="b0edc-164">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b0edc-164">Boolean</span></span>|<span data-ttu-id="b0edc-165">Status der importierten Geräte Identität</span><span class="sxs-lookup"><span data-stu-id="b0edc-165">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="b0edc-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0edc-166">Response</span></span>
<span data-ttu-id="b0edc-167">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b0edc-167">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0edc-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b0edc-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0edc-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0edc-169">Request</span></span>
<span data-ttu-id="b0edc-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b0edc-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="b0edc-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0edc-171">Response</span></span>
<span data-ttu-id="b0edc-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b0edc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




