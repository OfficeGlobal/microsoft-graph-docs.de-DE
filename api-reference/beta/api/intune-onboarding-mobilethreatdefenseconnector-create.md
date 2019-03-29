---
title: Erstellen von mobileThreatDefenseConnector
description: Erstellt neue Objekte des Typs mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30936d9ef9c89cc7859b5e649a7b125e40edf0b2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977674"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="13121-103">Erstellen von mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="13121-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="13121-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13121-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13121-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="13121-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13121-106">Erstellt neue Objekte des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="13121-106">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13121-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="13121-107">Prerequisites</span></span>
<span data-ttu-id="13121-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13121-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13121-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="13121-110">Permission type</span></span>|<span data-ttu-id="13121-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="13121-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13121-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="13121-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13121-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13121-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="13121-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="13121-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13121-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13121-115">Not supported.</span></span>|
|<span data-ttu-id="13121-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="13121-116">Application</span></span>|<span data-ttu-id="13121-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13121-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13121-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13121-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="13121-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="13121-119">Request headers</span></span>
|<span data-ttu-id="13121-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="13121-120">Header</span></span>|<span data-ttu-id="13121-121">Wert</span><span class="sxs-lookup"><span data-stu-id="13121-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13121-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="13121-122">Authorization</span></span>|<span data-ttu-id="13121-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="13121-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13121-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="13121-124">Accept</span></span>|<span data-ttu-id="13121-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13121-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13121-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="13121-126">Request body</span></span>
<span data-ttu-id="13121-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs mobileThreatDefenseConnector an.</span><span class="sxs-lookup"><span data-stu-id="13121-127">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="13121-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs mobileThreatDefenseConnector erstellen.</span><span class="sxs-lookup"><span data-stu-id="13121-128">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="13121-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13121-129">Property</span></span>|<span data-ttu-id="13121-130">Typ</span><span class="sxs-lookup"><span data-stu-id="13121-130">Type</span></span>|<span data-ttu-id="13121-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13121-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13121-132">id</span><span class="sxs-lookup"><span data-stu-id="13121-132">id</span></span>|<span data-ttu-id="13121-133">String</span><span class="sxs-lookup"><span data-stu-id="13121-133">String</span></span>|<span data-ttu-id="13121-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="13121-134">Not yet documented</span></span>|
|<span data-ttu-id="13121-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="13121-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="13121-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13121-136">DateTimeOffset</span></span>|<span data-ttu-id="13121-137">DateTime des letzten vom Datensynchronisierungspartner empfangenen Heartbeats</span><span class="sxs-lookup"><span data-stu-id="13121-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="13121-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="13121-138">partnerState</span></span>|[<span data-ttu-id="13121-139">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="13121-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="13121-140">Daten Synchronisierungs Partner Status für dieses Konto.</span><span class="sxs-lookup"><span data-stu-id="13121-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="13121-141">Mögliche Werte sind: `unavailable`, `available`, `enabled` und `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="13121-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="13121-142">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="13121-142">androidEnabled</span></span>|<span data-ttu-id="13121-143">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13121-143">Boolean</span></span>|<span data-ttu-id="13121-144">Legen Sie für Android fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="13121-144">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="13121-145">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="13121-145">iosEnabled</span></span>|<span data-ttu-id="13121-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13121-146">Boolean</span></span>|<span data-ttu-id="13121-147">Für iOS: Rufen Sie ab oder legen Sie fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="13121-147">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="13121-148">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="13121-148">windowsEnabled</span></span>|<span data-ttu-id="13121-149">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13121-149">Boolean</span></span>|<span data-ttu-id="13121-150">Für Windows: Abrufen oder festlegen, ob Daten vom Daten Synchronisierungspartner während der Konformitätsbewertung verwendet werden sollen</span><span class="sxs-lookup"><span data-stu-id="13121-150">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="13121-151">macEnabled</span><span class="sxs-lookup"><span data-stu-id="13121-151">macEnabled</span></span>|<span data-ttu-id="13121-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13121-152">Boolean</span></span>|<span data-ttu-id="13121-153">Für Mac: Abrufen oder festlegen, ob Daten vom Daten Synchronisierungspartner während der Konformitätsbewertung verwendet werden sollen</span><span class="sxs-lookup"><span data-stu-id="13121-153">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="13121-154">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="13121-154">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="13121-155">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13121-155">Boolean</span></span>|<span data-ttu-id="13121-156">Für Android: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.</span><span class="sxs-lookup"><span data-stu-id="13121-156">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="13121-157">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="13121-157">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="13121-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13121-158">Boolean</span></span>|<span data-ttu-id="13121-159">Für iOS: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.</span><span class="sxs-lookup"><span data-stu-id="13121-159">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="13121-160">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="13121-160">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="13121-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13121-161">Boolean</span></span>|<span data-ttu-id="13121-162">Legen Sie unter Windows fest, ob InTune Daten vom Daten Synchronisierungspartner empfangen muss, bevor ein Gerät kompatibel markiert wird.</span><span class="sxs-lookup"><span data-stu-id="13121-162">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="13121-163">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="13121-163">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="13121-164">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13121-164">Boolean</span></span>|<span data-ttu-id="13121-165">Für Mac: Abrufen oder festlegen, ob InTune Daten vom Daten Synchronisierungspartner empfangen muss, bevor ein Gerät kompatibel markiert wird.</span><span class="sxs-lookup"><span data-stu-id="13121-165">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="13121-166">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="13121-166">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="13121-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="13121-167">Boolean</span></span>|<span data-ttu-id="13121-168">Rufen Sie ab bzw. legen Sie fest, ob Geräte auf den aktivierten Plattformen, die nicht die Mindestversionsanforderungen des Datensynchronisierungspartners erfüllen, blockiert werden.</span><span class="sxs-lookup"><span data-stu-id="13121-168">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="13121-169">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="13121-169">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="13121-170">Int32</span><span class="sxs-lookup"><span data-stu-id="13121-170">Int32</span></span>|<span data-ttu-id="13121-171">Erlaubt das Abrufen oder das Festlegen des für die betreffende Partnerintegration geltenden Zeitraums in Tagen, während dessen ein Nichtreagieren des Mandanten toleriert wird.</span><span class="sxs-lookup"><span data-stu-id="13121-171">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="13121-172">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="13121-172">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="13121-173">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13121-173">Boolean</span></span>|<span data-ttu-id="13121-174">Ermöglicht dem Administrator für IOS-Geräte, zu konfigurieren, ob der Daten Synchronisierungspartner auch Metadaten zu installierten Anwendungen von InTune erfassen kann.</span><span class="sxs-lookup"><span data-stu-id="13121-174">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="13121-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="13121-175">Response</span></span>
<span data-ttu-id="13121-176">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="13121-176">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13121-177">Beispiel</span><span class="sxs-lookup"><span data-stu-id="13121-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="13121-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="13121-178">Request</span></span>
<span data-ttu-id="13121-179">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="13121-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
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

### <a name="response"></a><span data-ttu-id="13121-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="13121-180">Response</span></span>
<span data-ttu-id="13121-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="13121-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




