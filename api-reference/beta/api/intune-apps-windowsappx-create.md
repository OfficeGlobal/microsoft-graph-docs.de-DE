---
title: Erstellen von windowsAppX
description: Erstellen eines neuen WindowsAppX-Objekts.
ms.openlocfilehash: bf4445303a49e23e892514524913e602fa69e917
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064088"
---
# <a name="create-windowsappx"></a><span data-ttu-id="d2cd3-103">Erstellen von windowsAppX</span><span class="sxs-lookup"><span data-stu-id="d2cd3-103">Create windowsAppX</span></span>

> <span data-ttu-id="d2cd3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2cd3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2cd3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2cd3-107">Erstellen eines neuen [WindowsAppX](../resources/intune-apps-windowsappx.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-107">Create a new [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2cd3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d2cd3-108">Prerequisites</span></span>
<span data-ttu-id="d2cd3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2cd3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d2cd3-111">Permission type</span></span>|<span data-ttu-id="d2cd3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d2cd3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2cd3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d2cd3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2cd3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2cd3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d2cd3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d2cd3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2cd3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d2cd3-116">Not supported.</span></span>|
|<span data-ttu-id="d2cd3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d2cd3-117">Application</span></span>|<span data-ttu-id="d2cd3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d2cd3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2cd3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2cd3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d2cd3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d2cd3-120">Request headers</span></span>
|<span data-ttu-id="d2cd3-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d2cd3-121">Header</span></span>|<span data-ttu-id="d2cd3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d2cd3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2cd3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2cd3-123">Authorization</span></span>|<span data-ttu-id="d2cd3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d2cd3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2cd3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d2cd3-125">Accept</span></span>|<span data-ttu-id="d2cd3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2cd3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2cd3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d2cd3-127">Request body</span></span>
<span data-ttu-id="d2cd3-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsAppX eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-128">In the request body, supply a JSON representation for the windowsAppX object.</span></span>

<span data-ttu-id="d2cd3-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsAppX erstellen.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-129">The following table shows the properties that are required when you create the windowsAppX.</span></span>

|<span data-ttu-id="d2cd3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d2cd3-130">Property</span></span>|<span data-ttu-id="d2cd3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d2cd3-131">Type</span></span>|<span data-ttu-id="d2cd3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2cd3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2cd3-133">id</span><span class="sxs-lookup"><span data-stu-id="d2cd3-133">id</span></span>|<span data-ttu-id="d2cd3-134">String</span><span class="sxs-lookup"><span data-stu-id="d2cd3-134">String</span></span>|<span data-ttu-id="d2cd3-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d2cd3-135">Key of the entity.</span></span> <span data-ttu-id="d2cd3-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d2cd3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d2cd3-137">displayName</span></span>|<span data-ttu-id="d2cd3-138">String</span><span class="sxs-lookup"><span data-stu-id="d2cd3-138">String</span></span>|<span data-ttu-id="d2cd3-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d2cd3-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d2cd3-141">description</span><span class="sxs-lookup"><span data-stu-id="d2cd3-141">description</span></span>|<span data-ttu-id="d2cd3-142">String</span><span class="sxs-lookup"><span data-stu-id="d2cd3-142">String</span></span>|<span data-ttu-id="d2cd3-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-143">The description of the app.</span></span> <span data-ttu-id="d2cd3-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d2cd3-145">publisher</span><span class="sxs-lookup"><span data-stu-id="d2cd3-145">publisher</span></span>|<span data-ttu-id="d2cd3-146">String</span><span class="sxs-lookup"><span data-stu-id="d2cd3-146">String</span></span>|<span data-ttu-id="d2cd3-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-147">The publisher of the app.</span></span> <span data-ttu-id="d2cd3-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d2cd3-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d2cd3-149">largeIcon</span></span>|[<span data-ttu-id="d2cd3-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d2cd3-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d2cd3-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d2cd3-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d2cd3-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2cd3-153">createdDateTime</span></span>|<span data-ttu-id="d2cd3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2cd3-154">DateTimeOffset</span></span>|<span data-ttu-id="d2cd3-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-155">The date and time the app was created.</span></span> <span data-ttu-id="d2cd3-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d2cd3-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2cd3-157">lastModifiedDateTime</span></span>|<span data-ttu-id="d2cd3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2cd3-158">DateTimeOffset</span></span>|<span data-ttu-id="d2cd3-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-159">The date and time the app was last modified.</span></span> <span data-ttu-id="d2cd3-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d2cd3-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d2cd3-161">isFeatured</span></span>|<span data-ttu-id="d2cd3-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d2cd3-162">Boolean</span></span>|<span data-ttu-id="d2cd3-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d2cd3-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d2cd3-164">privacyInformationUrl</span></span>|<span data-ttu-id="d2cd3-165">String</span><span class="sxs-lookup"><span data-stu-id="d2cd3-165">String</span></span>|<span data-ttu-id="d2cd3-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-166">The privacy statement Url.</span></span> <span data-ttu-id="d2cd3-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d2cd3-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d2cd3-168">informationUrl</span></span>|<span data-ttu-id="d2cd3-169">String</span><span class="sxs-lookup"><span data-stu-id="d2cd3-169">String</span></span>|<span data-ttu-id="d2cd3-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-170">The more information Url.</span></span> <span data-ttu-id="d2cd3-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d2cd3-172">owner</span><span class="sxs-lookup"><span data-stu-id="d2cd3-172">owner</span></span>|<span data-ttu-id="d2cd3-173">String</span><span class="sxs-lookup"><span data-stu-id="d2cd3-173">String</span></span>|<span data-ttu-id="d2cd3-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-174">The owner of the app.</span></span> <span data-ttu-id="d2cd3-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d2cd3-176">developer</span><span class="sxs-lookup"><span data-stu-id="d2cd3-176">developer</span></span>|<span data-ttu-id="d2cd3-177">String</span><span class="sxs-lookup"><span data-stu-id="d2cd3-177">String</span></span>|<span data-ttu-id="d2cd3-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-178">The developer of the app.</span></span> <span data-ttu-id="d2cd3-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d2cd3-180">notes</span><span class="sxs-lookup"><span data-stu-id="d2cd3-180">notes</span></span>|<span data-ttu-id="d2cd3-181">String</span><span class="sxs-lookup"><span data-stu-id="d2cd3-181">String</span></span>|<span data-ttu-id="d2cd3-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-182">Notes for the app.</span></span> <span data-ttu-id="d2cd3-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d2cd3-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="d2cd3-184">uploadState</span></span>|<span data-ttu-id="d2cd3-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d2cd3-185">Int32</span></span>|<span data-ttu-id="d2cd3-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-186">The upload state.</span></span> <span data-ttu-id="d2cd3-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d2cd3-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="d2cd3-188">publishingState</span></span>|[<span data-ttu-id="d2cd3-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d2cd3-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d2cd3-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-190">The publishing state for the app.</span></span> <span data-ttu-id="d2cd3-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d2cd3-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d2cd3-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d2cd3-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d2cd3-194">committedContentVersion</span></span>|<span data-ttu-id="d2cd3-195">String</span><span class="sxs-lookup"><span data-stu-id="d2cd3-195">String</span></span>|<span data-ttu-id="d2cd3-196">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-196">The internal committed content version.</span></span> <span data-ttu-id="d2cd3-197">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d2cd3-198">fileName</span><span class="sxs-lookup"><span data-stu-id="d2cd3-198">fileName</span></span>|<span data-ttu-id="d2cd3-199">String</span><span class="sxs-lookup"><span data-stu-id="d2cd3-199">String</span></span>|<span data-ttu-id="d2cd3-200">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-200">The name of the main Lob application file.</span></span> <span data-ttu-id="d2cd3-201">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d2cd3-202">size</span><span class="sxs-lookup"><span data-stu-id="d2cd3-202">size</span></span>|<span data-ttu-id="d2cd3-203">Int64</span><span class="sxs-lookup"><span data-stu-id="d2cd3-203">Int64</span></span>|<span data-ttu-id="d2cd3-204">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="d2cd3-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2cd3-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d2cd3-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="d2cd3-206">applicableArchitectures</span></span>|[<span data-ttu-id="d2cd3-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="d2cd3-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="d2cd3-208">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="d2cd3-209">Mögliche Werte: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-209">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="d2cd3-210">identityName</span><span class="sxs-lookup"><span data-stu-id="d2cd3-210">identityName</span></span>|<span data-ttu-id="d2cd3-211">String</span><span class="sxs-lookup"><span data-stu-id="d2cd3-211">String</span></span>|<span data-ttu-id="d2cd3-212">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="d2cd3-212">The Identity Name.</span></span>|
|<span data-ttu-id="d2cd3-213">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="d2cd3-213">identityPublisherHash</span></span>|<span data-ttu-id="d2cd3-214">String</span><span class="sxs-lookup"><span data-stu-id="d2cd3-214">String</span></span>|<span data-ttu-id="d2cd3-215">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-215">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="d2cd3-216">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="d2cd3-216">identityResourceIdentifier</span></span>|<span data-ttu-id="d2cd3-217">String</span><span class="sxs-lookup"><span data-stu-id="d2cd3-217">String</span></span>|<span data-ttu-id="d2cd3-218">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-218">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="d2cd3-219">isBundle</span><span class="sxs-lookup"><span data-stu-id="d2cd3-219">isBundle</span></span>|<span data-ttu-id="d2cd3-220">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d2cd3-220">Boolean</span></span>|<span data-ttu-id="d2cd3-221">Gibt an, ob die App ein Bundle ist.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-221">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="d2cd3-222">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d2cd3-222">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d2cd3-223">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d2cd3-223">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="d2cd3-224">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-224">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d2cd3-225">identityVersion</span><span class="sxs-lookup"><span data-stu-id="d2cd3-225">identityVersion</span></span>|<span data-ttu-id="d2cd3-226">String</span><span class="sxs-lookup"><span data-stu-id="d2cd3-226">String</span></span>|<span data-ttu-id="d2cd3-227">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="d2cd3-227">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="d2cd3-228">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2cd3-228">Response</span></span>
<span data-ttu-id="d2cd3-229">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsAppX](../resources/intune-apps-windowsappx.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-229">If successful, this method returns a `201 Created` response code and a [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2cd3-230">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d2cd3-230">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2cd3-231">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2cd3-231">Request</span></span>
<span data-ttu-id="d2cd3-232">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-232">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1319

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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

### <a name="response"></a><span data-ttu-id="d2cd3-233">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2cd3-233">Response</span></span>
<span data-ttu-id="d2cd3-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1427

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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





