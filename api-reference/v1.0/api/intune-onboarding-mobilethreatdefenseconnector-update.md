---
title: mobileThreatDefenseConnector aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4b44062d2480a739cccf7501d4cfd41f2d977f0
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957248"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="81c87-103">mobileThreatDefenseConnector aktualisieren</span><span class="sxs-lookup"><span data-stu-id="81c87-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="81c87-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="81c87-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81c87-105">Aktualisiert die Eigenschaften von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="81c87-105">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81c87-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="81c87-106">Prerequisites</span></span>
<span data-ttu-id="81c87-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81c87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81c87-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="81c87-109">Permission type</span></span>|<span data-ttu-id="81c87-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="81c87-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81c87-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="81c87-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81c87-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81c87-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="81c87-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="81c87-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81c87-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="81c87-114">Not supported.</span></span>|
|<span data-ttu-id="81c87-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="81c87-115">Application</span></span>|<span data-ttu-id="81c87-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="81c87-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81c87-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="81c87-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="81c87-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="81c87-118">Request headers</span></span>
|<span data-ttu-id="81c87-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="81c87-119">Header</span></span>|<span data-ttu-id="81c87-120">Wert</span><span class="sxs-lookup"><span data-stu-id="81c87-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81c87-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="81c87-121">Authorization</span></span>|<span data-ttu-id="81c87-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="81c87-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81c87-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="81c87-123">Accept</span></span>|<span data-ttu-id="81c87-124">application/json</span><span class="sxs-lookup"><span data-stu-id="81c87-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81c87-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="81c87-125">Request body</span></span>
<span data-ttu-id="81c87-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) an.</span><span class="sxs-lookup"><span data-stu-id="81c87-126">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="81c87-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="81c87-127">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="81c87-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="81c87-128">Property</span></span>|<span data-ttu-id="81c87-129">Typ</span><span class="sxs-lookup"><span data-stu-id="81c87-129">Type</span></span>|<span data-ttu-id="81c87-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81c87-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81c87-131">id</span><span class="sxs-lookup"><span data-stu-id="81c87-131">id</span></span>|<span data-ttu-id="81c87-132">String</span><span class="sxs-lookup"><span data-stu-id="81c87-132">String</span></span>|<span data-ttu-id="81c87-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="81c87-133">Not yet documented</span></span>|
|<span data-ttu-id="81c87-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="81c87-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="81c87-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81c87-135">DateTimeOffset</span></span>|<span data-ttu-id="81c87-136">DateTime des letzten vom Datensynchronisierungspartner empfangenen Heartbeats</span><span class="sxs-lookup"><span data-stu-id="81c87-136">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="81c87-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="81c87-137">partnerState</span></span>|[<span data-ttu-id="81c87-138">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="81c87-138">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="81c87-139">Daten Synchronisierungs Partner Status für dieses Konto.</span><span class="sxs-lookup"><span data-stu-id="81c87-139">Data Sync Partner state for this account.</span></span> <span data-ttu-id="81c87-140">Mögliche Werte sind: `unavailable`, `available`, `enabled` und `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="81c87-140">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="81c87-141">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="81c87-141">androidEnabled</span></span>|<span data-ttu-id="81c87-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="81c87-142">Boolean</span></span>|<span data-ttu-id="81c87-143">Legen Sie für Android fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="81c87-143">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="81c87-144">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="81c87-144">iosEnabled</span></span>|<span data-ttu-id="81c87-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="81c87-145">Boolean</span></span>|<span data-ttu-id="81c87-146">Für iOS: Rufen Sie ab oder legen Sie fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="81c87-146">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="81c87-147">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="81c87-147">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="81c87-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="81c87-148">Boolean</span></span>|<span data-ttu-id="81c87-149">Für Android: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.</span><span class="sxs-lookup"><span data-stu-id="81c87-149">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="81c87-150">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="81c87-150">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="81c87-151">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="81c87-151">Boolean</span></span>|<span data-ttu-id="81c87-152">Für iOS: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.</span><span class="sxs-lookup"><span data-stu-id="81c87-152">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="81c87-153">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="81c87-153">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="81c87-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="81c87-154">Boolean</span></span>|<span data-ttu-id="81c87-155">Rufen Sie ab bzw. legen Sie fest, ob Geräte auf den aktivierten Plattformen, die nicht die Mindestversionsanforderungen des Datensynchronisierungspartners erfüllen, blockiert werden.</span><span class="sxs-lookup"><span data-stu-id="81c87-155">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="81c87-156">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="81c87-156">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="81c87-157">Int32</span><span class="sxs-lookup"><span data-stu-id="81c87-157">Int32</span></span>|<span data-ttu-id="81c87-158">Erlaubt das Abrufen oder das Festlegen des für die betreffende Partnerintegration geltenden Zeitraums in Tagen, während dessen ein Nichtreagieren des Mandanten toleriert wird.</span><span class="sxs-lookup"><span data-stu-id="81c87-158">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="81c87-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="81c87-159">Response</span></span>
<span data-ttu-id="81c87-160">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="81c87-160">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81c87-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="81c87-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="81c87-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="81c87-162">Request</span></span>
<span data-ttu-id="81c87-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="81c87-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a><span data-ttu-id="81c87-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="81c87-164">Response</span></span>
<span data-ttu-id="81c87-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="81c87-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```



