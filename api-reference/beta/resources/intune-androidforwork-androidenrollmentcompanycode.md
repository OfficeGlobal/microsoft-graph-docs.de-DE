---
title: androidEnrollmentCompanyCode-Ressourcentyp
description: Eine Klasse zum Speichern von Spezialdaten für die Registrierung über die Android-Verwaltungs-API von Google, wie Token-, URL-und QR-Code Inhalte
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0cd3ede4193ea3fdb33d33010349812150848e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169342"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="cd4c8-103">androidEnrollmentCompanyCode-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cd4c8-103">androidEnrollmentCompanyCode resource type</span></span>

> <span data-ttu-id="cd4c8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cd4c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd4c8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="cd4c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd4c8-106">Eine Klasse zum Speichern von Spezialdaten für die Registrierung über die Android-Verwaltungs-API von Google, wie Token-, URL-und QR-Code Inhalte</span><span class="sxs-lookup"><span data-stu-id="cd4c8-106">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="cd4c8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cd4c8-107">Properties</span></span>
|<span data-ttu-id="cd4c8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cd4c8-108">Property</span></span>|<span data-ttu-id="cd4c8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="cd4c8-109">Type</span></span>|<span data-ttu-id="cd4c8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd4c8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd4c8-111">enrollmentToken</span><span class="sxs-lookup"><span data-stu-id="cd4c8-111">enrollmentToken</span></span>|<span data-ttu-id="cd4c8-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd4c8-112">String</span></span>|<span data-ttu-id="cd4c8-113">Vom Benutzer zum Registrieren des Geräts verwendete Registrierungs Token.</span><span class="sxs-lookup"><span data-stu-id="cd4c8-113">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="cd4c8-114">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="cd4c8-114">qrCodeContent</span></span>|<span data-ttu-id="cd4c8-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd4c8-115">String</span></span>|<span data-ttu-id="cd4c8-116">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird</span><span class="sxs-lookup"><span data-stu-id="cd4c8-116">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="cd4c8-117">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="cd4c8-117">qrCodeImage</span></span>|[<span data-ttu-id="cd4c8-118">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cd4c8-118">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cd4c8-119">Generierter QR-Code für das Token.</span><span class="sxs-lookup"><span data-stu-id="cd4c8-119">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd4c8-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cd4c8-120">Relationships</span></span>
<span data-ttu-id="cd4c8-121">Keine</span><span class="sxs-lookup"><span data-stu-id="cd4c8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd4c8-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cd4c8-122">JSON Representation</span></span>
<span data-ttu-id="cd4c8-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cd4c8-123">Here is a JSON representation of the resource.</span></span>
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




