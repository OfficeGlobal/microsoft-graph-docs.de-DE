---
title: Erstellen von „windowsMobileMSI“
description: Erstellen eines neuen windowsMobileMSI-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9e9ba8c10d80ea75799046b951678d34bf88a2d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966376"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="3ded0-103">Erstellen von „windowsMobileMSI“</span><span class="sxs-lookup"><span data-stu-id="3ded0-103">Create windowsMobileMSI</span></span>

> <span data-ttu-id="3ded0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3ded0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ded0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3ded0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ded0-106">Erstellen eines neuen [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3ded0-106">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ded0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3ded0-107">Prerequisites</span></span>
<span data-ttu-id="3ded0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ded0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ded0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3ded0-110">Permission type</span></span>|<span data-ttu-id="3ded0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3ded0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ded0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3ded0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ded0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ded0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3ded0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3ded0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ded0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ded0-115">Not supported.</span></span>|
|<span data-ttu-id="3ded0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3ded0-116">Application</span></span>|<span data-ttu-id="3ded0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ded0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ded0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ded0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3ded0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3ded0-119">Request headers</span></span>
|<span data-ttu-id="3ded0-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3ded0-120">Header</span></span>|<span data-ttu-id="3ded0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3ded0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ded0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ded0-122">Authorization</span></span>|<span data-ttu-id="3ded0-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3ded0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ded0-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3ded0-124">Accept</span></span>|<span data-ttu-id="3ded0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ded0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ded0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3ded0-126">Request body</span></span>
<span data-ttu-id="3ded0-127">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsMobileMSI-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3ded0-127">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="3ded0-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsMobileMSI erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3ded0-128">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="3ded0-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3ded0-129">Property</span></span>|<span data-ttu-id="3ded0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="3ded0-130">Type</span></span>|<span data-ttu-id="3ded0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ded0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ded0-132">id</span><span class="sxs-lookup"><span data-stu-id="3ded0-132">id</span></span>|<span data-ttu-id="3ded0-133">String</span><span class="sxs-lookup"><span data-stu-id="3ded0-133">String</span></span>|<span data-ttu-id="3ded0-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3ded0-134">Key of the entity.</span></span> <span data-ttu-id="3ded0-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ded0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3ded0-136">displayName</span></span>|<span data-ttu-id="3ded0-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3ded0-137">String</span></span>|<span data-ttu-id="3ded0-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="3ded0-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3ded0-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ded0-140">description</span><span class="sxs-lookup"><span data-stu-id="3ded0-140">description</span></span>|<span data-ttu-id="3ded0-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3ded0-141">String</span></span>|<span data-ttu-id="3ded0-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="3ded0-142">The description of the app.</span></span> <span data-ttu-id="3ded0-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ded0-144">publisher</span><span class="sxs-lookup"><span data-stu-id="3ded0-144">publisher</span></span>|<span data-ttu-id="3ded0-145">String</span><span class="sxs-lookup"><span data-stu-id="3ded0-145">String</span></span>|<span data-ttu-id="3ded0-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="3ded0-146">The publisher of the app.</span></span> <span data-ttu-id="3ded0-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ded0-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3ded0-148">largeIcon</span></span>|[<span data-ttu-id="3ded0-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3ded0-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3ded0-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="3ded0-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3ded0-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ded0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ded0-152">createdDateTime</span></span>|<span data-ttu-id="3ded0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ded0-153">DateTimeOffset</span></span>|<span data-ttu-id="3ded0-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="3ded0-154">The date and time the app was created.</span></span> <span data-ttu-id="3ded0-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ded0-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ded0-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3ded0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ded0-157">DateTimeOffset</span></span>|<span data-ttu-id="3ded0-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="3ded0-158">The date and time the app was last modified.</span></span> <span data-ttu-id="3ded0-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ded0-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3ded0-160">isFeatured</span></span>|<span data-ttu-id="3ded0-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3ded0-161">Boolean</span></span>|<span data-ttu-id="3ded0-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ded0-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3ded0-163">privacyInformationUrl</span></span>|<span data-ttu-id="3ded0-164">String</span><span class="sxs-lookup"><span data-stu-id="3ded0-164">String</span></span>|<span data-ttu-id="3ded0-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="3ded0-165">The privacy statement Url.</span></span> <span data-ttu-id="3ded0-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ded0-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3ded0-167">informationUrl</span></span>|<span data-ttu-id="3ded0-168">String</span><span class="sxs-lookup"><span data-stu-id="3ded0-168">String</span></span>|<span data-ttu-id="3ded0-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="3ded0-169">The more information Url.</span></span> <span data-ttu-id="3ded0-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ded0-171">owner</span><span class="sxs-lookup"><span data-stu-id="3ded0-171">owner</span></span>|<span data-ttu-id="3ded0-172">String</span><span class="sxs-lookup"><span data-stu-id="3ded0-172">String</span></span>|<span data-ttu-id="3ded0-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="3ded0-173">The owner of the app.</span></span> <span data-ttu-id="3ded0-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ded0-175">developer</span><span class="sxs-lookup"><span data-stu-id="3ded0-175">developer</span></span>|<span data-ttu-id="3ded0-176">String</span><span class="sxs-lookup"><span data-stu-id="3ded0-176">String</span></span>|<span data-ttu-id="3ded0-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="3ded0-177">The developer of the app.</span></span> <span data-ttu-id="3ded0-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ded0-179">notes</span><span class="sxs-lookup"><span data-stu-id="3ded0-179">notes</span></span>|<span data-ttu-id="3ded0-180">String</span><span class="sxs-lookup"><span data-stu-id="3ded0-180">String</span></span>|<span data-ttu-id="3ded0-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="3ded0-181">Notes for the app.</span></span> <span data-ttu-id="3ded0-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ded0-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="3ded0-183">uploadState</span></span>|<span data-ttu-id="3ded0-184">Int32</span><span class="sxs-lookup"><span data-stu-id="3ded0-184">Int32</span></span>|<span data-ttu-id="3ded0-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="3ded0-185">The upload state.</span></span> <span data-ttu-id="3ded0-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ded0-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="3ded0-187">publishingState</span></span>|[<span data-ttu-id="3ded0-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3ded0-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3ded0-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="3ded0-189">The publishing state for the app.</span></span> <span data-ttu-id="3ded0-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="3ded0-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3ded0-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="3ded0-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3ded0-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="3ded0-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3ded0-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3ded0-193">isAssigned</span></span>|<span data-ttu-id="3ded0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ded0-194">Boolean</span></span>|<span data-ttu-id="3ded0-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="3ded0-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="3ded0-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ded0-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="3ded0-197">roleScopeTagIds</span></span>|<span data-ttu-id="3ded0-198">String collection</span><span class="sxs-lookup"><span data-stu-id="3ded0-198">String collection</span></span>|<span data-ttu-id="3ded0-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="3ded0-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="3ded0-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ded0-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="3ded0-201">committedContentVersion</span></span>|<span data-ttu-id="3ded0-202">String</span><span class="sxs-lookup"><span data-stu-id="3ded0-202">String</span></span>|<span data-ttu-id="3ded0-203">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="3ded0-203">The internal committed content version.</span></span> <span data-ttu-id="3ded0-204">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3ded0-205">fileName</span><span class="sxs-lookup"><span data-stu-id="3ded0-205">fileName</span></span>|<span data-ttu-id="3ded0-206">String</span><span class="sxs-lookup"><span data-stu-id="3ded0-206">String</span></span>|<span data-ttu-id="3ded0-207">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="3ded0-207">The name of the main Lob application file.</span></span> <span data-ttu-id="3ded0-208">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3ded0-209">size</span><span class="sxs-lookup"><span data-stu-id="3ded0-209">size</span></span>|<span data-ttu-id="3ded0-210">Int64</span><span class="sxs-lookup"><span data-stu-id="3ded0-210">Int64</span></span>|<span data-ttu-id="3ded0-211">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="3ded0-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="3ded0-212">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ded0-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3ded0-213">commandLine</span><span class="sxs-lookup"><span data-stu-id="3ded0-213">commandLine</span></span>|<span data-ttu-id="3ded0-214">String</span><span class="sxs-lookup"><span data-stu-id="3ded0-214">String</span></span>|<span data-ttu-id="3ded0-215">Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="3ded0-215">The command line.</span></span>|
|<span data-ttu-id="3ded0-216">productCode</span><span class="sxs-lookup"><span data-stu-id="3ded0-216">productCode</span></span>|<span data-ttu-id="3ded0-217">String</span><span class="sxs-lookup"><span data-stu-id="3ded0-217">String</span></span>|<span data-ttu-id="3ded0-218">Produktcode</span><span class="sxs-lookup"><span data-stu-id="3ded0-218">The product code.</span></span>|
|<span data-ttu-id="3ded0-219">productVersion</span><span class="sxs-lookup"><span data-stu-id="3ded0-219">productVersion</span></span>|<span data-ttu-id="3ded0-220">String</span><span class="sxs-lookup"><span data-stu-id="3ded0-220">String</span></span>|<span data-ttu-id="3ded0-221">Produktversion der branchenspezifischen Windows Mobile-MSI-App.</span><span class="sxs-lookup"><span data-stu-id="3ded0-221">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3ded0-222">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="3ded0-222">ignoreVersionDetection</span></span>|<span data-ttu-id="3ded0-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ded0-223">Boolean</span></span>|<span data-ttu-id="3ded0-224">Boolescher Wert, der steuert, ob nach der Installation der App auf einem Gerät die App-Version zur Erkennung der App verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="3ded0-224">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="3ded0-225">Setzen Sie diese Eigenschaft auf „true“ bei branchenspezifischen Windows Mobile-MSI-Apps, die sich selbstständig aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="3ded0-225">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="3ded0-226">identityVersion</span><span class="sxs-lookup"><span data-stu-id="3ded0-226">identityVersion</span></span>|<span data-ttu-id="3ded0-227">String</span><span class="sxs-lookup"><span data-stu-id="3ded0-227">String</span></span>|<span data-ttu-id="3ded0-228">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="3ded0-228">The identity version.</span></span>|
|<span data-ttu-id="3ded0-229">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="3ded0-229">useDeviceContext</span></span>|<span data-ttu-id="3ded0-230">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3ded0-230">Boolean</span></span>|<span data-ttu-id="3ded0-231">Gibt an, ob eine MSI im Gerätekontext installiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="3ded0-231">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="3ded0-232">Wenn true, wird die APP für alle Benutzer installiert.</span><span class="sxs-lookup"><span data-stu-id="3ded0-232">If true, app will be installed for all users.</span></span> <span data-ttu-id="3ded0-233">Wenn false, wird die APP pro Benutzer installiert.</span><span class="sxs-lookup"><span data-stu-id="3ded0-233">If false, app will be installed per-user.</span></span> <span data-ttu-id="3ded0-234">Wenn NULL, verwendet der Dienst den standardmäßigen Installations Kontext des MSI-Pakets.</span><span class="sxs-lookup"><span data-stu-id="3ded0-234">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="3ded0-235">Bei einem MSI mit zwei Modus ist dieser Standardwert pro Benutzer.</span><span class="sxs-lookup"><span data-stu-id="3ded0-235">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="3ded0-236">Kann nicht für nicht-Dual-Modus-apps festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="3ded0-236">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="3ded0-237">Nach der erstmaligen Erstellung der Anwendung kann nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="3ded0-237">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="3ded0-238">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ded0-238">Response</span></span>
<span data-ttu-id="3ded0-239">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3ded0-239">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ded0-240">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3ded0-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ded0-241">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ded0-241">Request</span></span>
<span data-ttu-id="3ded0-242">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3ded0-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1039

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="3ded0-243">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ded0-243">Response</span></span>
<span data-ttu-id="3ded0-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3ded0-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1211

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```




