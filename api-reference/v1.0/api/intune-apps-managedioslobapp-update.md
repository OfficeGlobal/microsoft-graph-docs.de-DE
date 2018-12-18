---
title: managedIOSLobApp aktualisieren
description: Aktualisieren der Eigenschaften eines managedIOSLobApp-Objekts.
author: tfitzmac
ms.openlocfilehash: adcd36af7354a9a0e4807fe38f6bc407fe235e83
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353648"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="17631-103">managedIOSLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="17631-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="17631-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="17631-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17631-105">Aktualisieren der Eigenschaften eines [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="17631-105">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="17631-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="17631-106">Prerequisites</span></span>
<span data-ttu-id="17631-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17631-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17631-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="17631-109">Permission type</span></span>|<span data-ttu-id="17631-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="17631-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17631-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="17631-111">Delegated (work or school account)</span></span>|<span data-ttu-id="17631-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17631-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="17631-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="17631-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17631-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="17631-114">Not supported.</span></span>|
|<span data-ttu-id="17631-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="17631-115">Application</span></span>|<span data-ttu-id="17631-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="17631-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17631-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="17631-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="17631-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="17631-118">Request headers</span></span>
|<span data-ttu-id="17631-119">Header</span><span class="sxs-lookup"><span data-stu-id="17631-119">Header</span></span>|<span data-ttu-id="17631-120">Wert</span><span class="sxs-lookup"><span data-stu-id="17631-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17631-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="17631-121">Authorization</span></span>|<span data-ttu-id="17631-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="17631-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17631-123">Accept</span><span class="sxs-lookup"><span data-stu-id="17631-123">Accept</span></span>|<span data-ttu-id="17631-124">application/json</span><span class="sxs-lookup"><span data-stu-id="17631-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17631-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="17631-125">Request body</span></span>
<span data-ttu-id="17631-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="17631-126">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="17631-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="17631-127">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="17631-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="17631-128">Property</span></span>|<span data-ttu-id="17631-129">Typ</span><span class="sxs-lookup"><span data-stu-id="17631-129">Type</span></span>|<span data-ttu-id="17631-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17631-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17631-131">id</span><span class="sxs-lookup"><span data-stu-id="17631-131">id</span></span>|<span data-ttu-id="17631-132">String</span><span class="sxs-lookup"><span data-stu-id="17631-132">String</span></span>|<span data-ttu-id="17631-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="17631-133">Key of the entity.</span></span> <span data-ttu-id="17631-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17631-135">displayName</span><span class="sxs-lookup"><span data-stu-id="17631-135">displayName</span></span>|<span data-ttu-id="17631-136">String</span><span class="sxs-lookup"><span data-stu-id="17631-136">String</span></span>|<span data-ttu-id="17631-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="17631-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="17631-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17631-139">description</span><span class="sxs-lookup"><span data-stu-id="17631-139">description</span></span>|<span data-ttu-id="17631-140">String</span><span class="sxs-lookup"><span data-stu-id="17631-140">String</span></span>|<span data-ttu-id="17631-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="17631-141">The description of the app.</span></span> <span data-ttu-id="17631-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17631-143">publisher</span><span class="sxs-lookup"><span data-stu-id="17631-143">publisher</span></span>|<span data-ttu-id="17631-144">String</span><span class="sxs-lookup"><span data-stu-id="17631-144">String</span></span>|<span data-ttu-id="17631-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="17631-145">The publisher of the app.</span></span> <span data-ttu-id="17631-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17631-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="17631-147">largeIcon</span></span>|[<span data-ttu-id="17631-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="17631-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="17631-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="17631-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="17631-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17631-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17631-151">createdDateTime</span></span>|<span data-ttu-id="17631-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17631-152">DateTimeOffset</span></span>|<span data-ttu-id="17631-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="17631-153">The date and time the app was created.</span></span> <span data-ttu-id="17631-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17631-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17631-155">lastModifiedDateTime</span></span>|<span data-ttu-id="17631-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17631-156">DateTimeOffset</span></span>|<span data-ttu-id="17631-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="17631-157">The date and time the app was last modified.</span></span> <span data-ttu-id="17631-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17631-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="17631-159">isFeatured</span></span>|<span data-ttu-id="17631-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="17631-160">Boolean</span></span>|<span data-ttu-id="17631-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17631-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="17631-162">privacyInformationUrl</span></span>|<span data-ttu-id="17631-163">String</span><span class="sxs-lookup"><span data-stu-id="17631-163">String</span></span>|<span data-ttu-id="17631-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="17631-164">The privacy statement Url.</span></span> <span data-ttu-id="17631-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17631-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="17631-166">informationUrl</span></span>|<span data-ttu-id="17631-167">String</span><span class="sxs-lookup"><span data-stu-id="17631-167">String</span></span>|<span data-ttu-id="17631-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="17631-168">The more information Url.</span></span> <span data-ttu-id="17631-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17631-170">owner</span><span class="sxs-lookup"><span data-stu-id="17631-170">owner</span></span>|<span data-ttu-id="17631-171">String</span><span class="sxs-lookup"><span data-stu-id="17631-171">String</span></span>|<span data-ttu-id="17631-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="17631-172">The owner of the app.</span></span> <span data-ttu-id="17631-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17631-174">developer</span><span class="sxs-lookup"><span data-stu-id="17631-174">developer</span></span>|<span data-ttu-id="17631-175">String</span><span class="sxs-lookup"><span data-stu-id="17631-175">String</span></span>|<span data-ttu-id="17631-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="17631-176">The developer of the app.</span></span> <span data-ttu-id="17631-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17631-178">notes</span><span class="sxs-lookup"><span data-stu-id="17631-178">notes</span></span>|<span data-ttu-id="17631-179">String</span><span class="sxs-lookup"><span data-stu-id="17631-179">String</span></span>|<span data-ttu-id="17631-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="17631-180">Notes for the app.</span></span> <span data-ttu-id="17631-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17631-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="17631-182">publishingState</span></span>|[<span data-ttu-id="17631-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="17631-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="17631-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="17631-184">The publishing state for the app.</span></span> <span data-ttu-id="17631-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="17631-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="17631-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="17631-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="17631-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="17631-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="17631-188">appAvailability</span></span>|[<span data-ttu-id="17631-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="17631-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="17631-190">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="17631-190">The Application's availability.</span></span> <span data-ttu-id="17631-191">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="17631-192">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="17631-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="17631-193">version</span><span class="sxs-lookup"><span data-stu-id="17631-193">version</span></span>|<span data-ttu-id="17631-194">String</span><span class="sxs-lookup"><span data-stu-id="17631-194">String</span></span>|<span data-ttu-id="17631-195">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="17631-195">The Application's version.</span></span> <span data-ttu-id="17631-196">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="17631-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="17631-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="17631-197">committedContentVersion</span></span>|<span data-ttu-id="17631-198">String</span><span class="sxs-lookup"><span data-stu-id="17631-198">String</span></span>|<span data-ttu-id="17631-199">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="17631-199">The internal committed content version.</span></span> <span data-ttu-id="17631-200">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="17631-201">fileName</span><span class="sxs-lookup"><span data-stu-id="17631-201">fileName</span></span>|<span data-ttu-id="17631-202">String</span><span class="sxs-lookup"><span data-stu-id="17631-202">String</span></span>|<span data-ttu-id="17631-203">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="17631-203">The name of the main Lob application file.</span></span> <span data-ttu-id="17631-204">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="17631-205">size</span><span class="sxs-lookup"><span data-stu-id="17631-205">size</span></span>|<span data-ttu-id="17631-206">Int64</span><span class="sxs-lookup"><span data-stu-id="17631-206">Int64</span></span>|<span data-ttu-id="17631-207">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="17631-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="17631-208">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="17631-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="17631-209">bundleId</span><span class="sxs-lookup"><span data-stu-id="17631-209">bundleId</span></span>|<span data-ttu-id="17631-210">String</span><span class="sxs-lookup"><span data-stu-id="17631-210">String</span></span>|<span data-ttu-id="17631-211">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="17631-211">The Identity Name.</span></span>|
|<span data-ttu-id="17631-212">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="17631-212">applicableDeviceType</span></span>|[<span data-ttu-id="17631-213">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="17631-213">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="17631-214">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="17631-214">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="17631-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="17631-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="17631-216">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="17631-216">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="17631-217">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="17631-217">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="17631-218">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="17631-218">expirationDateTime</span></span>|<span data-ttu-id="17631-219">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17631-219">DateTimeOffset</span></span>|<span data-ttu-id="17631-220">Das Ablaufdatum.</span><span class="sxs-lookup"><span data-stu-id="17631-220">The expiration time.</span></span>|
|<span data-ttu-id="17631-221">versionNumber</span><span class="sxs-lookup"><span data-stu-id="17631-221">versionNumber</span></span>|<span data-ttu-id="17631-222">String</span><span class="sxs-lookup"><span data-stu-id="17631-222">String</span></span>|<span data-ttu-id="17631-223">Die Versionsnummer der verwalteten branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="17631-223">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="17631-224">buildNumber</span><span class="sxs-lookup"><span data-stu-id="17631-224">buildNumber</span></span>|<span data-ttu-id="17631-225">String</span><span class="sxs-lookup"><span data-stu-id="17631-225">String</span></span>|<span data-ttu-id="17631-226">Die Buildnummer der verwalteten branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="17631-226">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="17631-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="17631-227">Response</span></span>
<span data-ttu-id="17631-228">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="17631-228">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17631-229">Beispiel</span><span class="sxs-lookup"><span data-stu-id="17631-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="17631-230">Anforderung</span><span class="sxs-lookup"><span data-stu-id="17631-230">Request</span></span>
<span data-ttu-id="17631-231">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="17631-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="17631-232">Antwort</span><span class="sxs-lookup"><span data-stu-id="17631-232">Response</span></span>
<span data-ttu-id="17631-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="17631-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



