---
title: Ressourcentyp iosSingleSignOnSettings
description: iOS Kerberos-Authentifizierungseinstellungen für einmaliges Anmelden
author: tfitzmac
ms.openlocfilehash: 6bde13865c1d6b34c433a92005681b247b99d984
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347369"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="2020f-103">Ressourcentyp iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="2020f-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="2020f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2020f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2020f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2020f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2020f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2020f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2020f-107">iOS Kerberos-Authentifizierungseinstellungen für einmaliges Anmelden</span><span class="sxs-lookup"><span data-stu-id="2020f-107">iOS Kerberos authentication settings for single sign-on</span></span>
## <a name="properties"></a><span data-ttu-id="2020f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2020f-108">Properties</span></span>
|<span data-ttu-id="2020f-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2020f-109">Property</span></span>|<span data-ttu-id="2020f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="2020f-110">Type</span></span>|<span data-ttu-id="2020f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2020f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2020f-112">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="2020f-112">allowedAppsList</span></span>|<span data-ttu-id="2020f-113">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="2020f-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="2020f-114">Liste der app-Bezeichner, die dieser Anmeldung verwenden dürfen.</span><span class="sxs-lookup"><span data-stu-id="2020f-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="2020f-115">Wenn dieses Feld nicht angegeben wird, gilt die Anmeldung auf alle Programme, auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="2020f-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="2020f-116">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="2020f-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2020f-117">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="2020f-117">allowedUrls</span></span>|<span data-ttu-id="2020f-118">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="2020f-118">String collection</span></span>|<span data-ttu-id="2020f-119">Liste der HTTP-URLs, die übereinstimmen muss, um diesen Benutzernamen verwenden.</span><span class="sxs-lookup"><span data-stu-id="2020f-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="2020f-120">IOS 9.0 oder höher können ein Platzhalterzeichen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="2020f-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="2020f-121">displayName</span><span class="sxs-lookup"><span data-stu-id="2020f-121">displayName</span></span>|<span data-ttu-id="2020f-122">String</span><span class="sxs-lookup"><span data-stu-id="2020f-122">String</span></span>|<span data-ttu-id="2020f-123">Der Anzeigename der Einstellungen für die Anmeldung auf dem empfangenden Gerät angezeigt.</span><span class="sxs-lookup"><span data-stu-id="2020f-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="2020f-124">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2020f-124">kerberosPrincipalName</span></span>|<span data-ttu-id="2020f-125">String</span><span class="sxs-lookup"><span data-stu-id="2020f-125">String</span></span>|<span data-ttu-id="2020f-126">Ein Kerberos principal Name.</span><span class="sxs-lookup"><span data-stu-id="2020f-126">A Kerberos principal name.</span></span> <span data-ttu-id="2020f-127">Wenn nicht angegeben, wird der Benutzer während der Profilinstallation dazu aufgefordert.</span><span class="sxs-lookup"><span data-stu-id="2020f-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="2020f-128">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="2020f-128">kerberosRealm</span></span>|<span data-ttu-id="2020f-129">String</span><span class="sxs-lookup"><span data-stu-id="2020f-129">String</span></span>|<span data-ttu-id="2020f-130">Ein Kerberos-Realm-Name.</span><span class="sxs-lookup"><span data-stu-id="2020f-130">A Kerberos realm name.</span></span> <span data-ttu-id="2020f-131">Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="2020f-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2020f-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2020f-132">Relationships</span></span>
<span data-ttu-id="2020f-133">Keine</span><span class="sxs-lookup"><span data-stu-id="2020f-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2020f-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2020f-134">JSON Representation</span></span>
<span data-ttu-id="2020f-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2020f-135">Here is a JSON representation of the resource.</span></span>
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





