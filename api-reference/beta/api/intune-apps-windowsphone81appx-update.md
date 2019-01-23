---
title: WindowsPhone81AppX aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windowsPhone81AppX-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 702fb466edb8437f1455688dc6493d9fbd163e59
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401201"
---
# <a name="update-windowsphone81appx"></a><span data-ttu-id="5c25b-103">WindowsPhone81AppX aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5c25b-103">Update windowsPhone81AppX</span></span>

> <span data-ttu-id="5c25b-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5c25b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5c25b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5c25b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c25b-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5c25b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c25b-107">Aktualisieren Sie die Eigenschaften eines [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5c25b-107">Update the properties of a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c25b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5c25b-108">Prerequisites</span></span>
<span data-ttu-id="5c25b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5c25b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5c25b-111">Permission type</span></span>|<span data-ttu-id="5c25b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5c25b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c25b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5c25b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c25b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c25b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5c25b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5c25b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c25b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c25b-116">Not supported.</span></span>|
|<span data-ttu-id="5c25b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5c25b-117">Application</span></span>|<span data-ttu-id="5c25b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c25b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c25b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c25b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="5c25b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5c25b-120">Request headers</span></span>
|<span data-ttu-id="5c25b-121">Header</span><span class="sxs-lookup"><span data-stu-id="5c25b-121">Header</span></span>|<span data-ttu-id="5c25b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5c25b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c25b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5c25b-123">Authorization</span></span>|<span data-ttu-id="5c25b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5c25b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c25b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5c25b-125">Accept</span></span>|<span data-ttu-id="5c25b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c25b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c25b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5c25b-127">Request body</span></span>
<span data-ttu-id="5c25b-128">Geben Sie im Textkörper Anforderung für das Objekt [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="5c25b-128">In the request body, supply a JSON representation for the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

<span data-ttu-id="5c25b-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="5c25b-129">The following table shows the properties that are required when you create the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span>

|<span data-ttu-id="5c25b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5c25b-130">Property</span></span>|<span data-ttu-id="5c25b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5c25b-131">Type</span></span>|<span data-ttu-id="5c25b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c25b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c25b-133">id</span><span class="sxs-lookup"><span data-stu-id="5c25b-133">id</span></span>|<span data-ttu-id="5c25b-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-134">String</span></span>|<span data-ttu-id="5c25b-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5c25b-135">Key of the entity.</span></span> <span data-ttu-id="5c25b-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c25b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5c25b-137">displayName</span></span>|<span data-ttu-id="5c25b-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-138">String</span></span>|<span data-ttu-id="5c25b-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="5c25b-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5c25b-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c25b-141">description</span><span class="sxs-lookup"><span data-stu-id="5c25b-141">description</span></span>|<span data-ttu-id="5c25b-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-142">String</span></span>|<span data-ttu-id="5c25b-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="5c25b-143">The description of the app.</span></span> <span data-ttu-id="5c25b-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c25b-145">publisher</span><span class="sxs-lookup"><span data-stu-id="5c25b-145">publisher</span></span>|<span data-ttu-id="5c25b-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-146">String</span></span>|<span data-ttu-id="5c25b-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="5c25b-147">The publisher of the app.</span></span> <span data-ttu-id="5c25b-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c25b-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5c25b-149">largeIcon</span></span>|[<span data-ttu-id="5c25b-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5c25b-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5c25b-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5c25b-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5c25b-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c25b-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c25b-153">createdDateTime</span></span>|<span data-ttu-id="5c25b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c25b-154">DateTimeOffset</span></span>|<span data-ttu-id="5c25b-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="5c25b-155">The date and time the app was created.</span></span> <span data-ttu-id="5c25b-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c25b-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c25b-157">lastModifiedDateTime</span></span>|<span data-ttu-id="5c25b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c25b-158">DateTimeOffset</span></span>|<span data-ttu-id="5c25b-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="5c25b-159">The date and time the app was last modified.</span></span> <span data-ttu-id="5c25b-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c25b-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5c25b-161">isFeatured</span></span>|<span data-ttu-id="5c25b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c25b-162">Boolean</span></span>|<span data-ttu-id="5c25b-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c25b-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5c25b-164">privacyInformationUrl</span></span>|<span data-ttu-id="5c25b-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-165">String</span></span>|<span data-ttu-id="5c25b-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="5c25b-166">The privacy statement Url.</span></span> <span data-ttu-id="5c25b-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c25b-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5c25b-168">informationUrl</span></span>|<span data-ttu-id="5c25b-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-169">String</span></span>|<span data-ttu-id="5c25b-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="5c25b-170">The more information Url.</span></span> <span data-ttu-id="5c25b-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c25b-172">owner</span><span class="sxs-lookup"><span data-stu-id="5c25b-172">owner</span></span>|<span data-ttu-id="5c25b-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-173">String</span></span>|<span data-ttu-id="5c25b-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="5c25b-174">The owner of the app.</span></span> <span data-ttu-id="5c25b-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c25b-176">developer</span><span class="sxs-lookup"><span data-stu-id="5c25b-176">developer</span></span>|<span data-ttu-id="5c25b-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-177">String</span></span>|<span data-ttu-id="5c25b-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="5c25b-178">The developer of the app.</span></span> <span data-ttu-id="5c25b-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c25b-180">notes</span><span class="sxs-lookup"><span data-stu-id="5c25b-180">notes</span></span>|<span data-ttu-id="5c25b-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-181">String</span></span>|<span data-ttu-id="5c25b-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="5c25b-182">Notes for the app.</span></span> <span data-ttu-id="5c25b-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c25b-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="5c25b-184">uploadState</span></span>|<span data-ttu-id="5c25b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="5c25b-185">Int32</span></span>|<span data-ttu-id="5c25b-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="5c25b-186">The upload state.</span></span> <span data-ttu-id="5c25b-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c25b-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="5c25b-188">publishingState</span></span>|[<span data-ttu-id="5c25b-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5c25b-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5c25b-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="5c25b-190">The publishing state for the app.</span></span> <span data-ttu-id="5c25b-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="5c25b-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5c25b-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5c25b-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="5c25b-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5c25b-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5c25b-194">isAssigned</span></span>|<span data-ttu-id="5c25b-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c25b-195">Boolean</span></span>|<span data-ttu-id="5c25b-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="5c25b-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="5c25b-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c25b-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5c25b-198">roleScopeTagIds</span></span>|<span data-ttu-id="5c25b-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="5c25b-199">String collection</span></span>|<span data-ttu-id="5c25b-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="5c25b-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="5c25b-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c25b-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="5c25b-202">committedContentVersion</span></span>|<span data-ttu-id="5c25b-203">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-203">String</span></span>|<span data-ttu-id="5c25b-204">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="5c25b-204">The internal committed content version.</span></span> <span data-ttu-id="5c25b-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5c25b-206">fileName</span><span class="sxs-lookup"><span data-stu-id="5c25b-206">fileName</span></span>|<span data-ttu-id="5c25b-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-207">String</span></span>|<span data-ttu-id="5c25b-208">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="5c25b-208">The name of the main Lob application file.</span></span> <span data-ttu-id="5c25b-209">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5c25b-210">size</span><span class="sxs-lookup"><span data-stu-id="5c25b-210">size</span></span>|<span data-ttu-id="5c25b-211">Int64</span><span class="sxs-lookup"><span data-stu-id="5c25b-211">Int64</span></span>|<span data-ttu-id="5c25b-212">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="5c25b-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="5c25b-213">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c25b-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5c25b-214">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="5c25b-214">applicableArchitectures</span></span>|[<span data-ttu-id="5c25b-215">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="5c25b-215">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="5c25b-216">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="5c25b-216">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="5c25b-217">Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral` und `arm64`.</span><span class="sxs-lookup"><span data-stu-id="5c25b-217">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="5c25b-218">identityName</span><span class="sxs-lookup"><span data-stu-id="5c25b-218">identityName</span></span>|<span data-ttu-id="5c25b-219">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-219">String</span></span>|<span data-ttu-id="5c25b-220">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="5c25b-220">The Identity Name.</span></span>|
|<span data-ttu-id="5c25b-221">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="5c25b-221">identityPublisherHash</span></span>|<span data-ttu-id="5c25b-222">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-222">String</span></span>|<span data-ttu-id="5c25b-223">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="5c25b-223">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="5c25b-224">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="5c25b-224">identityResourceIdentifier</span></span>|<span data-ttu-id="5c25b-225">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-225">String</span></span>|<span data-ttu-id="5c25b-226">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="5c25b-226">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="5c25b-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5c25b-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5c25b-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5c25b-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="5c25b-229">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="5c25b-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="5c25b-230">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="5c25b-230">phoneProductIdentifier</span></span>|<span data-ttu-id="5c25b-231">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-231">String</span></span>|<span data-ttu-id="5c25b-232">Die Produkt-ID des Telefons.</span><span class="sxs-lookup"><span data-stu-id="5c25b-232">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="5c25b-233">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="5c25b-233">phonePublisherId</span></span>|<span data-ttu-id="5c25b-234">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-234">String</span></span>|<span data-ttu-id="5c25b-235">Die Telefon Publisher-Id.</span><span class="sxs-lookup"><span data-stu-id="5c25b-235">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="5c25b-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="5c25b-236">identityVersion</span></span>|<span data-ttu-id="5c25b-237">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c25b-237">String</span></span>|<span data-ttu-id="5c25b-238">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="5c25b-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="5c25b-239">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c25b-239">Response</span></span>
<span data-ttu-id="5c25b-240">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5c25b-240">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c25b-241">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5c25b-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c25b-242">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c25b-242">Request</span></span>
<span data-ttu-id="5c25b-243">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5c25b-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1440

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="5c25b-244">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c25b-244">Response</span></span>
<span data-ttu-id="5c25b-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c25b-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1612

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```




