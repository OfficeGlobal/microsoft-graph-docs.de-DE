---
title: Erstellen von „androidForWorkEnrollmentProfile“
description: Erstellen eines neuen androidForWorkEnrollmentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cc51a0a5eede602e0757571b186a7995d8f4867b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27992042"
---
# <a name="create-androidforworkenrollmentprofile"></a><span data-ttu-id="33ed4-103">Erstellen von „androidForWorkEnrollmentProfile“</span><span class="sxs-lookup"><span data-stu-id="33ed4-103">Create androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="33ed4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="33ed4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33ed4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33ed4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33ed4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="33ed4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33ed4-107">Erstellen eines neuen [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="33ed4-107">Create a new [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33ed4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="33ed4-108">Prerequisites</span></span>
<span data-ttu-id="33ed4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33ed4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33ed4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="33ed4-111">Permission type</span></span>|<span data-ttu-id="33ed4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="33ed4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33ed4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="33ed4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33ed4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33ed4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33ed4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="33ed4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33ed4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33ed4-116">Not supported.</span></span>|
|<span data-ttu-id="33ed4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="33ed4-117">Application</span></span>|<span data-ttu-id="33ed4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33ed4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33ed4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="33ed4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="33ed4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="33ed4-120">Request headers</span></span>
|<span data-ttu-id="33ed4-121">Header</span><span class="sxs-lookup"><span data-stu-id="33ed4-121">Header</span></span>|<span data-ttu-id="33ed4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="33ed4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33ed4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="33ed4-123">Authorization</span></span>|<span data-ttu-id="33ed4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="33ed4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33ed4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="33ed4-125">Accept</span></span>|<span data-ttu-id="33ed4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33ed4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33ed4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="33ed4-127">Request body</span></span>
<span data-ttu-id="33ed4-128">Geben Sie im Anforderungstext eine JSON-Darstellung des androidForWorkEnrollmentProfile-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="33ed4-128">In the request body, supply a JSON representation for the androidForWorkEnrollmentProfile object.</span></span>

<span data-ttu-id="33ed4-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des androidForWorkEnrollmentProfile erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="33ed4-129">The following table shows the properties that are required when you create the androidForWorkEnrollmentProfile.</span></span>

|<span data-ttu-id="33ed4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33ed4-130">Property</span></span>|<span data-ttu-id="33ed4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="33ed4-131">Type</span></span>|<span data-ttu-id="33ed4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33ed4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33ed4-133">accountId</span><span class="sxs-lookup"><span data-stu-id="33ed4-133">accountId</span></span>|<span data-ttu-id="33ed4-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33ed4-134">String</span></span>|<span data-ttu-id="33ed4-135">Mandanten-GUID, zu der das Registrierungsprofil gehört</span><span class="sxs-lookup"><span data-stu-id="33ed4-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="33ed4-136">id</span><span class="sxs-lookup"><span data-stu-id="33ed4-136">id</span></span>|<span data-ttu-id="33ed4-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33ed4-137">String</span></span>|<span data-ttu-id="33ed4-138">Eindeutige GUID des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="33ed4-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="33ed4-139">displayName</span><span class="sxs-lookup"><span data-stu-id="33ed4-139">displayName</span></span>|<span data-ttu-id="33ed4-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33ed4-140">String</span></span>|<span data-ttu-id="33ed4-141">Anzeigename des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="33ed4-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="33ed4-142">description</span><span class="sxs-lookup"><span data-stu-id="33ed4-142">description</span></span>|<span data-ttu-id="33ed4-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33ed4-143">String</span></span>|<span data-ttu-id="33ed4-144">Beschreibung des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="33ed4-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="33ed4-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33ed4-145">createdDateTime</span></span>|<span data-ttu-id="33ed4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33ed4-146">DateTimeOffset</span></span>|<span data-ttu-id="33ed4-147">Datum und Uhrzeit der Erstellung des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="33ed4-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="33ed4-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33ed4-148">lastModifiedDateTime</span></span>|<span data-ttu-id="33ed4-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33ed4-149">DateTimeOffset</span></span>|<span data-ttu-id="33ed4-150">Datum und Uhrzeit der letzten Änderung des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="33ed4-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="33ed4-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="33ed4-151">tokenValue</span></span>|<span data-ttu-id="33ed4-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33ed4-152">String</span></span>|<span data-ttu-id="33ed4-153">Wert des zuletzt für das Registrierungsprofil erstellten Tokens</span><span class="sxs-lookup"><span data-stu-id="33ed4-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="33ed4-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="33ed4-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="33ed4-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33ed4-155">DateTimeOffset</span></span>|<span data-ttu-id="33ed4-156">Datum und Uhrzeit des Ablaufs des zuletzt erstellten Tokens</span><span class="sxs-lookup"><span data-stu-id="33ed4-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="33ed4-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="33ed4-157">enrolledDeviceCount</span></span>|<span data-ttu-id="33ed4-158">Int32</span><span class="sxs-lookup"><span data-stu-id="33ed4-158">Int32</span></span>|<span data-ttu-id="33ed4-159">Gesamtzahl der mit dem Registrierungsprofil registrierten Android-Geräte</span><span class="sxs-lookup"><span data-stu-id="33ed4-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="33ed4-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="33ed4-160">qrCodeContent</span></span>|<span data-ttu-id="33ed4-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33ed4-161">String</span></span>|<span data-ttu-id="33ed4-162">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird</span><span class="sxs-lookup"><span data-stu-id="33ed4-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="33ed4-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="33ed4-163">qrCodeImage</span></span>|[<span data-ttu-id="33ed4-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="33ed4-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="33ed4-165">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird</span><span class="sxs-lookup"><span data-stu-id="33ed4-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="33ed4-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="33ed4-166">Response</span></span>
<span data-ttu-id="33ed4-167">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33ed4-167">If successful, this method returns a `201 Created` response code and a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33ed4-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33ed4-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="33ed4-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33ed4-169">Request</span></span>
<span data-ttu-id="33ed4-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="33ed4-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles
Content-type: application/json
Content-length: 560

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
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

### <a name="response"></a><span data-ttu-id="33ed4-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="33ed4-171">Response</span></span>
<span data-ttu-id="33ed4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33ed4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





