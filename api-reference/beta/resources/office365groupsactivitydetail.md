---
title: Ressourcentyp office365GroupsActivityDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2968a3a5459f286e4aac69e2fd606adc1b38e39b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951824"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="550fa-103">Ressourcentyp office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="550fa-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="550fa-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="550fa-104">Properties</span></span>

| <span data-ttu-id="550fa-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="550fa-105">Property</span></span>                          | <span data-ttu-id="550fa-106">Typ</span><span class="sxs-lookup"><span data-stu-id="550fa-106">Type</span></span>    | <span data-ttu-id="550fa-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="550fa-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="550fa-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="550fa-108">reportRefreshDate</span></span>                 | <span data-ttu-id="550fa-109">Datum</span><span class="sxs-lookup"><span data-stu-id="550fa-109">Date</span></span>    | <span data-ttu-id="550fa-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="550fa-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="550fa-111">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="550fa-111">groupDisplayName</span></span>                  | <span data-ttu-id="550fa-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="550fa-112">String</span></span>  | <span data-ttu-id="550fa-113">Der Anzeigename der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="550fa-113">The display name of the group.</span></span>           |
| <span data-ttu-id="550fa-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="550fa-114">isDeleted</span></span>                         | <span data-ttu-id="550fa-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="550fa-115">Boolean</span></span> | <span data-ttu-id="550fa-116">Ob dieser Benutzer gelöschte oder weiche wurde gelöscht.</span><span class="sxs-lookup"><span data-stu-id="550fa-116">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="550fa-117">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="550fa-117">ownerPrincipalName</span></span>                | <span data-ttu-id="550fa-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="550fa-118">String</span></span>  | <span data-ttu-id="550fa-119">Der Gruppe Besitzer principal Name.</span><span class="sxs-lookup"><span data-stu-id="550fa-119">The group owner principal name.</span></span>          |
| <span data-ttu-id="550fa-120">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="550fa-120">lastActivityDate</span></span>                  | <span data-ttu-id="550fa-121">Datum</span><span class="sxs-lookup"><span data-stu-id="550fa-121">Date</span></span>    | <span data-ttu-id="550fa-122">Datum der letzten Aktivität für die folgenden Szenarien: Postfach empfangene e-Mails; gruppieren Benutzer angezeigt, bearbeitet, freigegebene oder Dateien in SharePoint-Dokumentbibliothek synchronisiert; SharePoint-Seiten angezeigt; Benutzer gebucht, lesen oder gefallen Nachrichten in Yammer-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="550fa-122">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="550fa-123">groupType</span><span class="sxs-lookup"><span data-stu-id="550fa-123">groupType</span></span>                         | <span data-ttu-id="550fa-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="550fa-124">String</span></span>  | <span data-ttu-id="550fa-125">Der Gruppentyp.</span><span class="sxs-lookup"><span data-stu-id="550fa-125">The group type.</span></span> <span data-ttu-id="550fa-126">Mögliche Werte sind: **öffentlich** oder **Privat**.</span><span class="sxs-lookup"><span data-stu-id="550fa-126">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="550fa-127">memberCount</span><span class="sxs-lookup"><span data-stu-id="550fa-127">memberCount</span></span>                       | <span data-ttu-id="550fa-128">Int64</span><span class="sxs-lookup"><span data-stu-id="550fa-128">Int64</span></span>   | <span data-ttu-id="550fa-129">Die Gruppe Elementanzahl.</span><span class="sxs-lookup"><span data-stu-id="550fa-129">The group member count.</span></span>                  |
| <span data-ttu-id="550fa-130">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="550fa-130">externalMemberCount</span></span>               | <span data-ttu-id="550fa-131">Int64</span><span class="sxs-lookup"><span data-stu-id="550fa-131">Int64</span></span>   | <span data-ttu-id="550fa-132">Die Gruppe externe Elementanzahl.</span><span class="sxs-lookup"><span data-stu-id="550fa-132">The group external member count.</span></span>         |
| <span data-ttu-id="550fa-133">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="550fa-133">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="550fa-134">Int64</span><span class="sxs-lookup"><span data-stu-id="550fa-134">Int64</span></span>   | <span data-ttu-id="550fa-135">Die Anzahl der e-Mail, die das Gruppenpostfach empfangen.</span><span class="sxs-lookup"><span data-stu-id="550fa-135">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="550fa-136">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="550fa-136">sharePointActiveFileCount</span></span>         | <span data-ttu-id="550fa-137">Int64</span><span class="sxs-lookup"><span data-stu-id="550fa-137">Int64</span></span>   | <span data-ttu-id="550fa-138">Die Anzahl der aktiven Dateien in der Website der SharePoint-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="550fa-138">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="550fa-139">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="550fa-139">yammerPostedMessageCount</span></span>          | <span data-ttu-id="550fa-140">Int64</span><span class="sxs-lookup"><span data-stu-id="550fa-140">Int64</span></span>   | <span data-ttu-id="550fa-141">Die Anzahl von Nachrichten zu Yammer-Gruppen bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="550fa-141">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="550fa-142">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="550fa-142">yammerReadMessageCount</span></span>            | <span data-ttu-id="550fa-143">Int64</span><span class="sxs-lookup"><span data-stu-id="550fa-143">Int64</span></span>   | <span data-ttu-id="550fa-144">Lesen Sie die Anzahl der Nachrichten in Yammer-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="550fa-144">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="550fa-145">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="550fa-145">yammerLikedMessageCount</span></span>           | <span data-ttu-id="550fa-146">Int64</span><span class="sxs-lookup"><span data-stu-id="550fa-146">Int64</span></span>   | <span data-ttu-id="550fa-147">Die Anzahl der Nachrichten in Yammer-Gruppen gefallen.</span><span class="sxs-lookup"><span data-stu-id="550fa-147">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="550fa-148">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="550fa-148">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="550fa-149">Int64</span><span class="sxs-lookup"><span data-stu-id="550fa-149">Int64</span></span>   | <span data-ttu-id="550fa-150">Die Anzahl der Elemente in der Gruppenpostfach.</span><span class="sxs-lookup"><span data-stu-id="550fa-150">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="550fa-151">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="550fa-151">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="550fa-152">Int64</span><span class="sxs-lookup"><span data-stu-id="550fa-152">Int64</span></span>   | <span data-ttu-id="550fa-153">Der Speicher des Postfachs Gruppe verwendet.</span><span class="sxs-lookup"><span data-stu-id="550fa-153">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="550fa-154">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="550fa-154">sharePointTotalFileCount</span></span>          | <span data-ttu-id="550fa-155">Int64</span><span class="sxs-lookup"><span data-stu-id="550fa-155">Int64</span></span>   | <span data-ttu-id="550fa-156">Die Gesamtzahl der Dateien in der Website der SharePoint-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="550fa-156">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="550fa-157">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="550fa-157">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="550fa-158">Int64</span><span class="sxs-lookup"><span data-stu-id="550fa-158">Int64</span></span>   | <span data-ttu-id="550fa-159">Die Speicherung von SharePoint-Gruppe der Website verwendet.</span><span class="sxs-lookup"><span data-stu-id="550fa-159">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="550fa-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="550fa-160">reportPeriod</span></span>                      | <span data-ttu-id="550fa-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="550fa-161">String</span></span>  | <span data-ttu-id="550fa-162">Die Anzahl der Tage, die der Bericht wird behandelt.</span><span class="sxs-lookup"><span data-stu-id="550fa-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="550fa-163">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="550fa-163">JSON representation</span></span>

<span data-ttu-id="550fa-164">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="550fa-164">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "memberCount": 1024, 
  "externalMemberCount": 1024, 
  "exchangeReceivedEmailCount": 1024, 
  "sharePointActiveFileCount": 1024, 
  "yammerPostedMessageCount": 1024, 
  "yammerReadMessageCount": 1024, 
  "yammerLikedMessageCount": 1024, 
  "exchangeMailboxTotalItemCount": 1024, 
  "exchangeMailboxStorageUsedInBytes": 1024, 
  "sharePointTotalFileCount": 1024, 
  "sharePointSiteStorageUsedInBytes": 1024, 
  "reportPeriod": "String"
}
```
