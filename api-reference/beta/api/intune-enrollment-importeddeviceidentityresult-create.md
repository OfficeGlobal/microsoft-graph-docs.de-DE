---
title: Erstellen von importedDeviceIdentityResult
description: Erstellen eines neuen ImportedDeviceIdentityResult-Objekts.
ms.openlocfilehash: 4dec2ac709274dd30e3412a299bb1b561c9514b7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065091"
---
# <a name="create-importeddeviceidentityresult"></a><span data-ttu-id="2879e-103">Erstellen von importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="2879e-103">Create importedDeviceIdentityResult</span></span>

> <span data-ttu-id="2879e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2879e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2879e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2879e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2879e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2879e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2879e-107">Erstellen eines neuen [ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2879e-107">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2879e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2879e-108">Prerequisites</span></span>
<span data-ttu-id="2879e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2879e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2879e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2879e-111">Permission type</span></span>|<span data-ttu-id="2879e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2879e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2879e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2879e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2879e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2879e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2879e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2879e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2879e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2879e-116">Not supported.</span></span>|
|<span data-ttu-id="2879e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2879e-117">Application</span></span>|<span data-ttu-id="2879e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2879e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2879e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2879e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="2879e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2879e-120">Request headers</span></span>
|<span data-ttu-id="2879e-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2879e-121">Header</span></span>|<span data-ttu-id="2879e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2879e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2879e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2879e-123">Authorization</span></span>|<span data-ttu-id="2879e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2879e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2879e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2879e-125">Accept</span></span>|<span data-ttu-id="2879e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2879e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2879e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2879e-127">Request body</span></span>
<span data-ttu-id="2879e-128">Geben Sie im Textkörper Anforderung für das Objekt ImportedDeviceIdentityResult eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="2879e-128">In the request body, supply a JSON representation for the importedDeviceIdentityResult object.</span></span>

<span data-ttu-id="2879e-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die ImportedDeviceIdentityResult erstellen.</span><span class="sxs-lookup"><span data-stu-id="2879e-129">The following table shows the properties that are required when you create the importedDeviceIdentityResult.</span></span>

|<span data-ttu-id="2879e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2879e-130">Property</span></span>|<span data-ttu-id="2879e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2879e-131">Type</span></span>|<span data-ttu-id="2879e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2879e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2879e-133">id</span><span class="sxs-lookup"><span data-stu-id="2879e-133">id</span></span>|<span data-ttu-id="2879e-134">String</span><span class="sxs-lookup"><span data-stu-id="2879e-134">String</span></span>|<span data-ttu-id="2879e-135">ID der importierten Gerät Identität Inherited aus [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="2879e-135">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="2879e-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="2879e-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="2879e-137">String</span><span class="sxs-lookup"><span data-stu-id="2879e-137">String</span></span>|<span data-ttu-id="2879e-138">Importierte Geräte-ID geerbt von [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="2879e-138">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="2879e-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="2879e-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="2879e-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="2879e-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="2879e-141">Typ des importiert Gerät Identität geerbt von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="2879e-141">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="2879e-142">Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="2879e-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="2879e-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2879e-143">lastModifiedDateTime</span></span>|<span data-ttu-id="2879e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2879e-144">DateTimeOffset</span></span>|<span data-ttu-id="2879e-145">Letzte Änderung DateTime der Beschreibung Inherited aus [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="2879e-145">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="2879e-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2879e-146">createdDateTime</span></span>|<span data-ttu-id="2879e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2879e-147">DateTimeOffset</span></span>|<span data-ttu-id="2879e-148">Datum-Uhrzeit des Geräts Inherited aus [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) erstellt</span><span class="sxs-lookup"><span data-stu-id="2879e-148">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="2879e-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="2879e-149">lastContactedDateTime</span></span>|<span data-ttu-id="2879e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2879e-150">DateTimeOffset</span></span>|<span data-ttu-id="2879e-151">Letzte kontaktiert Datum-Uhrzeit des Geräts Inherited aus [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="2879e-151">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="2879e-152">description</span><span class="sxs-lookup"><span data-stu-id="2879e-152">description</span></span>|<span data-ttu-id="2879e-153">String</span><span class="sxs-lookup"><span data-stu-id="2879e-153">String</span></span>|<span data-ttu-id="2879e-154">Die Beschreibung des Geräts Inherited aus [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="2879e-154">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="2879e-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="2879e-155">enrollmentState</span></span>|[<span data-ttu-id="2879e-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="2879e-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="2879e-157">Der Zustand des Geräts in Intune geerbt von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="2879e-157">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="2879e-158">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="2879e-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="2879e-159">Plattform</span><span class="sxs-lookup"><span data-stu-id="2879e-159">platform</span></span>|[<span data-ttu-id="2879e-160">Plattform</span><span class="sxs-lookup"><span data-stu-id="2879e-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="2879e-161">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="2879e-161">The platform of the Device.</span></span> <span data-ttu-id="2879e-162">Geerbt von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="2879e-162">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="2879e-163">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="2879e-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="2879e-164">status</span><span class="sxs-lookup"><span data-stu-id="2879e-164">status</span></span>|<span data-ttu-id="2879e-165">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2879e-165">Boolean</span></span>|<span data-ttu-id="2879e-166">Status der importierten Gerät Identität</span><span class="sxs-lookup"><span data-stu-id="2879e-166">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="2879e-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="2879e-167">Response</span></span>
<span data-ttu-id="2879e-168">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2879e-168">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2879e-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2879e-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="2879e-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2879e-170">Request</span></span>
<span data-ttu-id="2879e-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2879e-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
Content-type: application/json
Content-length: 421

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="2879e-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="2879e-172">Response</span></span>
<span data-ttu-id="2879e-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2879e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





