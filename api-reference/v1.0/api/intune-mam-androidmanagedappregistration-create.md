---
title: Erstellen von „androidManagedAppRegistration“
description: Diese Methode erstellt ein neues Objekt des Typs androidManagedAppRegistration.
author: tfitzmac
ms.openlocfilehash: c05c698179f2f8fa54ab12282be6e397b9275408
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339508"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="6bf20-103">Erstellen von „androidManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="6bf20-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="6bf20-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6bf20-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bf20-105">Diese Methode erstellt ein neues Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6bf20-105">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6bf20-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6bf20-106">Prerequisites</span></span>
<span data-ttu-id="6bf20-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bf20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bf20-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6bf20-109">Permission type</span></span>|<span data-ttu-id="6bf20-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6bf20-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bf20-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6bf20-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6bf20-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bf20-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6bf20-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6bf20-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bf20-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6bf20-114">Not supported.</span></span>|
|<span data-ttu-id="6bf20-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6bf20-115">Application</span></span>|<span data-ttu-id="6bf20-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6bf20-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bf20-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6bf20-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="6bf20-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6bf20-118">Request headers</span></span>
|<span data-ttu-id="6bf20-119">Header</span><span class="sxs-lookup"><span data-stu-id="6bf20-119">Header</span></span>|<span data-ttu-id="6bf20-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6bf20-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bf20-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6bf20-121">Authorization</span></span>|<span data-ttu-id="6bf20-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6bf20-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bf20-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6bf20-123">Accept</span></span>|<span data-ttu-id="6bf20-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6bf20-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bf20-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6bf20-125">Request body</span></span>
<span data-ttu-id="6bf20-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidManagedAppRegistration“ an.</span><span class="sxs-lookup"><span data-stu-id="6bf20-126">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="6bf20-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidManagedAppRegistration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="6bf20-127">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="6bf20-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6bf20-128">Property</span></span>|<span data-ttu-id="6bf20-129">Typ</span><span class="sxs-lookup"><span data-stu-id="6bf20-129">Type</span></span>|<span data-ttu-id="6bf20-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6bf20-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bf20-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6bf20-131">createdDateTime</span></span>|<span data-ttu-id="6bf20-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bf20-132">DateTimeOffset</span></span>|<span data-ttu-id="6bf20-133">Datum und Uhrzeit der Erstellung. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6bf20-133">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bf20-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6bf20-134">lastSyncDateTime</span></span>|<span data-ttu-id="6bf20-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bf20-135">DateTimeOffset</span></span>|<span data-ttu-id="6bf20-136">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst.</span><span class="sxs-lookup"><span data-stu-id="6bf20-136">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="6bf20-137">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6bf20-137">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bf20-138">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="6bf20-138">applicationVersion</span></span>|<span data-ttu-id="6bf20-139">String</span><span class="sxs-lookup"><span data-stu-id="6bf20-139">String</span></span>|<span data-ttu-id="6bf20-140">App-Version. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6bf20-140">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bf20-141">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="6bf20-141">managementSdkVersion</span></span>|<span data-ttu-id="6bf20-142">String</span><span class="sxs-lookup"><span data-stu-id="6bf20-142">String</span></span>|<span data-ttu-id="6bf20-143">Version des App-Verwaltungs-SDK. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6bf20-143">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bf20-144">platformVersion</span><span class="sxs-lookup"><span data-stu-id="6bf20-144">platformVersion</span></span>|<span data-ttu-id="6bf20-145">String</span><span class="sxs-lookup"><span data-stu-id="6bf20-145">String</span></span>|<span data-ttu-id="6bf20-146">Version des Betriebssystems. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6bf20-146">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bf20-147">deviceType</span><span class="sxs-lookup"><span data-stu-id="6bf20-147">deviceType</span></span>|<span data-ttu-id="6bf20-148">String</span><span class="sxs-lookup"><span data-stu-id="6bf20-148">String</span></span>|<span data-ttu-id="6bf20-149">Gerätetyp des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6bf20-149">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bf20-150">deviceTag</span><span class="sxs-lookup"><span data-stu-id="6bf20-150">deviceTag</span></span>|<span data-ttu-id="6bf20-151">String</span><span class="sxs-lookup"><span data-stu-id="6bf20-151">String</span></span>|<span data-ttu-id="6bf20-152">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="6bf20-152">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="6bf20-153">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="6bf20-153">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="6bf20-154">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6bf20-154">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bf20-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="6bf20-155">deviceName</span></span>|<span data-ttu-id="6bf20-156">String</span><span class="sxs-lookup"><span data-stu-id="6bf20-156">String</span></span>|<span data-ttu-id="6bf20-157">Gerätename des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6bf20-157">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bf20-158">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="6bf20-158">flaggedReasons</span></span>|<span data-ttu-id="6bf20-159">[ManagedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6bf20-159">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="6bf20-160">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="6bf20-160">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="6bf20-161">E.g.</span><span class="sxs-lookup"><span data-stu-id="6bf20-161">E.g.</span></span> <span data-ttu-id="6bf20-162">die App auf Stamm Gerät Inherited verlaufende [ManagedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6bf20-162">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="6bf20-163">Mögliche Werte sind: `none` und `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="6bf20-163">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="6bf20-164">userId</span><span class="sxs-lookup"><span data-stu-id="6bf20-164">userId</span></span>|<span data-ttu-id="6bf20-165">String</span><span class="sxs-lookup"><span data-stu-id="6bf20-165">String</span></span>|<span data-ttu-id="6bf20-166">Benutzer-ID, zu der die App-Registrierung gehört.</span><span class="sxs-lookup"><span data-stu-id="6bf20-166">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="6bf20-167">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6bf20-167">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bf20-168">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="6bf20-168">appIdentifier</span></span>|[<span data-ttu-id="6bf20-169">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="6bf20-169">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="6bf20-170">Bezeichner des App-Pakets. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6bf20-170">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bf20-171">id</span><span class="sxs-lookup"><span data-stu-id="6bf20-171">id</span></span>|<span data-ttu-id="6bf20-172">String</span><span class="sxs-lookup"><span data-stu-id="6bf20-172">String</span></span>|<span data-ttu-id="6bf20-173">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6bf20-173">Key of the entity.</span></span> <span data-ttu-id="6bf20-174">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6bf20-174">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bf20-175">Version</span><span class="sxs-lookup"><span data-stu-id="6bf20-175">version</span></span>|<span data-ttu-id="6bf20-176">String</span><span class="sxs-lookup"><span data-stu-id="6bf20-176">String</span></span>|<span data-ttu-id="6bf20-177">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="6bf20-177">Version of the entity.</span></span> <span data-ttu-id="6bf20-178">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6bf20-178">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="6bf20-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="6bf20-179">Response</span></span>
<span data-ttu-id="6bf20-180">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6bf20-180">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bf20-181">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6bf20-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="6bf20-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6bf20-182">Request</span></span>
<span data-ttu-id="6bf20-183">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6bf20-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
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

### <a name="response"></a><span data-ttu-id="6bf20-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="6bf20-184">Response</span></span>
<span data-ttu-id="6bf20-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6bf20-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 753

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



