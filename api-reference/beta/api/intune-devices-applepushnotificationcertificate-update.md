---
title: Aktualisieren von „applePushNotificationCertificate“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs applePushNotificationCertificate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e14e4056f0428548e0b910c8647dc4442efe4abd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397484"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="1e4b6-103">Aktualisieren von „applePushNotificationCertificate“</span><span class="sxs-lookup"><span data-stu-id="1e4b6-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="1e4b6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1e4b6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1e4b6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1e4b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e4b6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1e4b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e4b6-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="1e4b6-107">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e4b6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1e4b6-108">Prerequisites</span></span>
<span data-ttu-id="1e4b6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1e4b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1e4b6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1e4b6-111">Permission type</span></span>|<span data-ttu-id="1e4b6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1e4b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e4b6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1e4b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e4b6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e4b6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1e4b6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1e4b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e4b6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e4b6-116">Not supported.</span></span>|
|<span data-ttu-id="1e4b6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1e4b6-117">Application</span></span>|<span data-ttu-id="1e4b6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e4b6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e4b6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e4b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="1e4b6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1e4b6-120">Request headers</span></span>
|<span data-ttu-id="1e4b6-121">Header</span><span class="sxs-lookup"><span data-stu-id="1e4b6-121">Header</span></span>|<span data-ttu-id="1e4b6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1e4b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e4b6-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1e4b6-123">Authorization</span></span>|<span data-ttu-id="1e4b6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1e4b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e4b6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1e4b6-125">Accept</span></span>|<span data-ttu-id="1e4b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e4b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e4b6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1e4b6-127">Request body</span></span>
<span data-ttu-id="1e4b6-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) an.</span><span class="sxs-lookup"><span data-stu-id="1e4b6-128">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="1e4b6-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="1e4b6-129">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="1e4b6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1e4b6-130">Property</span></span>|<span data-ttu-id="1e4b6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1e4b6-131">Type</span></span>|<span data-ttu-id="1e4b6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e4b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e4b6-133">id</span><span class="sxs-lookup"><span data-stu-id="1e4b6-133">id</span></span>|<span data-ttu-id="1e4b6-134">String</span><span class="sxs-lookup"><span data-stu-id="1e4b6-134">String</span></span>|<span data-ttu-id="1e4b6-135">Eindeutiger Bezeichner für das Zertifikat</span><span class="sxs-lookup"><span data-stu-id="1e4b6-135">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="1e4b6-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="1e4b6-136">appleIdentifier</span></span>|<span data-ttu-id="1e4b6-137">String</span><span class="sxs-lookup"><span data-stu-id="1e4b6-137">String</span></span>|<span data-ttu-id="1e4b6-138">Apple-ID des Kontos, mit dem das MDM-Push-Zertifikat erstellt wurde</span><span class="sxs-lookup"><span data-stu-id="1e4b6-138">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="1e4b6-139">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="1e4b6-139">topicIdentifier</span></span>|<span data-ttu-id="1e4b6-140">String</span><span class="sxs-lookup"><span data-stu-id="1e4b6-140">String</span></span>|<span data-ttu-id="1e4b6-141">Thema-ID</span><span class="sxs-lookup"><span data-stu-id="1e4b6-141">Topic Id.</span></span>|
|<span data-ttu-id="1e4b6-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e4b6-142">lastModifiedDateTime</span></span>|<span data-ttu-id="1e4b6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e4b6-143">DateTimeOffset</span></span>|<span data-ttu-id="1e4b6-144">Datum und Uhrzeit der letzten Änderung des Apple Push Notification-Zertifikats</span><span class="sxs-lookup"><span data-stu-id="1e4b6-144">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="1e4b6-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1e4b6-145">expirationDateTime</span></span>|<span data-ttu-id="1e4b6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e4b6-146">DateTimeOffset</span></span>|<span data-ttu-id="1e4b6-147">Datum und Uhrzeit des Ablaufs des Apple Push Notification-Zertifikats</span><span class="sxs-lookup"><span data-stu-id="1e4b6-147">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="1e4b6-148">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="1e4b6-148">certificateUploadStatus</span></span>|<span data-ttu-id="1e4b6-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e4b6-149">String</span></span>|<span data-ttu-id="1e4b6-150">Der Status des Zertifikats hochladen.</span><span class="sxs-lookup"><span data-stu-id="1e4b6-150">The certificate upload status.</span></span>|
|<span data-ttu-id="1e4b6-151">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="1e4b6-151">certificateUploadFailureReason</span></span>|<span data-ttu-id="1e4b6-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e4b6-152">String</span></span>|<span data-ttu-id="1e4b6-153">Der Grund dafür ist das Zertifikat Upload ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="1e4b6-153">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="1e4b6-154">certificate</span><span class="sxs-lookup"><span data-stu-id="1e4b6-154">certificate</span></span>|<span data-ttu-id="1e4b6-155">String</span><span class="sxs-lookup"><span data-stu-id="1e4b6-155">String</span></span>|<span data-ttu-id="1e4b6-156">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1e4b6-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1e4b6-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e4b6-157">Response</span></span>
<span data-ttu-id="1e4b6-158">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1e4b6-158">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e4b6-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1e4b6-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e4b6-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e4b6-160">Request</span></span>
<span data-ttu-id="1e4b6-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1e4b6-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1e4b6-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e4b6-162">Response</span></span>
<span data-ttu-id="1e4b6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e4b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




