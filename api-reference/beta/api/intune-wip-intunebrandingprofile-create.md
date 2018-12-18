---
title: Erstellen von intuneBrandingProfile
description: Erstellen eines neuen IntuneBrandingProfile-Objekts.
author: tfitzmac
ms.openlocfilehash: 4058e30fe858c261a59b105652d198946b630222
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314875"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="d532e-103">Erstellen von intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="d532e-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="d532e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d532e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d532e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d532e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d532e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d532e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d532e-107">Erstellen eines neuen [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d532e-107">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d532e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d532e-108">Prerequisites</span></span>
<span data-ttu-id="d532e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d532e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d532e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d532e-111">Permission type</span></span>|<span data-ttu-id="d532e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d532e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d532e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d532e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d532e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d532e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d532e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d532e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d532e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d532e-116">Not supported.</span></span>|
|<span data-ttu-id="d532e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d532e-117">Application</span></span>|<span data-ttu-id="d532e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d532e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d532e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d532e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="d532e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d532e-120">Request headers</span></span>
|<span data-ttu-id="d532e-121">Header</span><span class="sxs-lookup"><span data-stu-id="d532e-121">Header</span></span>|<span data-ttu-id="d532e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d532e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d532e-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d532e-123">Authorization</span></span>|<span data-ttu-id="d532e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d532e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d532e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d532e-125">Accept</span></span>|<span data-ttu-id="d532e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d532e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d532e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d532e-127">Request body</span></span>
<span data-ttu-id="d532e-128">Geben Sie im Textkörper Anforderung für das Objekt IntuneBrandingProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d532e-128">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="d532e-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die IntuneBrandingProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="d532e-129">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="d532e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d532e-130">Property</span></span>|<span data-ttu-id="d532e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d532e-131">Type</span></span>|<span data-ttu-id="d532e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d532e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d532e-133">id</span><span class="sxs-lookup"><span data-stu-id="d532e-133">id</span></span>|<span data-ttu-id="d532e-134">String</span><span class="sxs-lookup"><span data-stu-id="d532e-134">String</span></span>|<span data-ttu-id="d532e-135">Profil-Taste</span><span class="sxs-lookup"><span data-stu-id="d532e-135">Profile Key</span></span>|
|<span data-ttu-id="d532e-136">Profilname</span><span class="sxs-lookup"><span data-stu-id="d532e-136">profileName</span></span>|<span data-ttu-id="d532e-137">String</span><span class="sxs-lookup"><span data-stu-id="d532e-137">String</span></span>|<span data-ttu-id="d532e-138">Name des Profils</span><span class="sxs-lookup"><span data-stu-id="d532e-138">Name of the profile</span></span>|
|<span data-ttu-id="d532e-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="d532e-139">profileDescription</span></span>|<span data-ttu-id="d532e-140">String</span><span class="sxs-lookup"><span data-stu-id="d532e-140">String</span></span>|<span data-ttu-id="d532e-141">Beschreibung des Profils</span><span class="sxs-lookup"><span data-stu-id="d532e-141">Description of the profile</span></span>|
|<span data-ttu-id="d532e-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="d532e-142">isDefaultProfile</span></span>|<span data-ttu-id="d532e-143">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d532e-143">Boolean</span></span>|<span data-ttu-id="d532e-144">Zeigt an, wenn das Profil für standardmäßig verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="d532e-144">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="d532e-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d532e-145">createdDateTime</span></span>|<span data-ttu-id="d532e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d532e-146">DateTimeOffset</span></span>|<span data-ttu-id="d532e-147">Wenn die BrandingProfile erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="d532e-147">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="d532e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d532e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="d532e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d532e-149">DateTimeOffset</span></span>|<span data-ttu-id="d532e-150">Wann die BrandingProfile zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="d532e-150">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="d532e-151">displayName</span><span class="sxs-lookup"><span data-stu-id="d532e-151">displayName</span></span>|<span data-ttu-id="d532e-152">String</span><span class="sxs-lookup"><span data-stu-id="d532e-152">String</span></span>|<span data-ttu-id="d532e-153">Unternehmensname/Organisationsname, der Endbenutzern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="d532e-153">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="d532e-154">contactITName</span><span class="sxs-lookup"><span data-stu-id="d532e-154">contactITName</span></span>|<span data-ttu-id="d532e-155">String</span><span class="sxs-lookup"><span data-stu-id="d532e-155">String</span></span>|<span data-ttu-id="d532e-156">Name der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="d532e-156">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="d532e-157">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="d532e-157">contactITPhoneNumber</span></span>|<span data-ttu-id="d532e-158">String</span><span class="sxs-lookup"><span data-stu-id="d532e-158">String</span></span>|<span data-ttu-id="d532e-159">Telefonnummer der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="d532e-159">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="d532e-160">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="d532e-160">contactITEmailAddress</span></span>|<span data-ttu-id="d532e-161">String</span><span class="sxs-lookup"><span data-stu-id="d532e-161">String</span></span>|<span data-ttu-id="d532e-162">E-Mail-Adresse der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="d532e-162">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="d532e-163">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="d532e-163">contactITNotes</span></span>|<span data-ttu-id="d532e-164">String</span><span class="sxs-lookup"><span data-stu-id="d532e-164">String</span></span>|<span data-ttu-id="d532e-165">Textkommentare zu der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="d532e-165">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="d532e-166">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="d532e-166">privacyUrl</span></span>|<span data-ttu-id="d532e-167">String</span><span class="sxs-lookup"><span data-stu-id="d532e-167">String</span></span>|<span data-ttu-id="d532e-168">URL zur Datenschutzrichtlinie des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="d532e-168">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="d532e-169">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="d532e-169">onlineSupportSiteUrl</span></span>|<span data-ttu-id="d532e-170">String</span><span class="sxs-lookup"><span data-stu-id="d532e-170">String</span></span>|<span data-ttu-id="d532e-171">URL zur IT-Helpdesk-Website des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="d532e-171">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="d532e-172">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="d532e-172">onlineSupportSiteName</span></span>|<span data-ttu-id="d532e-173">String</span><span class="sxs-lookup"><span data-stu-id="d532e-173">String</span></span>|<span data-ttu-id="d532e-174">Anzeigename der IT-Helpdesk-Website des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="d532e-174">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="d532e-175">themeColor</span><span class="sxs-lookup"><span data-stu-id="d532e-175">themeColor</span></span>|[<span data-ttu-id="d532e-176">rgbColor</span><span class="sxs-lookup"><span data-stu-id="d532e-176">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="d532e-177">Primäres Farbdesign für die Unternehmensportal-Anwendungen und das Webportal</span><span class="sxs-lookup"><span data-stu-id="d532e-177">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="d532e-178">showLogo</span><span class="sxs-lookup"><span data-stu-id="d532e-178">showLogo</span></span>|<span data-ttu-id="d532e-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="d532e-179">Boolean</span></span>|<span data-ttu-id="d532e-180">Boolescher Wert, der angibt, ob die vom Administrator bereitgestellten Logobilder angezeigt werden sollen</span><span class="sxs-lookup"><span data-stu-id="d532e-180">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="d532e-181">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="d532e-181">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="d532e-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="d532e-182">Boolean</span></span>|<span data-ttu-id="d532e-183">Boolescher Wert, der angibt, ob der vom Administrator angegebene Anzeigename neben dem Logobild angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="d532e-183">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="d532e-184">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="d532e-184">themeColorLogo</span></span>|[<span data-ttu-id="d532e-185">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d532e-185">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d532e-186">Logo-Bilds im Unternehmensportal apps auf Design farbigen Hintergrund angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d532e-186">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="d532e-187">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="d532e-187">lightBackgroundLogo</span></span>|[<span data-ttu-id="d532e-188">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d532e-188">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d532e-189">Logo-Bilds im Unternehmensportal apps heller Hintergrund angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d532e-189">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="d532e-190">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="d532e-190">landingPageCustomizedImage</span></span>|[<span data-ttu-id="d532e-191">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d532e-191">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d532e-192">Angepasste Bild im Unternehmensportal apps Zielseite</span><span class="sxs-lookup"><span data-stu-id="d532e-192">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="d532e-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="d532e-193">Response</span></span>
<span data-ttu-id="d532e-194">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d532e-194">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d532e-195">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d532e-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="d532e-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d532e-196">Request</span></span>
<span data-ttu-id="d532e-197">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d532e-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1269

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="d532e-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="d532e-198">Response</span></span>
<span data-ttu-id="d532e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d532e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1377

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```





