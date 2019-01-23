---
title: Erstellen von macOsVppApp
description: Erstellen eines neuen MacOsVppApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 64ab6fcec54beab2de2da6a5ac44f0a6b49d8ea6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430084"
---
# <a name="create-macosvppapp"></a><span data-ttu-id="c33f3-103">Erstellen von macOsVppApp</span><span class="sxs-lookup"><span data-stu-id="c33f3-103">Create macOsVppApp</span></span>

> <span data-ttu-id="c33f3-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c33f3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c33f3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c33f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c33f3-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c33f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c33f3-107">Erstellen eines neuen [MacOsVppApp](../resources/intune-apps-macosvppapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c33f3-107">Create a new [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c33f3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c33f3-108">Prerequisites</span></span>
<span data-ttu-id="c33f3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c33f3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c33f3-111">Permission type</span></span>|<span data-ttu-id="c33f3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c33f3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c33f3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c33f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c33f3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c33f3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c33f3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c33f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c33f3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c33f3-116">Not supported.</span></span>|
|<span data-ttu-id="c33f3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c33f3-117">Application</span></span>|<span data-ttu-id="c33f3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c33f3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c33f3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c33f3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c33f3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c33f3-120">Request headers</span></span>
|<span data-ttu-id="c33f3-121">Header</span><span class="sxs-lookup"><span data-stu-id="c33f3-121">Header</span></span>|<span data-ttu-id="c33f3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c33f3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c33f3-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c33f3-123">Authorization</span></span>|<span data-ttu-id="c33f3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c33f3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c33f3-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c33f3-125">Accept</span></span>|<span data-ttu-id="c33f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c33f3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c33f3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c33f3-127">Request body</span></span>
<span data-ttu-id="c33f3-128">Geben Sie im Textkörper Anforderung für das Objekt MacOsVppApp eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="c33f3-128">In the request body, supply a JSON representation for the macOsVppApp object.</span></span>

<span data-ttu-id="c33f3-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die MacOsVppApp erstellen.</span><span class="sxs-lookup"><span data-stu-id="c33f3-129">The following table shows the properties that are required when you create the macOsVppApp.</span></span>

|<span data-ttu-id="c33f3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c33f3-130">Property</span></span>|<span data-ttu-id="c33f3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c33f3-131">Type</span></span>|<span data-ttu-id="c33f3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c33f3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c33f3-133">id</span><span class="sxs-lookup"><span data-stu-id="c33f3-133">id</span></span>|<span data-ttu-id="c33f3-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c33f3-134">String</span></span>|<span data-ttu-id="c33f3-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c33f3-135">Key of the entity.</span></span> <span data-ttu-id="c33f3-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c33f3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c33f3-137">displayName</span></span>|<span data-ttu-id="c33f3-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c33f3-138">String</span></span>|<span data-ttu-id="c33f3-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="c33f3-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c33f3-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c33f3-141">description</span><span class="sxs-lookup"><span data-stu-id="c33f3-141">description</span></span>|<span data-ttu-id="c33f3-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c33f3-142">String</span></span>|<span data-ttu-id="c33f3-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="c33f3-143">The description of the app.</span></span> <span data-ttu-id="c33f3-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c33f3-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c33f3-145">publisher</span></span>|<span data-ttu-id="c33f3-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c33f3-146">String</span></span>|<span data-ttu-id="c33f3-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="c33f3-147">The publisher of the app.</span></span> <span data-ttu-id="c33f3-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c33f3-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c33f3-149">largeIcon</span></span>|[<span data-ttu-id="c33f3-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c33f3-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c33f3-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c33f3-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c33f3-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c33f3-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c33f3-153">createdDateTime</span></span>|<span data-ttu-id="c33f3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c33f3-154">DateTimeOffset</span></span>|<span data-ttu-id="c33f3-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="c33f3-155">The date and time the app was created.</span></span> <span data-ttu-id="c33f3-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c33f3-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c33f3-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c33f3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c33f3-158">DateTimeOffset</span></span>|<span data-ttu-id="c33f3-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="c33f3-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c33f3-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c33f3-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c33f3-161">isFeatured</span></span>|<span data-ttu-id="c33f3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c33f3-162">Boolean</span></span>|<span data-ttu-id="c33f3-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c33f3-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c33f3-164">privacyInformationUrl</span></span>|<span data-ttu-id="c33f3-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c33f3-165">String</span></span>|<span data-ttu-id="c33f3-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="c33f3-166">The privacy statement Url.</span></span> <span data-ttu-id="c33f3-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c33f3-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c33f3-168">informationUrl</span></span>|<span data-ttu-id="c33f3-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c33f3-169">String</span></span>|<span data-ttu-id="c33f3-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="c33f3-170">The more information Url.</span></span> <span data-ttu-id="c33f3-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c33f3-172">owner</span><span class="sxs-lookup"><span data-stu-id="c33f3-172">owner</span></span>|<span data-ttu-id="c33f3-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c33f3-173">String</span></span>|<span data-ttu-id="c33f3-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="c33f3-174">The owner of the app.</span></span> <span data-ttu-id="c33f3-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c33f3-176">developer</span><span class="sxs-lookup"><span data-stu-id="c33f3-176">developer</span></span>|<span data-ttu-id="c33f3-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c33f3-177">String</span></span>|<span data-ttu-id="c33f3-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="c33f3-178">The developer of the app.</span></span> <span data-ttu-id="c33f3-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c33f3-180">notes</span><span class="sxs-lookup"><span data-stu-id="c33f3-180">notes</span></span>|<span data-ttu-id="c33f3-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c33f3-181">String</span></span>|<span data-ttu-id="c33f3-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="c33f3-182">Notes for the app.</span></span> <span data-ttu-id="c33f3-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c33f3-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c33f3-184">uploadState</span></span>|<span data-ttu-id="c33f3-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c33f3-185">Int32</span></span>|<span data-ttu-id="c33f3-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="c33f3-186">The upload state.</span></span> <span data-ttu-id="c33f3-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c33f3-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="c33f3-188">publishingState</span></span>|[<span data-ttu-id="c33f3-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c33f3-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c33f3-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="c33f3-190">The publishing state for the app.</span></span> <span data-ttu-id="c33f3-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="c33f3-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c33f3-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c33f3-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="c33f3-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c33f3-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c33f3-194">isAssigned</span></span>|<span data-ttu-id="c33f3-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c33f3-195">Boolean</span></span>|<span data-ttu-id="c33f3-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="c33f3-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c33f3-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c33f3-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c33f3-198">roleScopeTagIds</span></span>|<span data-ttu-id="c33f3-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="c33f3-199">String collection</span></span>|<span data-ttu-id="c33f3-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="c33f3-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c33f3-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c33f3-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c33f3-202">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c33f3-202">usedLicenseCount</span></span>|<span data-ttu-id="c33f3-203">Int32</span><span class="sxs-lookup"><span data-stu-id="c33f3-203">Int32</span></span>|<span data-ttu-id="c33f3-204">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="c33f3-204">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="c33f3-205">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c33f3-205">totalLicenseCount</span></span>|<span data-ttu-id="c33f3-206">Int32</span><span class="sxs-lookup"><span data-stu-id="c33f3-206">Int32</span></span>|<span data-ttu-id="c33f3-207">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="c33f3-207">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="c33f3-208">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="c33f3-208">releaseDateTime</span></span>|<span data-ttu-id="c33f3-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c33f3-209">DateTimeOffset</span></span>|<span data-ttu-id="c33f3-210">Datum und Uhrzeit der Veröffentlichung der VPP-Anwendung.</span><span class="sxs-lookup"><span data-stu-id="c33f3-210">The VPP application release date and time.</span></span>|
|<span data-ttu-id="c33f3-211">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c33f3-211">appStoreUrl</span></span>|<span data-ttu-id="c33f3-212">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c33f3-212">String</span></span>|<span data-ttu-id="c33f3-213">Store-URL</span><span class="sxs-lookup"><span data-stu-id="c33f3-213">The store URL.</span></span>|
|<span data-ttu-id="c33f3-214">licensingType</span><span class="sxs-lookup"><span data-stu-id="c33f3-214">licensingType</span></span>|[<span data-ttu-id="c33f3-215">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="c33f3-215">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="c33f3-216">Unterstützter Lizenztyp</span><span class="sxs-lookup"><span data-stu-id="c33f3-216">The supported License Type.</span></span>|
|<span data-ttu-id="c33f3-217">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="c33f3-217">vppTokenOrganizationName</span></span>|<span data-ttu-id="c33f3-218">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c33f3-218">String</span></span>|<span data-ttu-id="c33f3-219">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="c33f3-219">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="c33f3-220">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="c33f3-220">vppTokenAccountType</span></span>|[<span data-ttu-id="c33f3-221">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="c33f3-221">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="c33f3-222">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="c33f3-222">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="c33f3-223">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="c33f3-223">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="c33f3-224">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="c33f3-224">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="c33f3-225">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="c33f3-225">vppTokenAppleId</span></span>|<span data-ttu-id="c33f3-226">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c33f3-226">String</span></span>|<span data-ttu-id="c33f3-227">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="c33f3-227">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="c33f3-228">bundleId</span><span class="sxs-lookup"><span data-stu-id="c33f3-228">bundleId</span></span>|<span data-ttu-id="c33f3-229">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c33f3-229">String</span></span>|<span data-ttu-id="c33f3-230">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="c33f3-230">The Identity Name.</span></span>|
|<span data-ttu-id="c33f3-231">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="c33f3-231">vppTokenId</span></span>|<span data-ttu-id="c33f3-232">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c33f3-232">String</span></span>|<span data-ttu-id="c33f3-233">Bezeichner des Tokens VPP diese app zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="c33f3-233">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="c33f3-234">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="c33f3-234">revokeLicenseActionResults</span></span>|<span data-ttu-id="c33f3-235">[MacOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c33f3-235">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="c33f3-236">Ergebnisse der widerrufen diese app-Lizenz Aktionen.</span><span class="sxs-lookup"><span data-stu-id="c33f3-236">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="c33f3-237">Antwort</span><span class="sxs-lookup"><span data-stu-id="c33f3-237">Response</span></span>
<span data-ttu-id="c33f3-238">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [MacOsVppApp](../resources/intune-apps-macosvppapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c33f3-238">If successful, this method returns a `201 Created` response code and a [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c33f3-239">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c33f3-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="c33f3-240">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c33f3-240">Request</span></span>
<span data-ttu-id="c33f3-241">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c33f3-241">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1842

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c33f3-242">Antwort</span><span class="sxs-lookup"><span data-stu-id="c33f3-242">Response</span></span>
<span data-ttu-id="c33f3-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c33f3-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2014

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
  "id": "10b95265-5265-10b9-6552-b9106552b910",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```




