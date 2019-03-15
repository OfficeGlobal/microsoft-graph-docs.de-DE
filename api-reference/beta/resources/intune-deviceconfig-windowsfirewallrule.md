---
title: windowsFirewallRule-Ressourcentyp
description: Eine Regel, die den Datenverkehr über die Windows-Firewall steuert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3753eeade1dce32e4332becd7575710a2f6ea1a
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30631539"
---
# <a name="windowsfirewallrule-resource-type"></a><span data-ttu-id="df0a9-103">windowsFirewallRule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="df0a9-103">windowsFirewallRule resource type</span></span>

> <span data-ttu-id="df0a9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df0a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df0a9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="df0a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df0a9-106">Eine Regel, die den Datenverkehr über die Windows-Firewall steuert.</span><span class="sxs-lookup"><span data-stu-id="df0a9-106">A rule controlling traffic through the Windows Firewall.</span></span>

## <a name="properties"></a><span data-ttu-id="df0a9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="df0a9-107">Properties</span></span>
|<span data-ttu-id="df0a9-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="df0a9-108">Property</span></span>|<span data-ttu-id="df0a9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="df0a9-109">Type</span></span>|<span data-ttu-id="df0a9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df0a9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df0a9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="df0a9-111">displayName</span></span>|<span data-ttu-id="df0a9-112">String</span><span class="sxs-lookup"><span data-stu-id="df0a9-112">String</span></span>|<span data-ttu-id="df0a9-113">Der Anzeigename der Regel.</span><span class="sxs-lookup"><span data-stu-id="df0a9-113">The display name of the rule.</span></span> <span data-ttu-id="df0a9-114">Muss nicht eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="df0a9-114">Does not need to be unique.</span></span>|
|<span data-ttu-id="df0a9-115">description</span><span class="sxs-lookup"><span data-stu-id="df0a9-115">description</span></span>|<span data-ttu-id="df0a9-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df0a9-116">String</span></span>|<span data-ttu-id="df0a9-117">Die Beschreibung der Regel.</span><span class="sxs-lookup"><span data-stu-id="df0a9-117">The description of the rule.</span></span>|
|<span data-ttu-id="df0a9-118">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="df0a9-118">packageFamilyName</span></span>|<span data-ttu-id="df0a9-119">String</span><span class="sxs-lookup"><span data-stu-id="df0a9-119">String</span></span>|<span data-ttu-id="df0a9-120">Der Name der paketfamilie einer Microsoft Store-Anwendung, die von der Firewallregel betroffen ist.</span><span class="sxs-lookup"><span data-stu-id="df0a9-120">The package family name of a Microsoft Store application that's affected by the firewall rule.</span></span>|
|<span data-ttu-id="df0a9-121">filePath</span><span class="sxs-lookup"><span data-stu-id="df0a9-121">filePath</span></span>|<span data-ttu-id="df0a9-122">String</span><span class="sxs-lookup"><span data-stu-id="df0a9-122">String</span></span>|<span data-ttu-id="df0a9-123">Der vollständige Dateipfad einer APP, die von der Firewallregel betroffen ist.</span><span class="sxs-lookup"><span data-stu-id="df0a9-123">The full file path of an app that's affected by the firewall rule.</span></span>|
|<span data-ttu-id="df0a9-124">Wert Service Name</span><span class="sxs-lookup"><span data-stu-id="df0a9-124">serviceName</span></span>|<span data-ttu-id="df0a9-125">String</span><span class="sxs-lookup"><span data-stu-id="df0a9-125">String</span></span>|<span data-ttu-id="df0a9-126">Der Name, der in Fällen verwendet wird, in denen ein Dienst, nicht eine Anwendung, Datenverkehr sendet oder empfängt.</span><span class="sxs-lookup"><span data-stu-id="df0a9-126">The name used in cases when a service, not an application, is sending or receiving traffic.</span></span>|
|<span data-ttu-id="df0a9-127">Protokoll</span><span class="sxs-lookup"><span data-stu-id="df0a9-127">protocol</span></span>|<span data-ttu-id="df0a9-128">Int32</span><span class="sxs-lookup"><span data-stu-id="df0a9-128">Int32</span></span>|<span data-ttu-id="df0a9-129">0-255 Zahl, die das IP-Protokoll (TCP = 6, UDP = 17) darstellt.</span><span class="sxs-lookup"><span data-stu-id="df0a9-129">0-255 number representing the IP protocol (TCP = 6, UDP = 17).</span></span> <span data-ttu-id="df0a9-130">Wenn nicht angegeben, ist der Standardwert all.</span><span class="sxs-lookup"><span data-stu-id="df0a9-130">If not specified, the default is All.</span></span> <span data-ttu-id="df0a9-131">Gültige Werte 0 bis 255</span><span class="sxs-lookup"><span data-stu-id="df0a9-131">Valid values 0 to 255</span></span>|
|<span data-ttu-id="df0a9-132">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="df0a9-132">localPortRanges</span></span>|<span data-ttu-id="df0a9-133">String collection</span><span class="sxs-lookup"><span data-stu-id="df0a9-133">String collection</span></span>|<span data-ttu-id="df0a9-134">Liste der lokalen Portierungs Bereiche.</span><span class="sxs-lookup"><span data-stu-id="df0a9-134">List of local port ranges.</span></span> <span data-ttu-id="df0a9-135">Beispiel: "100-120", "200", "300-320".</span><span class="sxs-lookup"><span data-stu-id="df0a9-135">For example, "100-120", "200", "300-320".</span></span> <span data-ttu-id="df0a9-136">Wenn nicht angegeben, ist der Standardwert all.</span><span class="sxs-lookup"><span data-stu-id="df0a9-136">If not specified, the default is All.</span></span>|
|<span data-ttu-id="df0a9-137">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="df0a9-137">remotePortRanges</span></span>|<span data-ttu-id="df0a9-138">String collection</span><span class="sxs-lookup"><span data-stu-id="df0a9-138">String collection</span></span>|<span data-ttu-id="df0a9-139">Liste der Remote-Portierungs Bereiche.</span><span class="sxs-lookup"><span data-stu-id="df0a9-139">List of remote port ranges.</span></span> <span data-ttu-id="df0a9-140">Beispiel: "100-120", "200", "300-320".</span><span class="sxs-lookup"><span data-stu-id="df0a9-140">For example, "100-120", "200", "300-320".</span></span> <span data-ttu-id="df0a9-141">Wenn nicht angegeben, ist der Standardwert all.</span><span class="sxs-lookup"><span data-stu-id="df0a9-141">If not specified, the default is All.</span></span>|
|<span data-ttu-id="df0a9-142">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="df0a9-142">localAddressRanges</span></span>|<span data-ttu-id="df0a9-143">String collection</span><span class="sxs-lookup"><span data-stu-id="df0a9-143">String collection</span></span>|<span data-ttu-id="df0a9-144">Liste der lokalen Adressen, die von der Regel abgedeckt werden.</span><span class="sxs-lookup"><span data-stu-id="df0a9-144">List of local addresses covered by the rule.</span></span> <span data-ttu-id="df0a9-145">Gültige Token sind:</span><span class="sxs-lookup"><span data-stu-id="df0a9-145">Valid tokens include:</span></span>
- <span data-ttu-id="df0a9-146">"\*" gibt eine beliebige lokale Adresse an.</span><span class="sxs-lookup"><span data-stu-id="df0a9-146">"\*" indicates any local address.</span></span> <span data-ttu-id="df0a9-147">Falls vorhanden, muss es sich dabei um das einzige Token handeln, das enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="df0a9-147">If present, this must be the only token included.</span></span>
- <span data-ttu-id="df0a9-148">Ein Subnetz kann entweder mit der Subnetzmaske oder mit der Netzwerkpräfix Notation angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="df0a9-148">A subnet can be specified using either the subnet mask or network prefix notation.</span></span> <span data-ttu-id="df0a9-149">Wenn weder eine Subnetzmaske noch ein Netzwerkpräfix angegeben wird, ist die Subnetzmaske standardmäßig 255.255.255.255.</span><span class="sxs-lookup"><span data-stu-id="df0a9-149">If neither a subnet mask nor a network prefix is specified, the subnet mask defaults to 255.255.255.255.</span></span>
- <span data-ttu-id="df0a9-150">Eine gültige IPv6-Adresse.</span><span class="sxs-lookup"><span data-stu-id="df0a9-150">A valid IPv6 address.</span></span>
- <span data-ttu-id="df0a9-151">Ein IPv4-Adressbereich im Format "Start address-End Address" ohne Leerzeichen.</span><span class="sxs-lookup"><span data-stu-id="df0a9-151">An IPv4 address range in the format of "start address - end address" with no spaces included.</span></span>
- <span data-ttu-id="df0a9-152">Ein IPv6-Adressbereich im Format "Start address-End Address" ohne Leerzeichen.</span><span class="sxs-lookup"><span data-stu-id="df0a9-152">An IPv6 address range in the format of "start address - end address" with no spaces included.</span></span>
<span data-ttu-id="df0a9-153">Default ist eine beliebige Adresse. | | remoteAddressRanges | Zeichenfolgensammlung | Liste der Token, die die von der Regel abgedeckten Remoteadressen angeben.</span><span class="sxs-lookup"><span data-stu-id="df0a9-153">Default is any address.| |remoteAddressRanges|String collection|List of tokens specifying the remote addresses covered by the rule.</span></span> <span data-ttu-id="df0a9-154">Bei Token wird die Groß-/Kleinschreibung nicht beachtet.</span><span class="sxs-lookup"><span data-stu-id="df0a9-154">Tokens are case insensitive.</span></span> <span data-ttu-id="df0a9-155">Gültige Token sind:</span><span class="sxs-lookup"><span data-stu-id="df0a9-155">Valid tokens include:</span></span>
- <span data-ttu-id="df0a9-156">"\*" gibt eine beliebige Remoteadresse an.</span><span class="sxs-lookup"><span data-stu-id="df0a9-156">"\*" indicates any remote address.</span></span> <span data-ttu-id="df0a9-157">Falls vorhanden, muss es sich dabei um das einzige Token handeln, das enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="df0a9-157">If present, this must be the only token included.</span></span>
- <span data-ttu-id="df0a9-158">DefaultGateway</span><span class="sxs-lookup"><span data-stu-id="df0a9-158">"Defaultgateway"</span></span>
- <span data-ttu-id="df0a9-159">DHCP</span><span class="sxs-lookup"><span data-stu-id="df0a9-159">"DHCP"</span></span>
- <span data-ttu-id="df0a9-160">DNS</span><span class="sxs-lookup"><span data-stu-id="df0a9-160">"DNS"</span></span>
- <span data-ttu-id="df0a9-161">GEWINNT</span><span class="sxs-lookup"><span data-stu-id="df0a9-161">"WINS"</span></span>
- <span data-ttu-id="df0a9-162">"Intranet" (unter Windows-Versionen 1809 und höher)</span><span class="sxs-lookup"><span data-stu-id="df0a9-162">"Intranet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="df0a9-163">"RmtIntranet" (unter Windows-Versionen 1809 und höher)</span><span class="sxs-lookup"><span data-stu-id="df0a9-163">"RmtIntranet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="df0a9-164">"Internet" (unter Windows-Versionen 1809 und höher)</span><span class="sxs-lookup"><span data-stu-id="df0a9-164">"Internet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="df0a9-165">"Ply2Renders" (unter Windows-Versionen 1809 und höher)</span><span class="sxs-lookup"><span data-stu-id="df0a9-165">"Ply2Renders" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="df0a9-166">"LocalSubnet" gibt eine beliebige lokale Adresse im lokalen Subnetz an.</span><span class="sxs-lookup"><span data-stu-id="df0a9-166">"LocalSubnet" indicates any local address on the local subnet.</span></span>
- <span data-ttu-id="df0a9-167">Ein Subnetz kann entweder mit der Subnetzmaske oder mit der Netzwerkpräfix Notation angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="df0a9-167">A subnet can be specified using either the subnet mask or network prefix notation.</span></span> <span data-ttu-id="df0a9-168">Wenn weder eine Subnetzmaske noch ein Netzwerkpräfix angegeben wird, ist die Subnetzmaske standardmäßig 255.255.255.255.</span><span class="sxs-lookup"><span data-stu-id="df0a9-168">If neither a subnet mask nor a network prefix is specified, the subnet mask defaults to 255.255.255.255.</span></span>
- <span data-ttu-id="df0a9-169">Eine gültige IPv6-Adresse.</span><span class="sxs-lookup"><span data-stu-id="df0a9-169">A valid IPv6 address.</span></span>
- <span data-ttu-id="df0a9-170">Ein IPv4-Adressbereich im Format "Start address-End Address" ohne Leerzeichen.</span><span class="sxs-lookup"><span data-stu-id="df0a9-170">An IPv4 address range in the format of "start address - end address" with no spaces included.</span></span>
- <span data-ttu-id="df0a9-171">Ein IPv6-Adressbereich im Format "Start address-End Address" ohne Leerzeichen.</span><span class="sxs-lookup"><span data-stu-id="df0a9-171">An IPv6 address range in the format of "start address - end address" with no spaces included.</span></span>
<span data-ttu-id="df0a9-172">Default ist eine beliebige Adresse. | | profileTypes | [windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)| Gibt die Profile an, zu denen die Regel gehört.</span><span class="sxs-lookup"><span data-stu-id="df0a9-172">Default is any address.| |profileTypes|[windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)|Specifies the profiles to which the rule belongs.</span></span> <span data-ttu-id="df0a9-173">Wenn nicht angegeben, ist der Standardwert all.</span><span class="sxs-lookup"><span data-stu-id="df0a9-173">If not specified, the default is All.</span></span> <span data-ttu-id="df0a9-174">Mögliche Werte sind: `notConfigured`, `domain`, `private`, `public`. | | Aktion | [stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)| Die Aktion, die von der Regel erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="df0a9-174">Possible values are: `notConfigured`, `domain`, `private`, `public`.| |action|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|The action the rule enforces.</span></span> <span data-ttu-id="df0a9-175">Wenn nicht angegeben, ist der Standardwert zulässig.</span><span class="sxs-lookup"><span data-stu-id="df0a9-175">If not specified, the default is Allowed.</span></span> <span data-ttu-id="df0a9-176">Mögliche Werte sind: `notConfigured`, `blocked`, `allowed`. | | trafficDirection | [windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)| Die datenverkehrsrichtung, für die die Regel aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="df0a9-176">Possible values are: `notConfigured`, `blocked`, `allowed`.| |trafficDirection|[windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)|The traffic direction that the rule is enabled for.</span></span> <span data-ttu-id="df0a9-177">Wenn nicht angegeben, ist der Standardwert out. Mögliche Werte sind: `notConfigured`, `out`, `in`. | | interfaceTypes | [windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)| Die Schnittstellentypen der Regel.</span><span class="sxs-lookup"><span data-stu-id="df0a9-177">If not specified, the default is Out. Possible values are: `notConfigured`, `out`, `in`.| |interfaceTypes|[windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)|The interface types of the rule.</span></span> <span data-ttu-id="df0a9-178">Mögliche Werte sind: `notConfigured`, `remoteAccess`, `wireless`, `lan`. | | localUserAuthorizations | Zeichenfolge | Gibt die Liste der autorisierten lokalen Benutzer für den App-Container an.</span><span class="sxs-lookup"><span data-stu-id="df0a9-178">Possible values are: `notConfigured`, `remoteAccess`, `wireless`, `lan`.| |localUserAuthorizations|String|Specifies the list of authorized local users for the app container.</span></span> <span data-ttu-id="df0a9-179">Dies ist eine Zeichenfolge im SDDL-Format (Security Descriptor Definition Language). |</span><span class="sxs-lookup"><span data-stu-id="df0a9-179">This is a string in Security Descriptor Definition Language (SDDL) format.|</span></span>

## <a name="relationships"></a><span data-ttu-id="df0a9-180">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="df0a9-180">Relationships</span></span>
<span data-ttu-id="df0a9-181">Keine</span><span class="sxs-lookup"><span data-stu-id="df0a9-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df0a9-182">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="df0a9-182">JSON Representation</span></span>
<span data-ttu-id="df0a9-183">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="df0a9-183">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallRule",
  "displayName": "String",
  "description": "String",
  "packageFamilyName": "String",
  "filePath": "String",
  "serviceName": "String",
  "protocol": 1024,
  "localPortRanges": [
    "String"
  ],
  "remotePortRanges": [
    "String"
  ],
  "localAddressRanges": [
    "String"
  ],
  "remoteAddressRanges": [
    "String"
  ],
  "profileTypes": "String",
  "action": "String",
  "trafficDirection": "String",
  "interfaceTypes": "String",
  "localUserAuthorizations": "String"
}
```




