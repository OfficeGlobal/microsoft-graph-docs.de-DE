---
title: iosStoreApp aktualisieren
description: Aktualisieren der Eigenschaften eines iosStoreApp-Objekts.
ms.openlocfilehash: 47fdc0b9f22f049818300deacb6dc3cb7ab58800
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061916"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="1f6a0-103">iosStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1f6a0-103">Update iosStoreApp</span></span>

> <span data-ttu-id="1f6a0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f6a0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f6a0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f6a0-107">Aktualisieren der Eigenschaften eines [iosStoreApp](../resources/intune-apps-iosstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-107">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1f6a0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1f6a0-108">Prerequisites</span></span>
<span data-ttu-id="1f6a0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f6a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f6a0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f6a0-111">Permission type</span></span>|<span data-ttu-id="1f6a0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f6a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f6a0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f6a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f6a0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f6a0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1f6a0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1f6a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f6a0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f6a0-116">Not supported.</span></span>|
|<span data-ttu-id="1f6a0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f6a0-117">Application</span></span>|<span data-ttu-id="1f6a0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f6a0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f6a0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f6a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="1f6a0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f6a0-120">Request headers</span></span>
|<span data-ttu-id="1f6a0-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1f6a0-121">Header</span></span>|<span data-ttu-id="1f6a0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1f6a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f6a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f6a0-123">Authorization</span></span>|<span data-ttu-id="1f6a0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1f6a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f6a0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1f6a0-125">Accept</span></span>|<span data-ttu-id="1f6a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f6a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f6a0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f6a0-127">Request body</span></span>
<span data-ttu-id="1f6a0-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosStoreApp](../resources/intune-apps-iosstoreapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-128">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="1f6a0-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosStoreApp](../resources/intune-apps-iosstoreapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-129">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="1f6a0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1f6a0-130">Property</span></span>|<span data-ttu-id="1f6a0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1f6a0-131">Type</span></span>|<span data-ttu-id="1f6a0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f6a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f6a0-133">id</span><span class="sxs-lookup"><span data-stu-id="1f6a0-133">id</span></span>|<span data-ttu-id="1f6a0-134">String</span><span class="sxs-lookup"><span data-stu-id="1f6a0-134">String</span></span>|<span data-ttu-id="1f6a0-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1f6a0-135">Key of the entity.</span></span> <span data-ttu-id="1f6a0-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1f6a0-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f6a0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1f6a0-137">displayName</span></span>|<span data-ttu-id="1f6a0-138">String</span><span class="sxs-lookup"><span data-stu-id="1f6a0-138">String</span></span>|<span data-ttu-id="1f6a0-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1f6a0-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1f6a0-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f6a0-141">description</span><span class="sxs-lookup"><span data-stu-id="1f6a0-141">description</span></span>|<span data-ttu-id="1f6a0-142">String</span><span class="sxs-lookup"><span data-stu-id="1f6a0-142">String</span></span>|<span data-ttu-id="1f6a0-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-143">The description of the app.</span></span> <span data-ttu-id="1f6a0-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1f6a0-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f6a0-145">publisher</span><span class="sxs-lookup"><span data-stu-id="1f6a0-145">publisher</span></span>|<span data-ttu-id="1f6a0-146">String</span><span class="sxs-lookup"><span data-stu-id="1f6a0-146">String</span></span>|<span data-ttu-id="1f6a0-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-147">The publisher of the app.</span></span> <span data-ttu-id="1f6a0-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1f6a0-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f6a0-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1f6a0-149">largeIcon</span></span>|[<span data-ttu-id="1f6a0-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1f6a0-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1f6a0-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1f6a0-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1f6a0-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f6a0-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f6a0-153">createdDateTime</span></span>|<span data-ttu-id="1f6a0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f6a0-154">DateTimeOffset</span></span>|<span data-ttu-id="1f6a0-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-155">The date and time the app was created.</span></span> <span data-ttu-id="1f6a0-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1f6a0-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f6a0-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f6a0-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1f6a0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f6a0-158">DateTimeOffset</span></span>|<span data-ttu-id="1f6a0-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1f6a0-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1f6a0-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f6a0-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1f6a0-161">isFeatured</span></span>|<span data-ttu-id="1f6a0-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1f6a0-162">Boolean</span></span>|<span data-ttu-id="1f6a0-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1f6a0-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f6a0-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1f6a0-164">privacyInformationUrl</span></span>|<span data-ttu-id="1f6a0-165">String</span><span class="sxs-lookup"><span data-stu-id="1f6a0-165">String</span></span>|<span data-ttu-id="1f6a0-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-166">The privacy statement Url.</span></span> <span data-ttu-id="1f6a0-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1f6a0-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f6a0-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1f6a0-168">informationUrl</span></span>|<span data-ttu-id="1f6a0-169">String</span><span class="sxs-lookup"><span data-stu-id="1f6a0-169">String</span></span>|<span data-ttu-id="1f6a0-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-170">The more information Url.</span></span> <span data-ttu-id="1f6a0-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1f6a0-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f6a0-172">owner</span><span class="sxs-lookup"><span data-stu-id="1f6a0-172">owner</span></span>|<span data-ttu-id="1f6a0-173">String</span><span class="sxs-lookup"><span data-stu-id="1f6a0-173">String</span></span>|<span data-ttu-id="1f6a0-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-174">The owner of the app.</span></span> <span data-ttu-id="1f6a0-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1f6a0-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f6a0-176">developer</span><span class="sxs-lookup"><span data-stu-id="1f6a0-176">developer</span></span>|<span data-ttu-id="1f6a0-177">String</span><span class="sxs-lookup"><span data-stu-id="1f6a0-177">String</span></span>|<span data-ttu-id="1f6a0-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-178">The developer of the app.</span></span> <span data-ttu-id="1f6a0-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1f6a0-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f6a0-180">notes</span><span class="sxs-lookup"><span data-stu-id="1f6a0-180">notes</span></span>|<span data-ttu-id="1f6a0-181">String</span><span class="sxs-lookup"><span data-stu-id="1f6a0-181">String</span></span>|<span data-ttu-id="1f6a0-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-182">Notes for the app.</span></span> <span data-ttu-id="1f6a0-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1f6a0-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f6a0-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1f6a0-184">uploadState</span></span>|<span data-ttu-id="1f6a0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1f6a0-185">Int32</span></span>|<span data-ttu-id="1f6a0-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-186">The upload state.</span></span> <span data-ttu-id="1f6a0-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1f6a0-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f6a0-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="1f6a0-188">publishingState</span></span>|[<span data-ttu-id="1f6a0-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1f6a0-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1f6a0-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-190">The publishing state for the app.</span></span> <span data-ttu-id="1f6a0-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1f6a0-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1f6a0-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1f6a0-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1f6a0-194">bundleId</span><span class="sxs-lookup"><span data-stu-id="1f6a0-194">bundleId</span></span>|<span data-ttu-id="1f6a0-195">String</span><span class="sxs-lookup"><span data-stu-id="1f6a0-195">String</span></span>|<span data-ttu-id="1f6a0-196">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="1f6a0-196">The Identity Name.</span></span>|
|<span data-ttu-id="1f6a0-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1f6a0-197">appStoreUrl</span></span>|<span data-ttu-id="1f6a0-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f6a0-198">String</span></span>|<span data-ttu-id="1f6a0-199">URL des Apple-App-Stores</span><span class="sxs-lookup"><span data-stu-id="1f6a0-199">The Apple App Store URL</span></span>|
|<span data-ttu-id="1f6a0-200">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="1f6a0-200">applicableDeviceType</span></span>|[<span data-ttu-id="1f6a0-201">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="1f6a0-201">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="1f6a0-202">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-202">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="1f6a0-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1f6a0-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1f6a0-204">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1f6a0-204">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="1f6a0-205">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-205">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="1f6a0-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f6a0-206">Response</span></span>
<span data-ttu-id="1f6a0-207">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [iosStoreApp](../resources/intune-apps-iosstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-207">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f6a0-208">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f6a0-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f6a0-209">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f6a0-209">Request</span></span>
<span data-ttu-id="1f6a0-210">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1042

{
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="1f6a0-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f6a0-211">Response</span></span>
<span data-ttu-id="1f6a0-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f6a0-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1200

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```





