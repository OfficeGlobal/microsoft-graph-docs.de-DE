---
title: Erstellen von importedDeviceIdentity
description: Erstellen eines neuen ImportedDeviceIdentity-Objekts.
author: tfitzmac
ms.openlocfilehash: 4a1180bd924b2f8d7c2d66fdd1f4fff76ae8f685
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354789"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="1d500-103">Erstellen von importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="1d500-103">Create importedDeviceIdentity</span></span>

> <span data-ttu-id="1d500-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1d500-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d500-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d500-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d500-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1d500-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d500-107">Erstellen eines neuen [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1d500-107">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d500-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1d500-108">Prerequisites</span></span>
<span data-ttu-id="1d500-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d500-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d500-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1d500-111">Permission type</span></span>|<span data-ttu-id="1d500-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1d500-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d500-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1d500-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d500-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d500-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1d500-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1d500-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d500-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d500-116">Not supported.</span></span>|
|<span data-ttu-id="1d500-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1d500-117">Application</span></span>|<span data-ttu-id="1d500-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d500-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d500-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d500-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="1d500-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1d500-120">Request headers</span></span>
|<span data-ttu-id="1d500-121">Header</span><span class="sxs-lookup"><span data-stu-id="1d500-121">Header</span></span>|<span data-ttu-id="1d500-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1d500-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d500-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1d500-123">Authorization</span></span>|<span data-ttu-id="1d500-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1d500-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d500-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d500-125">Accept</span></span>|<span data-ttu-id="1d500-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d500-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d500-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1d500-127">Request body</span></span>
<span data-ttu-id="1d500-128">Geben Sie im Textkörper Anforderung für das Objekt ImportedDeviceIdentity eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="1d500-128">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="1d500-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die ImportedDeviceIdentity erstellen.</span><span class="sxs-lookup"><span data-stu-id="1d500-129">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="1d500-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1d500-130">Property</span></span>|<span data-ttu-id="1d500-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1d500-131">Type</span></span>|<span data-ttu-id="1d500-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d500-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d500-133">id</span><span class="sxs-lookup"><span data-stu-id="1d500-133">id</span></span>|<span data-ttu-id="1d500-134">String</span><span class="sxs-lookup"><span data-stu-id="1d500-134">String</span></span>|<span data-ttu-id="1d500-135">ID der Identität des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="1d500-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="1d500-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="1d500-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="1d500-137">String</span><span class="sxs-lookup"><span data-stu-id="1d500-137">String</span></span>|<span data-ttu-id="1d500-138">Importierte Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="1d500-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="1d500-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="1d500-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="1d500-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="1d500-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="1d500-141">Art der importierten Gerät Identität.</span><span class="sxs-lookup"><span data-stu-id="1d500-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="1d500-142">Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="1d500-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="1d500-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d500-143">lastModifiedDateTime</span></span>|<span data-ttu-id="1d500-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d500-144">DateTimeOffset</span></span>|<span data-ttu-id="1d500-145">Letzte Änderung DateTime der Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d500-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="1d500-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d500-146">createdDateTime</span></span>|<span data-ttu-id="1d500-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d500-147">DateTimeOffset</span></span>|<span data-ttu-id="1d500-148">Erstellte Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="1d500-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="1d500-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d500-149">lastContactedDateTime</span></span>|<span data-ttu-id="1d500-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d500-150">DateTimeOffset</span></span>|<span data-ttu-id="1d500-151">Letzte kontaktiert Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="1d500-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="1d500-152">description</span><span class="sxs-lookup"><span data-stu-id="1d500-152">description</span></span>|<span data-ttu-id="1d500-153">String</span><span class="sxs-lookup"><span data-stu-id="1d500-153">String</span></span>|<span data-ttu-id="1d500-154">Die Beschreibung des Geräts</span><span class="sxs-lookup"><span data-stu-id="1d500-154">The description of the device</span></span>|
|<span data-ttu-id="1d500-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="1d500-155">enrollmentState</span></span>|[<span data-ttu-id="1d500-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="1d500-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="1d500-157">Der Zustand des Geräts in Intune.</span><span class="sxs-lookup"><span data-stu-id="1d500-157">The state of the device in Intune.</span></span> <span data-ttu-id="1d500-158">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="1d500-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="1d500-159">Plattform</span><span class="sxs-lookup"><span data-stu-id="1d500-159">platform</span></span>|[<span data-ttu-id="1d500-160">Plattform</span><span class="sxs-lookup"><span data-stu-id="1d500-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="1d500-161">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="1d500-161">The platform of the Device.</span></span> <span data-ttu-id="1d500-162">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="1d500-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="1d500-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d500-163">Response</span></span>
<span data-ttu-id="1d500-164">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1d500-164">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d500-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1d500-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d500-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d500-166">Request</span></span>
<span data-ttu-id="1d500-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1d500-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
Content-type: application/json
Content-length: 396

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="1d500-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d500-168">Response</span></span>
<span data-ttu-id="1d500-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1d500-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





