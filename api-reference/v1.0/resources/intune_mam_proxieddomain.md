# <a name="proxieddomain-resource-type"></a><span data-ttu-id="5f312-101">proxiedDomain-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5f312-101">proxiedDomain resource type</span></span>

> <span data-ttu-id="5f312-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5f312-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f312-103">Proxydomäne</span><span class="sxs-lookup"><span data-stu-id="5f312-103">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="5f312-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5f312-104">Properties</span></span>
|<span data-ttu-id="5f312-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5f312-105">Property</span></span>|<span data-ttu-id="5f312-106">Typ</span><span class="sxs-lookup"><span data-stu-id="5f312-106">Type</span></span>|<span data-ttu-id="5f312-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f312-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f312-108">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="5f312-108">ipAddressOrFQDN</span></span>|<span data-ttu-id="5f312-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f312-109">String</span></span>|<span data-ttu-id="5f312-110">Die IP-Adresse oder der FQDN</span><span class="sxs-lookup"><span data-stu-id="5f312-110">The IP address or FQDN</span></span>|
|<span data-ttu-id="5f312-111">Proxy</span><span class="sxs-lookup"><span data-stu-id="5f312-111">web proxy</span></span>|<span data-ttu-id="5f312-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f312-112">String</span></span>|<span data-ttu-id="5f312-113">Proxy-IP</span><span class="sxs-lookup"><span data-stu-id="5f312-113">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f312-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5f312-114">Relationships</span></span>
<span data-ttu-id="5f312-115">Keine</span><span class="sxs-lookup"><span data-stu-id="5f312-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5f312-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5f312-116">JSON Representation</span></span>
<span data-ttu-id="5f312-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5f312-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



