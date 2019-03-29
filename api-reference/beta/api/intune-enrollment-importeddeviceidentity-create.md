---
title: ImportedDeviceIdentity erstellen
description: Erstellen eines neuen importedDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d91ebc37a348f86a83d0a17c3b2af1ab7f0292e6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977730"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="666c1-103">ImportedDeviceIdentity erstellen</span><span class="sxs-lookup"><span data-stu-id="666c1-103">Create importedDeviceIdentity</span></span>

> <span data-ttu-id="666c1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="666c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="666c1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="666c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="666c1-106">Erstellen eines neuen [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="666c1-106">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="666c1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="666c1-107">Prerequisites</span></span>
<span data-ttu-id="666c1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="666c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="666c1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="666c1-110">Permission type</span></span>|<span data-ttu-id="666c1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="666c1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="666c1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="666c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="666c1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="666c1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="666c1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="666c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="666c1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="666c1-115">Not supported.</span></span>|
|<span data-ttu-id="666c1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="666c1-116">Application</span></span>|<span data-ttu-id="666c1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="666c1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="666c1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="666c1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="666c1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="666c1-119">Request headers</span></span>
|<span data-ttu-id="666c1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="666c1-120">Header</span></span>|<span data-ttu-id="666c1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="666c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="666c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="666c1-122">Authorization</span></span>|<span data-ttu-id="666c1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="666c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="666c1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="666c1-124">Accept</span></span>|<span data-ttu-id="666c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="666c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="666c1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="666c1-126">Request body</span></span>
<span data-ttu-id="666c1-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das importedDeviceIdentity-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="666c1-127">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="666c1-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der importedDeviceIdentity erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="666c1-128">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="666c1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="666c1-129">Property</span></span>|<span data-ttu-id="666c1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="666c1-130">Type</span></span>|<span data-ttu-id="666c1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="666c1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="666c1-132">id</span><span class="sxs-lookup"><span data-stu-id="666c1-132">id</span></span>|<span data-ttu-id="666c1-133">String</span><span class="sxs-lookup"><span data-stu-id="666c1-133">String</span></span>|<span data-ttu-id="666c1-134">ID der importierten Geräte Identität</span><span class="sxs-lookup"><span data-stu-id="666c1-134">Id of the imported device identity</span></span>|
|<span data-ttu-id="666c1-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="666c1-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="666c1-136">String</span><span class="sxs-lookup"><span data-stu-id="666c1-136">String</span></span>|<span data-ttu-id="666c1-137">Importierter Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="666c1-137">Imported Device Identifier</span></span>|
|<span data-ttu-id="666c1-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="666c1-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="666c1-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="666c1-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="666c1-140">Typ der importierten Geräte Identität.</span><span class="sxs-lookup"><span data-stu-id="666c1-140">Type of Imported Device Identity.</span></span> <span data-ttu-id="666c1-141">Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="666c1-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="666c1-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="666c1-142">lastModifiedDateTime</span></span>|<span data-ttu-id="666c1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="666c1-143">DateTimeOffset</span></span>|<span data-ttu-id="666c1-144">Datum der letzten Änderung der Beschreibung</span><span class="sxs-lookup"><span data-stu-id="666c1-144">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="666c1-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="666c1-145">createdDateTime</span></span>|<span data-ttu-id="666c1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="666c1-146">DateTimeOffset</span></span>|<span data-ttu-id="666c1-147">ErstellungsDatum des Geräts</span><span class="sxs-lookup"><span data-stu-id="666c1-147">Created Date Time of the device</span></span>|
|<span data-ttu-id="666c1-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="666c1-148">lastContactedDateTime</span></span>|<span data-ttu-id="666c1-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="666c1-149">DateTimeOffset</span></span>|<span data-ttu-id="666c1-150">Datum der letzten Kontaktaufnahme des Geräts</span><span class="sxs-lookup"><span data-stu-id="666c1-150">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="666c1-151">description</span><span class="sxs-lookup"><span data-stu-id="666c1-151">description</span></span>|<span data-ttu-id="666c1-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="666c1-152">String</span></span>|<span data-ttu-id="666c1-153">Die Beschreibung des Geräts</span><span class="sxs-lookup"><span data-stu-id="666c1-153">The description of the device</span></span>|
|<span data-ttu-id="666c1-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="666c1-154">enrollmentState</span></span>|[<span data-ttu-id="666c1-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="666c1-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="666c1-156">Der Status des Geräts in InTune.</span><span class="sxs-lookup"><span data-stu-id="666c1-156">The state of the device in Intune.</span></span> <span data-ttu-id="666c1-157">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="666c1-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="666c1-158">Plattform</span><span class="sxs-lookup"><span data-stu-id="666c1-158">platform</span></span>|[<span data-ttu-id="666c1-159">Plattform</span><span class="sxs-lookup"><span data-stu-id="666c1-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="666c1-160">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="666c1-160">The platform of the Device.</span></span> <span data-ttu-id="666c1-161">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="666c1-161">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="666c1-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="666c1-162">Response</span></span>
<span data-ttu-id="666c1-163">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="666c1-163">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="666c1-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="666c1-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="666c1-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="666c1-165">Request</span></span>
<span data-ttu-id="666c1-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="666c1-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="666c1-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="666c1-167">Response</span></span>
<span data-ttu-id="666c1-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="666c1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




