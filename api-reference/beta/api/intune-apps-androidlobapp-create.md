---
title: AndroidLobApp erstellen
description: Erstellen eines neuen androidLobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d6a8e741164135b9223aea55fc8a074e3d764619
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828987"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="aae67-103">AndroidLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="aae67-103">Create androidLobApp</span></span>

> <span data-ttu-id="aae67-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aae67-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aae67-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aae67-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aae67-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="aae67-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aae67-107">Erstellen eines neuen [androidLobApp](../resources/intune-apps-androidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="aae67-107">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aae67-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="aae67-108">Prerequisites</span></span>
<span data-ttu-id="aae67-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aae67-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aae67-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aae67-111">Permission type</span></span>|<span data-ttu-id="aae67-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aae67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aae67-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aae67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aae67-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aae67-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aae67-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aae67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aae67-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aae67-116">Not supported.</span></span>|
|<span data-ttu-id="aae67-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aae67-117">Application</span></span>|<span data-ttu-id="aae67-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aae67-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aae67-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aae67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="aae67-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aae67-120">Request headers</span></span>
|<span data-ttu-id="aae67-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="aae67-121">Header</span></span>|<span data-ttu-id="aae67-122">Wert</span><span class="sxs-lookup"><span data-stu-id="aae67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aae67-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aae67-123">Authorization</span></span>|<span data-ttu-id="aae67-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="aae67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aae67-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="aae67-125">Accept</span></span>|<span data-ttu-id="aae67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aae67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aae67-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aae67-127">Request body</span></span>
<span data-ttu-id="aae67-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs androidLobApp an.</span><span class="sxs-lookup"><span data-stu-id="aae67-128">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="aae67-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs androidLobApp erstellen.</span><span class="sxs-lookup"><span data-stu-id="aae67-129">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="aae67-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aae67-130">Property</span></span>|<span data-ttu-id="aae67-131">Typ</span><span class="sxs-lookup"><span data-stu-id="aae67-131">Type</span></span>|<span data-ttu-id="aae67-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aae67-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aae67-133">id</span><span class="sxs-lookup"><span data-stu-id="aae67-133">id</span></span>|<span data-ttu-id="aae67-134">String</span><span class="sxs-lookup"><span data-stu-id="aae67-134">String</span></span>|<span data-ttu-id="aae67-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="aae67-135">Key of the entity.</span></span> <span data-ttu-id="aae67-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="aae67-137">displayName</span><span class="sxs-lookup"><span data-stu-id="aae67-137">displayName</span></span>|<span data-ttu-id="aae67-138">String</span><span class="sxs-lookup"><span data-stu-id="aae67-138">String</span></span>|<span data-ttu-id="aae67-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="aae67-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="aae67-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="aae67-141">description</span><span class="sxs-lookup"><span data-stu-id="aae67-141">description</span></span>|<span data-ttu-id="aae67-142">String</span><span class="sxs-lookup"><span data-stu-id="aae67-142">String</span></span>|<span data-ttu-id="aae67-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="aae67-143">The description of the app.</span></span> <span data-ttu-id="aae67-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="aae67-145">publisher</span><span class="sxs-lookup"><span data-stu-id="aae67-145">publisher</span></span>|<span data-ttu-id="aae67-146">String</span><span class="sxs-lookup"><span data-stu-id="aae67-146">String</span></span>|<span data-ttu-id="aae67-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="aae67-147">The publisher of the app.</span></span> <span data-ttu-id="aae67-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="aae67-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="aae67-149">largeIcon</span></span>|[<span data-ttu-id="aae67-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="aae67-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="aae67-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="aae67-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="aae67-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="aae67-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aae67-153">createdDateTime</span></span>|<span data-ttu-id="aae67-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aae67-154">DateTimeOffset</span></span>|<span data-ttu-id="aae67-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="aae67-155">The date and time the app was created.</span></span> <span data-ttu-id="aae67-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="aae67-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aae67-157">lastModifiedDateTime</span></span>|<span data-ttu-id="aae67-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aae67-158">DateTimeOffset</span></span>|<span data-ttu-id="aae67-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="aae67-159">The date and time the app was last modified.</span></span> <span data-ttu-id="aae67-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="aae67-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="aae67-161">isFeatured</span></span>|<span data-ttu-id="aae67-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="aae67-162">Boolean</span></span>|<span data-ttu-id="aae67-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="aae67-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="aae67-164">privacyInformationUrl</span></span>|<span data-ttu-id="aae67-165">String</span><span class="sxs-lookup"><span data-stu-id="aae67-165">String</span></span>|<span data-ttu-id="aae67-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="aae67-166">The privacy statement Url.</span></span> <span data-ttu-id="aae67-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="aae67-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="aae67-168">informationUrl</span></span>|<span data-ttu-id="aae67-169">String</span><span class="sxs-lookup"><span data-stu-id="aae67-169">String</span></span>|<span data-ttu-id="aae67-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="aae67-170">The more information Url.</span></span> <span data-ttu-id="aae67-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="aae67-172">owner</span><span class="sxs-lookup"><span data-stu-id="aae67-172">owner</span></span>|<span data-ttu-id="aae67-173">String</span><span class="sxs-lookup"><span data-stu-id="aae67-173">String</span></span>|<span data-ttu-id="aae67-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="aae67-174">The owner of the app.</span></span> <span data-ttu-id="aae67-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="aae67-176">developer</span><span class="sxs-lookup"><span data-stu-id="aae67-176">developer</span></span>|<span data-ttu-id="aae67-177">String</span><span class="sxs-lookup"><span data-stu-id="aae67-177">String</span></span>|<span data-ttu-id="aae67-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="aae67-178">The developer of the app.</span></span> <span data-ttu-id="aae67-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="aae67-180">notes</span><span class="sxs-lookup"><span data-stu-id="aae67-180">notes</span></span>|<span data-ttu-id="aae67-181">String</span><span class="sxs-lookup"><span data-stu-id="aae67-181">String</span></span>|<span data-ttu-id="aae67-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="aae67-182">Notes for the app.</span></span> <span data-ttu-id="aae67-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="aae67-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="aae67-184">uploadState</span></span>|<span data-ttu-id="aae67-185">Int32</span><span class="sxs-lookup"><span data-stu-id="aae67-185">Int32</span></span>|<span data-ttu-id="aae67-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="aae67-186">The upload state.</span></span> <span data-ttu-id="aae67-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="aae67-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="aae67-188">publishingState</span></span>|[<span data-ttu-id="aae67-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="aae67-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="aae67-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="aae67-190">The publishing state for the app.</span></span> <span data-ttu-id="aae67-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="aae67-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="aae67-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="aae67-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="aae67-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="aae67-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="aae67-194">committedContentVersion</span></span>|<span data-ttu-id="aae67-195">String</span><span class="sxs-lookup"><span data-stu-id="aae67-195">String</span></span>|<span data-ttu-id="aae67-196">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="aae67-196">The internal committed content version.</span></span> <span data-ttu-id="aae67-197">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="aae67-198">fileName</span><span class="sxs-lookup"><span data-stu-id="aae67-198">fileName</span></span>|<span data-ttu-id="aae67-199">String</span><span class="sxs-lookup"><span data-stu-id="aae67-199">String</span></span>|<span data-ttu-id="aae67-200">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="aae67-200">The name of the main Lob application file.</span></span> <span data-ttu-id="aae67-201">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="aae67-202">size</span><span class="sxs-lookup"><span data-stu-id="aae67-202">size</span></span>|<span data-ttu-id="aae67-203">Int64</span><span class="sxs-lookup"><span data-stu-id="aae67-203">Int64</span></span>|<span data-ttu-id="aae67-204">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="aae67-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="aae67-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="aae67-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="aae67-206">packageId</span><span class="sxs-lookup"><span data-stu-id="aae67-206">packageId</span></span>|<span data-ttu-id="aae67-207">String</span><span class="sxs-lookup"><span data-stu-id="aae67-207">String</span></span>|<span data-ttu-id="aae67-208">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="aae67-208">The package identifier.</span></span>|
|<span data-ttu-id="aae67-209">identityName</span><span class="sxs-lookup"><span data-stu-id="aae67-209">identityName</span></span>|<span data-ttu-id="aae67-210">String</span><span class="sxs-lookup"><span data-stu-id="aae67-210">String</span></span>|<span data-ttu-id="aae67-211">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="aae67-211">The Identity Name.</span></span>|
|<span data-ttu-id="aae67-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="aae67-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="aae67-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="aae67-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="aae67-214">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="aae67-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="aae67-215">versionName</span><span class="sxs-lookup"><span data-stu-id="aae67-215">versionName</span></span>|<span data-ttu-id="aae67-216">String</span><span class="sxs-lookup"><span data-stu-id="aae67-216">String</span></span>|<span data-ttu-id="aae67-217">Der Versionsname der branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="aae67-217">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="aae67-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="aae67-218">versionCode</span></span>|<span data-ttu-id="aae67-219">String</span><span class="sxs-lookup"><span data-stu-id="aae67-219">String</span></span>|<span data-ttu-id="aae67-220">Der Versionscode der branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="aae67-220">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="aae67-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="aae67-221">identityVersion</span></span>|<span data-ttu-id="aae67-222">String</span><span class="sxs-lookup"><span data-stu-id="aae67-222">String</span></span>|<span data-ttu-id="aae67-223">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="aae67-223">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="aae67-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="aae67-224">Response</span></span>
<span data-ttu-id="aae67-225">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [androidLobApp](../resources/intune-apps-androidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aae67-225">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aae67-226">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aae67-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="aae67-227">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aae67-227">Request</span></span>
<span data-ttu-id="aae67-228">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aae67-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1365

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="aae67-229">Antwort</span><span class="sxs-lookup"><span data-stu-id="aae67-229">Response</span></span>
<span data-ttu-id="aae67-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aae67-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1473

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```





