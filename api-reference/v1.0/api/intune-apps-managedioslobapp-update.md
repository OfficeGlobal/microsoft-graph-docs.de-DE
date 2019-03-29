---
title: managedIOSLobApp aktualisieren
description: Aktualisieren der Eigenschaften eines managedIOSLobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6bbd9174ef791c6f0e5517131d9c757a2e5755e6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965249"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="4aefa-103">managedIOSLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4aefa-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="4aefa-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4aefa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4aefa-105">Aktualisieren der Eigenschaften eines [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4aefa-105">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4aefa-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4aefa-106">Prerequisites</span></span>
<span data-ttu-id="4aefa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4aefa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4aefa-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4aefa-109">Permission type</span></span>|<span data-ttu-id="4aefa-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4aefa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4aefa-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4aefa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4aefa-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4aefa-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4aefa-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4aefa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4aefa-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4aefa-114">Not supported.</span></span>|
|<span data-ttu-id="4aefa-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4aefa-115">Application</span></span>|<span data-ttu-id="4aefa-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4aefa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4aefa-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4aefa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="4aefa-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4aefa-118">Request headers</span></span>
|<span data-ttu-id="4aefa-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4aefa-119">Header</span></span>|<span data-ttu-id="4aefa-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4aefa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4aefa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4aefa-121">Authorization</span></span>|<span data-ttu-id="4aefa-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4aefa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4aefa-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4aefa-123">Accept</span></span>|<span data-ttu-id="4aefa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4aefa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4aefa-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4aefa-125">Request body</span></span>
<span data-ttu-id="4aefa-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4aefa-126">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="4aefa-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4aefa-127">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="4aefa-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4aefa-128">Property</span></span>|<span data-ttu-id="4aefa-129">Typ</span><span class="sxs-lookup"><span data-stu-id="4aefa-129">Type</span></span>|<span data-ttu-id="4aefa-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4aefa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4aefa-131">id</span><span class="sxs-lookup"><span data-stu-id="4aefa-131">id</span></span>|<span data-ttu-id="4aefa-132">String</span><span class="sxs-lookup"><span data-stu-id="4aefa-132">String</span></span>|<span data-ttu-id="4aefa-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4aefa-133">Key of the entity.</span></span> <span data-ttu-id="4aefa-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4aefa-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4aefa-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4aefa-135">displayName</span></span>|<span data-ttu-id="4aefa-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4aefa-136">String</span></span>|<span data-ttu-id="4aefa-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="4aefa-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4aefa-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4aefa-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4aefa-139">description</span><span class="sxs-lookup"><span data-stu-id="4aefa-139">description</span></span>|<span data-ttu-id="4aefa-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4aefa-140">String</span></span>|<span data-ttu-id="4aefa-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="4aefa-141">The description of the app.</span></span> <span data-ttu-id="4aefa-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4aefa-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4aefa-143">publisher</span><span class="sxs-lookup"><span data-stu-id="4aefa-143">publisher</span></span>|<span data-ttu-id="4aefa-144">String</span><span class="sxs-lookup"><span data-stu-id="4aefa-144">String</span></span>|<span data-ttu-id="4aefa-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="4aefa-145">The publisher of the app.</span></span> <span data-ttu-id="4aefa-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4aefa-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4aefa-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4aefa-147">largeIcon</span></span>|[<span data-ttu-id="4aefa-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4aefa-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4aefa-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="4aefa-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4aefa-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4aefa-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4aefa-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4aefa-151">createdDateTime</span></span>|<span data-ttu-id="4aefa-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4aefa-152">DateTimeOffset</span></span>|<span data-ttu-id="4aefa-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="4aefa-153">The date and time the app was created.</span></span> <span data-ttu-id="4aefa-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4aefa-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4aefa-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4aefa-155">lastModifiedDateTime</span></span>|<span data-ttu-id="4aefa-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4aefa-156">DateTimeOffset</span></span>|<span data-ttu-id="4aefa-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="4aefa-157">The date and time the app was last modified.</span></span> <span data-ttu-id="4aefa-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4aefa-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4aefa-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4aefa-159">isFeatured</span></span>|<span data-ttu-id="4aefa-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aefa-160">Boolean</span></span>|<span data-ttu-id="4aefa-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4aefa-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4aefa-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4aefa-162">privacyInformationUrl</span></span>|<span data-ttu-id="4aefa-163">String</span><span class="sxs-lookup"><span data-stu-id="4aefa-163">String</span></span>|<span data-ttu-id="4aefa-164">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="4aefa-164">The privacy statement Url.</span></span> <span data-ttu-id="4aefa-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4aefa-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4aefa-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4aefa-166">informationUrl</span></span>|<span data-ttu-id="4aefa-167">String</span><span class="sxs-lookup"><span data-stu-id="4aefa-167">String</span></span>|<span data-ttu-id="4aefa-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="4aefa-168">The more information Url.</span></span> <span data-ttu-id="4aefa-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4aefa-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4aefa-170">owner</span><span class="sxs-lookup"><span data-stu-id="4aefa-170">owner</span></span>|<span data-ttu-id="4aefa-171">String</span><span class="sxs-lookup"><span data-stu-id="4aefa-171">String</span></span>|<span data-ttu-id="4aefa-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="4aefa-172">The owner of the app.</span></span> <span data-ttu-id="4aefa-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4aefa-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4aefa-174">developer</span><span class="sxs-lookup"><span data-stu-id="4aefa-174">developer</span></span>|<span data-ttu-id="4aefa-175">String</span><span class="sxs-lookup"><span data-stu-id="4aefa-175">String</span></span>|<span data-ttu-id="4aefa-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="4aefa-176">The developer of the app.</span></span> <span data-ttu-id="4aefa-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4aefa-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4aefa-178">notes</span><span class="sxs-lookup"><span data-stu-id="4aefa-178">notes</span></span>|<span data-ttu-id="4aefa-179">String</span><span class="sxs-lookup"><span data-stu-id="4aefa-179">String</span></span>|<span data-ttu-id="4aefa-180">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="4aefa-180">Notes for the app.</span></span> <span data-ttu-id="4aefa-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4aefa-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4aefa-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="4aefa-182">publishingState</span></span>|[<span data-ttu-id="4aefa-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4aefa-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4aefa-184">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="4aefa-184">The publishing state for the app.</span></span> <span data-ttu-id="4aefa-185">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="4aefa-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4aefa-186">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="4aefa-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4aefa-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="4aefa-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4aefa-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="4aefa-188">appAvailability</span></span>|[<span data-ttu-id="4aefa-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="4aefa-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="4aefa-190">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="4aefa-190">The Application's availability.</span></span> <span data-ttu-id="4aefa-191">Von [ManagedApp](../resources/intune-apps-managedapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="4aefa-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="4aefa-192">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="4aefa-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="4aefa-193">version</span><span class="sxs-lookup"><span data-stu-id="4aefa-193">version</span></span>|<span data-ttu-id="4aefa-194">String</span><span class="sxs-lookup"><span data-stu-id="4aefa-194">String</span></span>|<span data-ttu-id="4aefa-195">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="4aefa-195">The Application's version.</span></span> <span data-ttu-id="4aefa-196">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="4aefa-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="4aefa-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4aefa-197">committedContentVersion</span></span>|<span data-ttu-id="4aefa-198">String</span><span class="sxs-lookup"><span data-stu-id="4aefa-198">String</span></span>|<span data-ttu-id="4aefa-199">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="4aefa-199">The internal committed content version.</span></span> <span data-ttu-id="4aefa-200">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4aefa-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4aefa-201">fileName</span><span class="sxs-lookup"><span data-stu-id="4aefa-201">fileName</span></span>|<span data-ttu-id="4aefa-202">String</span><span class="sxs-lookup"><span data-stu-id="4aefa-202">String</span></span>|<span data-ttu-id="4aefa-203">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="4aefa-203">The name of the main Lob application file.</span></span> <span data-ttu-id="4aefa-204">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4aefa-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4aefa-205">size</span><span class="sxs-lookup"><span data-stu-id="4aefa-205">size</span></span>|<span data-ttu-id="4aefa-206">Int64</span><span class="sxs-lookup"><span data-stu-id="4aefa-206">Int64</span></span>|<span data-ttu-id="4aefa-207">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="4aefa-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="4aefa-208">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4aefa-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4aefa-209">bundleId</span><span class="sxs-lookup"><span data-stu-id="4aefa-209">bundleId</span></span>|<span data-ttu-id="4aefa-210">String</span><span class="sxs-lookup"><span data-stu-id="4aefa-210">String</span></span>|<span data-ttu-id="4aefa-211">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="4aefa-211">The Identity Name.</span></span>|
|<span data-ttu-id="4aefa-212">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="4aefa-212">applicableDeviceType</span></span>|[<span data-ttu-id="4aefa-213">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="4aefa-213">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="4aefa-214">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="4aefa-214">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="4aefa-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4aefa-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4aefa-216">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4aefa-216">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="4aefa-217">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="4aefa-217">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="4aefa-218">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4aefa-218">expirationDateTime</span></span>|<span data-ttu-id="4aefa-219">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4aefa-219">DateTimeOffset</span></span>|<span data-ttu-id="4aefa-220">Das Ablaufdatum.</span><span class="sxs-lookup"><span data-stu-id="4aefa-220">The expiration time.</span></span>|
|<span data-ttu-id="4aefa-221">versionNumber</span><span class="sxs-lookup"><span data-stu-id="4aefa-221">versionNumber</span></span>|<span data-ttu-id="4aefa-222">String</span><span class="sxs-lookup"><span data-stu-id="4aefa-222">String</span></span>|<span data-ttu-id="4aefa-223">Die Versionsnummer der verwalteten branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="4aefa-223">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4aefa-224">buildNumber</span><span class="sxs-lookup"><span data-stu-id="4aefa-224">buildNumber</span></span>|<span data-ttu-id="4aefa-225">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4aefa-225">String</span></span>|<span data-ttu-id="4aefa-226">Die Buildnummer der verwalteten branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="4aefa-226">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="4aefa-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="4aefa-227">Response</span></span>
<span data-ttu-id="4aefa-228">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4aefa-228">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4aefa-229">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4aefa-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="4aefa-230">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4aefa-230">Request</span></span>
<span data-ttu-id="4aefa-231">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4aefa-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1287

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="4aefa-232">Antwort</span><span class="sxs-lookup"><span data-stu-id="4aefa-232">Response</span></span>
<span data-ttu-id="4aefa-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4aefa-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1459

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



