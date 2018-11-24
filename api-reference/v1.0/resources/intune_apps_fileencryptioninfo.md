# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="71dc7-101">fileEncryptionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="71dc7-101">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="71dc7-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="71dc7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71dc7-103">Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.</span><span class="sxs-lookup"><span data-stu-id="71dc7-103">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="71dc7-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="71dc7-104">Properties</span></span>
|<span data-ttu-id="71dc7-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71dc7-105">Property</span></span>|<span data-ttu-id="71dc7-106">Typ</span><span class="sxs-lookup"><span data-stu-id="71dc7-106">Type</span></span>|<span data-ttu-id="71dc7-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71dc7-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71dc7-108">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="71dc7-108">encryptionKey</span></span>|<span data-ttu-id="71dc7-109">Binary</span><span class="sxs-lookup"><span data-stu-id="71dc7-109">Binary</span></span>|<span data-ttu-id="71dc7-110">Der Schlüssel, der zum Verschlüsseln des Inhalts der Datei verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="71dc7-110">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="71dc7-111">initializationVector</span><span class="sxs-lookup"><span data-stu-id="71dc7-111">initializationVector</span></span>|<span data-ttu-id="71dc7-112">Binary</span><span class="sxs-lookup"><span data-stu-id="71dc7-112">Binary</span></span>|<span data-ttu-id="71dc7-113">Der Initialisierungsvektor, der für den Verschlüsselungsalgorithmus verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="71dc7-113">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="71dc7-114">mac</span><span class="sxs-lookup"><span data-stu-id="71dc7-114">mac</span></span>|<span data-ttu-id="71dc7-115">Binary</span><span class="sxs-lookup"><span data-stu-id="71dc7-115">Binary</span></span>|<span data-ttu-id="71dc7-116">Der Hash aus dem verschlüsselten Dateiinhalt + IV (Inhaltshash).</span><span class="sxs-lookup"><span data-stu-id="71dc7-116">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="71dc7-117">macKey</span><span class="sxs-lookup"><span data-stu-id="71dc7-117">macKey</span></span>|<span data-ttu-id="71dc7-118">Binary</span><span class="sxs-lookup"><span data-stu-id="71dc7-118">Binary</span></span>|<span data-ttu-id="71dc7-119">Der Schlüssel, der für den Abruf von mac verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="71dc7-119">The key used to get mac.</span></span>|
|<span data-ttu-id="71dc7-120">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="71dc7-120">profileIdentifier</span></span>|<span data-ttu-id="71dc7-121">String</span><span class="sxs-lookup"><span data-stu-id="71dc7-121">String</span></span>|<span data-ttu-id="71dc7-122">Die Bezeichner des Profils.</span><span class="sxs-lookup"><span data-stu-id="71dc7-122">The the profile identifier.</span></span>|
|<span data-ttu-id="71dc7-123">fileDigest</span><span class="sxs-lookup"><span data-stu-id="71dc7-123">fileDigest</span></span>|<span data-ttu-id="71dc7-124">Binary</span><span class="sxs-lookup"><span data-stu-id="71dc7-124">Binary</span></span>|<span data-ttu-id="71dc7-125">Der Digest der Datei vor der Verschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="71dc7-125">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="71dc7-126">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="71dc7-126">fileDigestAlgorithm</span></span>|<span data-ttu-id="71dc7-127">String</span><span class="sxs-lookup"><span data-stu-id="71dc7-127">String</span></span>|<span data-ttu-id="71dc7-128">Der Dateidigestalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="71dc7-128">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71dc7-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="71dc7-129">Relationships</span></span>
<span data-ttu-id="71dc7-130">Keine</span><span class="sxs-lookup"><span data-stu-id="71dc7-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="71dc7-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="71dc7-131">JSON Representation</span></span>
<span data-ttu-id="71dc7-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="71dc7-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```



