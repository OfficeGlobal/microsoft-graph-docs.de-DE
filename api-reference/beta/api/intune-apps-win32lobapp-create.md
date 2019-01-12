---
title: Erstellen von win32LobApp
description: Erstellen eines neuen win32LobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3ac82ba6d546fe64cb472686af2fcd0ee642d1eb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979264"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="e33b9-103">Erstellen von win32LobApp</span><span class="sxs-lookup"><span data-stu-id="e33b9-103">Create win32LobApp</span></span>

> <span data-ttu-id="e33b9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e33b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e33b9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e33b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e33b9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e33b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e33b9-107">Erstellen eines neuen [win32LobApp](../resources/intune-apps-win32lobapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e33b9-107">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e33b9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e33b9-108">Prerequisites</span></span>
<span data-ttu-id="e33b9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e33b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e33b9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e33b9-111">Permission type</span></span>|<span data-ttu-id="e33b9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e33b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e33b9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e33b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e33b9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e33b9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e33b9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e33b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e33b9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e33b9-116">Not supported.</span></span>|
|<span data-ttu-id="e33b9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e33b9-117">Application</span></span>|<span data-ttu-id="e33b9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e33b9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e33b9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e33b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e33b9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e33b9-120">Request headers</span></span>
|<span data-ttu-id="e33b9-121">Header</span><span class="sxs-lookup"><span data-stu-id="e33b9-121">Header</span></span>|<span data-ttu-id="e33b9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e33b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e33b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e33b9-123">Authorization</span></span>|<span data-ttu-id="e33b9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e33b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e33b9-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e33b9-125">Accept</span></span>|<span data-ttu-id="e33b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e33b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e33b9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e33b9-127">Request body</span></span>
<span data-ttu-id="e33b9-128">Geben Sie im Textkörper Anforderung für das Objekt win32LobApp eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="e33b9-128">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="e33b9-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die win32LobApp erstellen.</span><span class="sxs-lookup"><span data-stu-id="e33b9-129">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="e33b9-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e33b9-130">Property</span></span>|<span data-ttu-id="e33b9-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e33b9-131">Type</span></span>|<span data-ttu-id="e33b9-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e33b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e33b9-133">id</span><span class="sxs-lookup"><span data-stu-id="e33b9-133">id</span></span>|<span data-ttu-id="e33b9-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e33b9-134">String</span></span>|<span data-ttu-id="e33b9-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e33b9-135">Key of the entity.</span></span> <span data-ttu-id="e33b9-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e33b9-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e33b9-137">displayName</span></span>|<span data-ttu-id="e33b9-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e33b9-138">String</span></span>|<span data-ttu-id="e33b9-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="e33b9-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e33b9-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e33b9-141">description</span><span class="sxs-lookup"><span data-stu-id="e33b9-141">description</span></span>|<span data-ttu-id="e33b9-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e33b9-142">String</span></span>|<span data-ttu-id="e33b9-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="e33b9-143">The description of the app.</span></span> <span data-ttu-id="e33b9-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e33b9-145">publisher</span><span class="sxs-lookup"><span data-stu-id="e33b9-145">publisher</span></span>|<span data-ttu-id="e33b9-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e33b9-146">String</span></span>|<span data-ttu-id="e33b9-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="e33b9-147">The publisher of the app.</span></span> <span data-ttu-id="e33b9-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e33b9-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e33b9-149">largeIcon</span></span>|[<span data-ttu-id="e33b9-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e33b9-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e33b9-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e33b9-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e33b9-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e33b9-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e33b9-153">createdDateTime</span></span>|<span data-ttu-id="e33b9-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e33b9-154">DateTimeOffset</span></span>|<span data-ttu-id="e33b9-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="e33b9-155">The date and time the app was created.</span></span> <span data-ttu-id="e33b9-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e33b9-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e33b9-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e33b9-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e33b9-158">DateTimeOffset</span></span>|<span data-ttu-id="e33b9-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="e33b9-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e33b9-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e33b9-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e33b9-161">isFeatured</span></span>|<span data-ttu-id="e33b9-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e33b9-162">Boolean</span></span>|<span data-ttu-id="e33b9-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e33b9-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e33b9-164">privacyInformationUrl</span></span>|<span data-ttu-id="e33b9-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e33b9-165">String</span></span>|<span data-ttu-id="e33b9-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="e33b9-166">The privacy statement Url.</span></span> <span data-ttu-id="e33b9-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e33b9-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e33b9-168">informationUrl</span></span>|<span data-ttu-id="e33b9-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e33b9-169">String</span></span>|<span data-ttu-id="e33b9-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="e33b9-170">The more information Url.</span></span> <span data-ttu-id="e33b9-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e33b9-172">owner</span><span class="sxs-lookup"><span data-stu-id="e33b9-172">owner</span></span>|<span data-ttu-id="e33b9-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e33b9-173">String</span></span>|<span data-ttu-id="e33b9-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="e33b9-174">The owner of the app.</span></span> <span data-ttu-id="e33b9-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e33b9-176">developer</span><span class="sxs-lookup"><span data-stu-id="e33b9-176">developer</span></span>|<span data-ttu-id="e33b9-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e33b9-177">String</span></span>|<span data-ttu-id="e33b9-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="e33b9-178">The developer of the app.</span></span> <span data-ttu-id="e33b9-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e33b9-180">notes</span><span class="sxs-lookup"><span data-stu-id="e33b9-180">notes</span></span>|<span data-ttu-id="e33b9-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e33b9-181">String</span></span>|<span data-ttu-id="e33b9-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="e33b9-182">Notes for the app.</span></span> <span data-ttu-id="e33b9-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e33b9-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e33b9-184">uploadState</span></span>|<span data-ttu-id="e33b9-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e33b9-185">Int32</span></span>|<span data-ttu-id="e33b9-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="e33b9-186">The upload state.</span></span> <span data-ttu-id="e33b9-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e33b9-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="e33b9-188">publishingState</span></span>|[<span data-ttu-id="e33b9-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e33b9-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e33b9-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="e33b9-190">The publishing state for the app.</span></span> <span data-ttu-id="e33b9-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="e33b9-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e33b9-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e33b9-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="e33b9-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e33b9-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e33b9-194">committedContentVersion</span></span>|<span data-ttu-id="e33b9-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e33b9-195">String</span></span>|<span data-ttu-id="e33b9-196">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="e33b9-196">The internal committed content version.</span></span> <span data-ttu-id="e33b9-197">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e33b9-198">fileName</span><span class="sxs-lookup"><span data-stu-id="e33b9-198">fileName</span></span>|<span data-ttu-id="e33b9-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e33b9-199">String</span></span>|<span data-ttu-id="e33b9-200">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="e33b9-200">The name of the main Lob application file.</span></span> <span data-ttu-id="e33b9-201">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e33b9-202">size</span><span class="sxs-lookup"><span data-stu-id="e33b9-202">size</span></span>|<span data-ttu-id="e33b9-203">Int64</span><span class="sxs-lookup"><span data-stu-id="e33b9-203">Int64</span></span>|<span data-ttu-id="e33b9-204">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="e33b9-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="e33b9-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e33b9-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e33b9-206">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="e33b9-206">installCommandLine</span></span>|<span data-ttu-id="e33b9-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e33b9-207">String</span></span>|<span data-ttu-id="e33b9-208">So installieren Sie diese app die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="e33b9-208">The command line to install this app</span></span>|
|<span data-ttu-id="e33b9-209">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="e33b9-209">uninstallCommandLine</span></span>|<span data-ttu-id="e33b9-210">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e33b9-210">String</span></span>|<span data-ttu-id="e33b9-211">So deinstallieren Sie diese app die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="e33b9-211">The command line to uninstall this app</span></span>|
|<span data-ttu-id="e33b9-212">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="e33b9-212">applicableArchitectures</span></span>|[<span data-ttu-id="e33b9-213">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="e33b9-213">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="e33b9-214">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="e33b9-214">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="e33b9-215">Mögliche Werte: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="e33b9-215">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="e33b9-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e33b9-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e33b9-217">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e33b9-217">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="e33b9-218">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="e33b9-218">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e33b9-219">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="e33b9-219">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="e33b9-220">Int32</span><span class="sxs-lookup"><span data-stu-id="e33b9-220">Int32</span></span>|<span data-ttu-id="e33b9-221">Der Wert für den minimalen freien Speicherplatz der erforderlich ist, um diese app zu installieren.</span><span class="sxs-lookup"><span data-stu-id="e33b9-221">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="e33b9-222">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="e33b9-222">minimumMemoryInMB</span></span>|<span data-ttu-id="e33b9-223">Int32</span><span class="sxs-lookup"><span data-stu-id="e33b9-223">Int32</span></span>|<span data-ttu-id="e33b9-224">Der Wert für das minimale des Arbeitsspeichers erforderlich für diese app installieren.</span><span class="sxs-lookup"><span data-stu-id="e33b9-224">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="e33b9-225">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="e33b9-225">minimumNumberOfProcessors</span></span>|<span data-ttu-id="e33b9-226">Int32</span><span class="sxs-lookup"><span data-stu-id="e33b9-226">Int32</span></span>|<span data-ttu-id="e33b9-227">Der Wert für die minimale Anzahl der Prozessoren erforderlich ist, um diese app zu installieren.</span><span class="sxs-lookup"><span data-stu-id="e33b9-227">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="e33b9-228">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="e33b9-228">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="e33b9-229">Int32</span><span class="sxs-lookup"><span data-stu-id="e33b9-229">Int32</span></span>|<span data-ttu-id="e33b9-230">Der Wert für die minimale CPU-Geschwindigkeit der erforderlich ist, um diese app zu installieren.</span><span class="sxs-lookup"><span data-stu-id="e33b9-230">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="e33b9-231">detectionRules</span><span class="sxs-lookup"><span data-stu-id="e33b9-231">detectionRules</span></span>|<span data-ttu-id="e33b9-232">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e33b9-232">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="e33b9-233">Die Erkennung von Regeln zum Erkennen von Win32 Line of Business (LoB) app.</span><span class="sxs-lookup"><span data-stu-id="e33b9-233">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e33b9-234">installExperience</span><span class="sxs-lookup"><span data-stu-id="e33b9-234">installExperience</span></span>|[<span data-ttu-id="e33b9-235">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="e33b9-235">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="e33b9-236">Die Installation für diese app.</span><span class="sxs-lookup"><span data-stu-id="e33b9-236">The install experience for this app.</span></span>|
|<span data-ttu-id="e33b9-237">returnCodes</span><span class="sxs-lookup"><span data-stu-id="e33b9-237">returnCodes</span></span>|<span data-ttu-id="e33b9-238">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e33b9-238">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="e33b9-239">Die Rückgabecodes für buchen Verhalten bei der Installation.</span><span class="sxs-lookup"><span data-stu-id="e33b9-239">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="e33b9-240">msiInformation</span><span class="sxs-lookup"><span data-stu-id="e33b9-240">msiInformation</span></span>|[<span data-ttu-id="e33b9-241">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="e33b9-241">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="e33b9-242">Die MSI-Details, wenn diese Win32-app eine MSI-app ist.</span><span class="sxs-lookup"><span data-stu-id="e33b9-242">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="e33b9-243">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="e33b9-243">setupFilePath</span></span>|<span data-ttu-id="e33b9-244">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e33b9-244">String</span></span>|<span data-ttu-id="e33b9-245">Der relative Pfad der Datei in das verschlüsselte Win32LobApp-Paket.</span><span class="sxs-lookup"><span data-stu-id="e33b9-245">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="e33b9-246">Antwort</span><span class="sxs-lookup"><span data-stu-id="e33b9-246">Response</span></span>
<span data-ttu-id="e33b9-247">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [win32LobApp](../resources/intune-apps-win32lobapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e33b9-247">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e33b9-248">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e33b9-248">Example</span></span>
### <a name="request"></a><span data-ttu-id="e33b9-249">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e33b9-249">Request</span></span>
<span data-ttu-id="e33b9-250">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e33b9-250">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2264

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser"
  },
  "setupFilePath": "Setup File Path value"
}
```

### <a name="response"></a><span data-ttu-id="e33b9-251">Antwort</span><span class="sxs-lookup"><span data-stu-id="e33b9-251">Response</span></span>
<span data-ttu-id="e33b9-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e33b9-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2372

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser"
  },
  "setupFilePath": "Setup File Path value"
}
```





