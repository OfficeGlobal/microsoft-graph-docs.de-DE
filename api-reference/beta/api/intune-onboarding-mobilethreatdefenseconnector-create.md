---
title: Erstellen von mobileThreatDefenseConnector
description: Erstellt neue Objekte des Typs mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 056e732835fc14a56381796d7a42195300175b99
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934198"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="e614c-103">Erstellen von mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="e614c-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="e614c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e614c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e614c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e614c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e614c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e614c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e614c-107">Erstellt neue Objekte des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="e614c-107">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e614c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e614c-108">Prerequisites</span></span>
<span data-ttu-id="e614c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e614c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e614c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e614c-111">Permission type</span></span>|<span data-ttu-id="e614c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e614c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e614c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e614c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e614c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e614c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e614c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e614c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e614c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e614c-116">Not supported.</span></span>|
|<span data-ttu-id="e614c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e614c-117">Application</span></span>|<span data-ttu-id="e614c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e614c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e614c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e614c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="e614c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e614c-120">Request headers</span></span>
|<span data-ttu-id="e614c-121">Header</span><span class="sxs-lookup"><span data-stu-id="e614c-121">Header</span></span>|<span data-ttu-id="e614c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e614c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e614c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e614c-123">Authorization</span></span>|<span data-ttu-id="e614c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e614c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e614c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e614c-125">Accept</span></span>|<span data-ttu-id="e614c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e614c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e614c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e614c-127">Request body</span></span>
<span data-ttu-id="e614c-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs mobileThreatDefenseConnector an.</span><span class="sxs-lookup"><span data-stu-id="e614c-128">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="e614c-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs mobileThreatDefenseConnector erstellen.</span><span class="sxs-lookup"><span data-stu-id="e614c-129">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="e614c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e614c-130">Property</span></span>|<span data-ttu-id="e614c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e614c-131">Type</span></span>|<span data-ttu-id="e614c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e614c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e614c-133">id</span><span class="sxs-lookup"><span data-stu-id="e614c-133">id</span></span>|<span data-ttu-id="e614c-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e614c-134">String</span></span>|<span data-ttu-id="e614c-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e614c-135">Not yet documented</span></span>|
|<span data-ttu-id="e614c-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="e614c-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="e614c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e614c-137">DateTimeOffset</span></span>|<span data-ttu-id="e614c-138">DateTime des letzten vom Datensynchronisierungspartner empfangenen Heartbeats</span><span class="sxs-lookup"><span data-stu-id="e614c-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="e614c-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="e614c-139">partnerState</span></span>|[<span data-ttu-id="e614c-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="e614c-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="e614c-141">Daten Sync Partner Zustand für dieses Konto.</span><span class="sxs-lookup"><span data-stu-id="e614c-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="e614c-142">Mögliche Werte: sind `unavailable`, `available`, `enabled` und `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="e614c-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="e614c-143">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="e614c-143">androidEnabled</span></span>|<span data-ttu-id="e614c-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="e614c-144">Boolean</span></span>|<span data-ttu-id="e614c-145">Legen Sie für Android fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e614c-145">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="e614c-146">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="e614c-146">iosEnabled</span></span>|<span data-ttu-id="e614c-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="e614c-147">Boolean</span></span>|<span data-ttu-id="e614c-148">Für iOS: Rufen Sie ab oder legen Sie fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e614c-148">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="e614c-149">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="e614c-149">windowsEnabled</span></span>|<span data-ttu-id="e614c-150">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e614c-150">Boolean</span></span>|<span data-ttu-id="e614c-151">Abzurufen Sie für Windows oder festzulegen Sie, ob die Daten aus der Daten Sync Partner beim Testen der Kompatibilität verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="e614c-151">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="e614c-152">macEnabled</span><span class="sxs-lookup"><span data-stu-id="e614c-152">macEnabled</span></span>|<span data-ttu-id="e614c-153">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e614c-153">Boolean</span></span>|<span data-ttu-id="e614c-154">Abzurufen Sie für Mac oder festzulegen Sie, ob die Daten aus der Daten Sync Partner beim Testen der Kompatibilität verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="e614c-154">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="e614c-155">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="e614c-155">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="e614c-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="e614c-156">Boolean</span></span>|<span data-ttu-id="e614c-157">Für Android: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.</span><span class="sxs-lookup"><span data-stu-id="e614c-157">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="e614c-158">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="e614c-158">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="e614c-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="e614c-159">Boolean</span></span>|<span data-ttu-id="e614c-160">Für iOS: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.</span><span class="sxs-lookup"><span data-stu-id="e614c-160">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="e614c-161">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="e614c-161">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="e614c-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e614c-162">Boolean</span></span>|<span data-ttu-id="e614c-163">Festlegen Sie für Windows, ob Intune Daten vom Partner Sync Daten vor der Markierung ein Gerät kompatible empfangen muss</span><span class="sxs-lookup"><span data-stu-id="e614c-163">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="e614c-164">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="e614c-164">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="e614c-165">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e614c-165">Boolean</span></span>|<span data-ttu-id="e614c-166">Abzurufen Sie für Mac oder festzulegen Sie, ob Intune Daten vom Partner Sync Daten vor der Markierung ein Gerät kompatible empfangen muss</span><span class="sxs-lookup"><span data-stu-id="e614c-166">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="e614c-167">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="e614c-167">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="e614c-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="e614c-168">Boolean</span></span>|<span data-ttu-id="e614c-169">Rufen Sie ab bzw. legen Sie fest, ob Geräte auf den aktivierten Plattformen, die nicht die Mindestversionsanforderungen des Datensynchronisierungspartners erfüllen, blockiert werden.</span><span class="sxs-lookup"><span data-stu-id="e614c-169">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="e614c-170">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="e614c-170">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="e614c-171">Int32</span><span class="sxs-lookup"><span data-stu-id="e614c-171">Int32</span></span>|<span data-ttu-id="e614c-172">Erlaubt das Abrufen oder das Festlegen des für die betreffende Partnerintegration geltenden Zeitraums in Tagen, während dessen ein Nichtreagieren des Mandanten toleriert wird.</span><span class="sxs-lookup"><span data-stu-id="e614c-172">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="e614c-173">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="e614c-173">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="e614c-174">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e614c-174">Boolean</span></span>|<span data-ttu-id="e614c-175">IOS-Geräte ermöglicht den Administrator konfigurieren können, ob der Daten Sync Partner auch Metadaten für die installierten Programme auf Intune erfassen möglicherweise</span><span class="sxs-lookup"><span data-stu-id="e614c-175">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="e614c-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="e614c-176">Response</span></span>
<span data-ttu-id="e614c-177">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e614c-177">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e614c-178">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e614c-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="e614c-179">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e614c-179">Request</span></span>
<span data-ttu-id="e614c-180">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e614c-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e614c-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="e614c-181">Response</span></span>
<span data-ttu-id="e614c-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e614c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





