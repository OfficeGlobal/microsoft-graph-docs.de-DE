---
title: Erstellen von importedDeviceIdentity
description: Erstellen eines neuen ImportedDeviceIdentity-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d0274f3a48c3481cc5540eb9025da353f0ea0bf2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396714"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="e6828-103">Erstellen von importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="e6828-103">Create importedDeviceIdentity</span></span>

> <span data-ttu-id="e6828-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e6828-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e6828-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e6828-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6828-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e6828-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6828-107">Erstellen eines neuen [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e6828-107">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6828-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e6828-108">Prerequisites</span></span>
<span data-ttu-id="e6828-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e6828-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e6828-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e6828-111">Permission type</span></span>|<span data-ttu-id="e6828-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e6828-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6828-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e6828-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6828-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6828-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e6828-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e6828-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6828-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e6828-116">Not supported.</span></span>|
|<span data-ttu-id="e6828-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e6828-117">Application</span></span>|<span data-ttu-id="e6828-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e6828-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6828-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6828-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="e6828-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e6828-120">Request headers</span></span>
|<span data-ttu-id="e6828-121">Header</span><span class="sxs-lookup"><span data-stu-id="e6828-121">Header</span></span>|<span data-ttu-id="e6828-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e6828-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6828-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e6828-123">Authorization</span></span>|<span data-ttu-id="e6828-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e6828-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6828-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e6828-125">Accept</span></span>|<span data-ttu-id="e6828-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6828-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6828-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e6828-127">Request body</span></span>
<span data-ttu-id="e6828-128">Geben Sie im Textkörper Anforderung für das Objekt ImportedDeviceIdentity eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="e6828-128">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="e6828-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die ImportedDeviceIdentity erstellen.</span><span class="sxs-lookup"><span data-stu-id="e6828-129">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="e6828-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e6828-130">Property</span></span>|<span data-ttu-id="e6828-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e6828-131">Type</span></span>|<span data-ttu-id="e6828-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6828-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6828-133">id</span><span class="sxs-lookup"><span data-stu-id="e6828-133">id</span></span>|<span data-ttu-id="e6828-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6828-134">String</span></span>|<span data-ttu-id="e6828-135">ID der Identität des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="e6828-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="e6828-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e6828-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="e6828-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6828-137">String</span></span>|<span data-ttu-id="e6828-138">Importierte Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="e6828-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="e6828-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="e6828-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="e6828-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="e6828-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="e6828-141">Art der importierten Gerät Identität.</span><span class="sxs-lookup"><span data-stu-id="e6828-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="e6828-142">Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="e6828-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="e6828-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6828-143">lastModifiedDateTime</span></span>|<span data-ttu-id="e6828-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6828-144">DateTimeOffset</span></span>|<span data-ttu-id="e6828-145">Letzte Änderung DateTime der Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6828-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="e6828-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6828-146">createdDateTime</span></span>|<span data-ttu-id="e6828-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6828-147">DateTimeOffset</span></span>|<span data-ttu-id="e6828-148">Erstellte Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="e6828-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="e6828-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6828-149">lastContactedDateTime</span></span>|<span data-ttu-id="e6828-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6828-150">DateTimeOffset</span></span>|<span data-ttu-id="e6828-151">Letzte kontaktiert Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="e6828-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="e6828-152">description</span><span class="sxs-lookup"><span data-stu-id="e6828-152">description</span></span>|<span data-ttu-id="e6828-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6828-153">String</span></span>|<span data-ttu-id="e6828-154">Die Beschreibung des Geräts</span><span class="sxs-lookup"><span data-stu-id="e6828-154">The description of the device</span></span>|
|<span data-ttu-id="e6828-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="e6828-155">enrollmentState</span></span>|[<span data-ttu-id="e6828-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="e6828-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="e6828-157">Der Zustand des Geräts in Intune.</span><span class="sxs-lookup"><span data-stu-id="e6828-157">The state of the device in Intune.</span></span> <span data-ttu-id="e6828-158">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="e6828-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="e6828-159">Plattform</span><span class="sxs-lookup"><span data-stu-id="e6828-159">platform</span></span>|[<span data-ttu-id="e6828-160">Plattform</span><span class="sxs-lookup"><span data-stu-id="e6828-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="e6828-161">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="e6828-161">The platform of the Device.</span></span> <span data-ttu-id="e6828-162">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="e6828-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="e6828-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6828-163">Response</span></span>
<span data-ttu-id="e6828-164">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e6828-164">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6828-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e6828-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6828-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6828-166">Request</span></span>
<span data-ttu-id="e6828-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e6828-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e6828-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6828-168">Response</span></span>
<span data-ttu-id="e6828-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e6828-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




