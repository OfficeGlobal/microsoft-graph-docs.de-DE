# <a name="proxieddomain-resource-type"></a><span data-ttu-id="e227d-101">proxiedDomain-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e227d-101">proxiedDomain resource type</span></span>

> <span data-ttu-id="e227d-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e227d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e227d-103">Proxydomäne</span><span class="sxs-lookup"><span data-stu-id="e227d-103">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="e227d-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e227d-104">Properties</span></span>
|<span data-ttu-id="e227d-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e227d-105">Property</span></span>|<span data-ttu-id="e227d-106">Typ</span><span class="sxs-lookup"><span data-stu-id="e227d-106">Type</span></span>|<span data-ttu-id="e227d-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e227d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e227d-108">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="e227d-108">ipAddressOrFQDN</span></span>|<span data-ttu-id="e227d-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e227d-109">String</span></span>|<span data-ttu-id="e227d-110">Die IP-Adresse oder der FQDN</span><span class="sxs-lookup"><span data-stu-id="e227d-110">The IP address or FQDN</span></span>|
|<span data-ttu-id="e227d-111">Proxy</span><span class="sxs-lookup"><span data-stu-id="e227d-111">proxy</span></span>|<span data-ttu-id="e227d-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e227d-112">String</span></span>|<span data-ttu-id="e227d-113">Proxy-IP</span><span class="sxs-lookup"><span data-stu-id="e227d-113">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="e227d-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e227d-114">Relationships</span></span>
<span data-ttu-id="e227d-115">Keine</span><span class="sxs-lookup"><span data-stu-id="e227d-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e227d-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e227d-116">JSON Representation</span></span>
<span data-ttu-id="e227d-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e227d-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```



