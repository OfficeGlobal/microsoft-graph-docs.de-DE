# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="b71e6-101">bitLockerRemovableDrivePolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b71e6-101">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="b71e6-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b71e6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b71e6-103">BitLocker-Richtlinien für Wechseldatenträger.</span><span class="sxs-lookup"><span data-stu-id="b71e6-103">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="b71e6-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b71e6-104">Properties</span></span>
|<span data-ttu-id="b71e6-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b71e6-105">Property</span></span>|<span data-ttu-id="b71e6-106">Typ</span><span class="sxs-lookup"><span data-stu-id="b71e6-106">Type</span></span>|<span data-ttu-id="b71e6-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b71e6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b71e6-108">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="b71e6-108">encryptionMethod</span></span>|[<span data-ttu-id="b71e6-109">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="b71e6-109">bitLockerEncryptionMethod</span></span>](../resources/intune_deviceconfig_bitlockerencryptionmethod.md)|<span data-ttu-id="b71e6-110">Wählen Sie die Verschlüsselungsmethode für Wechseldatenträger aus.</span><span class="sxs-lookup"><span data-stu-id="b71e6-110">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="b71e6-111">Mögliche Werte sind: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="b71e6-111">The possible values are `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`, , , , , , , , or .</span></span>|
|<span data-ttu-id="b71e6-112">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="b71e6-112">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="b71e6-113">boolesch</span><span class="sxs-lookup"><span data-stu-id="b71e6-113">Boolean</span></span>|<span data-ttu-id="b71e6-114">Gibt an, ob der Schreibzugriff auf in einer anderen Organisation konfigurierte Geräte blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="b71e6-114">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="b71e6-115">Wenn „requireEncryptionForWriteAccess“ auf „false“ gesetzt ist, wirkt sich dieser Wert nicht aus.</span><span class="sxs-lookup"><span data-stu-id="b71e6-115">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="b71e6-116">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="b71e6-116">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="b71e6-117">boolesch</span><span class="sxs-lookup"><span data-stu-id="b71e6-117">Boolean</span></span>|<span data-ttu-id="b71e6-118">Diese Richtlinieneinstellung bestimmt, ob der BitLocker-Schutz erforderlich ist, damit Wechseldatenträger auf einem Computer beschreibbar sind.</span><span class="sxs-lookup"><span data-stu-id="b71e6-118">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b71e6-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b71e6-119">Relationships</span></span>
<span data-ttu-id="b71e6-120">Keine</span><span class="sxs-lookup"><span data-stu-id="b71e6-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b71e6-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b71e6-121">JSON Representation</span></span>
<span data-ttu-id="b71e6-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b71e6-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```



