---
title: Aktualisieren von „applePushNotificationCertificate“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs applePushNotificationCertificate.
ms.openlocfilehash: 7fbb7db93290fb6f455bdcca3053c6f3affb1375
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060433"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="5c235-103">Aktualisieren von „applePushNotificationCertificate“</span><span class="sxs-lookup"><span data-stu-id="5c235-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="5c235-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5c235-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c235-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5c235-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c235-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5c235-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c235-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="5c235-107">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c235-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5c235-108">Prerequisites</span></span>
<span data-ttu-id="5c235-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c235-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c235-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5c235-111">Permission type</span></span>|<span data-ttu-id="5c235-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5c235-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c235-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5c235-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c235-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c235-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5c235-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5c235-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c235-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c235-116">Not supported.</span></span>|
|<span data-ttu-id="5c235-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5c235-117">Application</span></span>|<span data-ttu-id="5c235-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c235-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c235-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c235-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="5c235-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5c235-120">Request headers</span></span>
|<span data-ttu-id="5c235-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5c235-121">Header</span></span>|<span data-ttu-id="5c235-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5c235-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c235-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c235-123">Authorization</span></span>|<span data-ttu-id="5c235-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5c235-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c235-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5c235-125">Accept</span></span>|<span data-ttu-id="5c235-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c235-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c235-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5c235-127">Request body</span></span>
<span data-ttu-id="5c235-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) an.</span><span class="sxs-lookup"><span data-stu-id="5c235-128">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="5c235-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="5c235-129">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="5c235-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5c235-130">Property</span></span>|<span data-ttu-id="5c235-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5c235-131">Type</span></span>|<span data-ttu-id="5c235-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c235-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c235-133">id</span><span class="sxs-lookup"><span data-stu-id="5c235-133">id</span></span>|<span data-ttu-id="5c235-134">String</span><span class="sxs-lookup"><span data-stu-id="5c235-134">String</span></span>|<span data-ttu-id="5c235-135">Eindeutiger Bezeichner für das Zertifikat</span><span class="sxs-lookup"><span data-stu-id="5c235-135">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="5c235-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="5c235-136">appleIdentifier</span></span>|<span data-ttu-id="5c235-137">String</span><span class="sxs-lookup"><span data-stu-id="5c235-137">String</span></span>|<span data-ttu-id="5c235-138">Apple-ID des Kontos, mit dem das MDM-Push-Zertifikat erstellt wurde</span><span class="sxs-lookup"><span data-stu-id="5c235-138">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="5c235-139">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="5c235-139">topicIdentifier</span></span>|<span data-ttu-id="5c235-140">String</span><span class="sxs-lookup"><span data-stu-id="5c235-140">String</span></span>|<span data-ttu-id="5c235-141">Thema-ID</span><span class="sxs-lookup"><span data-stu-id="5c235-141">Topic Id.</span></span>|
|<span data-ttu-id="5c235-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c235-142">lastModifiedDateTime</span></span>|<span data-ttu-id="5c235-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c235-143">DateTimeOffset</span></span>|<span data-ttu-id="5c235-144">Datum und Uhrzeit der letzten Änderung des Apple Push Notification-Zertifikats</span><span class="sxs-lookup"><span data-stu-id="5c235-144">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="5c235-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5c235-145">expirationDateTime</span></span>|<span data-ttu-id="5c235-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c235-146">DateTimeOffset</span></span>|<span data-ttu-id="5c235-147">Datum und Uhrzeit des Ablaufs des Apple Push Notification-Zertifikats</span><span class="sxs-lookup"><span data-stu-id="5c235-147">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="5c235-148">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="5c235-148">certificateUploadStatus</span></span>|<span data-ttu-id="5c235-149">String</span><span class="sxs-lookup"><span data-stu-id="5c235-149">String</span></span>|<span data-ttu-id="5c235-150">Der Status des Zertifikats hochladen.</span><span class="sxs-lookup"><span data-stu-id="5c235-150">The certificate upload status.</span></span>|
|<span data-ttu-id="5c235-151">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="5c235-151">certificateUploadFailureReason</span></span>|<span data-ttu-id="5c235-152">String</span><span class="sxs-lookup"><span data-stu-id="5c235-152">String</span></span>|<span data-ttu-id="5c235-153">Der Grund dafür ist das Zertifikat Upload ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="5c235-153">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="5c235-154">certificate</span><span class="sxs-lookup"><span data-stu-id="5c235-154">certificate</span></span>|<span data-ttu-id="5c235-155">String</span><span class="sxs-lookup"><span data-stu-id="5c235-155">String</span></span>|<span data-ttu-id="5c235-156">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="5c235-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5c235-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c235-157">Response</span></span>
<span data-ttu-id="5c235-158">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5c235-158">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c235-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5c235-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c235-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c235-160">Request</span></span>
<span data-ttu-id="5c235-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5c235-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 409

{
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="5c235-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c235-162">Response</span></span>
<span data-ttu-id="5c235-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c235-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificate": "Certificate value"
}
```





