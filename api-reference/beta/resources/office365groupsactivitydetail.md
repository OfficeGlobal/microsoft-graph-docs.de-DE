---
title: Ressourcentyp office365GroupsActivityDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: a849932d646be61f3cedec76ecdafdaca941baaf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058919"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="743fd-103">Ressourcentyp office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="743fd-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="743fd-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="743fd-104">Properties</span></span>

| <span data-ttu-id="743fd-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="743fd-105">Property</span></span>                          | <span data-ttu-id="743fd-106">Typ</span><span class="sxs-lookup"><span data-stu-id="743fd-106">Type</span></span>    | <span data-ttu-id="743fd-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="743fd-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="743fd-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="743fd-108">reportRefreshDate</span></span>                 | <span data-ttu-id="743fd-109">Datum</span><span class="sxs-lookup"><span data-stu-id="743fd-109">Date</span></span>    | <span data-ttu-id="743fd-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="743fd-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="743fd-111">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="743fd-111">groupDisplayName</span></span>                  | <span data-ttu-id="743fd-112">String</span><span class="sxs-lookup"><span data-stu-id="743fd-112">String</span></span>  | <span data-ttu-id="743fd-113">Der Anzeigename der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="743fd-113">The display name of the group.</span></span>           |
| <span data-ttu-id="743fd-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="743fd-114">isDeleted</span></span>                         | <span data-ttu-id="743fd-115">Boolesch</span><span class="sxs-lookup"><span data-stu-id="743fd-115">Boolean</span></span> | <span data-ttu-id="743fd-116">Ob dieser Benutzer gelöschte oder weiche wurde gelöscht.</span><span class="sxs-lookup"><span data-stu-id="743fd-116">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="743fd-117">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="743fd-117">ownerPrincipalName</span></span>                | <span data-ttu-id="743fd-118">String</span><span class="sxs-lookup"><span data-stu-id="743fd-118">String</span></span>  | <span data-ttu-id="743fd-119">Der Gruppe Besitzer principal Name.</span><span class="sxs-lookup"><span data-stu-id="743fd-119">The group owner principal name.</span></span>          |
| <span data-ttu-id="743fd-120">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="743fd-120">lastActivityDate</span></span>                  | <span data-ttu-id="743fd-121">Datum</span><span class="sxs-lookup"><span data-stu-id="743fd-121">Date</span></span>    | <span data-ttu-id="743fd-122">Datum der letzten Aktivität für die folgenden Szenarien: Postfach empfangene e-Mails; gruppieren Benutzer angezeigt, bearbeitet, freigegebene oder Dateien in SharePoint-Dokumentbibliothek synchronisiert; SharePoint-Seiten angezeigt; Benutzer gebucht, lesen oder gefallen Nachrichten in Yammer-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="743fd-122">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="743fd-123">groupType</span><span class="sxs-lookup"><span data-stu-id="743fd-123">groupType</span></span>                         | <span data-ttu-id="743fd-124">String</span><span class="sxs-lookup"><span data-stu-id="743fd-124">String</span></span>  | <span data-ttu-id="743fd-125">Der Gruppentyp.</span><span class="sxs-lookup"><span data-stu-id="743fd-125">The group type.</span></span> <span data-ttu-id="743fd-126">Mögliche Werte sind: **öffentlich** oder **Privat**.</span><span class="sxs-lookup"><span data-stu-id="743fd-126">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="743fd-127">memberCount</span><span class="sxs-lookup"><span data-stu-id="743fd-127">memberCount</span></span>                       | <span data-ttu-id="743fd-128">Int64</span><span class="sxs-lookup"><span data-stu-id="743fd-128">Int64</span></span>   | <span data-ttu-id="743fd-129">Die Gruppe Elementanzahl.</span><span class="sxs-lookup"><span data-stu-id="743fd-129">The group member count.</span></span>                  |
| <span data-ttu-id="743fd-130">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="743fd-130">externalMemberCount</span></span>               | <span data-ttu-id="743fd-131">Int64</span><span class="sxs-lookup"><span data-stu-id="743fd-131">Int64</span></span>   | <span data-ttu-id="743fd-132">Die Gruppe externe Elementanzahl.</span><span class="sxs-lookup"><span data-stu-id="743fd-132">The group external member count.</span></span>         |
| <span data-ttu-id="743fd-133">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="743fd-133">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="743fd-134">Int64</span><span class="sxs-lookup"><span data-stu-id="743fd-134">Int64</span></span>   | <span data-ttu-id="743fd-135">Die Anzahl der e-Mail, die das Gruppenpostfach empfangen.</span><span class="sxs-lookup"><span data-stu-id="743fd-135">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="743fd-136">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="743fd-136">sharePointActiveFileCount</span></span>         | <span data-ttu-id="743fd-137">Int64</span><span class="sxs-lookup"><span data-stu-id="743fd-137">Int64</span></span>   | <span data-ttu-id="743fd-138">Die Anzahl der aktiven Dateien in der Website der SharePoint-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="743fd-138">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="743fd-139">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="743fd-139">yammerPostedMessageCount</span></span>          | <span data-ttu-id="743fd-140">Int64</span><span class="sxs-lookup"><span data-stu-id="743fd-140">Int64</span></span>   | <span data-ttu-id="743fd-141">Die Anzahl von Nachrichten zu Yammer-Gruppen bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="743fd-141">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="743fd-142">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="743fd-142">yammerReadMessageCount</span></span>            | <span data-ttu-id="743fd-143">Int64</span><span class="sxs-lookup"><span data-stu-id="743fd-143">Int64</span></span>   | <span data-ttu-id="743fd-144">Lesen Sie die Anzahl der Nachrichten in Yammer-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="743fd-144">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="743fd-145">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="743fd-145">yammerLikedMessageCount</span></span>           | <span data-ttu-id="743fd-146">Int64</span><span class="sxs-lookup"><span data-stu-id="743fd-146">Int64</span></span>   | <span data-ttu-id="743fd-147">Die Anzahl der Nachrichten in Yammer-Gruppen gefallen.</span><span class="sxs-lookup"><span data-stu-id="743fd-147">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="743fd-148">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="743fd-148">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="743fd-149">Int64</span><span class="sxs-lookup"><span data-stu-id="743fd-149">Int64</span></span>   | <span data-ttu-id="743fd-150">Die Anzahl der Elemente in der Gruppenpostfach.</span><span class="sxs-lookup"><span data-stu-id="743fd-150">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="743fd-151">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="743fd-151">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="743fd-152">Int64</span><span class="sxs-lookup"><span data-stu-id="743fd-152">Int64</span></span>   | <span data-ttu-id="743fd-153">Der Speicher des Postfachs Gruppe verwendet.</span><span class="sxs-lookup"><span data-stu-id="743fd-153">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="743fd-154">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="743fd-154">sharePointTotalFileCount</span></span>          | <span data-ttu-id="743fd-155">Int64</span><span class="sxs-lookup"><span data-stu-id="743fd-155">Int64</span></span>   | <span data-ttu-id="743fd-156">Die Gesamtzahl der Dateien in der Website der SharePoint-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="743fd-156">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="743fd-157">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="743fd-157">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="743fd-158">Int64</span><span class="sxs-lookup"><span data-stu-id="743fd-158">Int64</span></span>   | <span data-ttu-id="743fd-159">Die Speicherung von SharePoint-Gruppe der Website verwendet.</span><span class="sxs-lookup"><span data-stu-id="743fd-159">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="743fd-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="743fd-160">reportPeriod</span></span>                      | <span data-ttu-id="743fd-161">String</span><span class="sxs-lookup"><span data-stu-id="743fd-161">String</span></span>  | <span data-ttu-id="743fd-162">Die Anzahl der Tage, die der Bericht wird behandelt.</span><span class="sxs-lookup"><span data-stu-id="743fd-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="743fd-163">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="743fd-163">JSON representation</span></span>

<span data-ttu-id="743fd-164">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="743fd-164">The following is a JSON representation of the resource.</span></span>

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
