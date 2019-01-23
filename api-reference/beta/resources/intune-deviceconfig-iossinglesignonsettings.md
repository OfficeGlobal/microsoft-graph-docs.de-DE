---
title: Ressourcentyp iosSingleSignOnSettings
description: iOS Kerberos-Authentifizierungseinstellungen für einmaliges Anmelden
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 189fb79be741bdf6b731b1e3c2b336934db8c86b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421319"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="667f9-103">Ressourcentyp iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="667f9-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="667f9-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="667f9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="667f9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="667f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="667f9-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="667f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="667f9-107">iOS Kerberos-Authentifizierungseinstellungen für einmaliges Anmelden</span><span class="sxs-lookup"><span data-stu-id="667f9-107">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="667f9-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="667f9-108">Properties</span></span>
|<span data-ttu-id="667f9-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="667f9-109">Property</span></span>|<span data-ttu-id="667f9-110">Typ</span><span class="sxs-lookup"><span data-stu-id="667f9-110">Type</span></span>|<span data-ttu-id="667f9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="667f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="667f9-112">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="667f9-112">allowedAppsList</span></span>|<span data-ttu-id="667f9-113">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="667f9-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="667f9-114">Liste der app-Bezeichner, die dieser Anmeldung verwenden dürfen.</span><span class="sxs-lookup"><span data-stu-id="667f9-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="667f9-115">Wenn dieses Feld nicht angegeben wird, gilt die Anmeldung auf alle Programme, auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="667f9-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="667f9-116">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="667f9-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="667f9-117">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="667f9-117">allowedUrls</span></span>|<span data-ttu-id="667f9-118">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="667f9-118">String collection</span></span>|<span data-ttu-id="667f9-119">Liste der HTTP-URLs, die übereinstimmen muss, um diesen Benutzernamen verwenden.</span><span class="sxs-lookup"><span data-stu-id="667f9-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="667f9-120">IOS 9.0 oder höher können ein Platzhalterzeichen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="667f9-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="667f9-121">displayName</span><span class="sxs-lookup"><span data-stu-id="667f9-121">displayName</span></span>|<span data-ttu-id="667f9-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="667f9-122">String</span></span>|<span data-ttu-id="667f9-123">Der Anzeigename der Einstellungen für die Anmeldung auf dem empfangenden Gerät angezeigt.</span><span class="sxs-lookup"><span data-stu-id="667f9-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="667f9-124">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="667f9-124">kerberosPrincipalName</span></span>|<span data-ttu-id="667f9-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="667f9-125">String</span></span>|<span data-ttu-id="667f9-126">Ein Kerberos principal Name.</span><span class="sxs-lookup"><span data-stu-id="667f9-126">A Kerberos principal name.</span></span> <span data-ttu-id="667f9-127">Wenn nicht angegeben, wird der Benutzer während der Profilinstallation dazu aufgefordert.</span><span class="sxs-lookup"><span data-stu-id="667f9-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="667f9-128">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="667f9-128">kerberosRealm</span></span>|<span data-ttu-id="667f9-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="667f9-129">String</span></span>|<span data-ttu-id="667f9-130">Ein Kerberos-Realm-Name.</span><span class="sxs-lookup"><span data-stu-id="667f9-130">A Kerberos realm name.</span></span> <span data-ttu-id="667f9-131">Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="667f9-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="667f9-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="667f9-132">Relationships</span></span>
<span data-ttu-id="667f9-133">Keine</span><span class="sxs-lookup"><span data-stu-id="667f9-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="667f9-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="667f9-134">JSON Representation</span></span>
<span data-ttu-id="667f9-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="667f9-135">Here is a JSON representation of the resource.</span></span>
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




