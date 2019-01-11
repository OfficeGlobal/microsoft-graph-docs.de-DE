---
title: AndroidDeviceOwnerEnrollmentProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidDeviceOwnerEnrollmentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 18ecb9728cd1f178112bc8542f147edc8af472a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814154"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="3caae-103">AndroidDeviceOwnerEnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3caae-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="3caae-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3caae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3caae-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3caae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3caae-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3caae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3caae-107">Aktualisieren Sie die Eigenschaften eines [AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3caae-107">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3caae-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3caae-108">Prerequisites</span></span>
<span data-ttu-id="3caae-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3caae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3caae-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3caae-111">Permission type</span></span>|<span data-ttu-id="3caae-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3caae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3caae-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3caae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3caae-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3caae-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3caae-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3caae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3caae-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3caae-116">Not supported.</span></span>|
|<span data-ttu-id="3caae-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3caae-117">Application</span></span>|<span data-ttu-id="3caae-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3caae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3caae-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3caae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="3caae-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3caae-120">Request headers</span></span>
|<span data-ttu-id="3caae-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3caae-121">Header</span></span>|<span data-ttu-id="3caae-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3caae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3caae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3caae-123">Authorization</span></span>|<span data-ttu-id="3caae-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3caae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3caae-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3caae-125">Accept</span></span>|<span data-ttu-id="3caae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3caae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3caae-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3caae-127">Request body</span></span>
<span data-ttu-id="3caae-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="3caae-128">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="3caae-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="3caae-129">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="3caae-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3caae-130">Property</span></span>|<span data-ttu-id="3caae-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3caae-131">Type</span></span>|<span data-ttu-id="3caae-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3caae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3caae-133">accountId</span><span class="sxs-lookup"><span data-stu-id="3caae-133">accountId</span></span>|<span data-ttu-id="3caae-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3caae-134">String</span></span>|<span data-ttu-id="3caae-135">Mandanten-GUID, zu der das Registrierungsprofil gehört</span><span class="sxs-lookup"><span data-stu-id="3caae-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="3caae-136">id</span><span class="sxs-lookup"><span data-stu-id="3caae-136">id</span></span>|<span data-ttu-id="3caae-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3caae-137">String</span></span>|<span data-ttu-id="3caae-138">Eindeutige GUID des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="3caae-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="3caae-139">displayName</span><span class="sxs-lookup"><span data-stu-id="3caae-139">displayName</span></span>|<span data-ttu-id="3caae-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3caae-140">String</span></span>|<span data-ttu-id="3caae-141">Anzeigename des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="3caae-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="3caae-142">description</span><span class="sxs-lookup"><span data-stu-id="3caae-142">description</span></span>|<span data-ttu-id="3caae-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3caae-143">String</span></span>|<span data-ttu-id="3caae-144">Beschreibung des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="3caae-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="3caae-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3caae-145">createdDateTime</span></span>|<span data-ttu-id="3caae-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3caae-146">DateTimeOffset</span></span>|<span data-ttu-id="3caae-147">Datum und Uhrzeit der Erstellung des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="3caae-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="3caae-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3caae-148">lastModifiedDateTime</span></span>|<span data-ttu-id="3caae-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3caae-149">DateTimeOffset</span></span>|<span data-ttu-id="3caae-150">Datum und Uhrzeit der letzten Änderung des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="3caae-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="3caae-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="3caae-151">tokenValue</span></span>|<span data-ttu-id="3caae-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3caae-152">String</span></span>|<span data-ttu-id="3caae-153">Wert des zuletzt für das Registrierungsprofil erstellten Tokens</span><span class="sxs-lookup"><span data-stu-id="3caae-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="3caae-154">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="3caae-154">tokenCreationDateTime</span></span>|<span data-ttu-id="3caae-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3caae-155">DateTimeOffset</span></span>|<span data-ttu-id="3caae-156">Datum-Uhrzeit das zuletzt erstellte Token erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="3caae-156">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="3caae-157">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3caae-157">tokenExpirationDateTime</span></span>|<span data-ttu-id="3caae-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3caae-158">DateTimeOffset</span></span>|<span data-ttu-id="3caae-159">Datum und Uhrzeit des Ablaufs des zuletzt erstellten Tokens</span><span class="sxs-lookup"><span data-stu-id="3caae-159">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="3caae-160">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3caae-160">enrolledDeviceCount</span></span>|<span data-ttu-id="3caae-161">Int32</span><span class="sxs-lookup"><span data-stu-id="3caae-161">Int32</span></span>|<span data-ttu-id="3caae-162">Gesamtzahl der mit dem Registrierungsprofil registrierten Android-Geräte</span><span class="sxs-lookup"><span data-stu-id="3caae-162">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="3caae-163">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="3caae-163">qrCodeContent</span></span>|<span data-ttu-id="3caae-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3caae-164">String</span></span>|<span data-ttu-id="3caae-165">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird</span><span class="sxs-lookup"><span data-stu-id="3caae-165">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="3caae-166">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="3caae-166">qrCodeImage</span></span>|[<span data-ttu-id="3caae-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3caae-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3caae-168">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird</span><span class="sxs-lookup"><span data-stu-id="3caae-168">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="3caae-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="3caae-169">Response</span></span>
<span data-ttu-id="3caae-170">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3caae-170">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3caae-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3caae-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="3caae-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3caae-172">Request</span></span>
<span data-ttu-id="3caae-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3caae-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
Content-type: application/json
Content-length: 555

{
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="3caae-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="3caae-174">Response</span></span>
<span data-ttu-id="3caae-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3caae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





