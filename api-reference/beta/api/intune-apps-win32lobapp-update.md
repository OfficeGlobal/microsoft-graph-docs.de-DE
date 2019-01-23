---
title: Win32LobApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines win32LobApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 962059965abb2691ba1777518ad8aabc64adafe7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405338"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="9a2aa-103">Win32LobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9a2aa-103">Update win32LobApp</span></span>

> <span data-ttu-id="9a2aa-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9a2aa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a2aa-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a2aa-107">Aktualisieren Sie die Eigenschaften eines [win32LobApp](../resources/intune-apps-win32lobapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-107">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a2aa-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9a2aa-108">Prerequisites</span></span>
<span data-ttu-id="9a2aa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9a2aa-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9a2aa-111">Permission type</span></span>|<span data-ttu-id="9a2aa-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9a2aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a2aa-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9a2aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a2aa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a2aa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9a2aa-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9a2aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a2aa-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a2aa-116">Not supported.</span></span>|
|<span data-ttu-id="9a2aa-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9a2aa-117">Application</span></span>|<span data-ttu-id="9a2aa-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a2aa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a2aa-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a2aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="9a2aa-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9a2aa-120">Request headers</span></span>
|<span data-ttu-id="9a2aa-121">Header</span><span class="sxs-lookup"><span data-stu-id="9a2aa-121">Header</span></span>|<span data-ttu-id="9a2aa-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9a2aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a2aa-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9a2aa-123">Authorization</span></span>|<span data-ttu-id="9a2aa-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9a2aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a2aa-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9a2aa-125">Accept</span></span>|<span data-ttu-id="9a2aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a2aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a2aa-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9a2aa-127">Request body</span></span>
<span data-ttu-id="9a2aa-128">Geben Sie im Textkörper Anforderung für das Objekt [win32LobApp](../resources/intune-apps-win32lobapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-128">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="9a2aa-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [win32LobApp](../resources/intune-apps-win32lobapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-129">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="9a2aa-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9a2aa-130">Property</span></span>|<span data-ttu-id="9a2aa-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9a2aa-131">Type</span></span>|<span data-ttu-id="9a2aa-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9a2aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a2aa-133">id</span><span class="sxs-lookup"><span data-stu-id="9a2aa-133">id</span></span>|<span data-ttu-id="9a2aa-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a2aa-134">String</span></span>|<span data-ttu-id="9a2aa-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9a2aa-135">Key of the entity.</span></span> <span data-ttu-id="9a2aa-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a2aa-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9a2aa-137">displayName</span></span>|<span data-ttu-id="9a2aa-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a2aa-138">String</span></span>|<span data-ttu-id="9a2aa-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9a2aa-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a2aa-141">description</span><span class="sxs-lookup"><span data-stu-id="9a2aa-141">description</span></span>|<span data-ttu-id="9a2aa-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a2aa-142">String</span></span>|<span data-ttu-id="9a2aa-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-143">The description of the app.</span></span> <span data-ttu-id="9a2aa-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a2aa-145">publisher</span><span class="sxs-lookup"><span data-stu-id="9a2aa-145">publisher</span></span>|<span data-ttu-id="9a2aa-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a2aa-146">String</span></span>|<span data-ttu-id="9a2aa-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-147">The publisher of the app.</span></span> <span data-ttu-id="9a2aa-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a2aa-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9a2aa-149">largeIcon</span></span>|[<span data-ttu-id="9a2aa-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9a2aa-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9a2aa-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9a2aa-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a2aa-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a2aa-153">createdDateTime</span></span>|<span data-ttu-id="9a2aa-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a2aa-154">DateTimeOffset</span></span>|<span data-ttu-id="9a2aa-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-155">The date and time the app was created.</span></span> <span data-ttu-id="9a2aa-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a2aa-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a2aa-157">lastModifiedDateTime</span></span>|<span data-ttu-id="9a2aa-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a2aa-158">DateTimeOffset</span></span>|<span data-ttu-id="9a2aa-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-159">The date and time the app was last modified.</span></span> <span data-ttu-id="9a2aa-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a2aa-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9a2aa-161">isFeatured</span></span>|<span data-ttu-id="9a2aa-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a2aa-162">Boolean</span></span>|<span data-ttu-id="9a2aa-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a2aa-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9a2aa-164">privacyInformationUrl</span></span>|<span data-ttu-id="9a2aa-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a2aa-165">String</span></span>|<span data-ttu-id="9a2aa-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-166">The privacy statement Url.</span></span> <span data-ttu-id="9a2aa-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a2aa-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9a2aa-168">informationUrl</span></span>|<span data-ttu-id="9a2aa-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a2aa-169">String</span></span>|<span data-ttu-id="9a2aa-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-170">The more information Url.</span></span> <span data-ttu-id="9a2aa-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a2aa-172">owner</span><span class="sxs-lookup"><span data-stu-id="9a2aa-172">owner</span></span>|<span data-ttu-id="9a2aa-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a2aa-173">String</span></span>|<span data-ttu-id="9a2aa-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-174">The owner of the app.</span></span> <span data-ttu-id="9a2aa-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a2aa-176">developer</span><span class="sxs-lookup"><span data-stu-id="9a2aa-176">developer</span></span>|<span data-ttu-id="9a2aa-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a2aa-177">String</span></span>|<span data-ttu-id="9a2aa-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-178">The developer of the app.</span></span> <span data-ttu-id="9a2aa-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a2aa-180">notes</span><span class="sxs-lookup"><span data-stu-id="9a2aa-180">notes</span></span>|<span data-ttu-id="9a2aa-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a2aa-181">String</span></span>|<span data-ttu-id="9a2aa-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-182">Notes for the app.</span></span> <span data-ttu-id="9a2aa-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a2aa-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="9a2aa-184">uploadState</span></span>|<span data-ttu-id="9a2aa-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9a2aa-185">Int32</span></span>|<span data-ttu-id="9a2aa-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-186">The upload state.</span></span> <span data-ttu-id="9a2aa-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a2aa-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="9a2aa-188">publishingState</span></span>|[<span data-ttu-id="9a2aa-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9a2aa-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9a2aa-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-190">The publishing state for the app.</span></span> <span data-ttu-id="9a2aa-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9a2aa-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9a2aa-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9a2aa-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9a2aa-194">isAssigned</span></span>|<span data-ttu-id="9a2aa-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a2aa-195">Boolean</span></span>|<span data-ttu-id="9a2aa-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9a2aa-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a2aa-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9a2aa-198">roleScopeTagIds</span></span>|<span data-ttu-id="9a2aa-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="9a2aa-199">String collection</span></span>|<span data-ttu-id="9a2aa-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9a2aa-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a2aa-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9a2aa-202">committedContentVersion</span></span>|<span data-ttu-id="9a2aa-203">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a2aa-203">String</span></span>|<span data-ttu-id="9a2aa-204">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-204">The internal committed content version.</span></span> <span data-ttu-id="9a2aa-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9a2aa-206">fileName</span><span class="sxs-lookup"><span data-stu-id="9a2aa-206">fileName</span></span>|<span data-ttu-id="9a2aa-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a2aa-207">String</span></span>|<span data-ttu-id="9a2aa-208">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-208">The name of the main Lob application file.</span></span> <span data-ttu-id="9a2aa-209">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9a2aa-210">size</span><span class="sxs-lookup"><span data-stu-id="9a2aa-210">size</span></span>|<span data-ttu-id="9a2aa-211">Int64</span><span class="sxs-lookup"><span data-stu-id="9a2aa-211">Int64</span></span>|<span data-ttu-id="9a2aa-212">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="9a2aa-213">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2aa-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9a2aa-214">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="9a2aa-214">installCommandLine</span></span>|<span data-ttu-id="9a2aa-215">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a2aa-215">String</span></span>|<span data-ttu-id="9a2aa-216">So installieren Sie diese app die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="9a2aa-216">The command line to install this app</span></span>|
|<span data-ttu-id="9a2aa-217">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="9a2aa-217">uninstallCommandLine</span></span>|<span data-ttu-id="9a2aa-218">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a2aa-218">String</span></span>|<span data-ttu-id="9a2aa-219">So deinstallieren Sie diese app die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="9a2aa-219">The command line to uninstall this app</span></span>|
|<span data-ttu-id="9a2aa-220">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="9a2aa-220">applicableArchitectures</span></span>|[<span data-ttu-id="9a2aa-221">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="9a2aa-221">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="9a2aa-222">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-222">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="9a2aa-223">Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral` und `arm64`.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-223">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="9a2aa-224">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9a2aa-224">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9a2aa-225">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9a2aa-225">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="9a2aa-226">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-226">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9a2aa-227">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="9a2aa-227">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="9a2aa-228">Int32</span><span class="sxs-lookup"><span data-stu-id="9a2aa-228">Int32</span></span>|<span data-ttu-id="9a2aa-229">Der Wert für den minimalen freien Speicherplatz der erforderlich ist, um diese app zu installieren.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-229">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="9a2aa-230">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="9a2aa-230">minimumMemoryInMB</span></span>|<span data-ttu-id="9a2aa-231">Int32</span><span class="sxs-lookup"><span data-stu-id="9a2aa-231">Int32</span></span>|<span data-ttu-id="9a2aa-232">Der Wert für das minimale des Arbeitsspeichers erforderlich für diese app installieren.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-232">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="9a2aa-233">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="9a2aa-233">minimumNumberOfProcessors</span></span>|<span data-ttu-id="9a2aa-234">Int32</span><span class="sxs-lookup"><span data-stu-id="9a2aa-234">Int32</span></span>|<span data-ttu-id="9a2aa-235">Der Wert für die minimale Anzahl der Prozessoren erforderlich ist, um diese app zu installieren.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-235">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="9a2aa-236">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="9a2aa-236">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="9a2aa-237">Int32</span><span class="sxs-lookup"><span data-stu-id="9a2aa-237">Int32</span></span>|<span data-ttu-id="9a2aa-238">Der Wert für die minimale CPU-Geschwindigkeit der erforderlich ist, um diese app zu installieren.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-238">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="9a2aa-239">detectionRules</span><span class="sxs-lookup"><span data-stu-id="9a2aa-239">detectionRules</span></span>|<span data-ttu-id="9a2aa-240">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9a2aa-240">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="9a2aa-241">Die Erkennung von Regeln zum Erkennen von Win32 Line of Business (LoB) app.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-241">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9a2aa-242">installExperience</span><span class="sxs-lookup"><span data-stu-id="9a2aa-242">installExperience</span></span>|[<span data-ttu-id="9a2aa-243">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="9a2aa-243">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="9a2aa-244">Die Installation für diese app.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-244">The install experience for this app.</span></span>|
|<span data-ttu-id="9a2aa-245">returnCodes</span><span class="sxs-lookup"><span data-stu-id="9a2aa-245">returnCodes</span></span>|<span data-ttu-id="9a2aa-246">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9a2aa-246">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="9a2aa-247">Die Rückgabecodes für buchen Verhalten bei der Installation.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-247">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="9a2aa-248">msiInformation</span><span class="sxs-lookup"><span data-stu-id="9a2aa-248">msiInformation</span></span>|[<span data-ttu-id="9a2aa-249">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="9a2aa-249">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="9a2aa-250">Die MSI-Details, wenn diese Win32-app eine MSI-app ist.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-250">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="9a2aa-251">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="9a2aa-251">setupFilePath</span></span>|<span data-ttu-id="9a2aa-252">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a2aa-252">String</span></span>|<span data-ttu-id="9a2aa-253">Der relative Pfad der Datei in das verschlüsselte Win32LobApp-Paket.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-253">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="9a2aa-254">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a2aa-254">Response</span></span>
<span data-ttu-id="9a2aa-255">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [win32LobApp](../resources/intune-apps-win32lobapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-255">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a2aa-256">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9a2aa-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a2aa-257">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a2aa-257">Request</span></span>
<span data-ttu-id="9a2aa-258">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-258">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2285

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

### <a name="response"></a><span data-ttu-id="9a2aa-259">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a2aa-259">Response</span></span>
<span data-ttu-id="9a2aa-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a2aa-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2457

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




