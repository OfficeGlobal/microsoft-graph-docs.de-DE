---
title: WindowsPhone81AppXBundle aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windowsPhone81AppXBundle-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 14f221eae60a64629eea3fd5e9a2246a36e76ae3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808596"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="0d510-103">WindowsPhone81AppXBundle aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0d510-103">Update windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="0d510-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0d510-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d510-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0d510-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d510-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0d510-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d510-107">Aktualisieren Sie die Eigenschaften eines [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0d510-107">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0d510-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0d510-108">Prerequisites</span></span>
<span data-ttu-id="0d510-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d510-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d510-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0d510-111">Permission type</span></span>|<span data-ttu-id="0d510-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0d510-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d510-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0d510-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d510-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d510-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0d510-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0d510-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d510-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d510-116">Not supported.</span></span>|
|<span data-ttu-id="0d510-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0d510-117">Application</span></span>|<span data-ttu-id="0d510-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d510-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d510-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d510-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="0d510-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0d510-120">Request headers</span></span>
|<span data-ttu-id="0d510-121">Header</span><span class="sxs-lookup"><span data-stu-id="0d510-121">Header</span></span>|<span data-ttu-id="0d510-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0d510-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d510-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d510-123">Authorization</span></span>|<span data-ttu-id="0d510-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0d510-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d510-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0d510-125">Accept</span></span>|<span data-ttu-id="0d510-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d510-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d510-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0d510-127">Request body</span></span>
<span data-ttu-id="0d510-128">Geben Sie im Textkörper Anforderung für das Objekt [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="0d510-128">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="0d510-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="0d510-129">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="0d510-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0d510-130">Property</span></span>|<span data-ttu-id="0d510-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0d510-131">Type</span></span>|<span data-ttu-id="0d510-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d510-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d510-133">id</span><span class="sxs-lookup"><span data-stu-id="0d510-133">id</span></span>|<span data-ttu-id="0d510-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-134">String</span></span>|<span data-ttu-id="0d510-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0d510-135">Key of the entity.</span></span> <span data-ttu-id="0d510-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d510-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0d510-137">displayName</span></span>|<span data-ttu-id="0d510-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-138">String</span></span>|<span data-ttu-id="0d510-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="0d510-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0d510-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d510-141">description</span><span class="sxs-lookup"><span data-stu-id="0d510-141">description</span></span>|<span data-ttu-id="0d510-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-142">String</span></span>|<span data-ttu-id="0d510-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="0d510-143">The description of the app.</span></span> <span data-ttu-id="0d510-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d510-145">publisher</span><span class="sxs-lookup"><span data-stu-id="0d510-145">publisher</span></span>|<span data-ttu-id="0d510-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-146">String</span></span>|<span data-ttu-id="0d510-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="0d510-147">The publisher of the app.</span></span> <span data-ttu-id="0d510-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d510-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0d510-149">largeIcon</span></span>|[<span data-ttu-id="0d510-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0d510-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0d510-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="0d510-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0d510-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d510-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d510-153">createdDateTime</span></span>|<span data-ttu-id="0d510-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d510-154">DateTimeOffset</span></span>|<span data-ttu-id="0d510-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="0d510-155">The date and time the app was created.</span></span> <span data-ttu-id="0d510-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d510-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d510-157">lastModifiedDateTime</span></span>|<span data-ttu-id="0d510-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d510-158">DateTimeOffset</span></span>|<span data-ttu-id="0d510-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="0d510-159">The date and time the app was last modified.</span></span> <span data-ttu-id="0d510-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d510-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0d510-161">isFeatured</span></span>|<span data-ttu-id="0d510-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0d510-162">Boolean</span></span>|<span data-ttu-id="0d510-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d510-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0d510-164">privacyInformationUrl</span></span>|<span data-ttu-id="0d510-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-165">String</span></span>|<span data-ttu-id="0d510-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="0d510-166">The privacy statement Url.</span></span> <span data-ttu-id="0d510-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d510-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0d510-168">informationUrl</span></span>|<span data-ttu-id="0d510-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-169">String</span></span>|<span data-ttu-id="0d510-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="0d510-170">The more information Url.</span></span> <span data-ttu-id="0d510-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d510-172">owner</span><span class="sxs-lookup"><span data-stu-id="0d510-172">owner</span></span>|<span data-ttu-id="0d510-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-173">String</span></span>|<span data-ttu-id="0d510-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="0d510-174">The owner of the app.</span></span> <span data-ttu-id="0d510-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d510-176">developer</span><span class="sxs-lookup"><span data-stu-id="0d510-176">developer</span></span>|<span data-ttu-id="0d510-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-177">String</span></span>|<span data-ttu-id="0d510-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="0d510-178">The developer of the app.</span></span> <span data-ttu-id="0d510-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d510-180">notes</span><span class="sxs-lookup"><span data-stu-id="0d510-180">notes</span></span>|<span data-ttu-id="0d510-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-181">String</span></span>|<span data-ttu-id="0d510-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="0d510-182">Notes for the app.</span></span> <span data-ttu-id="0d510-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d510-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="0d510-184">uploadState</span></span>|<span data-ttu-id="0d510-185">Int32</span><span class="sxs-lookup"><span data-stu-id="0d510-185">Int32</span></span>|<span data-ttu-id="0d510-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="0d510-186">The upload state.</span></span> <span data-ttu-id="0d510-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d510-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="0d510-188">publishingState</span></span>|[<span data-ttu-id="0d510-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0d510-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0d510-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="0d510-190">The publishing state for the app.</span></span> <span data-ttu-id="0d510-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="0d510-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0d510-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0d510-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="0d510-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0d510-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="0d510-194">committedContentVersion</span></span>|<span data-ttu-id="0d510-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-195">String</span></span>|<span data-ttu-id="0d510-196">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="0d510-196">The internal committed content version.</span></span> <span data-ttu-id="0d510-197">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0d510-198">fileName</span><span class="sxs-lookup"><span data-stu-id="0d510-198">fileName</span></span>|<span data-ttu-id="0d510-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-199">String</span></span>|<span data-ttu-id="0d510-200">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="0d510-200">The name of the main Lob application file.</span></span> <span data-ttu-id="0d510-201">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0d510-202">size</span><span class="sxs-lookup"><span data-stu-id="0d510-202">size</span></span>|<span data-ttu-id="0d510-203">Int64</span><span class="sxs-lookup"><span data-stu-id="0d510-203">Int64</span></span>|<span data-ttu-id="0d510-204">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="0d510-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="0d510-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0d510-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="0d510-206">applicableArchitectures</span></span>|[<span data-ttu-id="0d510-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="0d510-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="0d510-208">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="0d510-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="0d510-209">Geerbt von [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="0d510-209">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="0d510-210">Mögliche Werte: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="0d510-210">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="0d510-211">identityName</span><span class="sxs-lookup"><span data-stu-id="0d510-211">identityName</span></span>|<span data-ttu-id="0d510-212">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-212">String</span></span>|<span data-ttu-id="0d510-213">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="0d510-213">The Identity Name.</span></span> <span data-ttu-id="0d510-214">Geerbt von [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="0d510-214">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0d510-215">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="0d510-215">identityPublisherHash</span></span>|<span data-ttu-id="0d510-216">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-216">String</span></span>|<span data-ttu-id="0d510-217">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="0d510-217">The Identity Publisher Hash.</span></span> <span data-ttu-id="0d510-218">Geerbt von [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="0d510-218">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0d510-219">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="0d510-219">identityResourceIdentifier</span></span>|<span data-ttu-id="0d510-220">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-220">String</span></span>|<span data-ttu-id="0d510-221">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="0d510-221">The Identity Resource Identifier.</span></span> <span data-ttu-id="0d510-222">Geerbt von [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="0d510-222">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0d510-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0d510-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0d510-224">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0d510-224">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="0d510-225">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="0d510-225">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="0d510-226">Geerbt von [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="0d510-226">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0d510-227">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="0d510-227">phoneProductIdentifier</span></span>|<span data-ttu-id="0d510-228">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-228">String</span></span>|<span data-ttu-id="0d510-229">Die Produkt-ID des Telefons.</span><span class="sxs-lookup"><span data-stu-id="0d510-229">The Phone Product Identifier.</span></span> <span data-ttu-id="0d510-230">Geerbt von [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="0d510-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0d510-231">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="0d510-231">phonePublisherId</span></span>|<span data-ttu-id="0d510-232">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-232">String</span></span>|<span data-ttu-id="0d510-233">Geerbt von [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) Phone Publisher-Id.</span><span class="sxs-lookup"><span data-stu-id="0d510-233">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0d510-234">identityVersion</span><span class="sxs-lookup"><span data-stu-id="0d510-234">identityVersion</span></span>|<span data-ttu-id="0d510-235">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d510-235">String</span></span>|<span data-ttu-id="0d510-236">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="0d510-236">The identity version.</span></span> <span data-ttu-id="0d510-237">Geerbt von [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="0d510-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0d510-238">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="0d510-238">appXPackageInformationList</span></span>|<span data-ttu-id="0d510-239">[WindowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0d510-239">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="0d510-240">Die Liste der AppX Package Information.</span><span class="sxs-lookup"><span data-stu-id="0d510-240">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="0d510-241">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d510-241">Response</span></span>
<span data-ttu-id="0d510-242">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0d510-242">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d510-243">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0d510-243">Example</span></span>
### <a name="request"></a><span data-ttu-id="0d510-244">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d510-244">Request</span></span>
<span data-ttu-id="0d510-245">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0d510-245">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2100

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

### <a name="response"></a><span data-ttu-id="0d510-246">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d510-246">Response</span></span>
<span data-ttu-id="0d510-p127">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d510-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2271

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





