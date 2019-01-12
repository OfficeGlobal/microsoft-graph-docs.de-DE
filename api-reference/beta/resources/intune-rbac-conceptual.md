---
title: Rollenbasierte Zugriffssteuerung in Microsoft Intune
description: 'Die rollenbasierte Zugriffskontrolle in Intune bestimmt, wer Aktionen für Intune-Objekte ausführen und Änderungen an verwalteten Anwendungen, Benutzern und Geräten vornehmen kann.   '
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: cbbd04aacd80c8ad3c3082505ab052e2bdd65cbe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924356"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="ca96c-103">Rollenbasierte Zugriffssteuerung in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ca96c-103">Role-based access control in Microsoft Intune</span></span>

> <span data-ttu-id="ca96c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ca96c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca96c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ca96c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca96c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="ca96c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="ca96c-107">Die rollenbasierte Zugriffskontrolle in Intune bestimmt, wer Aktionen für Intune-Objekte ausführen und Änderungen an verwalteten Anwendungen, Benutzern und Geräten vornehmen kann.</span><span class="sxs-lookup"><span data-stu-id="ca96c-107">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="ca96c-108">Die folgenden Graph-Ressourcen stehen zur Verfügung, um die rollenbasierte Zugriffskontrolle in Intune zu verwalten:</span><span class="sxs-lookup"><span data-stu-id="ca96c-108">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="ca96c-109">Gerät und app Management Role Ids zugewiesen</span><span class="sxs-lookup"><span data-stu-id="ca96c-109">Device and app management assigned role ids</span></span>](intune-rbac-deviceandappmanagementassignedroleids.md)
- [<span data-ttu-id="ca96c-110">Geräte- und App-Verwaltungsrollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="ca96c-110">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="ca96c-111">Geräte- und App-Verwaltungsrollendefinition</span><span class="sxs-lookup"><span data-stu-id="ca96c-111">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="ca96c-112">Ressourcenaktion</span><span class="sxs-lookup"><span data-stu-id="ca96c-112">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="ca96c-113">Ressourcenvorgang</span><span class="sxs-lookup"><span data-stu-id="ca96c-113">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="ca96c-114">Rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="ca96c-114">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="ca96c-115">Rollentyp Assignment-Bereich</span><span class="sxs-lookup"><span data-stu-id="ca96c-115">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="ca96c-116">Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="ca96c-116">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="ca96c-117">Rollenberechtigung</span><span class="sxs-lookup"><span data-stu-id="ca96c-117">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="ca96c-118">Rolle Bereich tag</span><span class="sxs-lookup"><span data-stu-id="ca96c-118">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
