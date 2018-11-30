---
title: Erstellen von „androidManagedAppRegistration“
description: Diese Methode erstellt ein neues Objekt des Typs androidManagedAppRegistration.
ms.openlocfilehash: c1054b5c07784044071f8674a778bb1d4b98a46b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016236"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="ec8c0-103">Erstellen von „androidManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="ec8c0-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="ec8c0-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ec8c0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec8c0-105">Diese Methode erstellt ein neues Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ec8c0-105">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ec8c0-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ec8c0-106">Prerequisites</span></span>
<span data-ttu-id="ec8c0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec8c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec8c0-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ec8c0-109">Permission type</span></span>|<span data-ttu-id="ec8c0-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ec8c0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec8c0-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ec8c0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ec8c0-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec8c0-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ec8c0-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ec8c0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec8c0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec8c0-114">Not supported.</span></span>|
|<span data-ttu-id="ec8c0-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ec8c0-115">Application</span></span>|<span data-ttu-id="ec8c0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec8c0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec8c0-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec8c0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="ec8c0-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ec8c0-118">Request headers</span></span>
|<span data-ttu-id="ec8c0-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ec8c0-119">Header</span></span>|<span data-ttu-id="ec8c0-120">Wert</span><span class="sxs-lookup"><span data-stu-id="ec8c0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec8c0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec8c0-121">Authorization</span></span>|<span data-ttu-id="ec8c0-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ec8c0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec8c0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ec8c0-123">Accept</span></span>|<span data-ttu-id="ec8c0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ec8c0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec8c0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ec8c0-125">Request body</span></span>
<span data-ttu-id="ec8c0-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidManagedAppRegistration“ an.</span><span class="sxs-lookup"><span data-stu-id="ec8c0-126">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="ec8c0-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidManagedAppRegistration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="ec8c0-127">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="ec8c0-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ec8c0-128">Property</span></span>|<span data-ttu-id="ec8c0-129">Typ</span><span class="sxs-lookup"><span data-stu-id="ec8c0-129">Type</span></span>|<span data-ttu-id="ec8c0-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec8c0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec8c0-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ec8c0-131">createdDateTime</span></span>|<span data-ttu-id="ec8c0-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec8c0-132">DateTimeOffset</span></span>|<span data-ttu-id="ec8c0-133">Datum und Uhrzeit der Erstellung. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ec8c0-133">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ec8c0-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ec8c0-134">lastSyncDateTime</span></span>|<span data-ttu-id="ec8c0-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec8c0-135">DateTimeOffset</span></span>|<span data-ttu-id="ec8c0-136">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst.</span><span class="sxs-lookup"><span data-stu-id="ec8c0-136">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="ec8c0-137">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ec8c0-137">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ec8c0-138">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="ec8c0-138">applicationVersion</span></span>|<span data-ttu-id="ec8c0-139">String</span><span class="sxs-lookup"><span data-stu-id="ec8c0-139">String</span></span>|<span data-ttu-id="ec8c0-140">App-Version. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ec8c0-140">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ec8c0-141">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="ec8c0-141">managementSdkVersion</span></span>|<span data-ttu-id="ec8c0-142">String</span><span class="sxs-lookup"><span data-stu-id="ec8c0-142">String</span></span>|<span data-ttu-id="ec8c0-143">Version des App-Verwaltungs-SDK. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ec8c0-143">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ec8c0-144">platformVersion</span><span class="sxs-lookup"><span data-stu-id="ec8c0-144">platformVersion</span></span>|<span data-ttu-id="ec8c0-145">String</span><span class="sxs-lookup"><span data-stu-id="ec8c0-145">String</span></span>|<span data-ttu-id="ec8c0-146">Version des Betriebssystems. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ec8c0-146">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ec8c0-147">deviceType</span><span class="sxs-lookup"><span data-stu-id="ec8c0-147">deviceType</span></span>|<span data-ttu-id="ec8c0-148">String</span><span class="sxs-lookup"><span data-stu-id="ec8c0-148">String</span></span>|<span data-ttu-id="ec8c0-149">Gerätetyp des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ec8c0-149">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ec8c0-150">deviceTag</span><span class="sxs-lookup"><span data-stu-id="ec8c0-150">deviceTag</span></span>|<span data-ttu-id="ec8c0-151">String</span><span class="sxs-lookup"><span data-stu-id="ec8c0-151">String</span></span>|<span data-ttu-id="ec8c0-152">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="ec8c0-152">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="ec8c0-153">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="ec8c0-153">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="ec8c0-154">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ec8c0-154">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ec8c0-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="ec8c0-155">deviceName</span></span>|<span data-ttu-id="ec8c0-156">String</span><span class="sxs-lookup"><span data-stu-id="ec8c0-156">String</span></span>|<span data-ttu-id="ec8c0-157">Gerätename des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ec8c0-157">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ec8c0-158">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="ec8c0-158">flaggedReasons</span></span>|<span data-ttu-id="ec8c0-159">[ManagedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ec8c0-159">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="ec8c0-160">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="ec8c0-160">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="ec8c0-161">E.g.</span><span class="sxs-lookup"><span data-stu-id="ec8c0-161">E.g.</span></span> <span data-ttu-id="ec8c0-162">die App auf Stamm Gerät Inherited verlaufende [ManagedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ec8c0-162">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="ec8c0-163">Mögliche Werte sind: `none` und `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="ec8c0-163">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="ec8c0-164">userId</span><span class="sxs-lookup"><span data-stu-id="ec8c0-164">userId</span></span>|<span data-ttu-id="ec8c0-165">String</span><span class="sxs-lookup"><span data-stu-id="ec8c0-165">String</span></span>|<span data-ttu-id="ec8c0-166">Benutzer-ID, zu der die App-Registrierung gehört.</span><span class="sxs-lookup"><span data-stu-id="ec8c0-166">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="ec8c0-167">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ec8c0-167">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ec8c0-168">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="ec8c0-168">appIdentifier</span></span>|[<span data-ttu-id="ec8c0-169">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ec8c0-169">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="ec8c0-170">Bezeichner des App-Pakets. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ec8c0-170">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ec8c0-171">id</span><span class="sxs-lookup"><span data-stu-id="ec8c0-171">id</span></span>|<span data-ttu-id="ec8c0-172">String</span><span class="sxs-lookup"><span data-stu-id="ec8c0-172">String</span></span>|<span data-ttu-id="ec8c0-173">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ec8c0-173">Key of the entity.</span></span> <span data-ttu-id="ec8c0-174">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ec8c0-174">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ec8c0-175">Version</span><span class="sxs-lookup"><span data-stu-id="ec8c0-175">version</span></span>|<span data-ttu-id="ec8c0-176">String</span><span class="sxs-lookup"><span data-stu-id="ec8c0-176">String</span></span>|<span data-ttu-id="ec8c0-177">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="ec8c0-177">Version of the entity.</span></span> <span data-ttu-id="ec8c0-178">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ec8c0-178">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ec8c0-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec8c0-179">Response</span></span>
<span data-ttu-id="ec8c0-180">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ec8c0-180">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec8c0-181">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ec8c0-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="ec8c0-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec8c0-182">Request</span></span>
<span data-ttu-id="ec8c0-183">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ec8c0-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ec8c0-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec8c0-184">Response</span></span>
<span data-ttu-id="ec8c0-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec8c0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



