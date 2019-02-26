---
title: windowsUniversalAppX erstellen
description: Erstellen eines neuen windowsUniversalAppX-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02252ccfaf008d36d20d57d89ea2e0981d2c4c21
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254947"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="2afac-103">windowsUniversalAppX erstellen</span><span class="sxs-lookup"><span data-stu-id="2afac-103">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="2afac-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2afac-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2afac-105">Erstellen eines neuen [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2afac-105">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2afac-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2afac-106">Prerequisites</span></span>
<span data-ttu-id="2afac-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2afac-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2afac-109">Permission type</span></span>|<span data-ttu-id="2afac-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2afac-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2afac-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2afac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2afac-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2afac-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2afac-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2afac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2afac-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2afac-114">Not supported.</span></span>|
|<span data-ttu-id="2afac-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2afac-115">Application</span></span>|<span data-ttu-id="2afac-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2afac-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2afac-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2afac-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2afac-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2afac-118">Request headers</span></span>
|<span data-ttu-id="2afac-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2afac-119">Header</span></span>|<span data-ttu-id="2afac-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2afac-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2afac-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2afac-121">Authorization</span></span>|<span data-ttu-id="2afac-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2afac-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2afac-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2afac-123">Accept</span></span>|<span data-ttu-id="2afac-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2afac-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2afac-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2afac-125">Request body</span></span>
<span data-ttu-id="2afac-126">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsUniversalAppX-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="2afac-126">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="2afac-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsUniversalAppX erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2afac-127">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="2afac-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2afac-128">Property</span></span>|<span data-ttu-id="2afac-129">Typ</span><span class="sxs-lookup"><span data-stu-id="2afac-129">Type</span></span>|<span data-ttu-id="2afac-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2afac-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2afac-131">id</span><span class="sxs-lookup"><span data-stu-id="2afac-131">id</span></span>|<span data-ttu-id="2afac-132">string</span><span class="sxs-lookup"><span data-stu-id="2afac-132">String</span></span>|<span data-ttu-id="2afac-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2afac-133">Key of the entity.</span></span> <span data-ttu-id="2afac-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2afac-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2afac-135">displayName</span></span>|<span data-ttu-id="2afac-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2afac-136">String</span></span>|<span data-ttu-id="2afac-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="2afac-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2afac-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2afac-139">description</span><span class="sxs-lookup"><span data-stu-id="2afac-139">description</span></span>|<span data-ttu-id="2afac-140">String</span><span class="sxs-lookup"><span data-stu-id="2afac-140">String</span></span>|<span data-ttu-id="2afac-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="2afac-141">The description of the app.</span></span> <span data-ttu-id="2afac-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2afac-143">publisher</span><span class="sxs-lookup"><span data-stu-id="2afac-143">publisher</span></span>|<span data-ttu-id="2afac-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2afac-144">String</span></span>|<span data-ttu-id="2afac-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="2afac-145">The publisher of the app.</span></span> <span data-ttu-id="2afac-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2afac-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2afac-147">largeIcon</span></span>|[<span data-ttu-id="2afac-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2afac-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2afac-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="2afac-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2afac-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2afac-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2afac-151">createdDateTime</span></span>|<span data-ttu-id="2afac-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2afac-152">DateTimeOffset</span></span>|<span data-ttu-id="2afac-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="2afac-153">The date and time the app was created.</span></span> <span data-ttu-id="2afac-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2afac-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2afac-155">lastModifiedDateTime</span></span>|<span data-ttu-id="2afac-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2afac-156">DateTimeOffset</span></span>|<span data-ttu-id="2afac-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="2afac-157">The date and time the app was last modified.</span></span> <span data-ttu-id="2afac-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2afac-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2afac-159">isFeatured</span></span>|<span data-ttu-id="2afac-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afac-160">Boolean</span></span>|<span data-ttu-id="2afac-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2afac-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2afac-162">privacyInformationUrl</span></span>|<span data-ttu-id="2afac-163">String</span><span class="sxs-lookup"><span data-stu-id="2afac-163">String</span></span>|<span data-ttu-id="2afac-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="2afac-164">The privacy statement Url.</span></span> <span data-ttu-id="2afac-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2afac-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2afac-166">informationUrl</span></span>|<span data-ttu-id="2afac-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2afac-167">String</span></span>|<span data-ttu-id="2afac-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="2afac-168">The more information Url.</span></span> <span data-ttu-id="2afac-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2afac-170">owner</span><span class="sxs-lookup"><span data-stu-id="2afac-170">owner</span></span>|<span data-ttu-id="2afac-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2afac-171">String</span></span>|<span data-ttu-id="2afac-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="2afac-172">The owner of the app.</span></span> <span data-ttu-id="2afac-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2afac-174">developer</span><span class="sxs-lookup"><span data-stu-id="2afac-174">developer</span></span>|<span data-ttu-id="2afac-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2afac-175">String</span></span>|<span data-ttu-id="2afac-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="2afac-176">The developer of the app.</span></span> <span data-ttu-id="2afac-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2afac-178">notes</span><span class="sxs-lookup"><span data-stu-id="2afac-178">notes</span></span>|<span data-ttu-id="2afac-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2afac-179">String</span></span>|<span data-ttu-id="2afac-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="2afac-180">Notes for the app.</span></span> <span data-ttu-id="2afac-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2afac-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="2afac-182">publishingState</span></span>|[<span data-ttu-id="2afac-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2afac-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2afac-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="2afac-184">The publishing state for the app.</span></span> <span data-ttu-id="2afac-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="2afac-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2afac-186">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="2afac-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2afac-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="2afac-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2afac-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="2afac-188">committedContentVersion</span></span>|<span data-ttu-id="2afac-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2afac-189">String</span></span>|<span data-ttu-id="2afac-190">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="2afac-190">The internal committed content version.</span></span> <span data-ttu-id="2afac-191">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2afac-192">fileName</span><span class="sxs-lookup"><span data-stu-id="2afac-192">fileName</span></span>|<span data-ttu-id="2afac-193">String</span><span class="sxs-lookup"><span data-stu-id="2afac-193">String</span></span>|<span data-ttu-id="2afac-194">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="2afac-194">The name of the main Lob application file.</span></span> <span data-ttu-id="2afac-195">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2afac-196">size</span><span class="sxs-lookup"><span data-stu-id="2afac-196">size</span></span>|<span data-ttu-id="2afac-197">Int64</span><span class="sxs-lookup"><span data-stu-id="2afac-197">Int64</span></span>|<span data-ttu-id="2afac-198">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="2afac-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="2afac-199">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2afac-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2afac-200">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="2afac-200">applicableArchitectures</span></span>|[<span data-ttu-id="2afac-201">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="2afac-201">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="2afac-202">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="2afac-202">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="2afac-203">Mögliche Werte: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="2afac-203">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="2afac-204">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="2afac-204">applicableDeviceTypes</span></span>|[<span data-ttu-id="2afac-205">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="2afac-205">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="2afac-206">Die Windows-Gerätetypen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="2afac-206">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="2afac-207">Mögliche Werte: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="2afac-207">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="2afac-208">identityName</span><span class="sxs-lookup"><span data-stu-id="2afac-208">identityName</span></span>|<span data-ttu-id="2afac-209">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2afac-209">String</span></span>|<span data-ttu-id="2afac-210">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="2afac-210">The Identity Name.</span></span>|
|<span data-ttu-id="2afac-211">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="2afac-211">identityPublisherHash</span></span>|<span data-ttu-id="2afac-212">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2afac-212">String</span></span>|<span data-ttu-id="2afac-213">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="2afac-213">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="2afac-214">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="2afac-214">identityResourceIdentifier</span></span>|<span data-ttu-id="2afac-215">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2afac-215">String</span></span>|<span data-ttu-id="2afac-216">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="2afac-216">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="2afac-217">isBundle</span><span class="sxs-lookup"><span data-stu-id="2afac-217">isBundle</span></span>|<span data-ttu-id="2afac-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afac-218">Boolean</span></span>|<span data-ttu-id="2afac-219">Gibt an, ob die App ein Bundle ist.</span><span class="sxs-lookup"><span data-stu-id="2afac-219">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="2afac-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2afac-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2afac-221">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2afac-221">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="2afac-222">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="2afac-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="2afac-223">identityVersion</span><span class="sxs-lookup"><span data-stu-id="2afac-223">identityVersion</span></span>|<span data-ttu-id="2afac-224">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2afac-224">String</span></span>|<span data-ttu-id="2afac-225">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="2afac-225">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="2afac-226">Antwort</span><span class="sxs-lookup"><span data-stu-id="2afac-226">Response</span></span>
<span data-ttu-id="2afac-227">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2afac-227">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2afac-228">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2afac-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="2afac-229">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2afac-229">Request</span></span>
<span data-ttu-id="2afac-230">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2afac-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2afac-231">Antwort</span><span class="sxs-lookup"><span data-stu-id="2afac-231">Response</span></span>
<span data-ttu-id="2afac-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2afac-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



