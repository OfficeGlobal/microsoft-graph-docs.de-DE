---
title: Erstellen von „androidManagedAppRegistration“
description: Diese Methode erstellt ein neues Objekt des Typs androidManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f95b47292c5fb018e5406278fda84c8d6a15034a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890377"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="ed116-103">Erstellen von „androidManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="ed116-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="ed116-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ed116-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed116-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed116-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed116-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ed116-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed116-107">Diese Methode erstellt ein neues Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ed116-107">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed116-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ed116-108">Prerequisites</span></span>
<span data-ttu-id="ed116-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed116-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed116-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ed116-111">Permission type</span></span>|<span data-ttu-id="ed116-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ed116-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed116-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed116-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed116-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed116-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ed116-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed116-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed116-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed116-116">Not supported.</span></span>|
|<span data-ttu-id="ed116-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ed116-117">Application</span></span>|<span data-ttu-id="ed116-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed116-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed116-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed116-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="ed116-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed116-120">Request headers</span></span>
|<span data-ttu-id="ed116-121">Header</span><span class="sxs-lookup"><span data-stu-id="ed116-121">Header</span></span>|<span data-ttu-id="ed116-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ed116-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed116-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed116-123">Authorization</span></span>|<span data-ttu-id="ed116-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ed116-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed116-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ed116-125">Accept</span></span>|<span data-ttu-id="ed116-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed116-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed116-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ed116-127">Request body</span></span>
<span data-ttu-id="ed116-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidManagedAppRegistration“ an.</span><span class="sxs-lookup"><span data-stu-id="ed116-128">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="ed116-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidManagedAppRegistration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="ed116-129">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="ed116-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ed116-130">Property</span></span>|<span data-ttu-id="ed116-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ed116-131">Type</span></span>|<span data-ttu-id="ed116-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed116-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed116-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed116-133">createdDateTime</span></span>|<span data-ttu-id="ed116-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed116-134">DateTimeOffset</span></span>|<span data-ttu-id="ed116-135">Datum und Uhrzeit der Erstellung. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ed116-135">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ed116-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ed116-136">lastSyncDateTime</span></span>|<span data-ttu-id="ed116-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed116-137">DateTimeOffset</span></span>|<span data-ttu-id="ed116-138">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst.</span><span class="sxs-lookup"><span data-stu-id="ed116-138">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="ed116-139">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ed116-139">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ed116-140">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="ed116-140">applicationVersion</span></span>|<span data-ttu-id="ed116-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed116-141">String</span></span>|<span data-ttu-id="ed116-142">App-Version. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ed116-142">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ed116-143">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="ed116-143">managementSdkVersion</span></span>|<span data-ttu-id="ed116-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed116-144">String</span></span>|<span data-ttu-id="ed116-145">Version des App-Verwaltungs-SDK. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ed116-145">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ed116-146">platformVersion</span><span class="sxs-lookup"><span data-stu-id="ed116-146">platformVersion</span></span>|<span data-ttu-id="ed116-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed116-147">String</span></span>|<span data-ttu-id="ed116-148">Version des Betriebssystems. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ed116-148">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ed116-149">deviceType</span><span class="sxs-lookup"><span data-stu-id="ed116-149">deviceType</span></span>|<span data-ttu-id="ed116-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed116-150">String</span></span>|<span data-ttu-id="ed116-151">Gerätetyp des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ed116-151">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ed116-152">deviceTag</span><span class="sxs-lookup"><span data-stu-id="ed116-152">deviceTag</span></span>|<span data-ttu-id="ed116-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed116-153">String</span></span>|<span data-ttu-id="ed116-154">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="ed116-154">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="ed116-155">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="ed116-155">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="ed116-156">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ed116-156">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ed116-157">deviceName</span><span class="sxs-lookup"><span data-stu-id="ed116-157">deviceName</span></span>|<span data-ttu-id="ed116-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed116-158">String</span></span>|<span data-ttu-id="ed116-159">Gerätename des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ed116-159">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ed116-160">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="ed116-160">managedDeviceId</span></span>|<span data-ttu-id="ed116-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed116-161">String</span></span>|<span data-ttu-id="ed116-162">Die verwaltete Geräte-ID des Hostgeräts werden soll.</span><span class="sxs-lookup"><span data-stu-id="ed116-162">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="ed116-163">Wert kann leer sein, selbst wenn das Host-Gerät verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="ed116-163">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="ed116-164">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ed116-164">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ed116-165">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="ed116-165">azureADDeviceId</span></span>|<span data-ttu-id="ed116-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed116-166">String</span></span>|<span data-ttu-id="ed116-167">Der Azure Active Directory-Gerät Bezeichner des Hostgeräts.</span><span class="sxs-lookup"><span data-stu-id="ed116-167">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="ed116-168">Wert kann leer sein, auch wenn das Host-Gerät Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="ed116-168">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="ed116-169">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ed116-169">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ed116-170">deviceModel</span><span class="sxs-lookup"><span data-stu-id="ed116-170">deviceModel</span></span>|<span data-ttu-id="ed116-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed116-171">String</span></span>|<span data-ttu-id="ed116-172">Das Gerätemodell für die aktuelle app-Registrierung Inherited aus [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="ed116-172">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ed116-173">Einträge deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="ed116-173">deviceManufacturer</span></span>|<span data-ttu-id="ed116-174">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed116-174">String</span></span>|<span data-ttu-id="ed116-175">Hersteller des Geräts für die aktuelle app-Registrierung Inherited aus [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="ed116-175">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ed116-176">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="ed116-176">flaggedReasons</span></span>|<span data-ttu-id="ed116-177">[ManagedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ed116-177">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="ed116-178">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="ed116-178">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="ed116-179">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="ed116-179">E.g.</span></span> <span data-ttu-id="ed116-180">die App auf Stamm Gerät Inherited verlaufende [ManagedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ed116-180">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="ed116-181">Mögliche Werte sind: `none` und `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="ed116-181">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="ed116-182">userId</span><span class="sxs-lookup"><span data-stu-id="ed116-182">userId</span></span>|<span data-ttu-id="ed116-183">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed116-183">String</span></span>|<span data-ttu-id="ed116-184">Benutzer-ID, zu der die App-Registrierung gehört.</span><span class="sxs-lookup"><span data-stu-id="ed116-184">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="ed116-185">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ed116-185">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ed116-186">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="ed116-186">appIdentifier</span></span>|[<span data-ttu-id="ed116-187">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ed116-187">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="ed116-188">Bezeichner des App-Pakets. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ed116-188">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ed116-189">id</span><span class="sxs-lookup"><span data-stu-id="ed116-189">id</span></span>|<span data-ttu-id="ed116-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed116-190">String</span></span>|<span data-ttu-id="ed116-191">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ed116-191">Key of the entity.</span></span> <span data-ttu-id="ed116-192">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ed116-192">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ed116-193">Version</span><span class="sxs-lookup"><span data-stu-id="ed116-193">version</span></span>|<span data-ttu-id="ed116-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed116-194">String</span></span>|<span data-ttu-id="ed116-195">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="ed116-195">Version of the entity.</span></span> <span data-ttu-id="ed116-196">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ed116-196">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ed116-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed116-197">Response</span></span>
<span data-ttu-id="ed116-198">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ed116-198">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed116-199">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed116-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed116-200">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed116-200">Request</span></span>
<span data-ttu-id="ed116-201">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ed116-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 837

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="ed116-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed116-202">Response</span></span>
<span data-ttu-id="ed116-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed116-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 945

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value"
}
```





