---
title: iosLobApp erstellen
description: Erstellt ein neues iosLobApp-Objekt.
ms.openlocfilehash: 2720192b45dcc55f74881163c93205ad5fecb24c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059393"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="c42cb-103">iosLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="c42cb-103">Create iosLobApp</span></span>

> <span data-ttu-id="c42cb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c42cb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c42cb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c42cb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c42cb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c42cb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c42cb-107">Erstellt ein neues [iosLobApp](../resources/intune-apps-ioslobapp.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="c42cb-107">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c42cb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c42cb-108">Prerequisites</span></span>
<span data-ttu-id="c42cb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c42cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c42cb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c42cb-111">Permission type</span></span>|<span data-ttu-id="c42cb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c42cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c42cb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c42cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c42cb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c42cb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c42cb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c42cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c42cb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c42cb-116">Not supported.</span></span>|
|<span data-ttu-id="c42cb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c42cb-117">Application</span></span>|<span data-ttu-id="c42cb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c42cb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c42cb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c42cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c42cb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c42cb-120">Request headers</span></span>
|<span data-ttu-id="c42cb-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c42cb-121">Header</span></span>|<span data-ttu-id="c42cb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c42cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c42cb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c42cb-123">Authorization</span></span>|<span data-ttu-id="c42cb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c42cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c42cb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c42cb-125">Accept</span></span>|<span data-ttu-id="c42cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c42cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c42cb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c42cb-127">Request body</span></span>
<span data-ttu-id="c42cb-128">Geben Sie im Anforderungstext eine JSON-Darstellung des iosLobApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c42cb-128">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="c42cb-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosLobApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c42cb-129">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="c42cb-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c42cb-130">Property</span></span>|<span data-ttu-id="c42cb-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c42cb-131">Type</span></span>|<span data-ttu-id="c42cb-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c42cb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c42cb-133">id</span><span class="sxs-lookup"><span data-stu-id="c42cb-133">id</span></span>|<span data-ttu-id="c42cb-134">String</span><span class="sxs-lookup"><span data-stu-id="c42cb-134">String</span></span>|<span data-ttu-id="c42cb-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c42cb-135">Key of the entity.</span></span> <span data-ttu-id="c42cb-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c42cb-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c42cb-137">displayName</span></span>|<span data-ttu-id="c42cb-138">String</span><span class="sxs-lookup"><span data-stu-id="c42cb-138">String</span></span>|<span data-ttu-id="c42cb-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="c42cb-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c42cb-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c42cb-141">description</span><span class="sxs-lookup"><span data-stu-id="c42cb-141">description</span></span>|<span data-ttu-id="c42cb-142">String</span><span class="sxs-lookup"><span data-stu-id="c42cb-142">String</span></span>|<span data-ttu-id="c42cb-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="c42cb-143">The description of the app.</span></span> <span data-ttu-id="c42cb-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c42cb-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c42cb-145">publisher</span></span>|<span data-ttu-id="c42cb-146">String</span><span class="sxs-lookup"><span data-stu-id="c42cb-146">String</span></span>|<span data-ttu-id="c42cb-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="c42cb-147">The publisher of the app.</span></span> <span data-ttu-id="c42cb-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c42cb-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c42cb-149">largeIcon</span></span>|[<span data-ttu-id="c42cb-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c42cb-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c42cb-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c42cb-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c42cb-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c42cb-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c42cb-153">createdDateTime</span></span>|<span data-ttu-id="c42cb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c42cb-154">DateTimeOffset</span></span>|<span data-ttu-id="c42cb-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="c42cb-155">The date and time the app was created.</span></span> <span data-ttu-id="c42cb-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c42cb-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c42cb-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c42cb-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c42cb-158">DateTimeOffset</span></span>|<span data-ttu-id="c42cb-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="c42cb-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c42cb-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c42cb-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c42cb-161">isFeatured</span></span>|<span data-ttu-id="c42cb-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c42cb-162">Boolean</span></span>|<span data-ttu-id="c42cb-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c42cb-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c42cb-164">privacyInformationUrl</span></span>|<span data-ttu-id="c42cb-165">String</span><span class="sxs-lookup"><span data-stu-id="c42cb-165">String</span></span>|<span data-ttu-id="c42cb-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="c42cb-166">The privacy statement Url.</span></span> <span data-ttu-id="c42cb-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c42cb-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c42cb-168">informationUrl</span></span>|<span data-ttu-id="c42cb-169">String</span><span class="sxs-lookup"><span data-stu-id="c42cb-169">String</span></span>|<span data-ttu-id="c42cb-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="c42cb-170">The more information Url.</span></span> <span data-ttu-id="c42cb-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c42cb-172">owner</span><span class="sxs-lookup"><span data-stu-id="c42cb-172">owner</span></span>|<span data-ttu-id="c42cb-173">String</span><span class="sxs-lookup"><span data-stu-id="c42cb-173">String</span></span>|<span data-ttu-id="c42cb-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="c42cb-174">The owner of the app.</span></span> <span data-ttu-id="c42cb-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c42cb-176">developer</span><span class="sxs-lookup"><span data-stu-id="c42cb-176">developer</span></span>|<span data-ttu-id="c42cb-177">String</span><span class="sxs-lookup"><span data-stu-id="c42cb-177">String</span></span>|<span data-ttu-id="c42cb-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="c42cb-178">The developer of the app.</span></span> <span data-ttu-id="c42cb-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c42cb-180">notes</span><span class="sxs-lookup"><span data-stu-id="c42cb-180">notes</span></span>|<span data-ttu-id="c42cb-181">String</span><span class="sxs-lookup"><span data-stu-id="c42cb-181">String</span></span>|<span data-ttu-id="c42cb-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="c42cb-182">Notes for the app.</span></span> <span data-ttu-id="c42cb-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c42cb-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c42cb-184">uploadState</span></span>|<span data-ttu-id="c42cb-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c42cb-185">Int32</span></span>|<span data-ttu-id="c42cb-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="c42cb-186">The upload state.</span></span> <span data-ttu-id="c42cb-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c42cb-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="c42cb-188">publishingState</span></span>|[<span data-ttu-id="c42cb-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c42cb-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c42cb-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="c42cb-190">The publishing state for the app.</span></span> <span data-ttu-id="c42cb-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="c42cb-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c42cb-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c42cb-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="c42cb-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c42cb-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="c42cb-194">committedContentVersion</span></span>|<span data-ttu-id="c42cb-195">String</span><span class="sxs-lookup"><span data-stu-id="c42cb-195">String</span></span>|<span data-ttu-id="c42cb-196">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="c42cb-196">The internal committed content version.</span></span> <span data-ttu-id="c42cb-197">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c42cb-198">fileName</span><span class="sxs-lookup"><span data-stu-id="c42cb-198">fileName</span></span>|<span data-ttu-id="c42cb-199">String</span><span class="sxs-lookup"><span data-stu-id="c42cb-199">String</span></span>|<span data-ttu-id="c42cb-200">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="c42cb-200">The name of the main Lob application file.</span></span> <span data-ttu-id="c42cb-201">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c42cb-202">size</span><span class="sxs-lookup"><span data-stu-id="c42cb-202">size</span></span>|<span data-ttu-id="c42cb-203">Int64</span><span class="sxs-lookup"><span data-stu-id="c42cb-203">Int64</span></span>|<span data-ttu-id="c42cb-204">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="c42cb-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="c42cb-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c42cb-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c42cb-206">bundleId</span><span class="sxs-lookup"><span data-stu-id="c42cb-206">bundleId</span></span>|<span data-ttu-id="c42cb-207">String</span><span class="sxs-lookup"><span data-stu-id="c42cb-207">String</span></span>|<span data-ttu-id="c42cb-208">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="c42cb-208">The Identity Name.</span></span>|
|<span data-ttu-id="c42cb-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="c42cb-209">applicableDeviceType</span></span>|[<span data-ttu-id="c42cb-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="c42cb-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="c42cb-211">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="c42cb-211">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="c42cb-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c42cb-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c42cb-213">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c42cb-213">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="c42cb-214">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="c42cb-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="c42cb-215">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c42cb-215">expirationDateTime</span></span>|<span data-ttu-id="c42cb-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c42cb-216">DateTimeOffset</span></span>|<span data-ttu-id="c42cb-217">Das Ablaufdatum.</span><span class="sxs-lookup"><span data-stu-id="c42cb-217">The expiration time.</span></span>|
|<span data-ttu-id="c42cb-218">versionNumber</span><span class="sxs-lookup"><span data-stu-id="c42cb-218">versionNumber</span></span>|<span data-ttu-id="c42cb-219">String</span><span class="sxs-lookup"><span data-stu-id="c42cb-219">String</span></span>|<span data-ttu-id="c42cb-220">Die Versionsnummer der branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="c42cb-220">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c42cb-221">buildNumber</span><span class="sxs-lookup"><span data-stu-id="c42cb-221">buildNumber</span></span>|<span data-ttu-id="c42cb-222">String</span><span class="sxs-lookup"><span data-stu-id="c42cb-222">String</span></span>|<span data-ttu-id="c42cb-223">Die Buildnummer der branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="c42cb-223">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c42cb-224">identityVersion</span><span class="sxs-lookup"><span data-stu-id="c42cb-224">identityVersion</span></span>|<span data-ttu-id="c42cb-225">String</span><span class="sxs-lookup"><span data-stu-id="c42cb-225">String</span></span>|<span data-ttu-id="c42cb-226">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="c42cb-226">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="c42cb-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="c42cb-227">Response</span></span>
<span data-ttu-id="c42cb-228">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosLobApp](../resources/intune-apps-ioslobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c42cb-228">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c42cb-229">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c42cb-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="c42cb-230">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c42cb-230">Request</span></span>
<span data-ttu-id="c42cb-231">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c42cb-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1343

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
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
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
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="c42cb-232">Antwort</span><span class="sxs-lookup"><span data-stu-id="c42cb-232">Response</span></span>
<span data-ttu-id="c42cb-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c42cb-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1451

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
  "uploadState": 11,
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
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```





