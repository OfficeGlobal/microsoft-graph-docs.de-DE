---
title: AppLogUploadState Enum-Typ
description: AppLogUploadStatus
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 58dcc0d4a15370d6449772d917e8994f0eb9e7bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431576"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="9f620-103">AppLogUploadState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="9f620-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="9f620-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9f620-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9f620-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f620-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f620-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f620-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f620-107">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="9f620-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="9f620-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="9f620-108">Members</span></span>
|<span data-ttu-id="9f620-109">Member</span><span class="sxs-lookup"><span data-stu-id="9f620-109">Member</span></span>|<span data-ttu-id="9f620-110">Wert</span><span class="sxs-lookup"><span data-stu-id="9f620-110">Value</span></span>|<span data-ttu-id="9f620-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f620-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f620-112">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="9f620-112">pending</span></span>|<span data-ttu-id="9f620-113">0</span><span class="sxs-lookup"><span data-stu-id="9f620-113">0</span></span>|<span data-ttu-id="9f620-114">Anforderung wird wartet auf Verarbeitung oder unter verarbeitet</span><span class="sxs-lookup"><span data-stu-id="9f620-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="9f620-115">abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="9f620-115">completed</span></span>|<span data-ttu-id="9f620-116">1</span><span class="sxs-lookup"><span data-stu-id="9f620-116">1</span></span>|<span data-ttu-id="9f620-117">Anforderung wird mit der Datei hochgeladen in Azure Blob für den Download abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="9f620-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="9f620-118">failed</span><span class="sxs-lookup"><span data-stu-id="9f620-118">failed</span></span>|<span data-ttu-id="9f620-119">2</span><span class="sxs-lookup"><span data-stu-id="9f620-119">2</span></span>|<span data-ttu-id="9f620-120">Anforderung beendet Verarbeitung und Fehlerzustand.</span><span class="sxs-lookup"><span data-stu-id="9f620-120">Request finished processing and in error state.</span></span>|




