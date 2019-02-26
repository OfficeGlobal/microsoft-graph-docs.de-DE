---
title: AndroidLobApp aktualisieren
description: Aktualisieren der Eigenschaften eines androidLobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 101374a08b2ed6c74ad528d5ac5391b23ce64d54
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175409"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="3549d-103">AndroidLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3549d-103">Update androidLobApp</span></span>

> <span data-ttu-id="3549d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3549d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3549d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3549d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3549d-106">Aktualisieren der Eigenschaften eines [androidLobApp](../resources/intune-apps-androidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3549d-106">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3549d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3549d-107">Prerequisites</span></span>
<span data-ttu-id="3549d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3549d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3549d-110">Permission type</span></span>|<span data-ttu-id="3549d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3549d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3549d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3549d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3549d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3549d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3549d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3549d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3549d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3549d-115">Not supported.</span></span>|
|<span data-ttu-id="3549d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3549d-116">Application</span></span>|<span data-ttu-id="3549d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3549d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3549d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3549d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="3549d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3549d-119">Request headers</span></span>
|<span data-ttu-id="3549d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3549d-120">Header</span></span>|<span data-ttu-id="3549d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3549d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3549d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3549d-122">Authorization</span></span>|<span data-ttu-id="3549d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3549d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3549d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3549d-124">Accept</span></span>|<span data-ttu-id="3549d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3549d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3549d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3549d-126">Request body</span></span>
<span data-ttu-id="3549d-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidLobApp](../resources/intune-apps-androidlobapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="3549d-127">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="3549d-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidLobApp](../resources/intune-apps-androidlobapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="3549d-128">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="3549d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3549d-129">Property</span></span>|<span data-ttu-id="3549d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="3549d-130">Type</span></span>|<span data-ttu-id="3549d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3549d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3549d-132">id</span><span class="sxs-lookup"><span data-stu-id="3549d-132">id</span></span>|<span data-ttu-id="3549d-133">string</span><span class="sxs-lookup"><span data-stu-id="3549d-133">String</span></span>|<span data-ttu-id="3549d-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3549d-134">Key of the entity.</span></span> <span data-ttu-id="3549d-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3549d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3549d-136">displayName</span></span>|<span data-ttu-id="3549d-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3549d-137">String</span></span>|<span data-ttu-id="3549d-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="3549d-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3549d-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3549d-140">description</span><span class="sxs-lookup"><span data-stu-id="3549d-140">description</span></span>|<span data-ttu-id="3549d-141">String</span><span class="sxs-lookup"><span data-stu-id="3549d-141">String</span></span>|<span data-ttu-id="3549d-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="3549d-142">The description of the app.</span></span> <span data-ttu-id="3549d-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3549d-144">publisher</span><span class="sxs-lookup"><span data-stu-id="3549d-144">publisher</span></span>|<span data-ttu-id="3549d-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3549d-145">String</span></span>|<span data-ttu-id="3549d-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="3549d-146">The publisher of the app.</span></span> <span data-ttu-id="3549d-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3549d-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3549d-148">largeIcon</span></span>|[<span data-ttu-id="3549d-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3549d-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3549d-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="3549d-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3549d-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3549d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3549d-152">createdDateTime</span></span>|<span data-ttu-id="3549d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3549d-153">DateTimeOffset</span></span>|<span data-ttu-id="3549d-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="3549d-154">The date and time the app was created.</span></span> <span data-ttu-id="3549d-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3549d-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3549d-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3549d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3549d-157">DateTimeOffset</span></span>|<span data-ttu-id="3549d-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="3549d-158">The date and time the app was last modified.</span></span> <span data-ttu-id="3549d-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3549d-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3549d-160">isFeatured</span></span>|<span data-ttu-id="3549d-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3549d-161">Boolean</span></span>|<span data-ttu-id="3549d-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3549d-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3549d-163">privacyInformationUrl</span></span>|<span data-ttu-id="3549d-164">String</span><span class="sxs-lookup"><span data-stu-id="3549d-164">String</span></span>|<span data-ttu-id="3549d-165">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="3549d-165">The privacy statement Url.</span></span> <span data-ttu-id="3549d-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3549d-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3549d-167">informationUrl</span></span>|<span data-ttu-id="3549d-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3549d-168">String</span></span>|<span data-ttu-id="3549d-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="3549d-169">The more information Url.</span></span> <span data-ttu-id="3549d-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3549d-171">owner</span><span class="sxs-lookup"><span data-stu-id="3549d-171">owner</span></span>|<span data-ttu-id="3549d-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3549d-172">String</span></span>|<span data-ttu-id="3549d-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="3549d-173">The owner of the app.</span></span> <span data-ttu-id="3549d-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3549d-175">developer</span><span class="sxs-lookup"><span data-stu-id="3549d-175">developer</span></span>|<span data-ttu-id="3549d-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3549d-176">String</span></span>|<span data-ttu-id="3549d-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="3549d-177">The developer of the app.</span></span> <span data-ttu-id="3549d-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3549d-179">notes</span><span class="sxs-lookup"><span data-stu-id="3549d-179">notes</span></span>|<span data-ttu-id="3549d-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3549d-180">String</span></span>|<span data-ttu-id="3549d-181">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="3549d-181">Notes for the app.</span></span> <span data-ttu-id="3549d-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3549d-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="3549d-183">uploadState</span></span>|<span data-ttu-id="3549d-184">Int32</span><span class="sxs-lookup"><span data-stu-id="3549d-184">Int32</span></span>|<span data-ttu-id="3549d-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="3549d-185">The upload state.</span></span> <span data-ttu-id="3549d-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3549d-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="3549d-187">publishingState</span></span>|[<span data-ttu-id="3549d-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3549d-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3549d-189">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="3549d-189">The publishing state for the app.</span></span> <span data-ttu-id="3549d-190">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="3549d-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3549d-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="3549d-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3549d-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="3549d-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3549d-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3549d-193">isAssigned</span></span>|<span data-ttu-id="3549d-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="3549d-194">Boolean</span></span>|<span data-ttu-id="3549d-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="3549d-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="3549d-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3549d-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="3549d-197">roleScopeTagIds</span></span>|<span data-ttu-id="3549d-198">String collection</span><span class="sxs-lookup"><span data-stu-id="3549d-198">String collection</span></span>|<span data-ttu-id="3549d-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="3549d-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="3549d-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3549d-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="3549d-201">committedContentVersion</span></span>|<span data-ttu-id="3549d-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3549d-202">String</span></span>|<span data-ttu-id="3549d-203">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="3549d-203">The internal committed content version.</span></span> <span data-ttu-id="3549d-204">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3549d-205">fileName</span><span class="sxs-lookup"><span data-stu-id="3549d-205">fileName</span></span>|<span data-ttu-id="3549d-206">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3549d-206">String</span></span>|<span data-ttu-id="3549d-207">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="3549d-207">The name of the main Lob application file.</span></span> <span data-ttu-id="3549d-208">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3549d-209">size</span><span class="sxs-lookup"><span data-stu-id="3549d-209">size</span></span>|<span data-ttu-id="3549d-210">Int64</span><span class="sxs-lookup"><span data-stu-id="3549d-210">Int64</span></span>|<span data-ttu-id="3549d-211">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="3549d-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="3549d-212">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3549d-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3549d-213">packageId</span><span class="sxs-lookup"><span data-stu-id="3549d-213">packageId</span></span>|<span data-ttu-id="3549d-214">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3549d-214">String</span></span>|<span data-ttu-id="3549d-215">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="3549d-215">The package identifier.</span></span>|
|<span data-ttu-id="3549d-216">identityName</span><span class="sxs-lookup"><span data-stu-id="3549d-216">identityName</span></span>|<span data-ttu-id="3549d-217">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3549d-217">String</span></span>|<span data-ttu-id="3549d-218">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="3549d-218">The Identity Name.</span></span>|
|<span data-ttu-id="3549d-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3549d-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3549d-220">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3549d-220">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="3549d-221">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="3549d-221">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="3549d-222">versionName</span><span class="sxs-lookup"><span data-stu-id="3549d-222">versionName</span></span>|<span data-ttu-id="3549d-223">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3549d-223">String</span></span>|<span data-ttu-id="3549d-224">Der Versionsname der branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="3549d-224">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3549d-225">versionCode</span><span class="sxs-lookup"><span data-stu-id="3549d-225">versionCode</span></span>|<span data-ttu-id="3549d-226">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3549d-226">String</span></span>|<span data-ttu-id="3549d-227">Der Versionscode der branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="3549d-227">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3549d-228">identityVersion</span><span class="sxs-lookup"><span data-stu-id="3549d-228">identityVersion</span></span>|<span data-ttu-id="3549d-229">String</span><span class="sxs-lookup"><span data-stu-id="3549d-229">String</span></span>|<span data-ttu-id="3549d-230">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="3549d-230">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="3549d-231">Antwort</span><span class="sxs-lookup"><span data-stu-id="3549d-231">Response</span></span>
<span data-ttu-id="3549d-232">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [androidLobApp](../resources/intune-apps-androidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3549d-232">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3549d-233">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3549d-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="3549d-234">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3549d-234">Request</span></span>
<span data-ttu-id="3549d-235">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3549d-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1386

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

### <a name="response"></a><span data-ttu-id="3549d-236">Antwort</span><span class="sxs-lookup"><span data-stu-id="3549d-236">Response</span></span>
<span data-ttu-id="3549d-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3549d-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1558

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




