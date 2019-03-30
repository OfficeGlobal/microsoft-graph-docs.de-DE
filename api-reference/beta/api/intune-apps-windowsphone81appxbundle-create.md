---
title: WindowsPhone81AppXBundle erstellen
description: Erstellen eines neuen windowsPhone81AppXBundle-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b37d04f4c08d562529943ada7a64937c25ede324
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969904"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="9ce28-103">WindowsPhone81AppXBundle erstellen</span><span class="sxs-lookup"><span data-stu-id="9ce28-103">Create windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="9ce28-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9ce28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ce28-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9ce28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ce28-106">Erstellen eines neuen [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9ce28-106">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ce28-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9ce28-107">Prerequisites</span></span>
<span data-ttu-id="9ce28-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ce28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ce28-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ce28-110">Permission type</span></span>|<span data-ttu-id="9ce28-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ce28-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ce28-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ce28-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ce28-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ce28-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9ce28-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ce28-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ce28-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ce28-115">Not supported.</span></span>|
|<span data-ttu-id="9ce28-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ce28-116">Application</span></span>|<span data-ttu-id="9ce28-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ce28-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ce28-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ce28-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9ce28-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9ce28-119">Request headers</span></span>
|<span data-ttu-id="9ce28-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9ce28-120">Header</span></span>|<span data-ttu-id="9ce28-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9ce28-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ce28-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ce28-122">Authorization</span></span>|<span data-ttu-id="9ce28-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9ce28-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ce28-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9ce28-124">Accept</span></span>|<span data-ttu-id="9ce28-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9ce28-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ce28-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9ce28-126">Request body</span></span>
<span data-ttu-id="9ce28-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsPhone81AppXBundle-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="9ce28-127">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="9ce28-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsPhone81AppXBundle erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="9ce28-128">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="9ce28-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9ce28-129">Property</span></span>|<span data-ttu-id="9ce28-130">Typ</span><span class="sxs-lookup"><span data-stu-id="9ce28-130">Type</span></span>|<span data-ttu-id="9ce28-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ce28-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ce28-132">id</span><span class="sxs-lookup"><span data-stu-id="9ce28-132">id</span></span>|<span data-ttu-id="9ce28-133">String</span><span class="sxs-lookup"><span data-stu-id="9ce28-133">String</span></span>|<span data-ttu-id="9ce28-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9ce28-134">Key of the entity.</span></span> <span data-ttu-id="9ce28-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ce28-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9ce28-136">displayName</span></span>|<span data-ttu-id="9ce28-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ce28-137">String</span></span>|<span data-ttu-id="9ce28-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="9ce28-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9ce28-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ce28-140">description</span><span class="sxs-lookup"><span data-stu-id="9ce28-140">description</span></span>|<span data-ttu-id="9ce28-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ce28-141">String</span></span>|<span data-ttu-id="9ce28-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="9ce28-142">The description of the app.</span></span> <span data-ttu-id="9ce28-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ce28-144">publisher</span><span class="sxs-lookup"><span data-stu-id="9ce28-144">publisher</span></span>|<span data-ttu-id="9ce28-145">String</span><span class="sxs-lookup"><span data-stu-id="9ce28-145">String</span></span>|<span data-ttu-id="9ce28-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="9ce28-146">The publisher of the app.</span></span> <span data-ttu-id="9ce28-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ce28-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9ce28-148">largeIcon</span></span>|[<span data-ttu-id="9ce28-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9ce28-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9ce28-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="9ce28-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9ce28-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ce28-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ce28-152">createdDateTime</span></span>|<span data-ttu-id="9ce28-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ce28-153">DateTimeOffset</span></span>|<span data-ttu-id="9ce28-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="9ce28-154">The date and time the app was created.</span></span> <span data-ttu-id="9ce28-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ce28-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ce28-156">lastModifiedDateTime</span></span>|<span data-ttu-id="9ce28-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ce28-157">DateTimeOffset</span></span>|<span data-ttu-id="9ce28-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="9ce28-158">The date and time the app was last modified.</span></span> <span data-ttu-id="9ce28-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ce28-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9ce28-160">isFeatured</span></span>|<span data-ttu-id="9ce28-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ce28-161">Boolean</span></span>|<span data-ttu-id="9ce28-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ce28-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9ce28-163">privacyInformationUrl</span></span>|<span data-ttu-id="9ce28-164">String</span><span class="sxs-lookup"><span data-stu-id="9ce28-164">String</span></span>|<span data-ttu-id="9ce28-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="9ce28-165">The privacy statement Url.</span></span> <span data-ttu-id="9ce28-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ce28-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9ce28-167">informationUrl</span></span>|<span data-ttu-id="9ce28-168">String</span><span class="sxs-lookup"><span data-stu-id="9ce28-168">String</span></span>|<span data-ttu-id="9ce28-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="9ce28-169">The more information Url.</span></span> <span data-ttu-id="9ce28-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ce28-171">owner</span><span class="sxs-lookup"><span data-stu-id="9ce28-171">owner</span></span>|<span data-ttu-id="9ce28-172">String</span><span class="sxs-lookup"><span data-stu-id="9ce28-172">String</span></span>|<span data-ttu-id="9ce28-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="9ce28-173">The owner of the app.</span></span> <span data-ttu-id="9ce28-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ce28-175">developer</span><span class="sxs-lookup"><span data-stu-id="9ce28-175">developer</span></span>|<span data-ttu-id="9ce28-176">String</span><span class="sxs-lookup"><span data-stu-id="9ce28-176">String</span></span>|<span data-ttu-id="9ce28-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="9ce28-177">The developer of the app.</span></span> <span data-ttu-id="9ce28-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ce28-179">notes</span><span class="sxs-lookup"><span data-stu-id="9ce28-179">notes</span></span>|<span data-ttu-id="9ce28-180">String</span><span class="sxs-lookup"><span data-stu-id="9ce28-180">String</span></span>|<span data-ttu-id="9ce28-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="9ce28-181">Notes for the app.</span></span> <span data-ttu-id="9ce28-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ce28-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="9ce28-183">uploadState</span></span>|<span data-ttu-id="9ce28-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9ce28-184">Int32</span></span>|<span data-ttu-id="9ce28-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="9ce28-185">The upload state.</span></span> <span data-ttu-id="9ce28-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ce28-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="9ce28-187">publishingState</span></span>|[<span data-ttu-id="9ce28-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9ce28-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9ce28-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="9ce28-189">The publishing state for the app.</span></span> <span data-ttu-id="9ce28-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="9ce28-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9ce28-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="9ce28-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9ce28-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="9ce28-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9ce28-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9ce28-193">isAssigned</span></span>|<span data-ttu-id="9ce28-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ce28-194">Boolean</span></span>|<span data-ttu-id="9ce28-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="9ce28-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9ce28-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ce28-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="9ce28-197">roleScopeTagIds</span></span>|<span data-ttu-id="9ce28-198">String collection</span><span class="sxs-lookup"><span data-stu-id="9ce28-198">String collection</span></span>|<span data-ttu-id="9ce28-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="9ce28-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9ce28-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ce28-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9ce28-201">committedContentVersion</span></span>|<span data-ttu-id="9ce28-202">String</span><span class="sxs-lookup"><span data-stu-id="9ce28-202">String</span></span>|<span data-ttu-id="9ce28-203">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="9ce28-203">The internal committed content version.</span></span> <span data-ttu-id="9ce28-204">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9ce28-205">fileName</span><span class="sxs-lookup"><span data-stu-id="9ce28-205">fileName</span></span>|<span data-ttu-id="9ce28-206">String</span><span class="sxs-lookup"><span data-stu-id="9ce28-206">String</span></span>|<span data-ttu-id="9ce28-207">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="9ce28-207">The name of the main Lob application file.</span></span> <span data-ttu-id="9ce28-208">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9ce28-209">size</span><span class="sxs-lookup"><span data-stu-id="9ce28-209">size</span></span>|<span data-ttu-id="9ce28-210">Int64</span><span class="sxs-lookup"><span data-stu-id="9ce28-210">Int64</span></span>|<span data-ttu-id="9ce28-211">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="9ce28-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="9ce28-212">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce28-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9ce28-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="9ce28-213">applicableArchitectures</span></span>|[<span data-ttu-id="9ce28-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="9ce28-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="9ce28-215">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="9ce28-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="9ce28-216">Von [WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="9ce28-216">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="9ce28-217">Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral` und `arm64`.</span><span class="sxs-lookup"><span data-stu-id="9ce28-217">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="9ce28-218">identityName</span><span class="sxs-lookup"><span data-stu-id="9ce28-218">identityName</span></span>|<span data-ttu-id="9ce28-219">String</span><span class="sxs-lookup"><span data-stu-id="9ce28-219">String</span></span>|<span data-ttu-id="9ce28-220">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="9ce28-220">The Identity Name.</span></span> <span data-ttu-id="9ce28-221">Geerbt von [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="9ce28-221">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="9ce28-222">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="9ce28-222">identityPublisherHash</span></span>|<span data-ttu-id="9ce28-223">String</span><span class="sxs-lookup"><span data-stu-id="9ce28-223">String</span></span>|<span data-ttu-id="9ce28-224">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="9ce28-224">The Identity Publisher Hash.</span></span> <span data-ttu-id="9ce28-225">Geerbt von [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="9ce28-225">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="9ce28-226">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="9ce28-226">identityResourceIdentifier</span></span>|<span data-ttu-id="9ce28-227">String</span><span class="sxs-lookup"><span data-stu-id="9ce28-227">String</span></span>|<span data-ttu-id="9ce28-228">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="9ce28-228">The Identity Resource Identifier.</span></span> <span data-ttu-id="9ce28-229">Geerbt von [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="9ce28-229">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="9ce28-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9ce28-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9ce28-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9ce28-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="9ce28-232">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="9ce28-232">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="9ce28-233">Geerbt von [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="9ce28-233">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="9ce28-234">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="9ce28-234">phoneProductIdentifier</span></span>|<span data-ttu-id="9ce28-235">String</span><span class="sxs-lookup"><span data-stu-id="9ce28-235">String</span></span>|<span data-ttu-id="9ce28-236">Die ID des Telefon Produkts.</span><span class="sxs-lookup"><span data-stu-id="9ce28-236">The Phone Product Identifier.</span></span> <span data-ttu-id="9ce28-237">Geerbt von [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="9ce28-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="9ce28-238">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="9ce28-238">phonePublisherId</span></span>|<span data-ttu-id="9ce28-239">String</span><span class="sxs-lookup"><span data-stu-id="9ce28-239">String</span></span>|<span data-ttu-id="9ce28-240">Die Telefon Herausgeber-ID. geerbt von [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="9ce28-240">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="9ce28-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9ce28-241">identityVersion</span></span>|<span data-ttu-id="9ce28-242">String</span><span class="sxs-lookup"><span data-stu-id="9ce28-242">String</span></span>|<span data-ttu-id="9ce28-243">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="9ce28-243">The identity version.</span></span> <span data-ttu-id="9ce28-244">Geerbt von [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="9ce28-244">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="9ce28-245">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="9ce28-245">appXPackageInformationList</span></span>|<span data-ttu-id="9ce28-246">[dem windowspackageinformation](../resources/intune-apps-windowspackageinformation.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="9ce28-246">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="9ce28-247">Die Liste der AppX-Paketinformationen.</span><span class="sxs-lookup"><span data-stu-id="9ce28-247">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="9ce28-248">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ce28-248">Response</span></span>
<span data-ttu-id="9ce28-249">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9ce28-249">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ce28-250">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9ce28-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ce28-251">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ce28-251">Request</span></span>
<span data-ttu-id="9ce28-252">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9ce28-252">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2184

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="9ce28-253">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ce28-253">Response</span></span>
<span data-ttu-id="9ce28-p128">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ce28-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2356

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```




