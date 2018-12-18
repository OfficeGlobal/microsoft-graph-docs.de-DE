---
title: mobileThreatDefenseConnector aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs mobileThreatDefenseConnector.
author: tfitzmac
ms.openlocfilehash: bd53fb377adb160db1700b088e293217bdee5292
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313944"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="01cbc-103">mobileThreatDefenseConnector aktualisieren</span><span class="sxs-lookup"><span data-stu-id="01cbc-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="01cbc-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="01cbc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01cbc-105">Aktualisiert die Eigenschaften von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="01cbc-105">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01cbc-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="01cbc-106">Prerequisites</span></span>
<span data-ttu-id="01cbc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01cbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01cbc-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="01cbc-109">Permission type</span></span>|<span data-ttu-id="01cbc-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="01cbc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01cbc-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="01cbc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="01cbc-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01cbc-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="01cbc-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="01cbc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01cbc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="01cbc-114">Not supported.</span></span>|
|<span data-ttu-id="01cbc-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="01cbc-115">Application</span></span>|<span data-ttu-id="01cbc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="01cbc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01cbc-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="01cbc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="01cbc-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="01cbc-118">Request headers</span></span>
|<span data-ttu-id="01cbc-119">Header</span><span class="sxs-lookup"><span data-stu-id="01cbc-119">Header</span></span>|<span data-ttu-id="01cbc-120">Wert</span><span class="sxs-lookup"><span data-stu-id="01cbc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01cbc-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="01cbc-121">Authorization</span></span>|<span data-ttu-id="01cbc-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="01cbc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01cbc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="01cbc-123">Accept</span></span>|<span data-ttu-id="01cbc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="01cbc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01cbc-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="01cbc-125">Request body</span></span>
<span data-ttu-id="01cbc-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) an.</span><span class="sxs-lookup"><span data-stu-id="01cbc-126">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="01cbc-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="01cbc-127">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="01cbc-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="01cbc-128">Property</span></span>|<span data-ttu-id="01cbc-129">Typ</span><span class="sxs-lookup"><span data-stu-id="01cbc-129">Type</span></span>|<span data-ttu-id="01cbc-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="01cbc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01cbc-131">id</span><span class="sxs-lookup"><span data-stu-id="01cbc-131">id</span></span>|<span data-ttu-id="01cbc-132">String</span><span class="sxs-lookup"><span data-stu-id="01cbc-132">String</span></span>|<span data-ttu-id="01cbc-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="01cbc-133">Not yet documented</span></span>|
|<span data-ttu-id="01cbc-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="01cbc-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="01cbc-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01cbc-135">DateTimeOffset</span></span>|<span data-ttu-id="01cbc-136">DateTime des letzten vom Datensynchronisierungspartner empfangenen Heartbeats</span><span class="sxs-lookup"><span data-stu-id="01cbc-136">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="01cbc-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="01cbc-137">partnerState</span></span>|[<span data-ttu-id="01cbc-138">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="01cbc-138">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="01cbc-139">Daten Sync Partner Zustand für dieses Konto.</span><span class="sxs-lookup"><span data-stu-id="01cbc-139">Data Sync Partner state for this account.</span></span> <span data-ttu-id="01cbc-140">Mögliche Werte: sind `unavailable`, `available`, `enabled` und `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="01cbc-140">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="01cbc-141">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="01cbc-141">androidEnabled</span></span>|<span data-ttu-id="01cbc-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="01cbc-142">Boolean</span></span>|<span data-ttu-id="01cbc-143">Legen Sie für Android fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="01cbc-143">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="01cbc-144">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="01cbc-144">iosEnabled</span></span>|<span data-ttu-id="01cbc-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="01cbc-145">Boolean</span></span>|<span data-ttu-id="01cbc-146">Für iOS: Rufen Sie ab oder legen Sie fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="01cbc-146">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="01cbc-147">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="01cbc-147">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="01cbc-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="01cbc-148">Boolean</span></span>|<span data-ttu-id="01cbc-149">Für Android: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.</span><span class="sxs-lookup"><span data-stu-id="01cbc-149">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="01cbc-150">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="01cbc-150">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="01cbc-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="01cbc-151">Boolean</span></span>|<span data-ttu-id="01cbc-152">Für iOS: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.</span><span class="sxs-lookup"><span data-stu-id="01cbc-152">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="01cbc-153">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="01cbc-153">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="01cbc-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="01cbc-154">Boolean</span></span>|<span data-ttu-id="01cbc-155">Rufen Sie ab bzw. legen Sie fest, ob Geräte auf den aktivierten Plattformen, die nicht die Mindestversionsanforderungen des Datensynchronisierungspartners erfüllen, blockiert werden.</span><span class="sxs-lookup"><span data-stu-id="01cbc-155">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="01cbc-156">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="01cbc-156">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="01cbc-157">Int32</span><span class="sxs-lookup"><span data-stu-id="01cbc-157">Int32</span></span>|<span data-ttu-id="01cbc-158">Erlaubt das Abrufen oder das Festlegen des für die betreffende Partnerintegration geltenden Zeitraums in Tagen, während dessen ein Nichtreagieren des Mandanten toleriert wird.</span><span class="sxs-lookup"><span data-stu-id="01cbc-158">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="01cbc-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="01cbc-159">Response</span></span>
<span data-ttu-id="01cbc-160">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="01cbc-160">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01cbc-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="01cbc-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="01cbc-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="01cbc-162">Request</span></span>
<span data-ttu-id="01cbc-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="01cbc-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="01cbc-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="01cbc-164">Response</span></span>
<span data-ttu-id="01cbc-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="01cbc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



