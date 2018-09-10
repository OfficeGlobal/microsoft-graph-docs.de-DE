# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="a253c-101">windowsInformationProtectionProxiedDomainCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a253c-101">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="a253c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a253c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a253c-103">Windows Information Protection – Proxydomänensammlung</span><span class="sxs-lookup"><span data-stu-id="a253c-103">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="a253c-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a253c-104">Properties</span></span>
|<span data-ttu-id="a253c-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a253c-105">Property</span></span>|<span data-ttu-id="a253c-106">Typ</span><span class="sxs-lookup"><span data-stu-id="a253c-106">Type</span></span>|<span data-ttu-id="a253c-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a253c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a253c-108">displayName</span><span class="sxs-lookup"><span data-stu-id="a253c-108">displayName</span></span>|<span data-ttu-id="a253c-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a253c-109">String</span></span>|<span data-ttu-id="a253c-110">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="a253c-110">Display name</span></span>|
|<span data-ttu-id="a253c-111">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="a253c-111">proxiedDomains</span></span>|<span data-ttu-id="a253c-112">[proxiedDomain](../resources/intune_mam_proxieddomain.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a253c-112">[proxiedDomain](../resources/intune_mam_proxieddomain.md) collection</span></span>|<span data-ttu-id="a253c-113">Sammlung von Proxydomänen</span><span class="sxs-lookup"><span data-stu-id="a253c-113">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="a253c-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a253c-114">Relationships</span></span>
<span data-ttu-id="a253c-115">Keine</span><span class="sxs-lookup"><span data-stu-id="a253c-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a253c-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a253c-116">JSON Representation</span></span>
<span data-ttu-id="a253c-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a253c-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
  "displayName": "String",
  "proxiedDomains": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ]
}
```








