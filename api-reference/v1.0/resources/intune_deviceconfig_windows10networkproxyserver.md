# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="f6af7-101">windows10NetworkProxyServer-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f6af7-101">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="f6af7-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f6af7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6af7-103">Netzwerk-Proxyserverrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="f6af7-103">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="f6af7-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f6af7-104">Properties</span></span>
|<span data-ttu-id="f6af7-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f6af7-105">Property</span></span>|<span data-ttu-id="f6af7-106">Typ</span><span class="sxs-lookup"><span data-stu-id="f6af7-106">Type</span></span>|<span data-ttu-id="f6af7-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6af7-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6af7-108">address</span><span class="sxs-lookup"><span data-stu-id="f6af7-108">address</span></span>|<span data-ttu-id="f6af7-109">String</span><span class="sxs-lookup"><span data-stu-id="f6af7-109">String</span></span>|<span data-ttu-id="f6af7-110">Adresse des Proxyservers.</span><span class="sxs-lookup"><span data-stu-id="f6af7-110">Address to the proxy server.</span></span> <span data-ttu-id="f6af7-111">Geben Sie eine Adresse im Format <server>\[":"<port>\] an.</span><span class="sxs-lookup"><span data-stu-id="f6af7-111">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="f6af7-112">exceptions</span><span class="sxs-lookup"><span data-stu-id="f6af7-112">exceptions</span></span>|<span data-ttu-id="f6af7-113">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f6af7-113">String collection</span></span>|<span data-ttu-id="f6af7-114">Adressen, die den Proxyserver nicht verwenden sollten.</span><span class="sxs-lookup"><span data-stu-id="f6af7-114">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="f6af7-115">Das System verwendet den Proxyserver nicht für Adressen, die mit den Angaben in diesem Knoten beginnen.</span><span class="sxs-lookup"><span data-stu-id="f6af7-115">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="f6af7-116">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="f6af7-116">useForLocalAddresses</span></span>|<span data-ttu-id="f6af7-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6af7-117">Boolean</span></span>|<span data-ttu-id="f6af7-118">Gibt an, ob der Proxyserver für lokale (Intranet-)Adressen verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="f6af7-118">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6af7-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f6af7-119">Relationships</span></span>
<span data-ttu-id="f6af7-120">Keine</span><span class="sxs-lookup"><span data-stu-id="f6af7-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f6af7-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f6af7-121">JSON Representation</span></span>
<span data-ttu-id="f6af7-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f6af7-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```



