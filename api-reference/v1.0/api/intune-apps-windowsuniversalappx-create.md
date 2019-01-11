---
title: windowsUniversalAppX erstellen
description: Erstellen eines neuen windowsUniversalAppX-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d5e0a3d209b23377adfd50b4880b29c854761da3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894523"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="e0993-103">windowsUniversalAppX erstellen</span><span class="sxs-lookup"><span data-stu-id="e0993-103">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="e0993-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e0993-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0993-105">Erstellen eines neuen [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e0993-105">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0993-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e0993-106">Prerequisites</span></span>
<span data-ttu-id="e0993-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0993-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0993-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e0993-109">Permission type</span></span>|<span data-ttu-id="e0993-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e0993-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0993-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e0993-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e0993-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0993-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e0993-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e0993-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0993-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0993-114">Not supported.</span></span>|
|<span data-ttu-id="e0993-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e0993-115">Application</span></span>|<span data-ttu-id="e0993-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0993-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0993-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0993-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e0993-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e0993-118">Request headers</span></span>
|<span data-ttu-id="e0993-119">Header</span><span class="sxs-lookup"><span data-stu-id="e0993-119">Header</span></span>|<span data-ttu-id="e0993-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e0993-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0993-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0993-121">Authorization</span></span>|<span data-ttu-id="e0993-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e0993-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0993-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e0993-123">Accept</span></span>|<span data-ttu-id="e0993-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e0993-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0993-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e0993-125">Request body</span></span>
<span data-ttu-id="e0993-126">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsUniversalAppX-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e0993-126">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="e0993-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsUniversalAppX erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e0993-127">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="e0993-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e0993-128">Property</span></span>|<span data-ttu-id="e0993-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e0993-129">Type</span></span>|<span data-ttu-id="e0993-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0993-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0993-131">id</span><span class="sxs-lookup"><span data-stu-id="e0993-131">id</span></span>|<span data-ttu-id="e0993-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0993-132">String</span></span>|<span data-ttu-id="e0993-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e0993-133">Key of the entity.</span></span> <span data-ttu-id="e0993-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0993-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e0993-135">displayName</span></span>|<span data-ttu-id="e0993-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0993-136">String</span></span>|<span data-ttu-id="e0993-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="e0993-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e0993-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0993-139">description</span><span class="sxs-lookup"><span data-stu-id="e0993-139">description</span></span>|<span data-ttu-id="e0993-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0993-140">String</span></span>|<span data-ttu-id="e0993-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="e0993-141">The description of the app.</span></span> <span data-ttu-id="e0993-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0993-143">publisher</span><span class="sxs-lookup"><span data-stu-id="e0993-143">publisher</span></span>|<span data-ttu-id="e0993-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0993-144">String</span></span>|<span data-ttu-id="e0993-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="e0993-145">The publisher of the app.</span></span> <span data-ttu-id="e0993-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0993-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e0993-147">largeIcon</span></span>|[<span data-ttu-id="e0993-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e0993-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e0993-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e0993-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e0993-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0993-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0993-151">createdDateTime</span></span>|<span data-ttu-id="e0993-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0993-152">DateTimeOffset</span></span>|<span data-ttu-id="e0993-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="e0993-153">The date and time the app was created.</span></span> <span data-ttu-id="e0993-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0993-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0993-155">lastModifiedDateTime</span></span>|<span data-ttu-id="e0993-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0993-156">DateTimeOffset</span></span>|<span data-ttu-id="e0993-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="e0993-157">The date and time the app was last modified.</span></span> <span data-ttu-id="e0993-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0993-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e0993-159">isFeatured</span></span>|<span data-ttu-id="e0993-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e0993-160">Boolean</span></span>|<span data-ttu-id="e0993-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0993-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e0993-162">privacyInformationUrl</span></span>|<span data-ttu-id="e0993-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0993-163">String</span></span>|<span data-ttu-id="e0993-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="e0993-164">The privacy statement Url.</span></span> <span data-ttu-id="e0993-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0993-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e0993-166">informationUrl</span></span>|<span data-ttu-id="e0993-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0993-167">String</span></span>|<span data-ttu-id="e0993-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="e0993-168">The more information Url.</span></span> <span data-ttu-id="e0993-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0993-170">owner</span><span class="sxs-lookup"><span data-stu-id="e0993-170">owner</span></span>|<span data-ttu-id="e0993-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0993-171">String</span></span>|<span data-ttu-id="e0993-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="e0993-172">The owner of the app.</span></span> <span data-ttu-id="e0993-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0993-174">developer</span><span class="sxs-lookup"><span data-stu-id="e0993-174">developer</span></span>|<span data-ttu-id="e0993-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0993-175">String</span></span>|<span data-ttu-id="e0993-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="e0993-176">The developer of the app.</span></span> <span data-ttu-id="e0993-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0993-178">notes</span><span class="sxs-lookup"><span data-stu-id="e0993-178">notes</span></span>|<span data-ttu-id="e0993-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0993-179">String</span></span>|<span data-ttu-id="e0993-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="e0993-180">Notes for the app.</span></span> <span data-ttu-id="e0993-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0993-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="e0993-182">publishingState</span></span>|[<span data-ttu-id="e0993-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e0993-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e0993-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="e0993-184">The publishing state for the app.</span></span> <span data-ttu-id="e0993-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="e0993-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e0993-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e0993-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="e0993-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e0993-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e0993-188">committedContentVersion</span></span>|<span data-ttu-id="e0993-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0993-189">String</span></span>|<span data-ttu-id="e0993-190">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="e0993-190">The internal committed content version.</span></span> <span data-ttu-id="e0993-191">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e0993-192">fileName</span><span class="sxs-lookup"><span data-stu-id="e0993-192">fileName</span></span>|<span data-ttu-id="e0993-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0993-193">String</span></span>|<span data-ttu-id="e0993-194">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="e0993-194">The name of the main Lob application file.</span></span> <span data-ttu-id="e0993-195">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e0993-196">size</span><span class="sxs-lookup"><span data-stu-id="e0993-196">size</span></span>|<span data-ttu-id="e0993-197">Int64</span><span class="sxs-lookup"><span data-stu-id="e0993-197">Int64</span></span>|<span data-ttu-id="e0993-198">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="e0993-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="e0993-199">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0993-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e0993-200">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="e0993-200">applicableArchitectures</span></span>|[<span data-ttu-id="e0993-201">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="e0993-201">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="e0993-202">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="e0993-202">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="e0993-203">Mögliche Werte: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="e0993-203">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="e0993-204">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="e0993-204">applicableDeviceTypes</span></span>|[<span data-ttu-id="e0993-205">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="e0993-205">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="e0993-206">Die Windows-Gerätetypen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="e0993-206">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="e0993-207">Mögliche Werte: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="e0993-207">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="e0993-208">identityName</span><span class="sxs-lookup"><span data-stu-id="e0993-208">identityName</span></span>|<span data-ttu-id="e0993-209">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0993-209">String</span></span>|<span data-ttu-id="e0993-210">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="e0993-210">The Identity Name.</span></span>|
|<span data-ttu-id="e0993-211">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="e0993-211">identityPublisherHash</span></span>|<span data-ttu-id="e0993-212">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0993-212">String</span></span>|<span data-ttu-id="e0993-213">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="e0993-213">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="e0993-214">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e0993-214">identityResourceIdentifier</span></span>|<span data-ttu-id="e0993-215">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0993-215">String</span></span>|<span data-ttu-id="e0993-216">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="e0993-216">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="e0993-217">isBundle</span><span class="sxs-lookup"><span data-stu-id="e0993-217">isBundle</span></span>|<span data-ttu-id="e0993-218">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e0993-218">Boolean</span></span>|<span data-ttu-id="e0993-219">Gibt an, ob die App ein Bundle ist.</span><span class="sxs-lookup"><span data-stu-id="e0993-219">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="e0993-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e0993-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e0993-221">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e0993-221">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="e0993-222">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="e0993-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e0993-223">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e0993-223">identityVersion</span></span>|<span data-ttu-id="e0993-224">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0993-224">String</span></span>|<span data-ttu-id="e0993-225">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="e0993-225">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="e0993-226">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0993-226">Response</span></span>
<span data-ttu-id="e0993-227">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e0993-227">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0993-228">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e0993-228">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0993-229">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0993-229">Request</span></span>
<span data-ttu-id="e0993-230">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e0993-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="e0993-231">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0993-231">Response</span></span>
<span data-ttu-id="e0993-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0993-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```



