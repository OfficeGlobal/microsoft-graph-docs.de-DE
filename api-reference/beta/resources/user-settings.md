---
title: Ressourcentyp Einstellungen
description: 'Den aktuellen benutzereinstellungen. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 208d232af609f92d5924267ae26831b9929e357a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521096"
---
# <a name="settings-resource-type"></a><span data-ttu-id="11ad5-103">Ressourcentyp Einstellungen</span><span class="sxs-lookup"><span data-stu-id="11ad5-103">settings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11ad5-104">Den aktuellen benutzereinstellungen.</span><span class="sxs-lookup"><span data-stu-id="11ad5-104">The current user settings.</span></span> <span data-ttu-id="11ad5-105">Informationen zum Abrufen oder Aktualisieren von benutzereinstellungen, finden Sie unter [Abrufen von Einstellungen](../api/user-get-settings.md) und [Einstellungen aktualisieren](../api/user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="11ad5-105">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="11ad5-106">Diese Ressource unterstützt Folgendes:</span><span class="sxs-lookup"><span data-stu-id="11ad5-106">This resource supports:</span></span>

- <span data-ttu-id="11ad5-107">Überprüfen, ob ein Benutzer und die Organisation des Benutzers zu Content-Erkennung beitragen.</span><span class="sxs-lookup"><span data-stu-id="11ad5-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="11ad5-108">Deaktivieren oder Aktivieren der Content-Erkennung für bestimmte Benutzer.</span><span class="sxs-lookup"><span data-stu-id="11ad5-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="11ad5-109">Dadurch wird deaktiviert, Dokumente in Office eingegangen wird.</span><span class="sxs-lookup"><span data-stu-id="11ad5-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="11ad5-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="11ad5-110">Methods</span></span>
| <span data-ttu-id="11ad5-111">Methode</span><span class="sxs-lookup"><span data-stu-id="11ad5-111">Method</span></span>       | <span data-ttu-id="11ad5-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="11ad5-112">Return Type</span></span>  |<span data-ttu-id="11ad5-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11ad5-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11ad5-114">Abrufen der Benutzereinstellungen</span><span class="sxs-lookup"><span data-stu-id="11ad5-114">[Get user settings](../api/user-get-settings.md)</span></span> |<span data-ttu-id="11ad5-115">[](../resources/user-settings.md) Einstellungen</span><span class="sxs-lookup"><span data-stu-id="11ad5-115">[settings](../resources/user-settings.md)</span></span>| <span data-ttu-id="11ad5-116">Rufen Sie die Einstellungen für Benutzer und Organisation.</span><span class="sxs-lookup"><span data-stu-id="11ad5-116">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="11ad5-117">Aktualisieren von benutzereinstellungen</span><span class="sxs-lookup"><span data-stu-id="11ad5-117">Update user settings</span></span>](../api/user-update-settings.md) |<span data-ttu-id="11ad5-118">[](../resources/user-settings.md) Einstellungen</span><span class="sxs-lookup"><span data-stu-id="11ad5-118">[settings](../resources/user-settings.md)</span></span>| <span data-ttu-id="11ad5-119">Aktualisieren Sie die aktuellen benutzereinstellungen.</span><span class="sxs-lookup"><span data-stu-id="11ad5-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="11ad5-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="11ad5-120">Properties</span></span>

| <span data-ttu-id="11ad5-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="11ad5-121">Property</span></span>     | <span data-ttu-id="11ad5-122">Typ</span><span class="sxs-lookup"><span data-stu-id="11ad5-122">Type</span></span>   |<span data-ttu-id="11ad5-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11ad5-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11ad5-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="11ad5-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="11ad5-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="11ad5-125">Boolean</span></span>|<span data-ttu-id="11ad5-126">Bei Festlegung auf "true", das Delegieren des Zugriffs für des Benutzers ist [Trend](insights-trending.md) API deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="11ad5-126">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="11ad5-127">Bei Festlegung auf true fest, Dokumente in des Benutzers Office eingegangen sind deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="11ad5-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="11ad5-128">Bei Festlegung auf "true", die Relevanz des Inhalts in Office 365, beispielsweise in vorgeschlagene in SharePoint – Startseite angezeigt, und die Ansicht Discover in OneDrive für Unternehmen betroffen ist.</span><span class="sxs-lookup"><span data-stu-id="11ad5-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="11ad5-129">Benutzer können diese Einstellung in [Office eingegangen](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)steuern.</span><span class="sxs-lookup"><span data-stu-id="11ad5-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="11ad5-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="11ad5-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="11ad5-131">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="11ad5-131">Boolean</span></span>|<span data-ttu-id="11ad5-132">Gilt für die [Einstellung der Organisation](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) Steuern des Zugriffs auf die [Trend](insights-trending.md) -API-Delegaten.</span><span class="sxs-lookup"><span data-stu-id="11ad5-132">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="11ad5-133">Wenn nicht auf True festgelegt, der Organisation auf Office eingegangen zugreifen kann.</span><span class="sxs-lookup"><span data-stu-id="11ad5-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="11ad5-134">Die Relevanz des Inhalts in Office 365, beispielsweise in vorgeschlagene in SharePoint-Startseite und in der Ansicht Discover in OneDrive für Unternehmen angezeigt, ist für die gesamte Organisation betroffen.</span><span class="sxs-lookup"><span data-stu-id="11ad5-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="11ad5-135">Diese Einstellung ist schreibgeschützt und kann nur von Administratoren in der [SharePoint-Verwaltungskonsole](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)geändert werden.</span><span class="sxs-lookup"><span data-stu-id="11ad5-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11ad5-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="11ad5-136">JSON representation</span></span>

<span data-ttu-id="11ad5-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="11ad5-137">Here is a JSON representation of the resource.</span></span>

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/user-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
