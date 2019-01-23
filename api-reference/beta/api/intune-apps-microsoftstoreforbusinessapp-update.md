---
title: microsoftStoreForBusinessApp aktualisieren
description: Aktualisieren der Eigenschaften eines microsoftStoreForBusinessApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e5f2bee3e2cbbdd1f02bbd7a1779ea80b2340772
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417497"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="8d5bf-103">microsoftStoreForBusinessApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8d5bf-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="8d5bf-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8d5bf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d5bf-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d5bf-107">Aktualisieren der Eigenschaften eines [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-107">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d5bf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8d5bf-108">Prerequisites</span></span>
<span data-ttu-id="8d5bf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8d5bf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8d5bf-111">Permission type</span></span>|<span data-ttu-id="8d5bf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8d5bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d5bf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8d5bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d5bf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d5bf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8d5bf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8d5bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d5bf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d5bf-116">Not supported.</span></span>|
|<span data-ttu-id="8d5bf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8d5bf-117">Application</span></span>|<span data-ttu-id="8d5bf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d5bf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d5bf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d5bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8d5bf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8d5bf-120">Request headers</span></span>
|<span data-ttu-id="8d5bf-121">Header</span><span class="sxs-lookup"><span data-stu-id="8d5bf-121">Header</span></span>|<span data-ttu-id="8d5bf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8d5bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d5bf-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8d5bf-123">Authorization</span></span>|<span data-ttu-id="8d5bf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8d5bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d5bf-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8d5bf-125">Accept</span></span>|<span data-ttu-id="8d5bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d5bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d5bf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8d5bf-127">Request body</span></span>
<span data-ttu-id="8d5bf-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="8d5bf-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="8d5bf-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8d5bf-130">Property</span></span>|<span data-ttu-id="8d5bf-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8d5bf-131">Type</span></span>|<span data-ttu-id="8d5bf-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d5bf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d5bf-133">id</span><span class="sxs-lookup"><span data-stu-id="8d5bf-133">id</span></span>|<span data-ttu-id="8d5bf-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5bf-134">String</span></span>|<span data-ttu-id="8d5bf-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8d5bf-135">Key of the entity.</span></span> <span data-ttu-id="8d5bf-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5bf-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8d5bf-137">displayName</span></span>|<span data-ttu-id="8d5bf-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5bf-138">String</span></span>|<span data-ttu-id="8d5bf-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8d5bf-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5bf-141">description</span><span class="sxs-lookup"><span data-stu-id="8d5bf-141">description</span></span>|<span data-ttu-id="8d5bf-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5bf-142">String</span></span>|<span data-ttu-id="8d5bf-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-143">The description of the app.</span></span> <span data-ttu-id="8d5bf-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5bf-145">publisher</span><span class="sxs-lookup"><span data-stu-id="8d5bf-145">publisher</span></span>|<span data-ttu-id="8d5bf-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5bf-146">String</span></span>|<span data-ttu-id="8d5bf-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-147">The publisher of the app.</span></span> <span data-ttu-id="8d5bf-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5bf-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8d5bf-149">largeIcon</span></span>|[<span data-ttu-id="8d5bf-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8d5bf-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8d5bf-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8d5bf-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5bf-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d5bf-153">createdDateTime</span></span>|<span data-ttu-id="8d5bf-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d5bf-154">DateTimeOffset</span></span>|<span data-ttu-id="8d5bf-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-155">The date and time the app was created.</span></span> <span data-ttu-id="8d5bf-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5bf-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d5bf-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8d5bf-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d5bf-158">DateTimeOffset</span></span>|<span data-ttu-id="8d5bf-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8d5bf-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5bf-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8d5bf-161">isFeatured</span></span>|<span data-ttu-id="8d5bf-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d5bf-162">Boolean</span></span>|<span data-ttu-id="8d5bf-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5bf-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8d5bf-164">privacyInformationUrl</span></span>|<span data-ttu-id="8d5bf-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5bf-165">String</span></span>|<span data-ttu-id="8d5bf-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-166">The privacy statement Url.</span></span> <span data-ttu-id="8d5bf-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5bf-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8d5bf-168">informationUrl</span></span>|<span data-ttu-id="8d5bf-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5bf-169">String</span></span>|<span data-ttu-id="8d5bf-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-170">The more information Url.</span></span> <span data-ttu-id="8d5bf-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5bf-172">owner</span><span class="sxs-lookup"><span data-stu-id="8d5bf-172">owner</span></span>|<span data-ttu-id="8d5bf-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5bf-173">String</span></span>|<span data-ttu-id="8d5bf-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-174">The owner of the app.</span></span> <span data-ttu-id="8d5bf-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5bf-176">developer</span><span class="sxs-lookup"><span data-stu-id="8d5bf-176">developer</span></span>|<span data-ttu-id="8d5bf-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5bf-177">String</span></span>|<span data-ttu-id="8d5bf-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-178">The developer of the app.</span></span> <span data-ttu-id="8d5bf-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5bf-180">notes</span><span class="sxs-lookup"><span data-stu-id="8d5bf-180">notes</span></span>|<span data-ttu-id="8d5bf-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5bf-181">String</span></span>|<span data-ttu-id="8d5bf-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-182">Notes for the app.</span></span> <span data-ttu-id="8d5bf-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5bf-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8d5bf-184">uploadState</span></span>|<span data-ttu-id="8d5bf-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8d5bf-185">Int32</span></span>|<span data-ttu-id="8d5bf-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-186">The upload state.</span></span> <span data-ttu-id="8d5bf-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5bf-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="8d5bf-188">publishingState</span></span>|[<span data-ttu-id="8d5bf-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8d5bf-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8d5bf-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-190">The publishing state for the app.</span></span> <span data-ttu-id="8d5bf-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8d5bf-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8d5bf-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8d5bf-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8d5bf-194">isAssigned</span></span>|<span data-ttu-id="8d5bf-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d5bf-195">Boolean</span></span>|<span data-ttu-id="8d5bf-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8d5bf-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5bf-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8d5bf-198">roleScopeTagIds</span></span>|<span data-ttu-id="8d5bf-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="8d5bf-199">String collection</span></span>|<span data-ttu-id="8d5bf-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8d5bf-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5bf-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5bf-202">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8d5bf-202">usedLicenseCount</span></span>|<span data-ttu-id="8d5bf-203">Int32</span><span class="sxs-lookup"><span data-stu-id="8d5bf-203">Int32</span></span>|<span data-ttu-id="8d5bf-204">Die Anzahl von verwendeten Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-204">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="8d5bf-205">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8d5bf-205">totalLicenseCount</span></span>|<span data-ttu-id="8d5bf-206">Int32</span><span class="sxs-lookup"><span data-stu-id="8d5bf-206">Int32</span></span>|<span data-ttu-id="8d5bf-207">Die Gesamtzahl der Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-207">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="8d5bf-208">productKey</span><span class="sxs-lookup"><span data-stu-id="8d5bf-208">productKey</span></span>|<span data-ttu-id="8d5bf-209">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5bf-209">String</span></span>|<span data-ttu-id="8d5bf-210">Der Product Key der App</span><span class="sxs-lookup"><span data-stu-id="8d5bf-210">The app product key</span></span>|
|<span data-ttu-id="8d5bf-211">licenseType</span><span class="sxs-lookup"><span data-stu-id="8d5bf-211">licenseType</span></span>|[<span data-ttu-id="8d5bf-212">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="8d5bf-212">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="8d5bf-213">Der Typ des app-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-213">The app license type.</span></span> <span data-ttu-id="8d5bf-214">Mögliche Werte sind: `offline` und `online`.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-214">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="8d5bf-215">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="8d5bf-215">packageIdentityName</span></span>|<span data-ttu-id="8d5bf-216">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5bf-216">String</span></span>|<span data-ttu-id="8d5bf-217">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="8d5bf-217">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="8d5bf-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d5bf-218">Response</span></span>
<span data-ttu-id="8d5bf-219">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-219">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d5bf-220">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8d5bf-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d5bf-221">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d5bf-221">Request</span></span>
<span data-ttu-id="8d5bf-222">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 876

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="8d5bf-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d5bf-223">Response</span></span>
<span data-ttu-id="8d5bf-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d5bf-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1048

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```




