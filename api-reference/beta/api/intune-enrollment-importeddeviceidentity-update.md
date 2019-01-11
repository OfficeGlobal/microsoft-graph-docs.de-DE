---
title: ImportedDeviceIdentity aktualisieren
description: Aktualisieren Sie die Eigenschaften eines ImportedDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9072c0b5e8a01c72352b9250b4167cdb5ec190fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838430"
---
# <a name="update-importeddeviceidentity"></a><span data-ttu-id="2d127-103">ImportedDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2d127-103">Update importedDeviceIdentity</span></span>

> <span data-ttu-id="2d127-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2d127-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d127-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2d127-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2d127-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2d127-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d127-107">Aktualisieren Sie die Eigenschaften eines [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2d127-107">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2d127-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2d127-108">Prerequisites</span></span>
<span data-ttu-id="2d127-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d127-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d127-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2d127-111">Permission type</span></span>|<span data-ttu-id="2d127-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2d127-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d127-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2d127-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2d127-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d127-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2d127-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2d127-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d127-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d127-116">Not supported.</span></span>|
|<span data-ttu-id="2d127-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2d127-117">Application</span></span>|<span data-ttu-id="2d127-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d127-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d127-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d127-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="2d127-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2d127-120">Request headers</span></span>
|<span data-ttu-id="2d127-121">Header</span><span class="sxs-lookup"><span data-stu-id="2d127-121">Header</span></span>|<span data-ttu-id="2d127-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2d127-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d127-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d127-123">Authorization</span></span>|<span data-ttu-id="2d127-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2d127-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d127-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2d127-125">Accept</span></span>|<span data-ttu-id="2d127-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2d127-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d127-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2d127-127">Request body</span></span>
<span data-ttu-id="2d127-128">Geben Sie im Textkörper Anforderung für das Objekt [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="2d127-128">In the request body, supply a JSON representation for the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

<span data-ttu-id="2d127-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="2d127-129">The following table shows the properties that are required when you create the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>

|<span data-ttu-id="2d127-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2d127-130">Property</span></span>|<span data-ttu-id="2d127-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2d127-131">Type</span></span>|<span data-ttu-id="2d127-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d127-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d127-133">id</span><span class="sxs-lookup"><span data-stu-id="2d127-133">id</span></span>|<span data-ttu-id="2d127-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2d127-134">String</span></span>|<span data-ttu-id="2d127-135">ID der Identität des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="2d127-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="2d127-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="2d127-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="2d127-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2d127-137">String</span></span>|<span data-ttu-id="2d127-138">Importierte Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="2d127-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="2d127-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="2d127-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="2d127-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="2d127-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="2d127-141">Art der importierten Gerät Identität.</span><span class="sxs-lookup"><span data-stu-id="2d127-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="2d127-142">Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="2d127-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="2d127-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d127-143">lastModifiedDateTime</span></span>|<span data-ttu-id="2d127-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d127-144">DateTimeOffset</span></span>|<span data-ttu-id="2d127-145">Letzte Änderung DateTime der Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d127-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="2d127-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d127-146">createdDateTime</span></span>|<span data-ttu-id="2d127-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d127-147">DateTimeOffset</span></span>|<span data-ttu-id="2d127-148">Erstellte Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="2d127-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="2d127-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d127-149">lastContactedDateTime</span></span>|<span data-ttu-id="2d127-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d127-150">DateTimeOffset</span></span>|<span data-ttu-id="2d127-151">Letzte kontaktiert Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="2d127-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="2d127-152">description</span><span class="sxs-lookup"><span data-stu-id="2d127-152">description</span></span>|<span data-ttu-id="2d127-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2d127-153">String</span></span>|<span data-ttu-id="2d127-154">Die Beschreibung des Geräts</span><span class="sxs-lookup"><span data-stu-id="2d127-154">The description of the device</span></span>|
|<span data-ttu-id="2d127-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="2d127-155">enrollmentState</span></span>|[<span data-ttu-id="2d127-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="2d127-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="2d127-157">Der Zustand des Geräts in Intune.</span><span class="sxs-lookup"><span data-stu-id="2d127-157">The state of the device in Intune.</span></span> <span data-ttu-id="2d127-158">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="2d127-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="2d127-159">Plattform</span><span class="sxs-lookup"><span data-stu-id="2d127-159">platform</span></span>|[<span data-ttu-id="2d127-160">Plattform</span><span class="sxs-lookup"><span data-stu-id="2d127-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="2d127-161">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="2d127-161">The platform of the Device.</span></span> <span data-ttu-id="2d127-162">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="2d127-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="2d127-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d127-163">Response</span></span>
<span data-ttu-id="2d127-164">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2d127-164">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d127-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2d127-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="2d127-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d127-166">Request</span></span>
<span data-ttu-id="2d127-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d127-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2d127-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d127-168">Response</span></span>
<span data-ttu-id="2d127-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d127-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





