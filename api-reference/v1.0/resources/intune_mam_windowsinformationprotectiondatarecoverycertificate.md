# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="caebe-101">windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="caebe-101">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="caebe-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="caebe-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="caebe-103">Windows Information Protection – Datenwiederherstellungszertifikat</span><span class="sxs-lookup"><span data-stu-id="caebe-103">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="caebe-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="caebe-104">Properties</span></span>
|<span data-ttu-id="caebe-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="caebe-105">Property</span></span>|<span data-ttu-id="caebe-106">Typ</span><span class="sxs-lookup"><span data-stu-id="caebe-106">Type</span></span>|<span data-ttu-id="caebe-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="caebe-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caebe-108">subjectName</span><span class="sxs-lookup"><span data-stu-id="caebe-108">subjectName</span></span>|<span data-ttu-id="caebe-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="caebe-109">String</span></span>|<span data-ttu-id="caebe-110">Antragstellername des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="caebe-110">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="caebe-111">description</span><span class="sxs-lookup"><span data-stu-id="caebe-111">description</span></span>|<span data-ttu-id="caebe-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="caebe-112">String</span></span>|<span data-ttu-id="caebe-113">Beschreibung des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="caebe-113">Data recovery Certificate description</span></span>|
|<span data-ttu-id="caebe-114">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="caebe-114">expirationDateTime</span></span>|<span data-ttu-id="caebe-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caebe-115">DateTimeOffset</span></span>|<span data-ttu-id="caebe-116">Ablaufdatum des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="caebe-116">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="caebe-117">certificate</span><span class="sxs-lookup"><span data-stu-id="caebe-117">certificate</span></span>|<span data-ttu-id="caebe-118">Binär</span><span class="sxs-lookup"><span data-stu-id="caebe-118">Binary</span></span>|<span data-ttu-id="caebe-119">Datenwiederherstellungszertifikat</span><span class="sxs-lookup"><span data-stu-id="caebe-119">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="caebe-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="caebe-120">Relationships</span></span>
<span data-ttu-id="caebe-121">Keine</span><span class="sxs-lookup"><span data-stu-id="caebe-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="caebe-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="caebe-122">JSON Representation</span></span>
<span data-ttu-id="caebe-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="caebe-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```








