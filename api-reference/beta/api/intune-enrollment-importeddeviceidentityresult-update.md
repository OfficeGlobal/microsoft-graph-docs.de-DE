---
title: ImportedDeviceIdentityResult aktualisieren
description: Aktualisieren Sie die Eigenschaften eines ImportedDeviceIdentityResult-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7fe9472b0f63ada966c61dd8fc56a7865cf94408
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827573"
---
# <a name="update-importeddeviceidentityresult"></a><span data-ttu-id="4b6aa-103">ImportedDeviceIdentityResult aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4b6aa-103">Update importedDeviceIdentityResult</span></span>

> <span data-ttu-id="4b6aa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4b6aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b6aa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b6aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b6aa-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4b6aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b6aa-107">Aktualisieren Sie die Eigenschaften eines [ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4b6aa-107">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4b6aa-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4b6aa-108">Prerequisites</span></span>
<span data-ttu-id="4b6aa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b6aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b6aa-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b6aa-111">Permission type</span></span>|<span data-ttu-id="4b6aa-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4b6aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b6aa-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4b6aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b6aa-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b6aa-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4b6aa-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4b6aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b6aa-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b6aa-116">Not supported.</span></span>|
|<span data-ttu-id="4b6aa-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b6aa-117">Application</span></span>|<span data-ttu-id="4b6aa-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b6aa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b6aa-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b6aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="4b6aa-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4b6aa-120">Request headers</span></span>
|<span data-ttu-id="4b6aa-121">Header</span><span class="sxs-lookup"><span data-stu-id="4b6aa-121">Header</span></span>|<span data-ttu-id="4b6aa-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4b6aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b6aa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b6aa-123">Authorization</span></span>|<span data-ttu-id="4b6aa-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4b6aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b6aa-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4b6aa-125">Accept</span></span>|<span data-ttu-id="4b6aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b6aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b6aa-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4b6aa-127">Request body</span></span>
<span data-ttu-id="4b6aa-128">Geben Sie im Textkörper Anforderung für das Objekt [ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="4b6aa-128">In the request body, supply a JSON representation for the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

<span data-ttu-id="4b6aa-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="4b6aa-129">The following table shows the properties that are required when you create the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>

|<span data-ttu-id="4b6aa-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b6aa-130">Property</span></span>|<span data-ttu-id="4b6aa-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4b6aa-131">Type</span></span>|<span data-ttu-id="4b6aa-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b6aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b6aa-133">id</span><span class="sxs-lookup"><span data-stu-id="4b6aa-133">id</span></span>|<span data-ttu-id="4b6aa-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b6aa-134">String</span></span>|<span data-ttu-id="4b6aa-135">ID der importierten Gerät Identität Inherited aus [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4b6aa-135">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="4b6aa-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="4b6aa-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="4b6aa-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b6aa-137">String</span></span>|<span data-ttu-id="4b6aa-138">Importierte Geräte-ID geerbt von [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4b6aa-138">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="4b6aa-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="4b6aa-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="4b6aa-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="4b6aa-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="4b6aa-141">Typ des importiert Gerät Identität geerbt von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="4b6aa-141">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="4b6aa-142">Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="4b6aa-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="4b6aa-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b6aa-143">lastModifiedDateTime</span></span>|<span data-ttu-id="4b6aa-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b6aa-144">DateTimeOffset</span></span>|<span data-ttu-id="4b6aa-145">Letzte Änderung DateTime der Beschreibung Inherited aus [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4b6aa-145">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="4b6aa-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b6aa-146">createdDateTime</span></span>|<span data-ttu-id="4b6aa-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b6aa-147">DateTimeOffset</span></span>|<span data-ttu-id="4b6aa-148">Datum-Uhrzeit des Geräts Inherited aus [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) erstellt</span><span class="sxs-lookup"><span data-stu-id="4b6aa-148">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="4b6aa-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b6aa-149">lastContactedDateTime</span></span>|<span data-ttu-id="4b6aa-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b6aa-150">DateTimeOffset</span></span>|<span data-ttu-id="4b6aa-151">Letzte kontaktiert Datum-Uhrzeit des Geräts Inherited aus [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4b6aa-151">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="4b6aa-152">description</span><span class="sxs-lookup"><span data-stu-id="4b6aa-152">description</span></span>|<span data-ttu-id="4b6aa-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b6aa-153">String</span></span>|<span data-ttu-id="4b6aa-154">Die Beschreibung des Geräts Inherited aus [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4b6aa-154">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="4b6aa-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="4b6aa-155">enrollmentState</span></span>|[<span data-ttu-id="4b6aa-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="4b6aa-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="4b6aa-157">Der Zustand des Geräts in Intune geerbt von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="4b6aa-157">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="4b6aa-158">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="4b6aa-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="4b6aa-159">Plattform</span><span class="sxs-lookup"><span data-stu-id="4b6aa-159">platform</span></span>|[<span data-ttu-id="4b6aa-160">Plattform</span><span class="sxs-lookup"><span data-stu-id="4b6aa-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="4b6aa-161">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4b6aa-161">The platform of the Device.</span></span> <span data-ttu-id="4b6aa-162">Geerbt von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="4b6aa-162">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="4b6aa-163">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="4b6aa-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="4b6aa-164">status</span><span class="sxs-lookup"><span data-stu-id="4b6aa-164">status</span></span>|<span data-ttu-id="4b6aa-165">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4b6aa-165">Boolean</span></span>|<span data-ttu-id="4b6aa-166">Status der importierten Gerät Identität</span><span class="sxs-lookup"><span data-stu-id="4b6aa-166">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="4b6aa-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b6aa-167">Response</span></span>
<span data-ttu-id="4b6aa-168">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4b6aa-168">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b6aa-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b6aa-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="4b6aa-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b6aa-170">Request</span></span>
<span data-ttu-id="4b6aa-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4b6aa-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 354

{
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

### <a name="response"></a><span data-ttu-id="4b6aa-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b6aa-172">Response</span></span>
<span data-ttu-id="4b6aa-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b6aa-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





