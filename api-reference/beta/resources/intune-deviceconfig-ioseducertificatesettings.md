---
title: Ressourcentyp iosEduCertificateSettings
description: Vertrauenswürdige Stamm und PFX-Zertifikate für iOS EDU.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d23b379dea7a75e4ae79029845cd6e9f956503c0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423552"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="88deb-103">Ressourcentyp iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="88deb-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="88deb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="88deb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="88deb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="88deb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88deb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="88deb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88deb-107">Vertrauenswürdige Stamm und PFX-Zertifikate für iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="88deb-107">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="88deb-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="88deb-108">Properties</span></span>
|<span data-ttu-id="88deb-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88deb-109">Property</span></span>|<span data-ttu-id="88deb-110">Typ</span><span class="sxs-lookup"><span data-stu-id="88deb-110">Type</span></span>|<span data-ttu-id="88deb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88deb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88deb-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="88deb-112">trustedRootCertificate</span></span>|<span data-ttu-id="88deb-113">Binär</span><span class="sxs-lookup"><span data-stu-id="88deb-113">Binary</span></span>|<span data-ttu-id="88deb-114">Zertifikat der vertrauenswürdigen Stammzertifizierungsstellen.</span><span class="sxs-lookup"><span data-stu-id="88deb-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="88deb-115">Aus</span><span class="sxs-lookup"><span data-stu-id="88deb-115">certFileName</span></span>|<span data-ttu-id="88deb-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88deb-116">String</span></span>|<span data-ttu-id="88deb-117">Der Dateiname in der Benutzeroberfläche angezeigt.</span><span class="sxs-lookup"><span data-stu-id="88deb-117">File name to display in UI.</span></span>|
|<span data-ttu-id="88deb-118">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="88deb-118">certificationAuthority</span></span>|<span data-ttu-id="88deb-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88deb-119">String</span></span>|<span data-ttu-id="88deb-120">PKCS Zertifizierungsstelle.</span><span class="sxs-lookup"><span data-stu-id="88deb-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="88deb-121">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="88deb-121">certificationAuthorityName</span></span>|<span data-ttu-id="88deb-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88deb-122">String</span></span>|<span data-ttu-id="88deb-123">Name der Zertifizierungsstelle PKCS.</span><span class="sxs-lookup"><span data-stu-id="88deb-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="88deb-124">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="88deb-124">certificateTemplateName</span></span>|<span data-ttu-id="88deb-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88deb-125">String</span></span>|<span data-ttu-id="88deb-126">Name der PKCS Zertifikatsvorlage.</span><span class="sxs-lookup"><span data-stu-id="88deb-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="88deb-127">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="88deb-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="88deb-128">Int32</span><span class="sxs-lookup"><span data-stu-id="88deb-128">Int32</span></span>|<span data-ttu-id="88deb-129">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="88deb-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="88deb-130">Gültige Werte 1 bis 99</span><span class="sxs-lookup"><span data-stu-id="88deb-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="88deb-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="88deb-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="88deb-132">Int32</span><span class="sxs-lookup"><span data-stu-id="88deb-132">Int32</span></span>|<span data-ttu-id="88deb-133">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="88deb-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="88deb-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="88deb-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="88deb-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="88deb-135">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="88deb-136">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="88deb-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="88deb-137">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="88deb-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88deb-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="88deb-138">Relationships</span></span>
<span data-ttu-id="88deb-139">Keine</span><span class="sxs-lookup"><span data-stu-id="88deb-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88deb-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="88deb-140">JSON Representation</span></span>
<span data-ttu-id="88deb-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="88deb-141">Here is a JSON representation of the resource.</span></span>
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




