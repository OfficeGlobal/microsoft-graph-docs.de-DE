---
title: windowsUniversalAppX erstellen
description: Erstellen eines neuen windowsUniversalAppX-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc6678b950ca5894b5fd480e74f8a4ab4ed371dd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971563"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="a3548-103">windowsUniversalAppX erstellen</span><span class="sxs-lookup"><span data-stu-id="a3548-103">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="a3548-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a3548-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3548-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a3548-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3548-106">Erstellen eines neuen [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a3548-106">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3548-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a3548-107">Prerequisites</span></span>
<span data-ttu-id="a3548-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3548-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3548-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a3548-110">Permission type</span></span>|<span data-ttu-id="a3548-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a3548-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3548-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a3548-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3548-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3548-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a3548-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a3548-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3548-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3548-115">Not supported.</span></span>|
|<span data-ttu-id="a3548-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a3548-116">Application</span></span>|<span data-ttu-id="a3548-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3548-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3548-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3548-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a3548-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a3548-119">Request headers</span></span>
|<span data-ttu-id="a3548-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a3548-120">Header</span></span>|<span data-ttu-id="a3548-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a3548-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3548-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3548-122">Authorization</span></span>|<span data-ttu-id="a3548-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a3548-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3548-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a3548-124">Accept</span></span>|<span data-ttu-id="a3548-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3548-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3548-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a3548-126">Request body</span></span>
<span data-ttu-id="a3548-127">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsUniversalAppX-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a3548-127">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="a3548-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsUniversalAppX erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a3548-128">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="a3548-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a3548-129">Property</span></span>|<span data-ttu-id="a3548-130">Typ</span><span class="sxs-lookup"><span data-stu-id="a3548-130">Type</span></span>|<span data-ttu-id="a3548-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a3548-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3548-132">id</span><span class="sxs-lookup"><span data-stu-id="a3548-132">id</span></span>|<span data-ttu-id="a3548-133">String</span><span class="sxs-lookup"><span data-stu-id="a3548-133">String</span></span>|<span data-ttu-id="a3548-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a3548-134">Key of the entity.</span></span> <span data-ttu-id="a3548-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3548-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a3548-136">displayName</span></span>|<span data-ttu-id="a3548-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3548-137">String</span></span>|<span data-ttu-id="a3548-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="a3548-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a3548-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3548-140">description</span><span class="sxs-lookup"><span data-stu-id="a3548-140">description</span></span>|<span data-ttu-id="a3548-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3548-141">String</span></span>|<span data-ttu-id="a3548-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="a3548-142">The description of the app.</span></span> <span data-ttu-id="a3548-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3548-144">publisher</span><span class="sxs-lookup"><span data-stu-id="a3548-144">publisher</span></span>|<span data-ttu-id="a3548-145">String</span><span class="sxs-lookup"><span data-stu-id="a3548-145">String</span></span>|<span data-ttu-id="a3548-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="a3548-146">The publisher of the app.</span></span> <span data-ttu-id="a3548-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3548-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a3548-148">largeIcon</span></span>|[<span data-ttu-id="a3548-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a3548-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a3548-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a3548-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a3548-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3548-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3548-152">createdDateTime</span></span>|<span data-ttu-id="a3548-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3548-153">DateTimeOffset</span></span>|<span data-ttu-id="a3548-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="a3548-154">The date and time the app was created.</span></span> <span data-ttu-id="a3548-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3548-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3548-156">lastModifiedDateTime</span></span>|<span data-ttu-id="a3548-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3548-157">DateTimeOffset</span></span>|<span data-ttu-id="a3548-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="a3548-158">The date and time the app was last modified.</span></span> <span data-ttu-id="a3548-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3548-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a3548-160">isFeatured</span></span>|<span data-ttu-id="a3548-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3548-161">Boolean</span></span>|<span data-ttu-id="a3548-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3548-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a3548-163">privacyInformationUrl</span></span>|<span data-ttu-id="a3548-164">String</span><span class="sxs-lookup"><span data-stu-id="a3548-164">String</span></span>|<span data-ttu-id="a3548-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="a3548-165">The privacy statement Url.</span></span> <span data-ttu-id="a3548-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3548-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a3548-167">informationUrl</span></span>|<span data-ttu-id="a3548-168">String</span><span class="sxs-lookup"><span data-stu-id="a3548-168">String</span></span>|<span data-ttu-id="a3548-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="a3548-169">The more information Url.</span></span> <span data-ttu-id="a3548-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3548-171">owner</span><span class="sxs-lookup"><span data-stu-id="a3548-171">owner</span></span>|<span data-ttu-id="a3548-172">String</span><span class="sxs-lookup"><span data-stu-id="a3548-172">String</span></span>|<span data-ttu-id="a3548-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="a3548-173">The owner of the app.</span></span> <span data-ttu-id="a3548-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3548-175">developer</span><span class="sxs-lookup"><span data-stu-id="a3548-175">developer</span></span>|<span data-ttu-id="a3548-176">String</span><span class="sxs-lookup"><span data-stu-id="a3548-176">String</span></span>|<span data-ttu-id="a3548-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="a3548-177">The developer of the app.</span></span> <span data-ttu-id="a3548-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3548-179">notes</span><span class="sxs-lookup"><span data-stu-id="a3548-179">notes</span></span>|<span data-ttu-id="a3548-180">String</span><span class="sxs-lookup"><span data-stu-id="a3548-180">String</span></span>|<span data-ttu-id="a3548-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="a3548-181">Notes for the app.</span></span> <span data-ttu-id="a3548-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3548-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="a3548-183">uploadState</span></span>|<span data-ttu-id="a3548-184">Int32</span><span class="sxs-lookup"><span data-stu-id="a3548-184">Int32</span></span>|<span data-ttu-id="a3548-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="a3548-185">The upload state.</span></span> <span data-ttu-id="a3548-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3548-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="a3548-187">publishingState</span></span>|[<span data-ttu-id="a3548-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a3548-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a3548-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="a3548-189">The publishing state for the app.</span></span> <span data-ttu-id="a3548-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="a3548-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a3548-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="a3548-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a3548-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="a3548-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a3548-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a3548-193">isAssigned</span></span>|<span data-ttu-id="a3548-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3548-194">Boolean</span></span>|<span data-ttu-id="a3548-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="a3548-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a3548-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3548-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="a3548-197">roleScopeTagIds</span></span>|<span data-ttu-id="a3548-198">String collection</span><span class="sxs-lookup"><span data-stu-id="a3548-198">String collection</span></span>|<span data-ttu-id="a3548-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="a3548-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a3548-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3548-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a3548-201">committedContentVersion</span></span>|<span data-ttu-id="a3548-202">String</span><span class="sxs-lookup"><span data-stu-id="a3548-202">String</span></span>|<span data-ttu-id="a3548-203">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="a3548-203">The internal committed content version.</span></span> <span data-ttu-id="a3548-204">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a3548-205">fileName</span><span class="sxs-lookup"><span data-stu-id="a3548-205">fileName</span></span>|<span data-ttu-id="a3548-206">String</span><span class="sxs-lookup"><span data-stu-id="a3548-206">String</span></span>|<span data-ttu-id="a3548-207">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="a3548-207">The name of the main Lob application file.</span></span> <span data-ttu-id="a3548-208">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a3548-209">size</span><span class="sxs-lookup"><span data-stu-id="a3548-209">size</span></span>|<span data-ttu-id="a3548-210">Int64</span><span class="sxs-lookup"><span data-stu-id="a3548-210">Int64</span></span>|<span data-ttu-id="a3548-211">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="a3548-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="a3548-212">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3548-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a3548-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="a3548-213">applicableArchitectures</span></span>|[<span data-ttu-id="a3548-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="a3548-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="a3548-215">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="a3548-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="a3548-216">Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral` und `arm64`.</span><span class="sxs-lookup"><span data-stu-id="a3548-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="a3548-217">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="a3548-217">applicableDeviceTypes</span></span>|[<span data-ttu-id="a3548-218">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="a3548-218">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="a3548-219">Die Windows-Gerätetypen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="a3548-219">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="a3548-220">Mögliche Werte: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="a3548-220">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="a3548-221">identityName</span><span class="sxs-lookup"><span data-stu-id="a3548-221">identityName</span></span>|<span data-ttu-id="a3548-222">String</span><span class="sxs-lookup"><span data-stu-id="a3548-222">String</span></span>|<span data-ttu-id="a3548-223">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="a3548-223">The Identity Name.</span></span>|
|<span data-ttu-id="a3548-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="a3548-224">identityPublisherHash</span></span>|<span data-ttu-id="a3548-225">String</span><span class="sxs-lookup"><span data-stu-id="a3548-225">String</span></span>|<span data-ttu-id="a3548-226">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="a3548-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="a3548-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a3548-227">identityResourceIdentifier</span></span>|<span data-ttu-id="a3548-228">String</span><span class="sxs-lookup"><span data-stu-id="a3548-228">String</span></span>|<span data-ttu-id="a3548-229">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="a3548-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="a3548-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="a3548-230">isBundle</span></span>|<span data-ttu-id="a3548-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3548-231">Boolean</span></span>|<span data-ttu-id="a3548-232">Gibt an, ob die App ein Bundle ist.</span><span class="sxs-lookup"><span data-stu-id="a3548-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="a3548-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a3548-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a3548-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a3548-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="a3548-235">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="a3548-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="a3548-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="a3548-236">identityVersion</span></span>|<span data-ttu-id="a3548-237">String</span><span class="sxs-lookup"><span data-stu-id="a3548-237">String</span></span>|<span data-ttu-id="a3548-238">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="a3548-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="a3548-239">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3548-239">Response</span></span>
<span data-ttu-id="a3548-240">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a3548-240">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3548-241">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a3548-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3548-242">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3548-242">Request</span></span>
<span data-ttu-id="a3548-243">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a3548-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1388

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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="a3548-244">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3548-244">Response</span></span>
<span data-ttu-id="a3548-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a3548-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1560

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




