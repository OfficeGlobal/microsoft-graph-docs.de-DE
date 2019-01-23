---
title: mobileThreatDefenseConnector aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs mobileThreatDefenseConnector.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c8ed44a29f3e56f602689b58e3f58071998cde21
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411211"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="bf619-103">mobileThreatDefenseConnector aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bf619-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="bf619-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="bf619-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bf619-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bf619-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf619-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bf619-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf619-107">Aktualisiert die Eigenschaften von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="bf619-107">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf619-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bf619-108">Prerequisites</span></span>
<span data-ttu-id="bf619-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bf619-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bf619-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bf619-111">Permission type</span></span>|<span data-ttu-id="bf619-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bf619-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf619-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bf619-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf619-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf619-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bf619-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bf619-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf619-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf619-116">Not supported.</span></span>|
|<span data-ttu-id="bf619-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bf619-117">Application</span></span>|<span data-ttu-id="bf619-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf619-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf619-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf619-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="bf619-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bf619-120">Request headers</span></span>
|<span data-ttu-id="bf619-121">Header</span><span class="sxs-lookup"><span data-stu-id="bf619-121">Header</span></span>|<span data-ttu-id="bf619-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bf619-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf619-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="bf619-123">Authorization</span></span>|<span data-ttu-id="bf619-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bf619-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf619-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bf619-125">Accept</span></span>|<span data-ttu-id="bf619-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bf619-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf619-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bf619-127">Request body</span></span>
<span data-ttu-id="bf619-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) an.</span><span class="sxs-lookup"><span data-stu-id="bf619-128">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="bf619-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="bf619-129">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="bf619-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bf619-130">Property</span></span>|<span data-ttu-id="bf619-131">Typ</span><span class="sxs-lookup"><span data-stu-id="bf619-131">Type</span></span>|<span data-ttu-id="bf619-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf619-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf619-133">id</span><span class="sxs-lookup"><span data-stu-id="bf619-133">id</span></span>|<span data-ttu-id="bf619-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bf619-134">String</span></span>|<span data-ttu-id="bf619-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bf619-135">Not yet documented</span></span>|
|<span data-ttu-id="bf619-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="bf619-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="bf619-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf619-137">DateTimeOffset</span></span>|<span data-ttu-id="bf619-138">DateTime des letzten vom Datensynchronisierungspartner empfangenen Heartbeats</span><span class="sxs-lookup"><span data-stu-id="bf619-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="bf619-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="bf619-139">partnerState</span></span>|[<span data-ttu-id="bf619-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="bf619-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="bf619-141">Daten Sync Partner Zustand für dieses Konto.</span><span class="sxs-lookup"><span data-stu-id="bf619-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="bf619-142">Mögliche Werte: sind `unavailable`, `available`, `enabled` und `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="bf619-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="bf619-143">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="bf619-143">androidEnabled</span></span>|<span data-ttu-id="bf619-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf619-144">Boolean</span></span>|<span data-ttu-id="bf619-145">Legen Sie für Android fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="bf619-145">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="bf619-146">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="bf619-146">iosEnabled</span></span>|<span data-ttu-id="bf619-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf619-147">Boolean</span></span>|<span data-ttu-id="bf619-148">Für iOS: Rufen Sie ab oder legen Sie fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="bf619-148">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="bf619-149">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="bf619-149">windowsEnabled</span></span>|<span data-ttu-id="bf619-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf619-150">Boolean</span></span>|<span data-ttu-id="bf619-151">Abzurufen Sie für Windows oder festzulegen Sie, ob die Daten aus der Daten Sync Partner beim Testen der Kompatibilität verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="bf619-151">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="bf619-152">macEnabled</span><span class="sxs-lookup"><span data-stu-id="bf619-152">macEnabled</span></span>|<span data-ttu-id="bf619-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf619-153">Boolean</span></span>|<span data-ttu-id="bf619-154">Abzurufen Sie für Mac oder festzulegen Sie, ob die Daten aus der Daten Sync Partner beim Testen der Kompatibilität verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="bf619-154">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="bf619-155">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="bf619-155">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="bf619-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf619-156">Boolean</span></span>|<span data-ttu-id="bf619-157">Für Android: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.</span><span class="sxs-lookup"><span data-stu-id="bf619-157">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="bf619-158">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="bf619-158">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="bf619-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf619-159">Boolean</span></span>|<span data-ttu-id="bf619-160">Für iOS: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.</span><span class="sxs-lookup"><span data-stu-id="bf619-160">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="bf619-161">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="bf619-161">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="bf619-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf619-162">Boolean</span></span>|<span data-ttu-id="bf619-163">Festlegen Sie für Windows, ob Intune Daten vom Partner Sync Daten vor der Markierung ein Gerät kompatible empfangen muss</span><span class="sxs-lookup"><span data-stu-id="bf619-163">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="bf619-164">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="bf619-164">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="bf619-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf619-165">Boolean</span></span>|<span data-ttu-id="bf619-166">Abzurufen Sie für Mac oder festzulegen Sie, ob Intune Daten vom Partner Sync Daten vor der Markierung ein Gerät kompatible empfangen muss</span><span class="sxs-lookup"><span data-stu-id="bf619-166">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="bf619-167">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="bf619-167">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="bf619-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf619-168">Boolean</span></span>|<span data-ttu-id="bf619-169">Rufen Sie ab bzw. legen Sie fest, ob Geräte auf den aktivierten Plattformen, die nicht die Mindestversionsanforderungen des Datensynchronisierungspartners erfüllen, blockiert werden.</span><span class="sxs-lookup"><span data-stu-id="bf619-169">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="bf619-170">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="bf619-170">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="bf619-171">Int32</span><span class="sxs-lookup"><span data-stu-id="bf619-171">Int32</span></span>|<span data-ttu-id="bf619-172">Erlaubt das Abrufen oder das Festlegen des für die betreffende Partnerintegration geltenden Zeitraums in Tagen, während dessen ein Nichtreagieren des Mandanten toleriert wird.</span><span class="sxs-lookup"><span data-stu-id="bf619-172">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="bf619-173">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="bf619-173">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="bf619-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf619-174">Boolean</span></span>|<span data-ttu-id="bf619-175">IOS-Geräte ermöglicht den Administrator konfigurieren können, ob der Daten Sync Partner auch Metadaten für die installierten Programme auf Intune erfassen möglicherweise</span><span class="sxs-lookup"><span data-stu-id="bf619-175">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="bf619-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf619-176">Response</span></span>
<span data-ttu-id="bf619-177">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bf619-177">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf619-178">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bf619-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf619-179">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf619-179">Request</span></span>
<span data-ttu-id="bf619-180">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bf619-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 622

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```

### <a name="response"></a><span data-ttu-id="bf619-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf619-181">Response</span></span>
<span data-ttu-id="bf619-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bf619-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 671

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```




