---
title: windowsUniversalAppX erstellen
description: Erstellen eines neuen windowsUniversalAppX-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 324935bc9e72c3da05251c16171a68e1f1b08773
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875565"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="ff471-103">windowsUniversalAppX erstellen</span><span class="sxs-lookup"><span data-stu-id="ff471-103">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="ff471-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ff471-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff471-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff471-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff471-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ff471-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff471-107">Erstellen eines neuen [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ff471-107">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff471-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ff471-108">Prerequisites</span></span>
<span data-ttu-id="ff471-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff471-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff471-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff471-111">Permission type</span></span>|<span data-ttu-id="ff471-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff471-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff471-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff471-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff471-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff471-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ff471-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff471-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff471-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff471-116">Not supported.</span></span>|
|<span data-ttu-id="ff471-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff471-117">Application</span></span>|<span data-ttu-id="ff471-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff471-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff471-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff471-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ff471-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ff471-120">Request headers</span></span>
|<span data-ttu-id="ff471-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ff471-121">Header</span></span>|<span data-ttu-id="ff471-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ff471-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff471-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff471-123">Authorization</span></span>|<span data-ttu-id="ff471-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ff471-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff471-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ff471-125">Accept</span></span>|<span data-ttu-id="ff471-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff471-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff471-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff471-127">Request body</span></span>
<span data-ttu-id="ff471-128">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsUniversalAppX-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ff471-128">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="ff471-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsUniversalAppX erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ff471-129">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="ff471-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ff471-130">Property</span></span>|<span data-ttu-id="ff471-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ff471-131">Type</span></span>|<span data-ttu-id="ff471-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff471-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff471-133">id</span><span class="sxs-lookup"><span data-stu-id="ff471-133">id</span></span>|<span data-ttu-id="ff471-134">String</span><span class="sxs-lookup"><span data-stu-id="ff471-134">String</span></span>|<span data-ttu-id="ff471-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ff471-135">Key of the entity.</span></span> <span data-ttu-id="ff471-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff471-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ff471-137">displayName</span></span>|<span data-ttu-id="ff471-138">String</span><span class="sxs-lookup"><span data-stu-id="ff471-138">String</span></span>|<span data-ttu-id="ff471-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="ff471-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ff471-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff471-141">description</span><span class="sxs-lookup"><span data-stu-id="ff471-141">description</span></span>|<span data-ttu-id="ff471-142">String</span><span class="sxs-lookup"><span data-stu-id="ff471-142">String</span></span>|<span data-ttu-id="ff471-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="ff471-143">The description of the app.</span></span> <span data-ttu-id="ff471-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff471-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ff471-145">publisher</span></span>|<span data-ttu-id="ff471-146">String</span><span class="sxs-lookup"><span data-stu-id="ff471-146">String</span></span>|<span data-ttu-id="ff471-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="ff471-147">The publisher of the app.</span></span> <span data-ttu-id="ff471-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff471-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ff471-149">largeIcon</span></span>|[<span data-ttu-id="ff471-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ff471-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ff471-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff471-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ff471-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff471-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff471-153">createdDateTime</span></span>|<span data-ttu-id="ff471-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff471-154">DateTimeOffset</span></span>|<span data-ttu-id="ff471-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="ff471-155">The date and time the app was created.</span></span> <span data-ttu-id="ff471-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff471-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff471-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ff471-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff471-158">DateTimeOffset</span></span>|<span data-ttu-id="ff471-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="ff471-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ff471-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff471-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ff471-161">isFeatured</span></span>|<span data-ttu-id="ff471-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff471-162">Boolean</span></span>|<span data-ttu-id="ff471-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff471-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ff471-164">privacyInformationUrl</span></span>|<span data-ttu-id="ff471-165">String</span><span class="sxs-lookup"><span data-stu-id="ff471-165">String</span></span>|<span data-ttu-id="ff471-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="ff471-166">The privacy statement Url.</span></span> <span data-ttu-id="ff471-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff471-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ff471-168">informationUrl</span></span>|<span data-ttu-id="ff471-169">String</span><span class="sxs-lookup"><span data-stu-id="ff471-169">String</span></span>|<span data-ttu-id="ff471-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="ff471-170">The more information Url.</span></span> <span data-ttu-id="ff471-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff471-172">owner</span><span class="sxs-lookup"><span data-stu-id="ff471-172">owner</span></span>|<span data-ttu-id="ff471-173">String</span><span class="sxs-lookup"><span data-stu-id="ff471-173">String</span></span>|<span data-ttu-id="ff471-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="ff471-174">The owner of the app.</span></span> <span data-ttu-id="ff471-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff471-176">developer</span><span class="sxs-lookup"><span data-stu-id="ff471-176">developer</span></span>|<span data-ttu-id="ff471-177">String</span><span class="sxs-lookup"><span data-stu-id="ff471-177">String</span></span>|<span data-ttu-id="ff471-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="ff471-178">The developer of the app.</span></span> <span data-ttu-id="ff471-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff471-180">notes</span><span class="sxs-lookup"><span data-stu-id="ff471-180">notes</span></span>|<span data-ttu-id="ff471-181">String</span><span class="sxs-lookup"><span data-stu-id="ff471-181">String</span></span>|<span data-ttu-id="ff471-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="ff471-182">Notes for the app.</span></span> <span data-ttu-id="ff471-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff471-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ff471-184">uploadState</span></span>|<span data-ttu-id="ff471-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ff471-185">Int32</span></span>|<span data-ttu-id="ff471-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="ff471-186">The upload state.</span></span> <span data-ttu-id="ff471-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff471-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="ff471-188">publishingState</span></span>|[<span data-ttu-id="ff471-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ff471-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ff471-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="ff471-190">The publishing state for the app.</span></span> <span data-ttu-id="ff471-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="ff471-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ff471-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ff471-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="ff471-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ff471-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ff471-194">committedContentVersion</span></span>|<span data-ttu-id="ff471-195">String</span><span class="sxs-lookup"><span data-stu-id="ff471-195">String</span></span>|<span data-ttu-id="ff471-196">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="ff471-196">The internal committed content version.</span></span> <span data-ttu-id="ff471-197">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ff471-198">fileName</span><span class="sxs-lookup"><span data-stu-id="ff471-198">fileName</span></span>|<span data-ttu-id="ff471-199">String</span><span class="sxs-lookup"><span data-stu-id="ff471-199">String</span></span>|<span data-ttu-id="ff471-200">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="ff471-200">The name of the main Lob application file.</span></span> <span data-ttu-id="ff471-201">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ff471-202">size</span><span class="sxs-lookup"><span data-stu-id="ff471-202">size</span></span>|<span data-ttu-id="ff471-203">Int64</span><span class="sxs-lookup"><span data-stu-id="ff471-203">Int64</span></span>|<span data-ttu-id="ff471-204">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="ff471-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="ff471-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff471-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ff471-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="ff471-206">applicableArchitectures</span></span>|[<span data-ttu-id="ff471-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="ff471-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="ff471-208">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="ff471-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="ff471-209">Mögliche Werte: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="ff471-209">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="ff471-210">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="ff471-210">applicableDeviceTypes</span></span>|[<span data-ttu-id="ff471-211">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="ff471-211">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="ff471-212">Die Windows-Gerätetypen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="ff471-212">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="ff471-213">Mögliche Werte: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="ff471-213">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="ff471-214">identityName</span><span class="sxs-lookup"><span data-stu-id="ff471-214">identityName</span></span>|<span data-ttu-id="ff471-215">String</span><span class="sxs-lookup"><span data-stu-id="ff471-215">String</span></span>|<span data-ttu-id="ff471-216">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="ff471-216">The Identity Name.</span></span>|
|<span data-ttu-id="ff471-217">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="ff471-217">identityPublisherHash</span></span>|<span data-ttu-id="ff471-218">String</span><span class="sxs-lookup"><span data-stu-id="ff471-218">String</span></span>|<span data-ttu-id="ff471-219">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="ff471-219">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="ff471-220">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ff471-220">identityResourceIdentifier</span></span>|<span data-ttu-id="ff471-221">String</span><span class="sxs-lookup"><span data-stu-id="ff471-221">String</span></span>|<span data-ttu-id="ff471-222">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="ff471-222">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="ff471-223">isBundle</span><span class="sxs-lookup"><span data-stu-id="ff471-223">isBundle</span></span>|<span data-ttu-id="ff471-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff471-224">Boolean</span></span>|<span data-ttu-id="ff471-225">Gibt an, ob die App ein Bundle ist.</span><span class="sxs-lookup"><span data-stu-id="ff471-225">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="ff471-226">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ff471-226">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ff471-227">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ff471-227">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="ff471-228">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="ff471-228">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ff471-229">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ff471-229">identityVersion</span></span>|<span data-ttu-id="ff471-230">String</span><span class="sxs-lookup"><span data-stu-id="ff471-230">String</span></span>|<span data-ttu-id="ff471-231">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="ff471-231">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ff471-232">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff471-232">Response</span></span>
<span data-ttu-id="ff471-233">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ff471-233">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff471-234">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ff471-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff471-235">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff471-235">Request</span></span>
<span data-ttu-id="ff471-236">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ff471-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1367

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
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="ff471-237">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff471-237">Response</span></span>
<span data-ttu-id="ff471-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff471-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1475

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
  "uploadState": 11,
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
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```





