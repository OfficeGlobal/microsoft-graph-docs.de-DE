---
title: Erstellen von windowsAppX
description: Erstellen eines neuen WindowsAppX-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1bba1587ababb35a608663865209ad27d5f67738
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420318"
---
# <a name="create-windowsappx"></a><span data-ttu-id="17649-103">Erstellen von windowsAppX</span><span class="sxs-lookup"><span data-stu-id="17649-103">Create windowsAppX</span></span>

> <span data-ttu-id="17649-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="17649-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="17649-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="17649-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17649-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="17649-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17649-107">Erstellen eines neuen [WindowsAppX](../resources/intune-apps-windowsappx.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="17649-107">Create a new [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17649-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="17649-108">Prerequisites</span></span>
<span data-ttu-id="17649-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="17649-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="17649-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="17649-111">Permission type</span></span>|<span data-ttu-id="17649-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="17649-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17649-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="17649-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17649-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17649-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="17649-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="17649-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17649-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="17649-116">Not supported.</span></span>|
|<span data-ttu-id="17649-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="17649-117">Application</span></span>|<span data-ttu-id="17649-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="17649-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17649-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="17649-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="17649-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="17649-120">Request headers</span></span>
|<span data-ttu-id="17649-121">Header</span><span class="sxs-lookup"><span data-stu-id="17649-121">Header</span></span>|<span data-ttu-id="17649-122">Wert</span><span class="sxs-lookup"><span data-stu-id="17649-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17649-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="17649-123">Authorization</span></span>|<span data-ttu-id="17649-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="17649-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17649-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="17649-125">Accept</span></span>|<span data-ttu-id="17649-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17649-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17649-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="17649-127">Request body</span></span>
<span data-ttu-id="17649-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsAppX eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="17649-128">In the request body, supply a JSON representation for the windowsAppX object.</span></span>

<span data-ttu-id="17649-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsAppX erstellen.</span><span class="sxs-lookup"><span data-stu-id="17649-129">The following table shows the properties that are required when you create the windowsAppX.</span></span>

|<span data-ttu-id="17649-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="17649-130">Property</span></span>|<span data-ttu-id="17649-131">Typ</span><span class="sxs-lookup"><span data-stu-id="17649-131">Type</span></span>|<span data-ttu-id="17649-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17649-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17649-133">id</span><span class="sxs-lookup"><span data-stu-id="17649-133">id</span></span>|<span data-ttu-id="17649-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17649-134">String</span></span>|<span data-ttu-id="17649-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="17649-135">Key of the entity.</span></span> <span data-ttu-id="17649-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17649-137">displayName</span><span class="sxs-lookup"><span data-stu-id="17649-137">displayName</span></span>|<span data-ttu-id="17649-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17649-138">String</span></span>|<span data-ttu-id="17649-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="17649-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="17649-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17649-141">description</span><span class="sxs-lookup"><span data-stu-id="17649-141">description</span></span>|<span data-ttu-id="17649-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17649-142">String</span></span>|<span data-ttu-id="17649-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="17649-143">The description of the app.</span></span> <span data-ttu-id="17649-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17649-145">publisher</span><span class="sxs-lookup"><span data-stu-id="17649-145">publisher</span></span>|<span data-ttu-id="17649-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17649-146">String</span></span>|<span data-ttu-id="17649-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="17649-147">The publisher of the app.</span></span> <span data-ttu-id="17649-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17649-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="17649-149">largeIcon</span></span>|[<span data-ttu-id="17649-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="17649-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="17649-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="17649-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="17649-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17649-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17649-153">createdDateTime</span></span>|<span data-ttu-id="17649-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17649-154">DateTimeOffset</span></span>|<span data-ttu-id="17649-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="17649-155">The date and time the app was created.</span></span> <span data-ttu-id="17649-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17649-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17649-157">lastModifiedDateTime</span></span>|<span data-ttu-id="17649-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17649-158">DateTimeOffset</span></span>|<span data-ttu-id="17649-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="17649-159">The date and time the app was last modified.</span></span> <span data-ttu-id="17649-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17649-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="17649-161">isFeatured</span></span>|<span data-ttu-id="17649-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="17649-162">Boolean</span></span>|<span data-ttu-id="17649-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17649-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="17649-164">privacyInformationUrl</span></span>|<span data-ttu-id="17649-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17649-165">String</span></span>|<span data-ttu-id="17649-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="17649-166">The privacy statement Url.</span></span> <span data-ttu-id="17649-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17649-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="17649-168">informationUrl</span></span>|<span data-ttu-id="17649-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17649-169">String</span></span>|<span data-ttu-id="17649-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="17649-170">The more information Url.</span></span> <span data-ttu-id="17649-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17649-172">owner</span><span class="sxs-lookup"><span data-stu-id="17649-172">owner</span></span>|<span data-ttu-id="17649-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17649-173">String</span></span>|<span data-ttu-id="17649-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="17649-174">The owner of the app.</span></span> <span data-ttu-id="17649-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17649-176">developer</span><span class="sxs-lookup"><span data-stu-id="17649-176">developer</span></span>|<span data-ttu-id="17649-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17649-177">String</span></span>|<span data-ttu-id="17649-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="17649-178">The developer of the app.</span></span> <span data-ttu-id="17649-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17649-180">notes</span><span class="sxs-lookup"><span data-stu-id="17649-180">notes</span></span>|<span data-ttu-id="17649-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17649-181">String</span></span>|<span data-ttu-id="17649-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="17649-182">Notes for the app.</span></span> <span data-ttu-id="17649-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17649-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="17649-184">uploadState</span></span>|<span data-ttu-id="17649-185">Int32</span><span class="sxs-lookup"><span data-stu-id="17649-185">Int32</span></span>|<span data-ttu-id="17649-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="17649-186">The upload state.</span></span> <span data-ttu-id="17649-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17649-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="17649-188">publishingState</span></span>|[<span data-ttu-id="17649-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="17649-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="17649-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="17649-190">The publishing state for the app.</span></span> <span data-ttu-id="17649-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="17649-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="17649-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="17649-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="17649-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="17649-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="17649-194">isAssigned</span></span>|<span data-ttu-id="17649-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="17649-195">Boolean</span></span>|<span data-ttu-id="17649-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="17649-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="17649-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17649-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="17649-198">roleScopeTagIds</span></span>|<span data-ttu-id="17649-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="17649-199">String collection</span></span>|<span data-ttu-id="17649-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="17649-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="17649-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17649-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="17649-202">committedContentVersion</span></span>|<span data-ttu-id="17649-203">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17649-203">String</span></span>|<span data-ttu-id="17649-204">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="17649-204">The internal committed content version.</span></span> <span data-ttu-id="17649-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="17649-206">fileName</span><span class="sxs-lookup"><span data-stu-id="17649-206">fileName</span></span>|<span data-ttu-id="17649-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17649-207">String</span></span>|<span data-ttu-id="17649-208">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="17649-208">The name of the main Lob application file.</span></span> <span data-ttu-id="17649-209">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="17649-210">size</span><span class="sxs-lookup"><span data-stu-id="17649-210">size</span></span>|<span data-ttu-id="17649-211">Int64</span><span class="sxs-lookup"><span data-stu-id="17649-211">Int64</span></span>|<span data-ttu-id="17649-212">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="17649-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="17649-213">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="17649-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="17649-214">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="17649-214">applicableArchitectures</span></span>|[<span data-ttu-id="17649-215">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="17649-215">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="17649-216">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="17649-216">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="17649-217">Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral` und `arm64`.</span><span class="sxs-lookup"><span data-stu-id="17649-217">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="17649-218">identityName</span><span class="sxs-lookup"><span data-stu-id="17649-218">identityName</span></span>|<span data-ttu-id="17649-219">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17649-219">String</span></span>|<span data-ttu-id="17649-220">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="17649-220">The Identity Name.</span></span>|
|<span data-ttu-id="17649-221">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="17649-221">identityPublisherHash</span></span>|<span data-ttu-id="17649-222">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17649-222">String</span></span>|<span data-ttu-id="17649-223">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="17649-223">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="17649-224">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="17649-224">identityResourceIdentifier</span></span>|<span data-ttu-id="17649-225">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17649-225">String</span></span>|<span data-ttu-id="17649-226">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="17649-226">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="17649-227">isBundle</span><span class="sxs-lookup"><span data-stu-id="17649-227">isBundle</span></span>|<span data-ttu-id="17649-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="17649-228">Boolean</span></span>|<span data-ttu-id="17649-229">Gibt an, ob die App ein Bundle ist.</span><span class="sxs-lookup"><span data-stu-id="17649-229">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="17649-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="17649-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="17649-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="17649-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="17649-232">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="17649-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="17649-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="17649-233">identityVersion</span></span>|<span data-ttu-id="17649-234">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17649-234">String</span></span>|<span data-ttu-id="17649-235">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="17649-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="17649-236">Antwort</span><span class="sxs-lookup"><span data-stu-id="17649-236">Response</span></span>
<span data-ttu-id="17649-237">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsAppX](../resources/intune-apps-windowsappx.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="17649-237">If successful, this method returns a `201 Created` response code and a [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17649-238">Beispiel</span><span class="sxs-lookup"><span data-stu-id="17649-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="17649-239">Anforderung</span><span class="sxs-lookup"><span data-stu-id="17649-239">Request</span></span>
<span data-ttu-id="17649-240">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="17649-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1340

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

### <a name="response"></a><span data-ttu-id="17649-241">Antwort</span><span class="sxs-lookup"><span data-stu-id="17649-241">Response</span></span>
<span data-ttu-id="17649-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="17649-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1512

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




