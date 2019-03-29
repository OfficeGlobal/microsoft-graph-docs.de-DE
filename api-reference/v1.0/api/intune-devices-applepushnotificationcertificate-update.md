---
title: Aktualisieren von „applePushNotificationCertificate“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs applePushNotificationCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8bd100c743a79cb5a622e047dd4dcdac8441f6eb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30956940"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="9e771-103">Aktualisieren von „applePushNotificationCertificate“</span><span class="sxs-lookup"><span data-stu-id="9e771-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="9e771-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9e771-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e771-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="9e771-105">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e771-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9e771-106">Prerequisites</span></span>
<span data-ttu-id="9e771-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e771-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e771-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9e771-109">Permission type</span></span>|<span data-ttu-id="9e771-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9e771-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e771-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9e771-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9e771-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e771-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9e771-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9e771-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e771-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e771-114">Not supported.</span></span>|
|<span data-ttu-id="9e771-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9e771-115">Application</span></span>|<span data-ttu-id="9e771-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e771-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e771-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e771-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="9e771-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9e771-118">Request headers</span></span>
|<span data-ttu-id="9e771-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9e771-119">Header</span></span>|<span data-ttu-id="9e771-120">Wert</span><span class="sxs-lookup"><span data-stu-id="9e771-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e771-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e771-121">Authorization</span></span>|<span data-ttu-id="9e771-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9e771-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e771-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9e771-123">Accept</span></span>|<span data-ttu-id="9e771-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9e771-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e771-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9e771-125">Request body</span></span>
<span data-ttu-id="9e771-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) an.</span><span class="sxs-lookup"><span data-stu-id="9e771-126">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="9e771-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="9e771-127">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="9e771-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9e771-128">Property</span></span>|<span data-ttu-id="9e771-129">Typ</span><span class="sxs-lookup"><span data-stu-id="9e771-129">Type</span></span>|<span data-ttu-id="9e771-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e771-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e771-131">id</span><span class="sxs-lookup"><span data-stu-id="9e771-131">id</span></span>|<span data-ttu-id="9e771-132">String</span><span class="sxs-lookup"><span data-stu-id="9e771-132">String</span></span>|<span data-ttu-id="9e771-133">Eindeutiger Bezeichner für das Zertifikat</span><span class="sxs-lookup"><span data-stu-id="9e771-133">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="9e771-134">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="9e771-134">appleIdentifier</span></span>|<span data-ttu-id="9e771-135">String</span><span class="sxs-lookup"><span data-stu-id="9e771-135">String</span></span>|<span data-ttu-id="9e771-136">Apple-ID des Kontos, mit dem das MDM-Push-Zertifikat erstellt wurde</span><span class="sxs-lookup"><span data-stu-id="9e771-136">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="9e771-137">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="9e771-137">topicIdentifier</span></span>|<span data-ttu-id="9e771-138">String</span><span class="sxs-lookup"><span data-stu-id="9e771-138">String</span></span>|<span data-ttu-id="9e771-139">Thema-ID</span><span class="sxs-lookup"><span data-stu-id="9e771-139">Topic Id.</span></span>|
|<span data-ttu-id="9e771-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e771-140">lastModifiedDateTime</span></span>|<span data-ttu-id="9e771-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e771-141">DateTimeOffset</span></span>|<span data-ttu-id="9e771-142">Datum und Uhrzeit der letzten Änderung des Apple Push Notification-Zertifikats</span><span class="sxs-lookup"><span data-stu-id="9e771-142">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="9e771-143">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9e771-143">expirationDateTime</span></span>|<span data-ttu-id="9e771-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e771-144">DateTimeOffset</span></span>|<span data-ttu-id="9e771-145">Datum und Uhrzeit des Ablaufs des Apple Push Notification-Zertifikats</span><span class="sxs-lookup"><span data-stu-id="9e771-145">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="9e771-146">certificate</span><span class="sxs-lookup"><span data-stu-id="9e771-146">certificate</span></span>|<span data-ttu-id="9e771-147">String</span><span class="sxs-lookup"><span data-stu-id="9e771-147">String</span></span>|<span data-ttu-id="9e771-148">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="9e771-148">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9e771-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e771-149">Response</span></span>
<span data-ttu-id="9e771-150">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9e771-150">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e771-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9e771-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e771-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e771-152">Request</span></span>
<span data-ttu-id="9e771-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9e771-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="9e771-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e771-154">Response</span></span>
<span data-ttu-id="9e771-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9e771-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 384

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```



