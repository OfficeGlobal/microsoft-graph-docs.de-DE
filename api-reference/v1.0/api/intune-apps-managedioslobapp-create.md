---
title: managedIOSLobApp erstellen
description: Erstellen eines neuen managedIOSLobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c113c8c76029ee7a0d1c5f3e5d0b1d0ab5f31bba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987076"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="85581-103">managedIOSLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="85581-103">Create managedIOSLobApp</span></span>

> <span data-ttu-id="85581-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="85581-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85581-105">Erstellen eines neuen [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="85581-105">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85581-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="85581-106">Prerequisites</span></span>
<span data-ttu-id="85581-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85581-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85581-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="85581-109">Permission type</span></span>|<span data-ttu-id="85581-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="85581-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85581-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="85581-111">Delegated (work or school account)</span></span>|<span data-ttu-id="85581-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85581-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="85581-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="85581-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85581-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85581-114">Not supported.</span></span>|
|<span data-ttu-id="85581-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="85581-115">Application</span></span>|<span data-ttu-id="85581-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85581-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85581-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="85581-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="85581-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="85581-118">Request headers</span></span>
|<span data-ttu-id="85581-119">Header</span><span class="sxs-lookup"><span data-stu-id="85581-119">Header</span></span>|<span data-ttu-id="85581-120">Wert</span><span class="sxs-lookup"><span data-stu-id="85581-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85581-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="85581-121">Authorization</span></span>|<span data-ttu-id="85581-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="85581-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85581-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="85581-123">Accept</span></span>|<span data-ttu-id="85581-124">application/json</span><span class="sxs-lookup"><span data-stu-id="85581-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85581-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="85581-125">Request body</span></span>
<span data-ttu-id="85581-126">Geben Sie im Anforderungstext eine JSON-Darstellung des managedIOSLobApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="85581-126">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="85581-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedIOSLobApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="85581-127">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="85581-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="85581-128">Property</span></span>|<span data-ttu-id="85581-129">Typ</span><span class="sxs-lookup"><span data-stu-id="85581-129">Type</span></span>|<span data-ttu-id="85581-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85581-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85581-131">id</span><span class="sxs-lookup"><span data-stu-id="85581-131">id</span></span>|<span data-ttu-id="85581-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85581-132">String</span></span>|<span data-ttu-id="85581-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="85581-133">Key of the entity.</span></span> <span data-ttu-id="85581-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85581-135">displayName</span><span class="sxs-lookup"><span data-stu-id="85581-135">displayName</span></span>|<span data-ttu-id="85581-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85581-136">String</span></span>|<span data-ttu-id="85581-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="85581-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="85581-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85581-139">description</span><span class="sxs-lookup"><span data-stu-id="85581-139">description</span></span>|<span data-ttu-id="85581-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85581-140">String</span></span>|<span data-ttu-id="85581-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="85581-141">The description of the app.</span></span> <span data-ttu-id="85581-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85581-143">publisher</span><span class="sxs-lookup"><span data-stu-id="85581-143">publisher</span></span>|<span data-ttu-id="85581-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85581-144">String</span></span>|<span data-ttu-id="85581-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="85581-145">The publisher of the app.</span></span> <span data-ttu-id="85581-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85581-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="85581-147">largeIcon</span></span>|[<span data-ttu-id="85581-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="85581-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="85581-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="85581-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="85581-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85581-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85581-151">createdDateTime</span></span>|<span data-ttu-id="85581-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85581-152">DateTimeOffset</span></span>|<span data-ttu-id="85581-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="85581-153">The date and time the app was created.</span></span> <span data-ttu-id="85581-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85581-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85581-155">lastModifiedDateTime</span></span>|<span data-ttu-id="85581-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85581-156">DateTimeOffset</span></span>|<span data-ttu-id="85581-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="85581-157">The date and time the app was last modified.</span></span> <span data-ttu-id="85581-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85581-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="85581-159">isFeatured</span></span>|<span data-ttu-id="85581-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="85581-160">Boolean</span></span>|<span data-ttu-id="85581-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85581-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="85581-162">privacyInformationUrl</span></span>|<span data-ttu-id="85581-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85581-163">String</span></span>|<span data-ttu-id="85581-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="85581-164">The privacy statement Url.</span></span> <span data-ttu-id="85581-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85581-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="85581-166">informationUrl</span></span>|<span data-ttu-id="85581-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85581-167">String</span></span>|<span data-ttu-id="85581-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="85581-168">The more information Url.</span></span> <span data-ttu-id="85581-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85581-170">owner</span><span class="sxs-lookup"><span data-stu-id="85581-170">owner</span></span>|<span data-ttu-id="85581-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85581-171">String</span></span>|<span data-ttu-id="85581-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="85581-172">The owner of the app.</span></span> <span data-ttu-id="85581-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85581-174">developer</span><span class="sxs-lookup"><span data-stu-id="85581-174">developer</span></span>|<span data-ttu-id="85581-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85581-175">String</span></span>|<span data-ttu-id="85581-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="85581-176">The developer of the app.</span></span> <span data-ttu-id="85581-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85581-178">notes</span><span class="sxs-lookup"><span data-stu-id="85581-178">notes</span></span>|<span data-ttu-id="85581-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85581-179">String</span></span>|<span data-ttu-id="85581-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="85581-180">Notes for the app.</span></span> <span data-ttu-id="85581-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85581-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="85581-182">publishingState</span></span>|[<span data-ttu-id="85581-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="85581-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="85581-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="85581-184">The publishing state for the app.</span></span> <span data-ttu-id="85581-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="85581-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="85581-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="85581-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="85581-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="85581-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="85581-188">appAvailability</span></span>|[<span data-ttu-id="85581-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="85581-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="85581-190">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="85581-190">The Application's availability.</span></span> <span data-ttu-id="85581-191">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="85581-192">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="85581-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="85581-193">version</span><span class="sxs-lookup"><span data-stu-id="85581-193">version</span></span>|<span data-ttu-id="85581-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85581-194">String</span></span>|<span data-ttu-id="85581-195">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="85581-195">The Application's version.</span></span> <span data-ttu-id="85581-196">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="85581-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="85581-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="85581-197">committedContentVersion</span></span>|<span data-ttu-id="85581-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85581-198">String</span></span>|<span data-ttu-id="85581-199">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="85581-199">The internal committed content version.</span></span> <span data-ttu-id="85581-200">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="85581-201">fileName</span><span class="sxs-lookup"><span data-stu-id="85581-201">fileName</span></span>|<span data-ttu-id="85581-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85581-202">String</span></span>|<span data-ttu-id="85581-203">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="85581-203">The name of the main Lob application file.</span></span> <span data-ttu-id="85581-204">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="85581-205">size</span><span class="sxs-lookup"><span data-stu-id="85581-205">size</span></span>|<span data-ttu-id="85581-206">Int64</span><span class="sxs-lookup"><span data-stu-id="85581-206">Int64</span></span>|<span data-ttu-id="85581-207">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="85581-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="85581-208">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="85581-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="85581-209">bundleId</span><span class="sxs-lookup"><span data-stu-id="85581-209">bundleId</span></span>|<span data-ttu-id="85581-210">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85581-210">String</span></span>|<span data-ttu-id="85581-211">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="85581-211">The Identity Name.</span></span>|
|<span data-ttu-id="85581-212">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="85581-212">applicableDeviceType</span></span>|[<span data-ttu-id="85581-213">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="85581-213">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="85581-214">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="85581-214">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="85581-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="85581-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="85581-216">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="85581-216">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="85581-217">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="85581-217">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="85581-218">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="85581-218">expirationDateTime</span></span>|<span data-ttu-id="85581-219">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85581-219">DateTimeOffset</span></span>|<span data-ttu-id="85581-220">Das Ablaufdatum.</span><span class="sxs-lookup"><span data-stu-id="85581-220">The expiration time.</span></span>|
|<span data-ttu-id="85581-221">versionNumber</span><span class="sxs-lookup"><span data-stu-id="85581-221">versionNumber</span></span>|<span data-ttu-id="85581-222">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85581-222">String</span></span>|<span data-ttu-id="85581-223">Die Versionsnummer der verwalteten branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="85581-223">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="85581-224">buildNumber</span><span class="sxs-lookup"><span data-stu-id="85581-224">buildNumber</span></span>|<span data-ttu-id="85581-225">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85581-225">String</span></span>|<span data-ttu-id="85581-226">Die Buildnummer der verwalteten branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="85581-226">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="85581-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="85581-227">Response</span></span>
<span data-ttu-id="85581-228">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85581-228">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85581-229">Beispiel</span><span class="sxs-lookup"><span data-stu-id="85581-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="85581-230">Anforderung</span><span class="sxs-lookup"><span data-stu-id="85581-230">Request</span></span>
<span data-ttu-id="85581-231">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="85581-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="85581-232">Antwort</span><span class="sxs-lookup"><span data-stu-id="85581-232">Response</span></span>
<span data-ttu-id="85581-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85581-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



