---
title: iosLobApp aktualisieren
description: Aktualisieren der Eigenschaften eines iosLobApp-Objekts.
author: tfitzmac
ms.openlocfilehash: cffa5603cf92bd8e45c95ebb805618c1293851eb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354264"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="dc514-103">iosLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="dc514-103">Update iosLobApp</span></span>

> <span data-ttu-id="dc514-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dc514-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc514-105">Aktualisieren der Eigenschaften eines [iosLobApp](../resources/intune-apps-ioslobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="dc514-105">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc514-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dc514-106">Prerequisites</span></span>
<span data-ttu-id="dc514-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc514-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc514-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dc514-109">Permission type</span></span>|<span data-ttu-id="dc514-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dc514-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc514-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dc514-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dc514-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc514-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dc514-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dc514-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc514-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dc514-114">Not supported.</span></span>|
|<span data-ttu-id="dc514-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dc514-115">Application</span></span>|<span data-ttu-id="dc514-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dc514-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc514-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc514-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="dc514-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dc514-118">Request headers</span></span>
|<span data-ttu-id="dc514-119">Header</span><span class="sxs-lookup"><span data-stu-id="dc514-119">Header</span></span>|<span data-ttu-id="dc514-120">Wert</span><span class="sxs-lookup"><span data-stu-id="dc514-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc514-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="dc514-121">Authorization</span></span>|<span data-ttu-id="dc514-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dc514-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc514-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dc514-123">Accept</span></span>|<span data-ttu-id="dc514-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dc514-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc514-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dc514-125">Request body</span></span>
<span data-ttu-id="dc514-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosLobApp](../resources/intune-apps-ioslobapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="dc514-126">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="dc514-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosLobApp](../resources/intune-apps-ioslobapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="dc514-127">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="dc514-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dc514-128">Property</span></span>|<span data-ttu-id="dc514-129">Typ</span><span class="sxs-lookup"><span data-stu-id="dc514-129">Type</span></span>|<span data-ttu-id="dc514-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dc514-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc514-131">id</span><span class="sxs-lookup"><span data-stu-id="dc514-131">id</span></span>|<span data-ttu-id="dc514-132">String</span><span class="sxs-lookup"><span data-stu-id="dc514-132">String</span></span>|<span data-ttu-id="dc514-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="dc514-133">Key of the entity.</span></span> <span data-ttu-id="dc514-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc514-135">displayName</span><span class="sxs-lookup"><span data-stu-id="dc514-135">displayName</span></span>|<span data-ttu-id="dc514-136">String</span><span class="sxs-lookup"><span data-stu-id="dc514-136">String</span></span>|<span data-ttu-id="dc514-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="dc514-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="dc514-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc514-139">description</span><span class="sxs-lookup"><span data-stu-id="dc514-139">description</span></span>|<span data-ttu-id="dc514-140">String</span><span class="sxs-lookup"><span data-stu-id="dc514-140">String</span></span>|<span data-ttu-id="dc514-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="dc514-141">The description of the app.</span></span> <span data-ttu-id="dc514-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc514-143">publisher</span><span class="sxs-lookup"><span data-stu-id="dc514-143">publisher</span></span>|<span data-ttu-id="dc514-144">String</span><span class="sxs-lookup"><span data-stu-id="dc514-144">String</span></span>|<span data-ttu-id="dc514-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="dc514-145">The publisher of the app.</span></span> <span data-ttu-id="dc514-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc514-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="dc514-147">largeIcon</span></span>|[<span data-ttu-id="dc514-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="dc514-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="dc514-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="dc514-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="dc514-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc514-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dc514-151">createdDateTime</span></span>|<span data-ttu-id="dc514-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc514-152">DateTimeOffset</span></span>|<span data-ttu-id="dc514-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="dc514-153">The date and time the app was created.</span></span> <span data-ttu-id="dc514-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc514-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc514-155">lastModifiedDateTime</span></span>|<span data-ttu-id="dc514-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc514-156">DateTimeOffset</span></span>|<span data-ttu-id="dc514-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="dc514-157">The date and time the app was last modified.</span></span> <span data-ttu-id="dc514-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc514-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="dc514-159">isFeatured</span></span>|<span data-ttu-id="dc514-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc514-160">Boolean</span></span>|<span data-ttu-id="dc514-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc514-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="dc514-162">privacyInformationUrl</span></span>|<span data-ttu-id="dc514-163">String</span><span class="sxs-lookup"><span data-stu-id="dc514-163">String</span></span>|<span data-ttu-id="dc514-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="dc514-164">The privacy statement Url.</span></span> <span data-ttu-id="dc514-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc514-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="dc514-166">informationUrl</span></span>|<span data-ttu-id="dc514-167">String</span><span class="sxs-lookup"><span data-stu-id="dc514-167">String</span></span>|<span data-ttu-id="dc514-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="dc514-168">The more information Url.</span></span> <span data-ttu-id="dc514-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc514-170">owner</span><span class="sxs-lookup"><span data-stu-id="dc514-170">owner</span></span>|<span data-ttu-id="dc514-171">String</span><span class="sxs-lookup"><span data-stu-id="dc514-171">String</span></span>|<span data-ttu-id="dc514-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="dc514-172">The owner of the app.</span></span> <span data-ttu-id="dc514-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc514-174">developer</span><span class="sxs-lookup"><span data-stu-id="dc514-174">developer</span></span>|<span data-ttu-id="dc514-175">String</span><span class="sxs-lookup"><span data-stu-id="dc514-175">String</span></span>|<span data-ttu-id="dc514-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="dc514-176">The developer of the app.</span></span> <span data-ttu-id="dc514-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc514-178">notes</span><span class="sxs-lookup"><span data-stu-id="dc514-178">notes</span></span>|<span data-ttu-id="dc514-179">String</span><span class="sxs-lookup"><span data-stu-id="dc514-179">String</span></span>|<span data-ttu-id="dc514-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="dc514-180">Notes for the app.</span></span> <span data-ttu-id="dc514-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc514-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="dc514-182">publishingState</span></span>|[<span data-ttu-id="dc514-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="dc514-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="dc514-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="dc514-184">The publishing state for the app.</span></span> <span data-ttu-id="dc514-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="dc514-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="dc514-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="dc514-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="dc514-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="dc514-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="dc514-188">committedContentVersion</span></span>|<span data-ttu-id="dc514-189">String</span><span class="sxs-lookup"><span data-stu-id="dc514-189">String</span></span>|<span data-ttu-id="dc514-190">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="dc514-190">The internal committed content version.</span></span> <span data-ttu-id="dc514-191">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="dc514-192">fileName</span><span class="sxs-lookup"><span data-stu-id="dc514-192">fileName</span></span>|<span data-ttu-id="dc514-193">String</span><span class="sxs-lookup"><span data-stu-id="dc514-193">String</span></span>|<span data-ttu-id="dc514-194">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="dc514-194">The name of the main Lob application file.</span></span> <span data-ttu-id="dc514-195">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="dc514-196">size</span><span class="sxs-lookup"><span data-stu-id="dc514-196">size</span></span>|<span data-ttu-id="dc514-197">Int64</span><span class="sxs-lookup"><span data-stu-id="dc514-197">Int64</span></span>|<span data-ttu-id="dc514-198">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="dc514-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="dc514-199">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc514-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="dc514-200">bundleId</span><span class="sxs-lookup"><span data-stu-id="dc514-200">bundleId</span></span>|<span data-ttu-id="dc514-201">String</span><span class="sxs-lookup"><span data-stu-id="dc514-201">String</span></span>|<span data-ttu-id="dc514-202">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="dc514-202">The Identity Name.</span></span>|
|<span data-ttu-id="dc514-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="dc514-203">applicableDeviceType</span></span>|[<span data-ttu-id="dc514-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="dc514-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="dc514-205">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="dc514-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="dc514-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dc514-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="dc514-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dc514-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="dc514-208">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="dc514-208">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="dc514-209">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dc514-209">expirationDateTime</span></span>|<span data-ttu-id="dc514-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc514-210">DateTimeOffset</span></span>|<span data-ttu-id="dc514-211">Das Ablaufdatum.</span><span class="sxs-lookup"><span data-stu-id="dc514-211">The expiration time.</span></span>|
|<span data-ttu-id="dc514-212">versionNumber</span><span class="sxs-lookup"><span data-stu-id="dc514-212">versionNumber</span></span>|<span data-ttu-id="dc514-213">String</span><span class="sxs-lookup"><span data-stu-id="dc514-213">String</span></span>|<span data-ttu-id="dc514-214">Die Versionsnummer der branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="dc514-214">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="dc514-215">buildNumber</span><span class="sxs-lookup"><span data-stu-id="dc514-215">buildNumber</span></span>|<span data-ttu-id="dc514-216">String</span><span class="sxs-lookup"><span data-stu-id="dc514-216">String</span></span>|<span data-ttu-id="dc514-217">Die Buildnummer der branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="dc514-217">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="dc514-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc514-218">Response</span></span>
<span data-ttu-id="dc514-219">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [iosLobApp](../resources/intune-apps-ioslobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dc514-219">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc514-220">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dc514-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc514-221">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc514-221">Request</span></span>
<span data-ttu-id="dc514-222">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dc514-222">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dc514-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc514-223">Response</span></span>
<span data-ttu-id="dc514-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dc514-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



