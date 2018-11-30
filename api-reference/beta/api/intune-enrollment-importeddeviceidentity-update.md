---
title: ImportedDeviceIdentity aktualisieren
description: Aktualisieren Sie die Eigenschaften eines ImportedDeviceIdentity-Objekts.
ms.openlocfilehash: 4c5ce8e592f04cbda5d5ffbbde0e38bbf7ee3602
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061083"
---
# <a name="update-importeddeviceidentity"></a><span data-ttu-id="12fa6-103">ImportedDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="12fa6-103">Update importedDeviceIdentity</span></span>

> <span data-ttu-id="12fa6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="12fa6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12fa6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12fa6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12fa6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="12fa6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12fa6-107">Aktualisieren Sie die Eigenschaften eines [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="12fa6-107">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12fa6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="12fa6-108">Prerequisites</span></span>
<span data-ttu-id="12fa6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12fa6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12fa6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="12fa6-111">Permission type</span></span>|<span data-ttu-id="12fa6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="12fa6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12fa6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="12fa6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12fa6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12fa6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="12fa6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="12fa6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12fa6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12fa6-116">Not supported.</span></span>|
|<span data-ttu-id="12fa6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="12fa6-117">Application</span></span>|<span data-ttu-id="12fa6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12fa6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12fa6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="12fa6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="12fa6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="12fa6-120">Request headers</span></span>
|<span data-ttu-id="12fa6-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="12fa6-121">Header</span></span>|<span data-ttu-id="12fa6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="12fa6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12fa6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12fa6-123">Authorization</span></span>|<span data-ttu-id="12fa6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="12fa6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12fa6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="12fa6-125">Accept</span></span>|<span data-ttu-id="12fa6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12fa6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12fa6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="12fa6-127">Request body</span></span>
<span data-ttu-id="12fa6-128">Geben Sie im Textkörper Anforderung für das Objekt [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="12fa6-128">In the request body, supply a JSON representation for the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

<span data-ttu-id="12fa6-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="12fa6-129">The following table shows the properties that are required when you create the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>

|<span data-ttu-id="12fa6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="12fa6-130">Property</span></span>|<span data-ttu-id="12fa6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="12fa6-131">Type</span></span>|<span data-ttu-id="12fa6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12fa6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12fa6-133">id</span><span class="sxs-lookup"><span data-stu-id="12fa6-133">id</span></span>|<span data-ttu-id="12fa6-134">String</span><span class="sxs-lookup"><span data-stu-id="12fa6-134">String</span></span>|<span data-ttu-id="12fa6-135">ID der Identität des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="12fa6-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="12fa6-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="12fa6-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="12fa6-137">String</span><span class="sxs-lookup"><span data-stu-id="12fa6-137">String</span></span>|<span data-ttu-id="12fa6-138">Importierte Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="12fa6-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="12fa6-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="12fa6-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="12fa6-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="12fa6-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="12fa6-141">Art der importierten Gerät Identität.</span><span class="sxs-lookup"><span data-stu-id="12fa6-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="12fa6-142">Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="12fa6-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="12fa6-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12fa6-143">lastModifiedDateTime</span></span>|<span data-ttu-id="12fa6-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12fa6-144">DateTimeOffset</span></span>|<span data-ttu-id="12fa6-145">Letzte Änderung DateTime der Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12fa6-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="12fa6-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12fa6-146">createdDateTime</span></span>|<span data-ttu-id="12fa6-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12fa6-147">DateTimeOffset</span></span>|<span data-ttu-id="12fa6-148">Erstellte Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="12fa6-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="12fa6-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="12fa6-149">lastContactedDateTime</span></span>|<span data-ttu-id="12fa6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12fa6-150">DateTimeOffset</span></span>|<span data-ttu-id="12fa6-151">Letzte kontaktiert Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="12fa6-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="12fa6-152">description</span><span class="sxs-lookup"><span data-stu-id="12fa6-152">description</span></span>|<span data-ttu-id="12fa6-153">String</span><span class="sxs-lookup"><span data-stu-id="12fa6-153">String</span></span>|<span data-ttu-id="12fa6-154">Die Beschreibung des Geräts</span><span class="sxs-lookup"><span data-stu-id="12fa6-154">The description of the device</span></span>|
|<span data-ttu-id="12fa6-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="12fa6-155">enrollmentState</span></span>|[<span data-ttu-id="12fa6-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="12fa6-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="12fa6-157">Der Zustand des Geräts in Intune.</span><span class="sxs-lookup"><span data-stu-id="12fa6-157">The state of the device in Intune.</span></span> <span data-ttu-id="12fa6-158">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="12fa6-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="12fa6-159">Plattform</span><span class="sxs-lookup"><span data-stu-id="12fa6-159">platform</span></span>|[<span data-ttu-id="12fa6-160">Plattform</span><span class="sxs-lookup"><span data-stu-id="12fa6-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="12fa6-161">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="12fa6-161">The platform of the Device.</span></span> <span data-ttu-id="12fa6-162">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="12fa6-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="12fa6-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="12fa6-163">Response</span></span>
<span data-ttu-id="12fa6-164">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="12fa6-164">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12fa6-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="12fa6-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="12fa6-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12fa6-166">Request</span></span>
<span data-ttu-id="12fa6-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="12fa6-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 335

{
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="12fa6-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="12fa6-168">Response</span></span>
<span data-ttu-id="12fa6-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





