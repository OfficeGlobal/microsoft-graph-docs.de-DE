---
title: iosEduCertificateSettings-Ressourcentyp
description: Vertrauenswürdige Stamm-und PFX-Zertifikate für iOS EDU.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c94b7bc75022f8338a41da3b3b9d135dff47ac3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142651"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="470b3-103">iosEduCertificateSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="470b3-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="470b3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="470b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="470b3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="470b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="470b3-106">Vertrauenswürdige Stamm-und PFX-Zertifikate für iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="470b3-106">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="470b3-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="470b3-107">Properties</span></span>
|<span data-ttu-id="470b3-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="470b3-108">Property</span></span>|<span data-ttu-id="470b3-109">Typ</span><span class="sxs-lookup"><span data-stu-id="470b3-109">Type</span></span>|<span data-ttu-id="470b3-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="470b3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="470b3-111">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="470b3-111">trustedRootCertificate</span></span>|<span data-ttu-id="470b3-112">Binär</span><span class="sxs-lookup"><span data-stu-id="470b3-112">Binary</span></span>|<span data-ttu-id="470b3-113">Vertrauenswürdiges Stammzertifikat.</span><span class="sxs-lookup"><span data-stu-id="470b3-113">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="470b3-114">certFileName</span><span class="sxs-lookup"><span data-stu-id="470b3-114">certFileName</span></span>|<span data-ttu-id="470b3-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="470b3-115">String</span></span>|<span data-ttu-id="470b3-116">Dateiname, der in der Benutzeroberfläche angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="470b3-116">File name to display in UI.</span></span>|
|<span data-ttu-id="470b3-117">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="470b3-117">certificationAuthority</span></span>|<span data-ttu-id="470b3-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="470b3-118">String</span></span>|<span data-ttu-id="470b3-119">PKCS-ZertifizierungsStelle.</span><span class="sxs-lookup"><span data-stu-id="470b3-119">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="470b3-120">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="470b3-120">certificationAuthorityName</span></span>|<span data-ttu-id="470b3-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="470b3-121">String</span></span>|<span data-ttu-id="470b3-122">Name der PKCS-ZertifizierungsStelle.</span><span class="sxs-lookup"><span data-stu-id="470b3-122">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="470b3-123">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="470b3-123">certificateTemplateName</span></span>|<span data-ttu-id="470b3-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="470b3-124">String</span></span>|<span data-ttu-id="470b3-125">Name der PKCS-Zertifikatvorlage.</span><span class="sxs-lookup"><span data-stu-id="470b3-125">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="470b3-126">Eigenschaften renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="470b3-126">renewalThresholdPercentage</span></span>|<span data-ttu-id="470b3-127">Int32</span><span class="sxs-lookup"><span data-stu-id="470b3-127">Int32</span></span>|<span data-ttu-id="470b3-128">Schwellenwert für die Zertifikaterneuerung.</span><span class="sxs-lookup"><span data-stu-id="470b3-128">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="470b3-129">Gültige Werte 1 bis 99</span><span class="sxs-lookup"><span data-stu-id="470b3-129">Valid values 1 to 99</span></span>|
|<span data-ttu-id="470b3-130">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="470b3-130">certificateValidityPeriodValue</span></span>|<span data-ttu-id="470b3-131">Int32</span><span class="sxs-lookup"><span data-stu-id="470b3-131">Int32</span></span>|<span data-ttu-id="470b3-132">Wert für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="470b3-132">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="470b3-133">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="470b3-133">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="470b3-134">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="470b3-134">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="470b3-135">Skalierung für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="470b3-135">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="470b3-136">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="470b3-136">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="470b3-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="470b3-137">Relationships</span></span>
<span data-ttu-id="470b3-138">Keine</span><span class="sxs-lookup"><span data-stu-id="470b3-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="470b3-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="470b3-139">JSON Representation</span></span>
<span data-ttu-id="470b3-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="470b3-140">Here is a JSON representation of the resource.</span></span>
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




