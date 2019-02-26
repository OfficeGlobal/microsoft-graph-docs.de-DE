---
title: appLogUploadState-Enumerationstyp
description: AppLogUploadStatus
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f8243436fa9ec5a56f442626cea31819ca1eaef
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174389"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="a5f1c-103">appLogUploadState-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="a5f1c-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="a5f1c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a5f1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5f1c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a5f1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5f1c-106">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="a5f1c-106">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="a5f1c-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="a5f1c-107">Members</span></span>
|<span data-ttu-id="a5f1c-108">Element</span><span class="sxs-lookup"><span data-stu-id="a5f1c-108">Member</span></span>|<span data-ttu-id="a5f1c-109">Wert</span><span class="sxs-lookup"><span data-stu-id="a5f1c-109">Value</span></span>|<span data-ttu-id="a5f1c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5f1c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5f1c-111">ausstehenden</span><span class="sxs-lookup"><span data-stu-id="a5f1c-111">pending</span></span>|<span data-ttu-id="a5f1c-112">0</span><span class="sxs-lookup"><span data-stu-id="a5f1c-112">0</span></span>|<span data-ttu-id="a5f1c-113">Anforderung wartet auf Verarbeitung oder Bearbeitung</span><span class="sxs-lookup"><span data-stu-id="a5f1c-113">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="a5f1c-114">abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="a5f1c-114">completed</span></span>|<span data-ttu-id="a5f1c-115">1</span><span class="sxs-lookup"><span data-stu-id="a5f1c-115">1</span></span>|<span data-ttu-id="a5f1c-116">Die Anforderung wurde mit einer Datei in Azure BLOB zum Herunterladen hochgeladen.</span><span class="sxs-lookup"><span data-stu-id="a5f1c-116">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="a5f1c-117">failed</span><span class="sxs-lookup"><span data-stu-id="a5f1c-117">failed</span></span>|<span data-ttu-id="a5f1c-118">2</span><span class="sxs-lookup"><span data-stu-id="a5f1c-118">2</span></span>|<span data-ttu-id="a5f1c-119">Anforderungs fertige Verarbeitung und Fehlerstatus.</span><span class="sxs-lookup"><span data-stu-id="a5f1c-119">Request finished processing and in error state.</span></span>|




