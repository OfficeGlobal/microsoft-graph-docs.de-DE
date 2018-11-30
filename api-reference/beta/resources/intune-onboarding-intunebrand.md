---
title: Ressourcentyp „intuneBrand“
description: „intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.
ms.openlocfilehash: b8ed558e2be032110470cc4e2c64d27d8011af1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063848"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="94bcf-103">Ressourcentyp „intuneBrand“</span><span class="sxs-lookup"><span data-stu-id="94bcf-103">intuneBrand resource type</span></span>

> <span data-ttu-id="94bcf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="94bcf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94bcf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="94bcf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94bcf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="94bcf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94bcf-107">„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.</span><span class="sxs-lookup"><span data-stu-id="94bcf-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>
## <a name="properties"></a><span data-ttu-id="94bcf-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="94bcf-108">Properties</span></span>
|<span data-ttu-id="94bcf-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="94bcf-109">Property</span></span>|<span data-ttu-id="94bcf-110">Typ</span><span class="sxs-lookup"><span data-stu-id="94bcf-110">Type</span></span>|<span data-ttu-id="94bcf-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94bcf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94bcf-112">displayName</span><span class="sxs-lookup"><span data-stu-id="94bcf-112">displayName</span></span>|<span data-ttu-id="94bcf-113">String</span><span class="sxs-lookup"><span data-stu-id="94bcf-113">String</span></span>|<span data-ttu-id="94bcf-114">Unternehmensname/Organisationsname, der Endbenutzern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="94bcf-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="94bcf-115">contactITName</span><span class="sxs-lookup"><span data-stu-id="94bcf-115">contactITName</span></span>|<span data-ttu-id="94bcf-116">String</span><span class="sxs-lookup"><span data-stu-id="94bcf-116">String</span></span>|<span data-ttu-id="94bcf-117">Name der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="94bcf-117">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="94bcf-118">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="94bcf-118">contactITPhoneNumber</span></span>|<span data-ttu-id="94bcf-119">String</span><span class="sxs-lookup"><span data-stu-id="94bcf-119">String</span></span>|<span data-ttu-id="94bcf-120">Telefonnummer der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="94bcf-120">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="94bcf-121">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="94bcf-121">contactITEmailAddress</span></span>|<span data-ttu-id="94bcf-122">String</span><span class="sxs-lookup"><span data-stu-id="94bcf-122">String</span></span>|<span data-ttu-id="94bcf-123">E-Mail-Adresse der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="94bcf-123">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="94bcf-124">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="94bcf-124">contactITNotes</span></span>|<span data-ttu-id="94bcf-125">String</span><span class="sxs-lookup"><span data-stu-id="94bcf-125">String</span></span>|<span data-ttu-id="94bcf-126">Textkommentare zu der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="94bcf-126">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="94bcf-127">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="94bcf-127">privacyUrl</span></span>|<span data-ttu-id="94bcf-128">String</span><span class="sxs-lookup"><span data-stu-id="94bcf-128">String</span></span>|<span data-ttu-id="94bcf-129">URL zur Datenschutzrichtlinie des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="94bcf-129">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="94bcf-130">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="94bcf-130">onlineSupportSiteUrl</span></span>|<span data-ttu-id="94bcf-131">String</span><span class="sxs-lookup"><span data-stu-id="94bcf-131">String</span></span>|<span data-ttu-id="94bcf-132">URL zur IT-Helpdesk-Website des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="94bcf-132">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="94bcf-133">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="94bcf-133">onlineSupportSiteName</span></span>|<span data-ttu-id="94bcf-134">String</span><span class="sxs-lookup"><span data-stu-id="94bcf-134">String</span></span>|<span data-ttu-id="94bcf-135">Anzeigename der IT-Helpdesk-Website des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="94bcf-135">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="94bcf-136">themeColor</span><span class="sxs-lookup"><span data-stu-id="94bcf-136">themeColor</span></span>|[<span data-ttu-id="94bcf-137">rgbColor</span><span class="sxs-lookup"><span data-stu-id="94bcf-137">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="94bcf-138">Primäres Farbdesign für die Unternehmensportal-Anwendungen und das Webportal</span><span class="sxs-lookup"><span data-stu-id="94bcf-138">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="94bcf-139">showLogo</span><span class="sxs-lookup"><span data-stu-id="94bcf-139">showLogo</span></span>|<span data-ttu-id="94bcf-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="94bcf-140">Boolean</span></span>|<span data-ttu-id="94bcf-141">Boolescher Wert, der angibt, ob die vom Administrator bereitgestellten Logobilder angezeigt werden sollen</span><span class="sxs-lookup"><span data-stu-id="94bcf-141">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="94bcf-142">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="94bcf-142">lightBackgroundLogo</span></span>|[<span data-ttu-id="94bcf-143">mimeContent</span><span class="sxs-lookup"><span data-stu-id="94bcf-143">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="94bcf-144">Logobild, das in Unternehmensportal-Apps mit hellem Hintergrund hinter dem Logo angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="94bcf-144">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="94bcf-145">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="94bcf-145">darkBackgroundLogo</span></span>|[<span data-ttu-id="94bcf-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="94bcf-146">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="94bcf-147">Logobild, das in Unternehmensportal-Apps mit dunklem Hintergrund hinter dem Logo angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="94bcf-147">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="94bcf-148">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="94bcf-148">showNameNextToLogo</span></span>|<span data-ttu-id="94bcf-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="94bcf-149">Boolean</span></span>|<span data-ttu-id="94bcf-150">Boolescher Wert, der angibt, ob der vom Administrator angegebene Anzeigename neben dem Logobild angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="94bcf-150">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="94bcf-151">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="94bcf-151">landingPageCustomizedImage</span></span>|[<span data-ttu-id="94bcf-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="94bcf-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="94bcf-153">Angepasste Bild im Unternehmen Portal-Angebotsseite</span><span class="sxs-lookup"><span data-stu-id="94bcf-153">Customized image displayed in Compnay Portal app landing page</span></span>|
|<span data-ttu-id="94bcf-154">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="94bcf-154">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="94bcf-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="94bcf-155">Boolean</span></span>|<span data-ttu-id="94bcf-156">Boolescher Wert, der angibt, ob der vom Administrator angegebene Anzeigename neben dem Logobild angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="94bcf-156">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94bcf-157">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="94bcf-157">Relationships</span></span>
<span data-ttu-id="94bcf-158">Keine</span><span class="sxs-lookup"><span data-stu-id="94bcf-158">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="94bcf-159">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="94bcf-159">JSON Representation</span></span>
<span data-ttu-id="94bcf-160">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="94bcf-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "privacyUrl": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showNameNextToLogo": true,
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showDisplayNameNextToLogo": true
}
```





