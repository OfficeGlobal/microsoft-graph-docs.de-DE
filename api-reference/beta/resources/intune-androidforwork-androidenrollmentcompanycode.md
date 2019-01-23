---
title: Ressourcentyp androidEnrollmentCompanyCode
description: Einer Klasse zum halten Spezialisierung Anmeldedaten verwendet zum Registrieren von über Googles Android-Verwaltungs-API, wie beispielsweise Token, die Url und QR code Inhalte
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be5b2a94445e95fe18271467b6661320d8204d76
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429961"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="2dddf-103">Ressourcentyp androidEnrollmentCompanyCode</span><span class="sxs-lookup"><span data-stu-id="2dddf-103">androidEnrollmentCompanyCode resource type</span></span>

> <span data-ttu-id="2dddf-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2dddf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2dddf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2dddf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2dddf-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2dddf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dddf-107">Einer Klasse zum halten Spezialisierung Anmeldedaten verwendet zum Registrieren von über Googles Android-Verwaltungs-API, wie beispielsweise Token, die Url und QR code Inhalte</span><span class="sxs-lookup"><span data-stu-id="2dddf-107">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="2dddf-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2dddf-108">Properties</span></span>
|<span data-ttu-id="2dddf-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2dddf-109">Property</span></span>|<span data-ttu-id="2dddf-110">Typ</span><span class="sxs-lookup"><span data-stu-id="2dddf-110">Type</span></span>|<span data-ttu-id="2dddf-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2dddf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dddf-112">enrollmentToken</span><span class="sxs-lookup"><span data-stu-id="2dddf-112">enrollmentToken</span></span>|<span data-ttu-id="2dddf-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2dddf-113">String</span></span>|<span data-ttu-id="2dddf-114">Registrierung Token vom Benutzer verwendet werden, um ihr Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="2dddf-114">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="2dddf-115">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="2dddf-115">qrCodeContent</span></span>|<span data-ttu-id="2dddf-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2dddf-116">String</span></span>|<span data-ttu-id="2dddf-117">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird</span><span class="sxs-lookup"><span data-stu-id="2dddf-117">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="2dddf-118">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="2dddf-118">qrCodeImage</span></span>|[<span data-ttu-id="2dddf-119">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2dddf-119">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2dddf-120">Generierten QR-Code für das Token.</span><span class="sxs-lookup"><span data-stu-id="2dddf-120">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2dddf-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2dddf-121">Relationships</span></span>
<span data-ttu-id="2dddf-122">Keine</span><span class="sxs-lookup"><span data-stu-id="2dddf-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2dddf-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2dddf-123">JSON Representation</span></span>
<span data-ttu-id="2dddf-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2dddf-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnrollmentCompanyCode",
  "enrollmentToken": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```




