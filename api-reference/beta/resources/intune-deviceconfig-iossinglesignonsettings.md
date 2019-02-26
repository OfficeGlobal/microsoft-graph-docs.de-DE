---
title: iosSingleSignOnSettings-Ressourcentyp
description: iOS-Kerberos-Authentifizierungseinstellungen für einmaliges Anmelden
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b438ea8fadc30a0bf5fa3786e9b4cec3344093c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142623"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="123be-103">iosSingleSignOnSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="123be-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="123be-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="123be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="123be-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="123be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="123be-106">iOS-Kerberos-Authentifizierungseinstellungen für einmaliges Anmelden</span><span class="sxs-lookup"><span data-stu-id="123be-106">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="123be-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="123be-107">Properties</span></span>
|<span data-ttu-id="123be-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="123be-108">Property</span></span>|<span data-ttu-id="123be-109">Typ</span><span class="sxs-lookup"><span data-stu-id="123be-109">Type</span></span>|<span data-ttu-id="123be-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="123be-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="123be-111">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="123be-111">allowedAppsList</span></span>|<span data-ttu-id="123be-112">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="123be-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="123be-113">Liste der APP-IDs, die diese Anmeldung verwenden dürfen.</span><span class="sxs-lookup"><span data-stu-id="123be-113">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="123be-114">Wenn dieses Feld nicht angegeben wird, gilt die Anmeldung für alle Anwendungen auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="123be-114">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="123be-115">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="123be-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="123be-116">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="123be-116">allowedUrls</span></span>|<span data-ttu-id="123be-117">String collection</span><span class="sxs-lookup"><span data-stu-id="123be-117">String collection</span></span>|<span data-ttu-id="123be-118">Liste der HTTP-URLs, die abgeglichen werden müssen, um diese Anmeldung zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="123be-118">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="123be-119">Mit iOS 9,0 oder höher können Platzhalterzeichen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="123be-119">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="123be-120">displayName</span><span class="sxs-lookup"><span data-stu-id="123be-120">displayName</span></span>|<span data-ttu-id="123be-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="123be-121">String</span></span>|<span data-ttu-id="123be-122">Der Anzeigename der Anmeldeeinstellungen, die auf dem empfangenden Gerät angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="123be-122">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="123be-123">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="123be-123">kerberosPrincipalName</span></span>|<span data-ttu-id="123be-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="123be-124">String</span></span>|<span data-ttu-id="123be-125">Ein Kerberos-Prinzipalname.</span><span class="sxs-lookup"><span data-stu-id="123be-125">A Kerberos principal name.</span></span> <span data-ttu-id="123be-126">Wenn nicht angegeben, wird der Benutzer während der Profilinstallation zur Eingabe eines Eintrags aufgefordert.</span><span class="sxs-lookup"><span data-stu-id="123be-126">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="123be-127">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="123be-127">kerberosRealm</span></span>|<span data-ttu-id="123be-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="123be-128">String</span></span>|<span data-ttu-id="123be-129">Ein Kerberos-Bereichsname.</span><span class="sxs-lookup"><span data-stu-id="123be-129">A Kerberos realm name.</span></span> <span data-ttu-id="123be-130">Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="123be-130">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="123be-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="123be-131">Relationships</span></span>
<span data-ttu-id="123be-132">Keine</span><span class="sxs-lookup"><span data-stu-id="123be-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="123be-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="123be-133">JSON Representation</span></span>
<span data-ttu-id="123be-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="123be-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```




