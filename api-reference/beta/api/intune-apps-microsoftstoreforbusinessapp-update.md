---
title: microsoftStoreForBusinessApp aktualisieren
description: Aktualisieren der Eigenschaften eines microsoftStoreForBusinessApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e063091b1fde917ffa7b15607e74d425d2ebc29d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960875"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="c6e96-103">microsoftStoreForBusinessApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c6e96-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="c6e96-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c6e96-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6e96-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c6e96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6e96-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c6e96-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6e96-107">Aktualisieren der Eigenschaften eines [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c6e96-107">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c6e96-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c6e96-108">Prerequisites</span></span>
<span data-ttu-id="c6e96-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6e96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6e96-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c6e96-111">Permission type</span></span>|<span data-ttu-id="c6e96-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c6e96-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6e96-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c6e96-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6e96-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6e96-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c6e96-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c6e96-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6e96-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c6e96-116">Not supported.</span></span>|
|<span data-ttu-id="c6e96-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c6e96-117">Application</span></span>|<span data-ttu-id="c6e96-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c6e96-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6e96-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6e96-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="c6e96-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c6e96-120">Request headers</span></span>
|<span data-ttu-id="c6e96-121">Header</span><span class="sxs-lookup"><span data-stu-id="c6e96-121">Header</span></span>|<span data-ttu-id="c6e96-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c6e96-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6e96-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6e96-123">Authorization</span></span>|<span data-ttu-id="c6e96-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c6e96-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6e96-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c6e96-125">Accept</span></span>|<span data-ttu-id="c6e96-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6e96-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6e96-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c6e96-127">Request body</span></span>
<span data-ttu-id="c6e96-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c6e96-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="c6e96-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c6e96-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="c6e96-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c6e96-130">Property</span></span>|<span data-ttu-id="c6e96-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c6e96-131">Type</span></span>|<span data-ttu-id="c6e96-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6e96-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6e96-133">id</span><span class="sxs-lookup"><span data-stu-id="c6e96-133">id</span></span>|<span data-ttu-id="c6e96-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6e96-134">String</span></span>|<span data-ttu-id="c6e96-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c6e96-135">Key of the entity.</span></span> <span data-ttu-id="c6e96-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6e96-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e96-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c6e96-137">displayName</span></span>|<span data-ttu-id="c6e96-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6e96-138">String</span></span>|<span data-ttu-id="c6e96-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="c6e96-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c6e96-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6e96-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e96-141">description</span><span class="sxs-lookup"><span data-stu-id="c6e96-141">description</span></span>|<span data-ttu-id="c6e96-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6e96-142">String</span></span>|<span data-ttu-id="c6e96-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="c6e96-143">The description of the app.</span></span> <span data-ttu-id="c6e96-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6e96-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e96-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c6e96-145">publisher</span></span>|<span data-ttu-id="c6e96-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6e96-146">String</span></span>|<span data-ttu-id="c6e96-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="c6e96-147">The publisher of the app.</span></span> <span data-ttu-id="c6e96-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6e96-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e96-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c6e96-149">largeIcon</span></span>|[<span data-ttu-id="c6e96-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c6e96-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c6e96-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c6e96-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c6e96-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6e96-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e96-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6e96-153">createdDateTime</span></span>|<span data-ttu-id="c6e96-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6e96-154">DateTimeOffset</span></span>|<span data-ttu-id="c6e96-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="c6e96-155">The date and time the app was created.</span></span> <span data-ttu-id="c6e96-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6e96-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e96-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6e96-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c6e96-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6e96-158">DateTimeOffset</span></span>|<span data-ttu-id="c6e96-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="c6e96-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c6e96-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6e96-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e96-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c6e96-161">isFeatured</span></span>|<span data-ttu-id="c6e96-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c6e96-162">Boolean</span></span>|<span data-ttu-id="c6e96-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6e96-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e96-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c6e96-164">privacyInformationUrl</span></span>|<span data-ttu-id="c6e96-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6e96-165">String</span></span>|<span data-ttu-id="c6e96-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="c6e96-166">The privacy statement Url.</span></span> <span data-ttu-id="c6e96-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6e96-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e96-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c6e96-168">informationUrl</span></span>|<span data-ttu-id="c6e96-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6e96-169">String</span></span>|<span data-ttu-id="c6e96-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="c6e96-170">The more information Url.</span></span> <span data-ttu-id="c6e96-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6e96-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e96-172">owner</span><span class="sxs-lookup"><span data-stu-id="c6e96-172">owner</span></span>|<span data-ttu-id="c6e96-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6e96-173">String</span></span>|<span data-ttu-id="c6e96-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="c6e96-174">The owner of the app.</span></span> <span data-ttu-id="c6e96-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6e96-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e96-176">developer</span><span class="sxs-lookup"><span data-stu-id="c6e96-176">developer</span></span>|<span data-ttu-id="c6e96-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6e96-177">String</span></span>|<span data-ttu-id="c6e96-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="c6e96-178">The developer of the app.</span></span> <span data-ttu-id="c6e96-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6e96-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e96-180">notes</span><span class="sxs-lookup"><span data-stu-id="c6e96-180">notes</span></span>|<span data-ttu-id="c6e96-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6e96-181">String</span></span>|<span data-ttu-id="c6e96-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="c6e96-182">Notes for the app.</span></span> <span data-ttu-id="c6e96-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6e96-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e96-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c6e96-184">uploadState</span></span>|<span data-ttu-id="c6e96-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c6e96-185">Int32</span></span>|<span data-ttu-id="c6e96-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="c6e96-186">The upload state.</span></span> <span data-ttu-id="c6e96-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6e96-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e96-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="c6e96-188">publishingState</span></span>|[<span data-ttu-id="c6e96-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c6e96-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c6e96-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="c6e96-190">The publishing state for the app.</span></span> <span data-ttu-id="c6e96-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="c6e96-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c6e96-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6e96-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c6e96-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="c6e96-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c6e96-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c6e96-194">usedLicenseCount</span></span>|<span data-ttu-id="c6e96-195">Int32</span><span class="sxs-lookup"><span data-stu-id="c6e96-195">Int32</span></span>|<span data-ttu-id="c6e96-196">Die Anzahl von verwendeten Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="c6e96-196">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="c6e96-197">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c6e96-197">totalLicenseCount</span></span>|<span data-ttu-id="c6e96-198">Int32</span><span class="sxs-lookup"><span data-stu-id="c6e96-198">Int32</span></span>|<span data-ttu-id="c6e96-199">Die Gesamtzahl der Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="c6e96-199">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="c6e96-200">productKey</span><span class="sxs-lookup"><span data-stu-id="c6e96-200">productKey</span></span>|<span data-ttu-id="c6e96-201">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6e96-201">String</span></span>|<span data-ttu-id="c6e96-202">Der Product Key der App</span><span class="sxs-lookup"><span data-stu-id="c6e96-202">The app product key</span></span>|
|<span data-ttu-id="c6e96-203">licenseType</span><span class="sxs-lookup"><span data-stu-id="c6e96-203">licenseType</span></span>|[<span data-ttu-id="c6e96-204">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="c6e96-204">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="c6e96-205">Der Typ des app-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="c6e96-205">The app license type.</span></span> <span data-ttu-id="c6e96-206">Mögliche Werte sind: `offline` und `online`.</span><span class="sxs-lookup"><span data-stu-id="c6e96-206">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="c6e96-207">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="c6e96-207">packageIdentityName</span></span>|<span data-ttu-id="c6e96-208">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6e96-208">String</span></span>|<span data-ttu-id="c6e96-209">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="c6e96-209">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="c6e96-210">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6e96-210">Response</span></span>
<span data-ttu-id="c6e96-211">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c6e96-211">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6e96-212">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c6e96-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6e96-213">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6e96-213">Request</span></span>
<span data-ttu-id="c6e96-214">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c6e96-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 788

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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="c6e96-215">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6e96-215">Response</span></span>
<span data-ttu-id="c6e96-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c6e96-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 963

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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```





