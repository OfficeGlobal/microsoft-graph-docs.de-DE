---
title: Ressourcentyp iosEduCertificateSettings
description: Vertrauenswürdige Stamm und PFX-Zertifikate für iOS EDU.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8c48883caa9479638b1a727272abdd0bc5762db9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948675"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="67002-103">Ressourcentyp iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="67002-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="67002-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="67002-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67002-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="67002-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67002-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="67002-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67002-107">Vertrauenswürdige Stamm und PFX-Zertifikate für iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="67002-107">Trusted Root and PFX certificates for iOS EDU.</span></span>
## <a name="properties"></a><span data-ttu-id="67002-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="67002-108">Properties</span></span>
|<span data-ttu-id="67002-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="67002-109">Property</span></span>|<span data-ttu-id="67002-110">Typ</span><span class="sxs-lookup"><span data-stu-id="67002-110">Type</span></span>|<span data-ttu-id="67002-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67002-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67002-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="67002-112">trustedRootCertificate</span></span>|<span data-ttu-id="67002-113">Binär</span><span class="sxs-lookup"><span data-stu-id="67002-113">Binary</span></span>|<span data-ttu-id="67002-114">Zertifikat der vertrauenswürdigen Stammzertifizierungsstellen.</span><span class="sxs-lookup"><span data-stu-id="67002-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="67002-115">Aus</span><span class="sxs-lookup"><span data-stu-id="67002-115">certFileName</span></span>|<span data-ttu-id="67002-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67002-116">String</span></span>|<span data-ttu-id="67002-117">Der Dateiname in der Benutzeroberfläche angezeigt.</span><span class="sxs-lookup"><span data-stu-id="67002-117">File name to display in UI.</span></span>|
|<span data-ttu-id="67002-118">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="67002-118">certificationAuthority</span></span>|<span data-ttu-id="67002-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67002-119">String</span></span>|<span data-ttu-id="67002-120">PKCS Zertifizierungsstelle.</span><span class="sxs-lookup"><span data-stu-id="67002-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="67002-121">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="67002-121">certificationAuthorityName</span></span>|<span data-ttu-id="67002-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67002-122">String</span></span>|<span data-ttu-id="67002-123">Name der Zertifizierungsstelle PKCS.</span><span class="sxs-lookup"><span data-stu-id="67002-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="67002-124">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="67002-124">certificateTemplateName</span></span>|<span data-ttu-id="67002-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67002-125">String</span></span>|<span data-ttu-id="67002-126">Name der PKCS Zertifikatsvorlage.</span><span class="sxs-lookup"><span data-stu-id="67002-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="67002-127">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="67002-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="67002-128">Int32</span><span class="sxs-lookup"><span data-stu-id="67002-128">Int32</span></span>|<span data-ttu-id="67002-129">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="67002-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="67002-130">Gültige Werte 1 bis 99</span><span class="sxs-lookup"><span data-stu-id="67002-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="67002-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="67002-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="67002-132">Int32</span><span class="sxs-lookup"><span data-stu-id="67002-132">Int32</span></span>|<span data-ttu-id="67002-133">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="67002-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="67002-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="67002-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="67002-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="67002-135">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="67002-136">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="67002-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="67002-137">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="67002-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67002-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="67002-138">Relationships</span></span>
<span data-ttu-id="67002-139">Keine</span><span class="sxs-lookup"><span data-stu-id="67002-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="67002-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="67002-140">JSON Representation</span></span>
<span data-ttu-id="67002-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="67002-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosEduCertificateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduCertificateSettings",
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "renewalThresholdPercentage": 1024,
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String"
}
```





