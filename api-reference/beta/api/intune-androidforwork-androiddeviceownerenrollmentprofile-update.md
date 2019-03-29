---
title: Androiddeviceownerenrollmentprofile hinzugefügt aktualisieren
description: Aktualisieren der Eigenschaften eines Androiddeviceownerenrollmentprofile hinzugefügt-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee869f5c6cd6175f011536d757df8fd3d17b0389
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984891"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="84efa-103">Androiddeviceownerenrollmentprofile hinzugefügt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="84efa-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="84efa-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="84efa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84efa-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="84efa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84efa-106">Aktualisieren der Eigenschaften eines [androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="84efa-106">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84efa-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="84efa-107">Prerequisites</span></span>
<span data-ttu-id="84efa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84efa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84efa-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="84efa-110">Permission type</span></span>|<span data-ttu-id="84efa-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="84efa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84efa-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="84efa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84efa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84efa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84efa-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="84efa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84efa-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84efa-115">Not supported.</span></span>|
|<span data-ttu-id="84efa-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="84efa-116">Application</span></span>|<span data-ttu-id="84efa-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84efa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84efa-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="84efa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="84efa-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="84efa-119">Request headers</span></span>
|<span data-ttu-id="84efa-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="84efa-120">Header</span></span>|<span data-ttu-id="84efa-121">Wert</span><span class="sxs-lookup"><span data-stu-id="84efa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84efa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="84efa-122">Authorization</span></span>|<span data-ttu-id="84efa-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="84efa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84efa-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="84efa-124">Accept</span></span>|<span data-ttu-id="84efa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84efa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84efa-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="84efa-126">Request body</span></span>
<span data-ttu-id="84efa-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="84efa-127">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="84efa-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="84efa-128">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="84efa-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="84efa-129">Property</span></span>|<span data-ttu-id="84efa-130">Typ</span><span class="sxs-lookup"><span data-stu-id="84efa-130">Type</span></span>|<span data-ttu-id="84efa-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84efa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84efa-132">accountId</span><span class="sxs-lookup"><span data-stu-id="84efa-132">accountId</span></span>|<span data-ttu-id="84efa-133">String</span><span class="sxs-lookup"><span data-stu-id="84efa-133">String</span></span>|<span data-ttu-id="84efa-134">Mandanten-GUID, zu der das Registrierungsprofil gehört.</span><span class="sxs-lookup"><span data-stu-id="84efa-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="84efa-135">id</span><span class="sxs-lookup"><span data-stu-id="84efa-135">id</span></span>|<span data-ttu-id="84efa-136">String</span><span class="sxs-lookup"><span data-stu-id="84efa-136">String</span></span>|<span data-ttu-id="84efa-137">Eindeutige GUID des Registrierungsprofils.</span><span class="sxs-lookup"><span data-stu-id="84efa-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="84efa-138">displayName</span><span class="sxs-lookup"><span data-stu-id="84efa-138">displayName</span></span>|<span data-ttu-id="84efa-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84efa-139">String</span></span>|<span data-ttu-id="84efa-140">Anzeigename des Registrierungsprofils.</span><span class="sxs-lookup"><span data-stu-id="84efa-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="84efa-141">description</span><span class="sxs-lookup"><span data-stu-id="84efa-141">description</span></span>|<span data-ttu-id="84efa-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84efa-142">String</span></span>|<span data-ttu-id="84efa-143">Beschreibung des Registrierungsprofils.</span><span class="sxs-lookup"><span data-stu-id="84efa-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="84efa-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84efa-144">createdDateTime</span></span>|<span data-ttu-id="84efa-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84efa-145">DateTimeOffset</span></span>|<span data-ttu-id="84efa-146">Datum und Uhrzeit der Erstellung des Registrierungsprofils.</span><span class="sxs-lookup"><span data-stu-id="84efa-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="84efa-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84efa-147">lastModifiedDateTime</span></span>|<span data-ttu-id="84efa-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84efa-148">DateTimeOffset</span></span>|<span data-ttu-id="84efa-149">Datum und Uhrzeit der letzten Änderung des Registrierungsprofils.</span><span class="sxs-lookup"><span data-stu-id="84efa-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="84efa-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="84efa-150">tokenValue</span></span>|<span data-ttu-id="84efa-151">String</span><span class="sxs-lookup"><span data-stu-id="84efa-151">String</span></span>|<span data-ttu-id="84efa-152">Wert des zuletzt für das Registrierungsprofil erstellten Tokens.</span><span class="sxs-lookup"><span data-stu-id="84efa-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="84efa-153">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="84efa-153">tokenCreationDateTime</span></span>|<span data-ttu-id="84efa-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84efa-154">DateTimeOffset</span></span>|<span data-ttu-id="84efa-155">Datum der Erstellung des zuletzt erstellten Tokens.</span><span class="sxs-lookup"><span data-stu-id="84efa-155">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="84efa-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="84efa-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="84efa-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84efa-157">DateTimeOffset</span></span>|<span data-ttu-id="84efa-158">Datum und Uhrzeit des Ablaufs des zuletzt erstellten Tokens.</span><span class="sxs-lookup"><span data-stu-id="84efa-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="84efa-159">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="84efa-159">enrolledDeviceCount</span></span>|<span data-ttu-id="84efa-160">Int32</span><span class="sxs-lookup"><span data-stu-id="84efa-160">Int32</span></span>|<span data-ttu-id="84efa-161">Gesamtzahl der mit dem Registrierungsprofil registrierten Android-Geräte.</span><span class="sxs-lookup"><span data-stu-id="84efa-161">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="84efa-162">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="84efa-162">qrCodeContent</span></span>|<span data-ttu-id="84efa-163">String</span><span class="sxs-lookup"><span data-stu-id="84efa-163">String</span></span>|<span data-ttu-id="84efa-164">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="84efa-164">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="84efa-165">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="84efa-165">qrCodeImage</span></span>|[<span data-ttu-id="84efa-166">mimeContent</span><span class="sxs-lookup"><span data-stu-id="84efa-166">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="84efa-167">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="84efa-167">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="84efa-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="84efa-168">Response</span></span>
<span data-ttu-id="84efa-169">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="84efa-169">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84efa-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="84efa-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="84efa-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="84efa-171">Request</span></span>
<span data-ttu-id="84efa-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="84efa-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
Content-type: application/json
Content-length: 565

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "tokenValue": "Token Value value",
  "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
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

### <a name="response"></a><span data-ttu-id="84efa-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="84efa-173">Response</span></span>
<span data-ttu-id="84efa-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="84efa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 737

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
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




