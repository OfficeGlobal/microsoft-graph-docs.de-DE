---
title: ImportedDeviceIdentity erstellen
description: Erstellen eines neuen importedDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb0f95f2d459b1b1583b2bdf9cc18f40ff9e03d5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154670"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="f28dd-103">ImportedDeviceIdentity erstellen</span><span class="sxs-lookup"><span data-stu-id="f28dd-103">Create importedDeviceIdentity</span></span>

> <span data-ttu-id="f28dd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f28dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f28dd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f28dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f28dd-106">Erstellen eines neuen [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f28dd-106">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f28dd-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f28dd-107">Prerequisites</span></span>
<span data-ttu-id="f28dd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f28dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f28dd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f28dd-110">Permission type</span></span>|<span data-ttu-id="f28dd-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f28dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f28dd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f28dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f28dd-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f28dd-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f28dd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f28dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f28dd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f28dd-115">Not supported.</span></span>|
|<span data-ttu-id="f28dd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f28dd-116">Application</span></span>|<span data-ttu-id="f28dd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f28dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f28dd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f28dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="f28dd-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f28dd-119">Request headers</span></span>
|<span data-ttu-id="f28dd-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f28dd-120">Header</span></span>|<span data-ttu-id="f28dd-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f28dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f28dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f28dd-122">Authorization</span></span>|<span data-ttu-id="f28dd-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f28dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f28dd-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f28dd-124">Accept</span></span>|<span data-ttu-id="f28dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f28dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f28dd-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f28dd-126">Request body</span></span>
<span data-ttu-id="f28dd-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das importedDeviceIdentity-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="f28dd-127">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="f28dd-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der importedDeviceIdentity erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f28dd-128">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="f28dd-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f28dd-129">Property</span></span>|<span data-ttu-id="f28dd-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f28dd-130">Type</span></span>|<span data-ttu-id="f28dd-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f28dd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f28dd-132">id</span><span class="sxs-lookup"><span data-stu-id="f28dd-132">id</span></span>|<span data-ttu-id="f28dd-133">string</span><span class="sxs-lookup"><span data-stu-id="f28dd-133">String</span></span>|<span data-ttu-id="f28dd-134">ID der importierten Geräte Identität</span><span class="sxs-lookup"><span data-stu-id="f28dd-134">Id of the imported device identity</span></span>|
|<span data-ttu-id="f28dd-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f28dd-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="f28dd-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f28dd-136">String</span></span>|<span data-ttu-id="f28dd-137">Importierter Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="f28dd-137">Imported Device Identifier</span></span>|
|<span data-ttu-id="f28dd-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="f28dd-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="f28dd-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="f28dd-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="f28dd-140">Typ der importierten Geräte Identität.</span><span class="sxs-lookup"><span data-stu-id="f28dd-140">Type of Imported Device Identity.</span></span> <span data-ttu-id="f28dd-141">Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="f28dd-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="f28dd-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f28dd-142">lastModifiedDateTime</span></span>|<span data-ttu-id="f28dd-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f28dd-143">DateTimeOffset</span></span>|<span data-ttu-id="f28dd-144">Datum der letzten Änderung der Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f28dd-144">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="f28dd-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f28dd-145">createdDateTime</span></span>|<span data-ttu-id="f28dd-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f28dd-146">DateTimeOffset</span></span>|<span data-ttu-id="f28dd-147">ErstellungsDatum des Geräts</span><span class="sxs-lookup"><span data-stu-id="f28dd-147">Created Date Time of the device</span></span>|
|<span data-ttu-id="f28dd-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="f28dd-148">lastContactedDateTime</span></span>|<span data-ttu-id="f28dd-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f28dd-149">DateTimeOffset</span></span>|<span data-ttu-id="f28dd-150">Datum der letzten Kontaktaufnahme des Geräts</span><span class="sxs-lookup"><span data-stu-id="f28dd-150">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="f28dd-151">description</span><span class="sxs-lookup"><span data-stu-id="f28dd-151">description</span></span>|<span data-ttu-id="f28dd-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f28dd-152">String</span></span>|<span data-ttu-id="f28dd-153">Die Beschreibung des Geräts</span><span class="sxs-lookup"><span data-stu-id="f28dd-153">The description of the device</span></span>|
|<span data-ttu-id="f28dd-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="f28dd-154">enrollmentState</span></span>|[<span data-ttu-id="f28dd-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="f28dd-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="f28dd-156">Der Status des Geräts in InTune.</span><span class="sxs-lookup"><span data-stu-id="f28dd-156">The state of the device in Intune.</span></span> <span data-ttu-id="f28dd-157">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="f28dd-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="f28dd-158">Plattform</span><span class="sxs-lookup"><span data-stu-id="f28dd-158">platform</span></span>|[<span data-ttu-id="f28dd-159">Plattform</span><span class="sxs-lookup"><span data-stu-id="f28dd-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="f28dd-160">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="f28dd-160">The platform of the Device.</span></span> <span data-ttu-id="f28dd-161">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="f28dd-161">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="f28dd-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="f28dd-162">Response</span></span>
<span data-ttu-id="f28dd-163">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f28dd-163">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f28dd-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f28dd-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="f28dd-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f28dd-165">Request</span></span>
<span data-ttu-id="f28dd-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f28dd-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="f28dd-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="f28dd-167">Response</span></span>
<span data-ttu-id="f28dd-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f28dd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




