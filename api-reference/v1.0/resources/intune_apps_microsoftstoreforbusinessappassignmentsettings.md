# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="283b4-101">microsoftStoreForBusinessAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="283b4-101">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="283b4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="283b4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="283b4-103">Enthält die Eigenschaften, die verwendet werden, um eine mobile Microsoft Store für Unternehmen-App einer Gruppe zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="283b4-103">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="283b4-104">Erbt von [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="283b4-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="283b4-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="283b4-105">Properties</span></span>
|<span data-ttu-id="283b4-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="283b4-106">Property</span></span>|<span data-ttu-id="283b4-107">Typ</span><span class="sxs-lookup"><span data-stu-id="283b4-107">Type</span></span>|<span data-ttu-id="283b4-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="283b4-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="283b4-109">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="283b4-109">useDeviceContext</span></span>|<span data-ttu-id="283b4-110">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="283b4-110">Boolean</span></span>|<span data-ttu-id="283b4-111">Gibt an, ob der Geräte-Ausführungskontext für mobile Microsoft Store für Unternehmen-Apps verwendet werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="283b4-111">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="283b4-112">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="283b4-112">Relationships</span></span>
<span data-ttu-id="283b4-113">Keine</span><span class="sxs-lookup"><span data-stu-id="283b4-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="283b4-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="283b4-114">JSON Representation</span></span>
<span data-ttu-id="283b4-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="283b4-115">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileAppAssignmentSettings",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```



