---
title: Aktualisieren von „androidForWorkEnrollmentProfile“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs androidForWorkEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e276325bfc67651ec71cde49fef3705b77567911
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972102"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="2798d-103">Aktualisieren von „androidForWorkEnrollmentProfile“</span><span class="sxs-lookup"><span data-stu-id="2798d-103">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="2798d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2798d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2798d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2798d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2798d-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="2798d-106">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2798d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2798d-107">Prerequisites</span></span>
<span data-ttu-id="2798d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2798d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2798d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2798d-110">Permission type</span></span>|<span data-ttu-id="2798d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2798d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2798d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2798d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2798d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2798d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2798d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2798d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2798d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2798d-115">Not supported.</span></span>|
|<span data-ttu-id="2798d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2798d-116">Application</span></span>|<span data-ttu-id="2798d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2798d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2798d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2798d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="2798d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2798d-119">Request headers</span></span>
|<span data-ttu-id="2798d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2798d-120">Header</span></span>|<span data-ttu-id="2798d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2798d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2798d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2798d-122">Authorization</span></span>|<span data-ttu-id="2798d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2798d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2798d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2798d-124">Accept</span></span>|<span data-ttu-id="2798d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2798d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2798d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2798d-126">Request body</span></span>
<span data-ttu-id="2798d-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) an.</span><span class="sxs-lookup"><span data-stu-id="2798d-127">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="2798d-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2798d-128">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="2798d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2798d-129">Property</span></span>|<span data-ttu-id="2798d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2798d-130">Type</span></span>|<span data-ttu-id="2798d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2798d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2798d-132">accountId</span><span class="sxs-lookup"><span data-stu-id="2798d-132">accountId</span></span>|<span data-ttu-id="2798d-133">String</span><span class="sxs-lookup"><span data-stu-id="2798d-133">String</span></span>|<span data-ttu-id="2798d-134">Mandanten-GUID, zu der das Registrierungsprofil gehört.</span><span class="sxs-lookup"><span data-stu-id="2798d-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="2798d-135">id</span><span class="sxs-lookup"><span data-stu-id="2798d-135">id</span></span>|<span data-ttu-id="2798d-136">String</span><span class="sxs-lookup"><span data-stu-id="2798d-136">String</span></span>|<span data-ttu-id="2798d-137">Eindeutige GUID des Registrierungsprofils.</span><span class="sxs-lookup"><span data-stu-id="2798d-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="2798d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="2798d-138">displayName</span></span>|<span data-ttu-id="2798d-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2798d-139">String</span></span>|<span data-ttu-id="2798d-140">Anzeigename des Registrierungsprofils.</span><span class="sxs-lookup"><span data-stu-id="2798d-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="2798d-141">description</span><span class="sxs-lookup"><span data-stu-id="2798d-141">description</span></span>|<span data-ttu-id="2798d-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2798d-142">String</span></span>|<span data-ttu-id="2798d-143">Beschreibung des Registrierungsprofils.</span><span class="sxs-lookup"><span data-stu-id="2798d-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="2798d-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2798d-144">createdDateTime</span></span>|<span data-ttu-id="2798d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2798d-145">DateTimeOffset</span></span>|<span data-ttu-id="2798d-146">Datum und Uhrzeit der Erstellung des Registrierungsprofils.</span><span class="sxs-lookup"><span data-stu-id="2798d-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="2798d-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2798d-147">lastModifiedDateTime</span></span>|<span data-ttu-id="2798d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2798d-148">DateTimeOffset</span></span>|<span data-ttu-id="2798d-149">Datum und Uhrzeit der letzten Änderung des Registrierungsprofils.</span><span class="sxs-lookup"><span data-stu-id="2798d-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="2798d-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="2798d-150">tokenValue</span></span>|<span data-ttu-id="2798d-151">String</span><span class="sxs-lookup"><span data-stu-id="2798d-151">String</span></span>|<span data-ttu-id="2798d-152">Wert des zuletzt für das Registrierungsprofil erstellten Tokens.</span><span class="sxs-lookup"><span data-stu-id="2798d-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="2798d-153">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2798d-153">tokenExpirationDateTime</span></span>|<span data-ttu-id="2798d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2798d-154">DateTimeOffset</span></span>|<span data-ttu-id="2798d-155">Datum und Uhrzeit des Ablaufs des zuletzt erstellten Tokens.</span><span class="sxs-lookup"><span data-stu-id="2798d-155">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="2798d-156">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2798d-156">enrolledDeviceCount</span></span>|<span data-ttu-id="2798d-157">Int32</span><span class="sxs-lookup"><span data-stu-id="2798d-157">Int32</span></span>|<span data-ttu-id="2798d-158">Gesamtzahl der mit dem Registrierungsprofil registrierten Android-Geräte.</span><span class="sxs-lookup"><span data-stu-id="2798d-158">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="2798d-159">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="2798d-159">qrCodeContent</span></span>|<span data-ttu-id="2798d-160">String</span><span class="sxs-lookup"><span data-stu-id="2798d-160">String</span></span>|<span data-ttu-id="2798d-161">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="2798d-161">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="2798d-162">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="2798d-162">qrCodeImage</span></span>|[<span data-ttu-id="2798d-163">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2798d-163">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2798d-164">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="2798d-164">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="2798d-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="2798d-165">Response</span></span>
<span data-ttu-id="2798d-166">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2798d-166">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2798d-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2798d-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="2798d-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2798d-168">Request</span></span>
<span data-ttu-id="2798d-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2798d-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
Content-type: application/json
Content-length: 496

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="2798d-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="2798d-170">Response</span></span>
<span data-ttu-id="2798d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2798d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




