---
title: iosLobApp aktualisieren
description: Aktualisieren der Eigenschaften eines iosLobApp-Objekts.
ms.openlocfilehash: 159bdb4091d5ab0005ad0e9c1ba1720ee85a775e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018190"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="2b79a-103">iosLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2b79a-103">Update iosLobApp</span></span>

> <span data-ttu-id="2b79a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2b79a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b79a-105">Aktualisieren der Eigenschaften eines [iosLobApp](../resources/intune-apps-ioslobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2b79a-105">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b79a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2b79a-106">Prerequisites</span></span>
<span data-ttu-id="2b79a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b79a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b79a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2b79a-109">Permission type</span></span>|<span data-ttu-id="2b79a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2b79a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b79a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2b79a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2b79a-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b79a-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2b79a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2b79a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b79a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b79a-114">Not supported.</span></span>|
|<span data-ttu-id="2b79a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2b79a-115">Application</span></span>|<span data-ttu-id="2b79a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b79a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b79a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b79a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="2b79a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2b79a-118">Request headers</span></span>
|<span data-ttu-id="2b79a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2b79a-119">Header</span></span>|<span data-ttu-id="2b79a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2b79a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b79a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b79a-121">Authorization</span></span>|<span data-ttu-id="2b79a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2b79a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b79a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2b79a-123">Accept</span></span>|<span data-ttu-id="2b79a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2b79a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b79a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2b79a-125">Request body</span></span>
<span data-ttu-id="2b79a-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosLobApp](../resources/intune-apps-ioslobapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="2b79a-126">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="2b79a-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosLobApp](../resources/intune-apps-ioslobapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2b79a-127">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="2b79a-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2b79a-128">Property</span></span>|<span data-ttu-id="2b79a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="2b79a-129">Type</span></span>|<span data-ttu-id="2b79a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b79a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b79a-131">id</span><span class="sxs-lookup"><span data-stu-id="2b79a-131">id</span></span>|<span data-ttu-id="2b79a-132">String</span><span class="sxs-lookup"><span data-stu-id="2b79a-132">String</span></span>|<span data-ttu-id="2b79a-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2b79a-133">Key of the entity.</span></span> <span data-ttu-id="2b79a-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2b79a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2b79a-135">displayName</span></span>|<span data-ttu-id="2b79a-136">String</span><span class="sxs-lookup"><span data-stu-id="2b79a-136">String</span></span>|<span data-ttu-id="2b79a-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="2b79a-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2b79a-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2b79a-139">description</span><span class="sxs-lookup"><span data-stu-id="2b79a-139">description</span></span>|<span data-ttu-id="2b79a-140">String</span><span class="sxs-lookup"><span data-stu-id="2b79a-140">String</span></span>|<span data-ttu-id="2b79a-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="2b79a-141">The description of the app.</span></span> <span data-ttu-id="2b79a-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2b79a-143">publisher</span><span class="sxs-lookup"><span data-stu-id="2b79a-143">publisher</span></span>|<span data-ttu-id="2b79a-144">String</span><span class="sxs-lookup"><span data-stu-id="2b79a-144">String</span></span>|<span data-ttu-id="2b79a-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="2b79a-145">The publisher of the app.</span></span> <span data-ttu-id="2b79a-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2b79a-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2b79a-147">largeIcon</span></span>|[<span data-ttu-id="2b79a-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2b79a-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2b79a-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="2b79a-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2b79a-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2b79a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b79a-151">createdDateTime</span></span>|<span data-ttu-id="2b79a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b79a-152">DateTimeOffset</span></span>|<span data-ttu-id="2b79a-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="2b79a-153">The date and time the app was created.</span></span> <span data-ttu-id="2b79a-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2b79a-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b79a-155">lastModifiedDateTime</span></span>|<span data-ttu-id="2b79a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b79a-156">DateTimeOffset</span></span>|<span data-ttu-id="2b79a-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="2b79a-157">The date and time the app was last modified.</span></span> <span data-ttu-id="2b79a-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2b79a-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2b79a-159">isFeatured</span></span>|<span data-ttu-id="2b79a-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2b79a-160">Boolean</span></span>|<span data-ttu-id="2b79a-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2b79a-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2b79a-162">privacyInformationUrl</span></span>|<span data-ttu-id="2b79a-163">String</span><span class="sxs-lookup"><span data-stu-id="2b79a-163">String</span></span>|<span data-ttu-id="2b79a-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="2b79a-164">The privacy statement Url.</span></span> <span data-ttu-id="2b79a-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2b79a-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2b79a-166">informationUrl</span></span>|<span data-ttu-id="2b79a-167">String</span><span class="sxs-lookup"><span data-stu-id="2b79a-167">String</span></span>|<span data-ttu-id="2b79a-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="2b79a-168">The more information Url.</span></span> <span data-ttu-id="2b79a-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2b79a-170">owner</span><span class="sxs-lookup"><span data-stu-id="2b79a-170">owner</span></span>|<span data-ttu-id="2b79a-171">String</span><span class="sxs-lookup"><span data-stu-id="2b79a-171">String</span></span>|<span data-ttu-id="2b79a-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="2b79a-172">The owner of the app.</span></span> <span data-ttu-id="2b79a-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2b79a-174">developer</span><span class="sxs-lookup"><span data-stu-id="2b79a-174">developer</span></span>|<span data-ttu-id="2b79a-175">String</span><span class="sxs-lookup"><span data-stu-id="2b79a-175">String</span></span>|<span data-ttu-id="2b79a-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="2b79a-176">The developer of the app.</span></span> <span data-ttu-id="2b79a-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2b79a-178">notes</span><span class="sxs-lookup"><span data-stu-id="2b79a-178">notes</span></span>|<span data-ttu-id="2b79a-179">String</span><span class="sxs-lookup"><span data-stu-id="2b79a-179">String</span></span>|<span data-ttu-id="2b79a-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="2b79a-180">Notes for the app.</span></span> <span data-ttu-id="2b79a-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2b79a-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="2b79a-182">publishingState</span></span>|[<span data-ttu-id="2b79a-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2b79a-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2b79a-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="2b79a-184">The publishing state for the app.</span></span> <span data-ttu-id="2b79a-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="2b79a-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2b79a-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2b79a-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="2b79a-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2b79a-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="2b79a-188">committedContentVersion</span></span>|<span data-ttu-id="2b79a-189">String</span><span class="sxs-lookup"><span data-stu-id="2b79a-189">String</span></span>|<span data-ttu-id="2b79a-190">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="2b79a-190">The internal committed content version.</span></span> <span data-ttu-id="2b79a-191">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2b79a-192">fileName</span><span class="sxs-lookup"><span data-stu-id="2b79a-192">fileName</span></span>|<span data-ttu-id="2b79a-193">String</span><span class="sxs-lookup"><span data-stu-id="2b79a-193">String</span></span>|<span data-ttu-id="2b79a-194">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="2b79a-194">The name of the main Lob application file.</span></span> <span data-ttu-id="2b79a-195">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2b79a-196">size</span><span class="sxs-lookup"><span data-stu-id="2b79a-196">size</span></span>|<span data-ttu-id="2b79a-197">Int64</span><span class="sxs-lookup"><span data-stu-id="2b79a-197">Int64</span></span>|<span data-ttu-id="2b79a-198">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="2b79a-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="2b79a-199">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b79a-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2b79a-200">bundleId</span><span class="sxs-lookup"><span data-stu-id="2b79a-200">bundleId</span></span>|<span data-ttu-id="2b79a-201">String</span><span class="sxs-lookup"><span data-stu-id="2b79a-201">String</span></span>|<span data-ttu-id="2b79a-202">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="2b79a-202">The Identity Name.</span></span>|
|<span data-ttu-id="2b79a-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="2b79a-203">applicableDeviceType</span></span>|[<span data-ttu-id="2b79a-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="2b79a-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="2b79a-205">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="2b79a-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="2b79a-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2b79a-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2b79a-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2b79a-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="2b79a-208">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="2b79a-208">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="2b79a-209">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2b79a-209">expirationDateTime</span></span>|<span data-ttu-id="2b79a-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b79a-210">DateTimeOffset</span></span>|<span data-ttu-id="2b79a-211">Das Ablaufdatum.</span><span class="sxs-lookup"><span data-stu-id="2b79a-211">The expiration time.</span></span>|
|<span data-ttu-id="2b79a-212">versionNumber</span><span class="sxs-lookup"><span data-stu-id="2b79a-212">versionNumber</span></span>|<span data-ttu-id="2b79a-213">String</span><span class="sxs-lookup"><span data-stu-id="2b79a-213">String</span></span>|<span data-ttu-id="2b79a-214">Die Versionsnummer der branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="2b79a-214">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="2b79a-215">buildNumber</span><span class="sxs-lookup"><span data-stu-id="2b79a-215">buildNumber</span></span>|<span data-ttu-id="2b79a-216">String</span><span class="sxs-lookup"><span data-stu-id="2b79a-216">String</span></span>|<span data-ttu-id="2b79a-217">Die Buildnummer der branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="2b79a-217">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="2b79a-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b79a-218">Response</span></span>
<span data-ttu-id="2b79a-219">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [iosLobApp](../resources/intune-apps-ioslobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b79a-219">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b79a-220">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2b79a-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b79a-221">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b79a-221">Request</span></span>
<span data-ttu-id="2b79a-222">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2b79a-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1209

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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

### <a name="response"></a><span data-ttu-id="2b79a-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b79a-223">Response</span></span>
<span data-ttu-id="2b79a-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b79a-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1381

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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



