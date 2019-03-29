---
title: iosLobApp erstellen
description: Erstellt ein neues iosLobApp-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de00439364f0236625e337edef7cbd55def3fdba
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957661"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="1647f-103">iosLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="1647f-103">Create iosLobApp</span></span>

> <span data-ttu-id="1647f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1647f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1647f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1647f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1647f-106">Erstellt ein neues [iosLobApp](../resources/intune-apps-ioslobapp.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="1647f-106">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1647f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1647f-107">Prerequisites</span></span>
<span data-ttu-id="1647f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1647f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1647f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1647f-110">Permission type</span></span>|<span data-ttu-id="1647f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1647f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1647f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1647f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1647f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1647f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1647f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1647f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1647f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1647f-115">Not supported.</span></span>|
|<span data-ttu-id="1647f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1647f-116">Application</span></span>|<span data-ttu-id="1647f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1647f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1647f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1647f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1647f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1647f-119">Request headers</span></span>
|<span data-ttu-id="1647f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1647f-120">Header</span></span>|<span data-ttu-id="1647f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1647f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1647f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1647f-122">Authorization</span></span>|<span data-ttu-id="1647f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1647f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1647f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1647f-124">Accept</span></span>|<span data-ttu-id="1647f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1647f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1647f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1647f-126">Request body</span></span>
<span data-ttu-id="1647f-127">Geben Sie im Anforderungstext eine JSON-Darstellung des iosLobApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="1647f-127">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="1647f-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosLobApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1647f-128">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="1647f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1647f-129">Property</span></span>|<span data-ttu-id="1647f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1647f-130">Type</span></span>|<span data-ttu-id="1647f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1647f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1647f-132">id</span><span class="sxs-lookup"><span data-stu-id="1647f-132">id</span></span>|<span data-ttu-id="1647f-133">String</span><span class="sxs-lookup"><span data-stu-id="1647f-133">String</span></span>|<span data-ttu-id="1647f-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1647f-134">Key of the entity.</span></span> <span data-ttu-id="1647f-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1647f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1647f-136">displayName</span></span>|<span data-ttu-id="1647f-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1647f-137">String</span></span>|<span data-ttu-id="1647f-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="1647f-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1647f-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1647f-140">description</span><span class="sxs-lookup"><span data-stu-id="1647f-140">description</span></span>|<span data-ttu-id="1647f-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1647f-141">String</span></span>|<span data-ttu-id="1647f-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="1647f-142">The description of the app.</span></span> <span data-ttu-id="1647f-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1647f-144">publisher</span><span class="sxs-lookup"><span data-stu-id="1647f-144">publisher</span></span>|<span data-ttu-id="1647f-145">String</span><span class="sxs-lookup"><span data-stu-id="1647f-145">String</span></span>|<span data-ttu-id="1647f-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="1647f-146">The publisher of the app.</span></span> <span data-ttu-id="1647f-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1647f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1647f-148">largeIcon</span></span>|[<span data-ttu-id="1647f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1647f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1647f-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="1647f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1647f-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1647f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1647f-152">createdDateTime</span></span>|<span data-ttu-id="1647f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1647f-153">DateTimeOffset</span></span>|<span data-ttu-id="1647f-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="1647f-154">The date and time the app was created.</span></span> <span data-ttu-id="1647f-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1647f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1647f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="1647f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1647f-157">DateTimeOffset</span></span>|<span data-ttu-id="1647f-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="1647f-158">The date and time the app was last modified.</span></span> <span data-ttu-id="1647f-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1647f-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1647f-160">isFeatured</span></span>|<span data-ttu-id="1647f-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="1647f-161">Boolean</span></span>|<span data-ttu-id="1647f-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1647f-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1647f-163">privacyInformationUrl</span></span>|<span data-ttu-id="1647f-164">String</span><span class="sxs-lookup"><span data-stu-id="1647f-164">String</span></span>|<span data-ttu-id="1647f-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="1647f-165">The privacy statement Url.</span></span> <span data-ttu-id="1647f-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1647f-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1647f-167">informationUrl</span></span>|<span data-ttu-id="1647f-168">String</span><span class="sxs-lookup"><span data-stu-id="1647f-168">String</span></span>|<span data-ttu-id="1647f-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="1647f-169">The more information Url.</span></span> <span data-ttu-id="1647f-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1647f-171">owner</span><span class="sxs-lookup"><span data-stu-id="1647f-171">owner</span></span>|<span data-ttu-id="1647f-172">String</span><span class="sxs-lookup"><span data-stu-id="1647f-172">String</span></span>|<span data-ttu-id="1647f-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="1647f-173">The owner of the app.</span></span> <span data-ttu-id="1647f-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1647f-175">developer</span><span class="sxs-lookup"><span data-stu-id="1647f-175">developer</span></span>|<span data-ttu-id="1647f-176">String</span><span class="sxs-lookup"><span data-stu-id="1647f-176">String</span></span>|<span data-ttu-id="1647f-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="1647f-177">The developer of the app.</span></span> <span data-ttu-id="1647f-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1647f-179">notes</span><span class="sxs-lookup"><span data-stu-id="1647f-179">notes</span></span>|<span data-ttu-id="1647f-180">String</span><span class="sxs-lookup"><span data-stu-id="1647f-180">String</span></span>|<span data-ttu-id="1647f-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="1647f-181">Notes for the app.</span></span> <span data-ttu-id="1647f-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1647f-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="1647f-183">uploadState</span></span>|<span data-ttu-id="1647f-184">Int32</span><span class="sxs-lookup"><span data-stu-id="1647f-184">Int32</span></span>|<span data-ttu-id="1647f-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="1647f-185">The upload state.</span></span> <span data-ttu-id="1647f-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1647f-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="1647f-187">publishingState</span></span>|[<span data-ttu-id="1647f-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1647f-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1647f-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="1647f-189">The publishing state for the app.</span></span> <span data-ttu-id="1647f-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="1647f-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1647f-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="1647f-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1647f-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="1647f-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1647f-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1647f-193">isAssigned</span></span>|<span data-ttu-id="1647f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1647f-194">Boolean</span></span>|<span data-ttu-id="1647f-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="1647f-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1647f-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1647f-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="1647f-197">roleScopeTagIds</span></span>|<span data-ttu-id="1647f-198">String collection</span><span class="sxs-lookup"><span data-stu-id="1647f-198">String collection</span></span>|<span data-ttu-id="1647f-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="1647f-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1647f-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1647f-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1647f-201">committedContentVersion</span></span>|<span data-ttu-id="1647f-202">String</span><span class="sxs-lookup"><span data-stu-id="1647f-202">String</span></span>|<span data-ttu-id="1647f-203">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="1647f-203">The internal committed content version.</span></span> <span data-ttu-id="1647f-204">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1647f-205">fileName</span><span class="sxs-lookup"><span data-stu-id="1647f-205">fileName</span></span>|<span data-ttu-id="1647f-206">String</span><span class="sxs-lookup"><span data-stu-id="1647f-206">String</span></span>|<span data-ttu-id="1647f-207">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="1647f-207">The name of the main Lob application file.</span></span> <span data-ttu-id="1647f-208">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1647f-209">size</span><span class="sxs-lookup"><span data-stu-id="1647f-209">size</span></span>|<span data-ttu-id="1647f-210">Int64</span><span class="sxs-lookup"><span data-stu-id="1647f-210">Int64</span></span>|<span data-ttu-id="1647f-211">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="1647f-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="1647f-212">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="1647f-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1647f-213">bundleId</span><span class="sxs-lookup"><span data-stu-id="1647f-213">bundleId</span></span>|<span data-ttu-id="1647f-214">String</span><span class="sxs-lookup"><span data-stu-id="1647f-214">String</span></span>|<span data-ttu-id="1647f-215">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="1647f-215">The Identity Name.</span></span>|
|<span data-ttu-id="1647f-216">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="1647f-216">applicableDeviceType</span></span>|[<span data-ttu-id="1647f-217">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="1647f-217">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="1647f-218">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="1647f-218">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="1647f-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1647f-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1647f-220">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1647f-220">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="1647f-221">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="1647f-221">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="1647f-222">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1647f-222">expirationDateTime</span></span>|<span data-ttu-id="1647f-223">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1647f-223">DateTimeOffset</span></span>|<span data-ttu-id="1647f-224">Das Ablaufdatum.</span><span class="sxs-lookup"><span data-stu-id="1647f-224">The expiration time.</span></span>|
|<span data-ttu-id="1647f-225">versionNumber</span><span class="sxs-lookup"><span data-stu-id="1647f-225">versionNumber</span></span>|<span data-ttu-id="1647f-226">String</span><span class="sxs-lookup"><span data-stu-id="1647f-226">String</span></span>|<span data-ttu-id="1647f-227">Die Versionsnummer der branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="1647f-227">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1647f-228">buildNumber</span><span class="sxs-lookup"><span data-stu-id="1647f-228">buildNumber</span></span>|<span data-ttu-id="1647f-229">String</span><span class="sxs-lookup"><span data-stu-id="1647f-229">String</span></span>|<span data-ttu-id="1647f-230">Die Buildnummer der branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="1647f-230">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1647f-231">identityVersion</span><span class="sxs-lookup"><span data-stu-id="1647f-231">identityVersion</span></span>|<span data-ttu-id="1647f-232">String</span><span class="sxs-lookup"><span data-stu-id="1647f-232">String</span></span>|<span data-ttu-id="1647f-233">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="1647f-233">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="1647f-234">Antwort</span><span class="sxs-lookup"><span data-stu-id="1647f-234">Response</span></span>
<span data-ttu-id="1647f-235">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosLobApp](../resources/intune-apps-ioslobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1647f-235">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1647f-236">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1647f-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="1647f-237">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1647f-237">Request</span></span>
<span data-ttu-id="1647f-238">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1647f-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1364

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="1647f-239">Antwort</span><span class="sxs-lookup"><span data-stu-id="1647f-239">Response</span></span>
<span data-ttu-id="1647f-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1647f-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1536

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




