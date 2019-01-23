---
title: Erstellen von „androidManagedAppRegistration“
description: Diese Methode erstellt ein neues Objekt des Typs androidManagedAppRegistration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 83a2fd4c1967da5bdb401ab57bf603dace128f05
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408495"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="c903a-103">Erstellen von „androidManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="c903a-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="c903a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c903a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c903a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c903a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c903a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c903a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c903a-107">Diese Methode erstellt ein neues Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-107">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c903a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c903a-108">Prerequisites</span></span>
<span data-ttu-id="c903a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c903a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c903a-111">Permission type</span></span>|<span data-ttu-id="c903a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c903a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c903a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c903a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c903a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c903a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c903a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c903a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c903a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c903a-116">Not supported.</span></span>|
|<span data-ttu-id="c903a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c903a-117">Application</span></span>|<span data-ttu-id="c903a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c903a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c903a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c903a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="c903a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c903a-120">Request headers</span></span>
|<span data-ttu-id="c903a-121">Header</span><span class="sxs-lookup"><span data-stu-id="c903a-121">Header</span></span>|<span data-ttu-id="c903a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c903a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c903a-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c903a-123">Authorization</span></span>|<span data-ttu-id="c903a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c903a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c903a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c903a-125">Accept</span></span>|<span data-ttu-id="c903a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c903a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c903a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c903a-127">Request body</span></span>
<span data-ttu-id="c903a-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidManagedAppRegistration“ an.</span><span class="sxs-lookup"><span data-stu-id="c903a-128">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="c903a-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidManagedAppRegistration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="c903a-129">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="c903a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c903a-130">Property</span></span>|<span data-ttu-id="c903a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c903a-131">Type</span></span>|<span data-ttu-id="c903a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c903a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c903a-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c903a-133">createdDateTime</span></span>|<span data-ttu-id="c903a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c903a-134">DateTimeOffset</span></span>|<span data-ttu-id="c903a-135">Datum und Uhrzeit der Erstellung. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-135">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c903a-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c903a-136">lastSyncDateTime</span></span>|<span data-ttu-id="c903a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c903a-137">DateTimeOffset</span></span>|<span data-ttu-id="c903a-138">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst.</span><span class="sxs-lookup"><span data-stu-id="c903a-138">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="c903a-139">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-139">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c903a-140">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="c903a-140">applicationVersion</span></span>|<span data-ttu-id="c903a-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c903a-141">String</span></span>|<span data-ttu-id="c903a-142">App-Version. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-142">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c903a-143">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="c903a-143">managementSdkVersion</span></span>|<span data-ttu-id="c903a-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c903a-144">String</span></span>|<span data-ttu-id="c903a-145">Version des App-Verwaltungs-SDK. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-145">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c903a-146">platformVersion</span><span class="sxs-lookup"><span data-stu-id="c903a-146">platformVersion</span></span>|<span data-ttu-id="c903a-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c903a-147">String</span></span>|<span data-ttu-id="c903a-148">Version des Betriebssystems. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-148">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c903a-149">deviceType</span><span class="sxs-lookup"><span data-stu-id="c903a-149">deviceType</span></span>|<span data-ttu-id="c903a-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c903a-150">String</span></span>|<span data-ttu-id="c903a-151">Gerätetyp des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-151">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c903a-152">deviceTag</span><span class="sxs-lookup"><span data-stu-id="c903a-152">deviceTag</span></span>|<span data-ttu-id="c903a-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c903a-153">String</span></span>|<span data-ttu-id="c903a-154">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="c903a-154">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="c903a-155">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="c903a-155">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="c903a-156">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-156">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c903a-157">deviceName</span><span class="sxs-lookup"><span data-stu-id="c903a-157">deviceName</span></span>|<span data-ttu-id="c903a-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c903a-158">String</span></span>|<span data-ttu-id="c903a-159">Gerätename des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-159">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c903a-160">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="c903a-160">managedDeviceId</span></span>|<span data-ttu-id="c903a-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c903a-161">String</span></span>|<span data-ttu-id="c903a-162">Die verwaltete Geräte-ID des Hostgeräts werden soll.</span><span class="sxs-lookup"><span data-stu-id="c903a-162">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="c903a-163">Wert kann leer sein, selbst wenn das Host-Gerät verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="c903a-163">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="c903a-164">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-164">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c903a-165">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="c903a-165">azureADDeviceId</span></span>|<span data-ttu-id="c903a-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c903a-166">String</span></span>|<span data-ttu-id="c903a-167">Der Azure Active Directory-Gerät Bezeichner des Hostgeräts.</span><span class="sxs-lookup"><span data-stu-id="c903a-167">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="c903a-168">Wert kann leer sein, auch wenn das Host-Gerät Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="c903a-168">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="c903a-169">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-169">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c903a-170">deviceModel</span><span class="sxs-lookup"><span data-stu-id="c903a-170">deviceModel</span></span>|<span data-ttu-id="c903a-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c903a-171">String</span></span>|<span data-ttu-id="c903a-172">Das Gerätemodell für die aktuelle app-Registrierung Inherited aus [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c903a-172">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c903a-173">Einträge deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="c903a-173">deviceManufacturer</span></span>|<span data-ttu-id="c903a-174">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c903a-174">String</span></span>|<span data-ttu-id="c903a-175">Hersteller des Geräts für die aktuelle app-Registrierung Inherited aus [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c903a-175">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c903a-176">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="c903a-176">flaggedReasons</span></span>|<span data-ttu-id="c903a-177">[ManagedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c903a-177">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="c903a-178">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="c903a-178">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="c903a-179">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="c903a-179">E.g.</span></span> <span data-ttu-id="c903a-180">die App auf Stamm Gerät Inherited verlaufende [ManagedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-180">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="c903a-181">Mögliche Werte sind: `none` und `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="c903a-181">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="c903a-182">userId</span><span class="sxs-lookup"><span data-stu-id="c903a-182">userId</span></span>|<span data-ttu-id="c903a-183">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c903a-183">String</span></span>|<span data-ttu-id="c903a-184">Benutzer-ID, zu der die App-Registrierung gehört.</span><span class="sxs-lookup"><span data-stu-id="c903a-184">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="c903a-185">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-185">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c903a-186">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="c903a-186">appIdentifier</span></span>|[<span data-ttu-id="c903a-187">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c903a-187">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="c903a-188">Bezeichner des App-Pakets. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-188">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c903a-189">id</span><span class="sxs-lookup"><span data-stu-id="c903a-189">id</span></span>|<span data-ttu-id="c903a-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c903a-190">String</span></span>|<span data-ttu-id="c903a-191">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c903a-191">Key of the entity.</span></span> <span data-ttu-id="c903a-192">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-192">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c903a-193">Version</span><span class="sxs-lookup"><span data-stu-id="c903a-193">version</span></span>|<span data-ttu-id="c903a-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c903a-194">String</span></span>|<span data-ttu-id="c903a-195">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="c903a-195">Version of the entity.</span></span> <span data-ttu-id="c903a-196">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c903a-196">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c903a-197">patchVersion</span><span class="sxs-lookup"><span data-stu-id="c903a-197">patchVersion</span></span>|<span data-ttu-id="c903a-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c903a-198">String</span></span>|<span data-ttu-id="c903a-199">Die Patch-Version für die aktuelle android-app-Registrierung</span><span class="sxs-lookup"><span data-stu-id="c903a-199">The patch version for the current android app registration</span></span>|



## <a name="response"></a><span data-ttu-id="c903a-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="c903a-200">Response</span></span>
<span data-ttu-id="c903a-201">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c903a-201">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c903a-202">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c903a-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="c903a-203">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c903a-203">Request</span></span>
<span data-ttu-id="c903a-204">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c903a-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 879

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
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```

### <a name="response"></a><span data-ttu-id="c903a-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="c903a-205">Response</span></span>
<span data-ttu-id="c903a-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c903a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 987

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
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```




