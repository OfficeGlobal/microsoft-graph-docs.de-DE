---
title: Rollenbasierte Zugriffssteuerung in Microsoft Intune
description: Listet die Microsoft Graph-API für InTune-Endpunkte (REST) auf, die die rollenbasierte Zugriffssteuerung (Role-Based Access Control, RBAC) für eine mandantenorganisation definieren und verwalten.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 24280426585014f5e397dab39daa71f8930b26c4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160676"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="02a74-103">Rollenbasierte Zugriffssteuerung in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="02a74-103">Role-based access control in Microsoft Intune</span></span>

> <span data-ttu-id="02a74-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="02a74-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02a74-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02a74-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02a74-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="02a74-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="02a74-107">Die rollenbasierte Zugriffskontrolle in Intune bestimmt, wer Aktionen für Intune-Objekte ausführen und Änderungen an verwalteten Anwendungen, Benutzern und Geräten vornehmen kann.</span><span class="sxs-lookup"><span data-stu-id="02a74-107">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="02a74-108">Die folgenden Graph-Ressourcen stehen zur Verfügung, um die rollenbasierte Zugriffskontrolle in Intune zu verwalten:</span><span class="sxs-lookup"><span data-stu-id="02a74-108">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="02a74-109">Geräte- und App-Verwaltung – zugewiesene Rolle – Details</span><span class="sxs-lookup"><span data-stu-id="02a74-109">Device and app management assigned role details</span></span>](intune-rbac-deviceandappmanagementassignedroledetails.md)
- [<span data-ttu-id="02a74-110">Geräte- und App-Verwaltungsrollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="02a74-110">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="02a74-111">Geräte- und App-Verwaltungsrollendefinition</span><span class="sxs-lookup"><span data-stu-id="02a74-111">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="02a74-112">Ressourcenaktion</span><span class="sxs-lookup"><span data-stu-id="02a74-112">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="02a74-113">Ressourcenvorgang</span><span class="sxs-lookup"><span data-stu-id="02a74-113">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="02a74-114">Rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="02a74-114">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="02a74-115">Bereichstyp der Rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="02a74-115">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="02a74-116">Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="02a74-116">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="02a74-117">Rollenberechtigung</span><span class="sxs-lookup"><span data-stu-id="02a74-117">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="02a74-118">Rollenbereichsmarkierung</span><span class="sxs-lookup"><span data-stu-id="02a74-118">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
