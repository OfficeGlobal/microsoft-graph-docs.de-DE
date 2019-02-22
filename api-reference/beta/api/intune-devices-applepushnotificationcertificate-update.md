---
title: Aktualisieren von „applePushNotificationCertificate“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs applePushNotificationCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee760b38c8f684c0ca7f0c8bcca0c98d8a87d931
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172044"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="f9e63-103">Aktualisieren von „applePushNotificationCertificate“</span><span class="sxs-lookup"><span data-stu-id="f9e63-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="f9e63-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f9e63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9e63-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f9e63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9e63-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="f9e63-106">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9e63-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f9e63-107">Prerequisites</span></span>
<span data-ttu-id="f9e63-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f9e63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f9e63-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f9e63-110">Permission type</span></span>|<span data-ttu-id="f9e63-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f9e63-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9e63-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f9e63-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9e63-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9e63-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f9e63-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f9e63-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9e63-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9e63-115">Not supported.</span></span>|
|<span data-ttu-id="f9e63-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f9e63-116">Application</span></span>|<span data-ttu-id="f9e63-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9e63-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9e63-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9e63-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="f9e63-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f9e63-119">Request headers</span></span>
|<span data-ttu-id="f9e63-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f9e63-120">Header</span></span>|<span data-ttu-id="f9e63-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f9e63-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9e63-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9e63-122">Authorization</span></span>|<span data-ttu-id="f9e63-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f9e63-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9e63-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f9e63-124">Accept</span></span>|<span data-ttu-id="f9e63-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9e63-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9e63-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f9e63-126">Request body</span></span>
<span data-ttu-id="f9e63-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) an.</span><span class="sxs-lookup"><span data-stu-id="f9e63-127">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="f9e63-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="f9e63-128">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="f9e63-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f9e63-129">Property</span></span>|<span data-ttu-id="f9e63-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f9e63-130">Type</span></span>|<span data-ttu-id="f9e63-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9e63-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9e63-132">id</span><span class="sxs-lookup"><span data-stu-id="f9e63-132">id</span></span>|<span data-ttu-id="f9e63-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9e63-133">String</span></span>|<span data-ttu-id="f9e63-134">Eindeutiger Bezeichner für das Zertifikat</span><span class="sxs-lookup"><span data-stu-id="f9e63-134">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="f9e63-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="f9e63-135">appleIdentifier</span></span>|<span data-ttu-id="f9e63-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9e63-136">String</span></span>|<span data-ttu-id="f9e63-137">Apple-ID des Kontos, mit dem das MDM-Push-Zertifikat erstellt wurde</span><span class="sxs-lookup"><span data-stu-id="f9e63-137">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="f9e63-138">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="f9e63-138">topicIdentifier</span></span>|<span data-ttu-id="f9e63-139">String</span><span class="sxs-lookup"><span data-stu-id="f9e63-139">String</span></span>|<span data-ttu-id="f9e63-140">Thema-ID</span><span class="sxs-lookup"><span data-stu-id="f9e63-140">Topic Id.</span></span>|
|<span data-ttu-id="f9e63-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9e63-141">lastModifiedDateTime</span></span>|<span data-ttu-id="f9e63-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9e63-142">DateTimeOffset</span></span>|<span data-ttu-id="f9e63-143">Datum und Uhrzeit der letzten Änderung des Apple Push Notification-Zertifikats</span><span class="sxs-lookup"><span data-stu-id="f9e63-143">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="f9e63-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f9e63-144">expirationDateTime</span></span>|<span data-ttu-id="f9e63-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9e63-145">DateTimeOffset</span></span>|<span data-ttu-id="f9e63-146">Datum und Uhrzeit des Ablaufs des Apple Push Notification-Zertifikats</span><span class="sxs-lookup"><span data-stu-id="f9e63-146">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="f9e63-147">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="f9e63-147">certificateUploadStatus</span></span>|<span data-ttu-id="f9e63-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9e63-148">String</span></span>|<span data-ttu-id="f9e63-149">Der Zertifikat Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="f9e63-149">The certificate upload status.</span></span>|
|<span data-ttu-id="f9e63-150">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="f9e63-150">certificateUploadFailureReason</span></span>|<span data-ttu-id="f9e63-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9e63-151">String</span></span>|<span data-ttu-id="f9e63-152">Der Grund, warum der Zertifikat Upload fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="f9e63-152">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="f9e63-153">certificate</span><span class="sxs-lookup"><span data-stu-id="f9e63-153">certificate</span></span>|<span data-ttu-id="f9e63-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9e63-154">String</span></span>|<span data-ttu-id="f9e63-155">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f9e63-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f9e63-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9e63-156">Response</span></span>
<span data-ttu-id="f9e63-157">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f9e63-157">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9e63-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f9e63-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9e63-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9e63-159">Request</span></span>
<span data-ttu-id="f9e63-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f9e63-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 416

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="f9e63-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9e63-161">Response</span></span>
<span data-ttu-id="f9e63-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f9e63-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




