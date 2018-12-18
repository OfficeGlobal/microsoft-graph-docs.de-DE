---
title: Aktualisieren von „androidForWorkEnrollmentProfile“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs androidForWorkEnrollmentProfile.
author: tfitzmac
ms.openlocfilehash: 5ffbcfa51d94816b9a65a90e59cfc4c3a654006d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356014"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="50b63-103">Aktualisieren von „androidForWorkEnrollmentProfile“</span><span class="sxs-lookup"><span data-stu-id="50b63-103">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="50b63-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="50b63-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50b63-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50b63-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50b63-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="50b63-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50b63-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="50b63-107">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50b63-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="50b63-108">Prerequisites</span></span>
<span data-ttu-id="50b63-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50b63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50b63-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50b63-111">Permission type</span></span>|<span data-ttu-id="50b63-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50b63-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50b63-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50b63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50b63-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50b63-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50b63-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50b63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50b63-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50b63-116">Not supported.</span></span>|
|<span data-ttu-id="50b63-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50b63-117">Application</span></span>|<span data-ttu-id="50b63-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50b63-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50b63-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50b63-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="50b63-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="50b63-120">Request headers</span></span>
|<span data-ttu-id="50b63-121">Header</span><span class="sxs-lookup"><span data-stu-id="50b63-121">Header</span></span>|<span data-ttu-id="50b63-122">Wert</span><span class="sxs-lookup"><span data-stu-id="50b63-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50b63-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="50b63-123">Authorization</span></span>|<span data-ttu-id="50b63-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="50b63-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50b63-125">Accept</span><span class="sxs-lookup"><span data-stu-id="50b63-125">Accept</span></span>|<span data-ttu-id="50b63-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50b63-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50b63-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="50b63-127">Request body</span></span>
<span data-ttu-id="50b63-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) an.</span><span class="sxs-lookup"><span data-stu-id="50b63-128">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="50b63-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="50b63-129">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="50b63-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50b63-130">Property</span></span>|<span data-ttu-id="50b63-131">Typ</span><span class="sxs-lookup"><span data-stu-id="50b63-131">Type</span></span>|<span data-ttu-id="50b63-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50b63-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50b63-133">accountId</span><span class="sxs-lookup"><span data-stu-id="50b63-133">accountId</span></span>|<span data-ttu-id="50b63-134">String</span><span class="sxs-lookup"><span data-stu-id="50b63-134">String</span></span>|<span data-ttu-id="50b63-135">Mandanten-GUID, zu der das Registrierungsprofil gehört</span><span class="sxs-lookup"><span data-stu-id="50b63-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="50b63-136">id</span><span class="sxs-lookup"><span data-stu-id="50b63-136">id</span></span>|<span data-ttu-id="50b63-137">String</span><span class="sxs-lookup"><span data-stu-id="50b63-137">String</span></span>|<span data-ttu-id="50b63-138">Eindeutige GUID des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="50b63-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="50b63-139">displayName</span><span class="sxs-lookup"><span data-stu-id="50b63-139">displayName</span></span>|<span data-ttu-id="50b63-140">String</span><span class="sxs-lookup"><span data-stu-id="50b63-140">String</span></span>|<span data-ttu-id="50b63-141">Anzeigename des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="50b63-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="50b63-142">description</span><span class="sxs-lookup"><span data-stu-id="50b63-142">description</span></span>|<span data-ttu-id="50b63-143">String</span><span class="sxs-lookup"><span data-stu-id="50b63-143">String</span></span>|<span data-ttu-id="50b63-144">Beschreibung des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="50b63-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="50b63-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50b63-145">createdDateTime</span></span>|<span data-ttu-id="50b63-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50b63-146">DateTimeOffset</span></span>|<span data-ttu-id="50b63-147">Datum und Uhrzeit der Erstellung des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="50b63-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="50b63-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50b63-148">lastModifiedDateTime</span></span>|<span data-ttu-id="50b63-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50b63-149">DateTimeOffset</span></span>|<span data-ttu-id="50b63-150">Datum und Uhrzeit der letzten Änderung des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="50b63-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="50b63-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="50b63-151">tokenValue</span></span>|<span data-ttu-id="50b63-152">String</span><span class="sxs-lookup"><span data-stu-id="50b63-152">String</span></span>|<span data-ttu-id="50b63-153">Wert des zuletzt für das Registrierungsprofil erstellten Tokens</span><span class="sxs-lookup"><span data-stu-id="50b63-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="50b63-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="50b63-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="50b63-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50b63-155">DateTimeOffset</span></span>|<span data-ttu-id="50b63-156">Datum und Uhrzeit des Ablaufs des zuletzt erstellten Tokens</span><span class="sxs-lookup"><span data-stu-id="50b63-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="50b63-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="50b63-157">enrolledDeviceCount</span></span>|<span data-ttu-id="50b63-158">Int32</span><span class="sxs-lookup"><span data-stu-id="50b63-158">Int32</span></span>|<span data-ttu-id="50b63-159">Gesamtzahl der mit dem Registrierungsprofil registrierten Android-Geräte</span><span class="sxs-lookup"><span data-stu-id="50b63-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="50b63-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="50b63-160">qrCodeContent</span></span>|<span data-ttu-id="50b63-161">String</span><span class="sxs-lookup"><span data-stu-id="50b63-161">String</span></span>|<span data-ttu-id="50b63-162">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird</span><span class="sxs-lookup"><span data-stu-id="50b63-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="50b63-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="50b63-163">qrCodeImage</span></span>|[<span data-ttu-id="50b63-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="50b63-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="50b63-165">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird</span><span class="sxs-lookup"><span data-stu-id="50b63-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="50b63-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="50b63-166">Response</span></span>
<span data-ttu-id="50b63-167">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="50b63-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50b63-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="50b63-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="50b63-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="50b63-169">Request</span></span>
<span data-ttu-id="50b63-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50b63-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
Content-type: application/json
Content-length: 490

{
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="50b63-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="50b63-171">Response</span></span>
<span data-ttu-id="50b63-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50b63-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 668

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "e6742553-2553-e674-5325-74e6532574e6",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```





