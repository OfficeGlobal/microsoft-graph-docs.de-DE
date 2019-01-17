---
title: WindowsAppX aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsAppX-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7123364c618dbbdf0eb37dd9e080f54a67b6809b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946168"
---
# <a name="update-windowsappx"></a><span data-ttu-id="af2f4-103">WindowsAppX aktualisieren</span><span class="sxs-lookup"><span data-stu-id="af2f4-103">Update windowsAppX</span></span>

> <span data-ttu-id="af2f4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="af2f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af2f4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="af2f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af2f4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="af2f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af2f4-107">Aktualisieren Sie die Eigenschaften eines [WindowsAppX](../resources/intune-apps-windowsappx.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="af2f4-107">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af2f4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="af2f4-108">Prerequisites</span></span>
<span data-ttu-id="af2f4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af2f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af2f4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="af2f4-111">Permission type</span></span>|<span data-ttu-id="af2f4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="af2f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af2f4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="af2f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af2f4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af2f4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="af2f4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="af2f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af2f4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af2f4-116">Not supported.</span></span>|
|<span data-ttu-id="af2f4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="af2f4-117">Application</span></span>|<span data-ttu-id="af2f4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af2f4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af2f4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="af2f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="af2f4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="af2f4-120">Request headers</span></span>
|<span data-ttu-id="af2f4-121">Header</span><span class="sxs-lookup"><span data-stu-id="af2f4-121">Header</span></span>|<span data-ttu-id="af2f4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="af2f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af2f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="af2f4-123">Authorization</span></span>|<span data-ttu-id="af2f4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="af2f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af2f4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="af2f4-125">Accept</span></span>|<span data-ttu-id="af2f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af2f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af2f4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="af2f4-127">Request body</span></span>
<span data-ttu-id="af2f4-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsAppX](../resources/intune-apps-windowsappx.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="af2f4-128">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="af2f4-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsAppX](../resources/intune-apps-windowsappx.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="af2f4-129">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="af2f4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="af2f4-130">Property</span></span>|<span data-ttu-id="af2f4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="af2f4-131">Type</span></span>|<span data-ttu-id="af2f4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af2f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af2f4-133">id</span><span class="sxs-lookup"><span data-stu-id="af2f4-133">id</span></span>|<span data-ttu-id="af2f4-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af2f4-134">String</span></span>|<span data-ttu-id="af2f4-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="af2f4-135">Key of the entity.</span></span> <span data-ttu-id="af2f4-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af2f4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="af2f4-137">displayName</span></span>|<span data-ttu-id="af2f4-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af2f4-138">String</span></span>|<span data-ttu-id="af2f4-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="af2f4-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="af2f4-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af2f4-141">description</span><span class="sxs-lookup"><span data-stu-id="af2f4-141">description</span></span>|<span data-ttu-id="af2f4-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af2f4-142">String</span></span>|<span data-ttu-id="af2f4-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="af2f4-143">The description of the app.</span></span> <span data-ttu-id="af2f4-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af2f4-145">publisher</span><span class="sxs-lookup"><span data-stu-id="af2f4-145">publisher</span></span>|<span data-ttu-id="af2f4-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af2f4-146">String</span></span>|<span data-ttu-id="af2f4-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="af2f4-147">The publisher of the app.</span></span> <span data-ttu-id="af2f4-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af2f4-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="af2f4-149">largeIcon</span></span>|[<span data-ttu-id="af2f4-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="af2f4-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="af2f4-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="af2f4-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="af2f4-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af2f4-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af2f4-153">createdDateTime</span></span>|<span data-ttu-id="af2f4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af2f4-154">DateTimeOffset</span></span>|<span data-ttu-id="af2f4-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="af2f4-155">The date and time the app was created.</span></span> <span data-ttu-id="af2f4-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af2f4-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af2f4-157">lastModifiedDateTime</span></span>|<span data-ttu-id="af2f4-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af2f4-158">DateTimeOffset</span></span>|<span data-ttu-id="af2f4-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="af2f4-159">The date and time the app was last modified.</span></span> <span data-ttu-id="af2f4-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af2f4-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="af2f4-161">isFeatured</span></span>|<span data-ttu-id="af2f4-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="af2f4-162">Boolean</span></span>|<span data-ttu-id="af2f4-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af2f4-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="af2f4-164">privacyInformationUrl</span></span>|<span data-ttu-id="af2f4-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af2f4-165">String</span></span>|<span data-ttu-id="af2f4-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="af2f4-166">The privacy statement Url.</span></span> <span data-ttu-id="af2f4-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af2f4-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="af2f4-168">informationUrl</span></span>|<span data-ttu-id="af2f4-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af2f4-169">String</span></span>|<span data-ttu-id="af2f4-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="af2f4-170">The more information Url.</span></span> <span data-ttu-id="af2f4-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af2f4-172">owner</span><span class="sxs-lookup"><span data-stu-id="af2f4-172">owner</span></span>|<span data-ttu-id="af2f4-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af2f4-173">String</span></span>|<span data-ttu-id="af2f4-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="af2f4-174">The owner of the app.</span></span> <span data-ttu-id="af2f4-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af2f4-176">developer</span><span class="sxs-lookup"><span data-stu-id="af2f4-176">developer</span></span>|<span data-ttu-id="af2f4-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af2f4-177">String</span></span>|<span data-ttu-id="af2f4-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="af2f4-178">The developer of the app.</span></span> <span data-ttu-id="af2f4-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af2f4-180">notes</span><span class="sxs-lookup"><span data-stu-id="af2f4-180">notes</span></span>|<span data-ttu-id="af2f4-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af2f4-181">String</span></span>|<span data-ttu-id="af2f4-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="af2f4-182">Notes for the app.</span></span> <span data-ttu-id="af2f4-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af2f4-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="af2f4-184">uploadState</span></span>|<span data-ttu-id="af2f4-185">Int32</span><span class="sxs-lookup"><span data-stu-id="af2f4-185">Int32</span></span>|<span data-ttu-id="af2f4-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="af2f4-186">The upload state.</span></span> <span data-ttu-id="af2f4-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af2f4-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="af2f4-188">publishingState</span></span>|[<span data-ttu-id="af2f4-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="af2f4-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="af2f4-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="af2f4-190">The publishing state for the app.</span></span> <span data-ttu-id="af2f4-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="af2f4-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="af2f4-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="af2f4-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="af2f4-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="af2f4-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="af2f4-194">committedContentVersion</span></span>|<span data-ttu-id="af2f4-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af2f4-195">String</span></span>|<span data-ttu-id="af2f4-196">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="af2f4-196">The internal committed content version.</span></span> <span data-ttu-id="af2f4-197">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="af2f4-198">fileName</span><span class="sxs-lookup"><span data-stu-id="af2f4-198">fileName</span></span>|<span data-ttu-id="af2f4-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af2f4-199">String</span></span>|<span data-ttu-id="af2f4-200">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="af2f4-200">The name of the main Lob application file.</span></span> <span data-ttu-id="af2f4-201">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="af2f4-202">size</span><span class="sxs-lookup"><span data-stu-id="af2f4-202">size</span></span>|<span data-ttu-id="af2f4-203">Int64</span><span class="sxs-lookup"><span data-stu-id="af2f4-203">Int64</span></span>|<span data-ttu-id="af2f4-204">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="af2f4-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="af2f4-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="af2f4-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="af2f4-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="af2f4-206">applicableArchitectures</span></span>|[<span data-ttu-id="af2f4-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="af2f4-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="af2f4-208">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="af2f4-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="af2f4-209">Mögliche Werte: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="af2f4-209">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="af2f4-210">identityName</span><span class="sxs-lookup"><span data-stu-id="af2f4-210">identityName</span></span>|<span data-ttu-id="af2f4-211">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af2f4-211">String</span></span>|<span data-ttu-id="af2f4-212">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="af2f4-212">The Identity Name.</span></span>|
|<span data-ttu-id="af2f4-213">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="af2f4-213">identityPublisherHash</span></span>|<span data-ttu-id="af2f4-214">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af2f4-214">String</span></span>|<span data-ttu-id="af2f4-215">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="af2f4-215">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="af2f4-216">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="af2f4-216">identityResourceIdentifier</span></span>|<span data-ttu-id="af2f4-217">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af2f4-217">String</span></span>|<span data-ttu-id="af2f4-218">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="af2f4-218">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="af2f4-219">isBundle</span><span class="sxs-lookup"><span data-stu-id="af2f4-219">isBundle</span></span>|<span data-ttu-id="af2f4-220">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="af2f4-220">Boolean</span></span>|<span data-ttu-id="af2f4-221">Gibt an, ob die App ein Bundle ist.</span><span class="sxs-lookup"><span data-stu-id="af2f4-221">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="af2f4-222">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="af2f4-222">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="af2f4-223">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="af2f4-223">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="af2f4-224">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="af2f4-224">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="af2f4-225">identityVersion</span><span class="sxs-lookup"><span data-stu-id="af2f4-225">identityVersion</span></span>|<span data-ttu-id="af2f4-226">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af2f4-226">String</span></span>|<span data-ttu-id="af2f4-227">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="af2f4-227">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="af2f4-228">Antwort</span><span class="sxs-lookup"><span data-stu-id="af2f4-228">Response</span></span>
<span data-ttu-id="af2f4-229">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsAppX](../resources/intune-apps-windowsappx.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="af2f4-229">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af2f4-230">Beispiel</span><span class="sxs-lookup"><span data-stu-id="af2f4-230">Example</span></span>
### <a name="request"></a><span data-ttu-id="af2f4-231">Anforderung</span><span class="sxs-lookup"><span data-stu-id="af2f4-231">Request</span></span>
<span data-ttu-id="af2f4-232">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="af2f4-232">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1269

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

### <a name="response"></a><span data-ttu-id="af2f4-233">Antwort</span><span class="sxs-lookup"><span data-stu-id="af2f4-233">Response</span></span>
<span data-ttu-id="af2f4-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="af2f4-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





