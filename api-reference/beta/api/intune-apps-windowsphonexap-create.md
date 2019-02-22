---
title: WindowsPhoneXAP erstellen
description: Erstellen eines neuen windowsPhoneXAP-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8bc66deefc23cc0f1b02dcbd927060d3fdb8cb16
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154334"
---
# <a name="create-windowsphonexap"></a><span data-ttu-id="2f5ff-103">WindowsPhoneXAP erstellen</span><span class="sxs-lookup"><span data-stu-id="2f5ff-103">Create windowsPhoneXAP</span></span>

> <span data-ttu-id="2f5ff-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f5ff-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f5ff-106">Erstellen eines neuen [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-106">Create a new [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f5ff-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2f5ff-107">Prerequisites</span></span>
<span data-ttu-id="2f5ff-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2f5ff-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f5ff-110">Permission type</span></span>|<span data-ttu-id="2f5ff-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f5ff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f5ff-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f5ff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f5ff-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f5ff-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2f5ff-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f5ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f5ff-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f5ff-115">Not supported.</span></span>|
|<span data-ttu-id="2f5ff-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f5ff-116">Application</span></span>|<span data-ttu-id="2f5ff-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f5ff-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f5ff-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f5ff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2f5ff-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f5ff-119">Request headers</span></span>
|<span data-ttu-id="2f5ff-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2f5ff-120">Header</span></span>|<span data-ttu-id="2f5ff-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2f5ff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f5ff-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f5ff-122">Authorization</span></span>|<span data-ttu-id="2f5ff-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2f5ff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f5ff-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2f5ff-124">Accept</span></span>|<span data-ttu-id="2f5ff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f5ff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f5ff-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f5ff-126">Request body</span></span>
<span data-ttu-id="2f5ff-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsPhoneXAP-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-127">In the request body, supply a JSON representation for the windowsPhoneXAP object.</span></span>

<span data-ttu-id="2f5ff-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsPhoneXAP erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-128">The following table shows the properties that are required when you create the windowsPhoneXAP.</span></span>

|<span data-ttu-id="2f5ff-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2f5ff-129">Property</span></span>|<span data-ttu-id="2f5ff-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2f5ff-130">Type</span></span>|<span data-ttu-id="2f5ff-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f5ff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f5ff-132">id</span><span class="sxs-lookup"><span data-stu-id="2f5ff-132">id</span></span>|<span data-ttu-id="2f5ff-133">string</span><span class="sxs-lookup"><span data-stu-id="2f5ff-133">String</span></span>|<span data-ttu-id="2f5ff-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2f5ff-134">Key of the entity.</span></span> <span data-ttu-id="2f5ff-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f5ff-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2f5ff-136">displayName</span></span>|<span data-ttu-id="2f5ff-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2f5ff-137">String</span></span>|<span data-ttu-id="2f5ff-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2f5ff-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f5ff-140">description</span><span class="sxs-lookup"><span data-stu-id="2f5ff-140">description</span></span>|<span data-ttu-id="2f5ff-141">String</span><span class="sxs-lookup"><span data-stu-id="2f5ff-141">String</span></span>|<span data-ttu-id="2f5ff-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-142">The description of the app.</span></span> <span data-ttu-id="2f5ff-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f5ff-144">publisher</span><span class="sxs-lookup"><span data-stu-id="2f5ff-144">publisher</span></span>|<span data-ttu-id="2f5ff-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2f5ff-145">String</span></span>|<span data-ttu-id="2f5ff-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-146">The publisher of the app.</span></span> <span data-ttu-id="2f5ff-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f5ff-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2f5ff-148">largeIcon</span></span>|[<span data-ttu-id="2f5ff-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2f5ff-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2f5ff-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2f5ff-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f5ff-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f5ff-152">createdDateTime</span></span>|<span data-ttu-id="2f5ff-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f5ff-153">DateTimeOffset</span></span>|<span data-ttu-id="2f5ff-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-154">The date and time the app was created.</span></span> <span data-ttu-id="2f5ff-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f5ff-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f5ff-156">lastModifiedDateTime</span></span>|<span data-ttu-id="2f5ff-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f5ff-157">DateTimeOffset</span></span>|<span data-ttu-id="2f5ff-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-158">The date and time the app was last modified.</span></span> <span data-ttu-id="2f5ff-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f5ff-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2f5ff-160">isFeatured</span></span>|<span data-ttu-id="2f5ff-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2f5ff-161">Boolean</span></span>|<span data-ttu-id="2f5ff-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f5ff-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2f5ff-163">privacyInformationUrl</span></span>|<span data-ttu-id="2f5ff-164">String</span><span class="sxs-lookup"><span data-stu-id="2f5ff-164">String</span></span>|<span data-ttu-id="2f5ff-165">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-165">The privacy statement Url.</span></span> <span data-ttu-id="2f5ff-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f5ff-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2f5ff-167">informationUrl</span></span>|<span data-ttu-id="2f5ff-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2f5ff-168">String</span></span>|<span data-ttu-id="2f5ff-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-169">The more information Url.</span></span> <span data-ttu-id="2f5ff-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f5ff-171">owner</span><span class="sxs-lookup"><span data-stu-id="2f5ff-171">owner</span></span>|<span data-ttu-id="2f5ff-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2f5ff-172">String</span></span>|<span data-ttu-id="2f5ff-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-173">The owner of the app.</span></span> <span data-ttu-id="2f5ff-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f5ff-175">developer</span><span class="sxs-lookup"><span data-stu-id="2f5ff-175">developer</span></span>|<span data-ttu-id="2f5ff-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2f5ff-176">String</span></span>|<span data-ttu-id="2f5ff-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-177">The developer of the app.</span></span> <span data-ttu-id="2f5ff-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f5ff-179">notes</span><span class="sxs-lookup"><span data-stu-id="2f5ff-179">notes</span></span>|<span data-ttu-id="2f5ff-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2f5ff-180">String</span></span>|<span data-ttu-id="2f5ff-181">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-181">Notes for the app.</span></span> <span data-ttu-id="2f5ff-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f5ff-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="2f5ff-183">uploadState</span></span>|<span data-ttu-id="2f5ff-184">Int32</span><span class="sxs-lookup"><span data-stu-id="2f5ff-184">Int32</span></span>|<span data-ttu-id="2f5ff-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-185">The upload state.</span></span> <span data-ttu-id="2f5ff-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f5ff-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="2f5ff-187">publishingState</span></span>|[<span data-ttu-id="2f5ff-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2f5ff-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2f5ff-189">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-189">The publishing state for the app.</span></span> <span data-ttu-id="2f5ff-190">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2f5ff-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2f5ff-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2f5ff-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2f5ff-193">isAssigned</span></span>|<span data-ttu-id="2f5ff-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f5ff-194">Boolean</span></span>|<span data-ttu-id="2f5ff-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="2f5ff-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f5ff-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="2f5ff-197">roleScopeTagIds</span></span>|<span data-ttu-id="2f5ff-198">String collection</span><span class="sxs-lookup"><span data-stu-id="2f5ff-198">String collection</span></span>|<span data-ttu-id="2f5ff-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="2f5ff-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f5ff-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="2f5ff-201">committedContentVersion</span></span>|<span data-ttu-id="2f5ff-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2f5ff-202">String</span></span>|<span data-ttu-id="2f5ff-203">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-203">The internal committed content version.</span></span> <span data-ttu-id="2f5ff-204">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2f5ff-205">fileName</span><span class="sxs-lookup"><span data-stu-id="2f5ff-205">fileName</span></span>|<span data-ttu-id="2f5ff-206">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2f5ff-206">String</span></span>|<span data-ttu-id="2f5ff-207">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-207">The name of the main Lob application file.</span></span> <span data-ttu-id="2f5ff-208">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2f5ff-209">size</span><span class="sxs-lookup"><span data-stu-id="2f5ff-209">size</span></span>|<span data-ttu-id="2f5ff-210">Int64</span><span class="sxs-lookup"><span data-stu-id="2f5ff-210">Int64</span></span>|<span data-ttu-id="2f5ff-211">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="2f5ff-212">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f5ff-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2f5ff-213">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2f5ff-213">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2f5ff-214">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2f5ff-214">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="2f5ff-215">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-215">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="2f5ff-216">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="2f5ff-216">productIdentifier</span></span>|<span data-ttu-id="2f5ff-217">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2f5ff-217">String</span></span>|<span data-ttu-id="2f5ff-218">Der Product Identifier.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-218">The Product Identifier.</span></span>|
|<span data-ttu-id="2f5ff-219">identityVersion</span><span class="sxs-lookup"><span data-stu-id="2f5ff-219">identityVersion</span></span>|<span data-ttu-id="2f5ff-220">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2f5ff-220">String</span></span>|<span data-ttu-id="2f5ff-221">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="2f5ff-221">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="2f5ff-222">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f5ff-222">Response</span></span>
<span data-ttu-id="2f5ff-223">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-223">If successful, this method returns a `201 Created` response code and a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f5ff-224">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f5ff-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f5ff-225">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f5ff-225">Request</span></span>
<span data-ttu-id="2f5ff-226">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1164

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
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
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="2f5ff-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f5ff-227">Response</span></span>
<span data-ttu-id="2f5ff-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f5ff-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1336

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```




