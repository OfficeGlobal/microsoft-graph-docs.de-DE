# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="11c40-101">onPremisesConditionalAccessSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="11c40-101">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="11c40-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="11c40-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11c40-103">Einzelne Entität, die die Exchange-Einstellungen für lokalen bedingten Zugriff für einen Mandanten darstellt.</span><span class="sxs-lookup"><span data-stu-id="11c40-103">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="11c40-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="11c40-104">Methods</span></span>
|<span data-ttu-id="11c40-105">Methode</span><span class="sxs-lookup"><span data-stu-id="11c40-105">Method</span></span>|<span data-ttu-id="11c40-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="11c40-106">Return Type</span></span>|<span data-ttu-id="11c40-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11c40-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="11c40-108">onpremisesConditionalAccessSettings abrufen</span><span class="sxs-lookup"><span data-stu-id="11c40-108">Get onPremisesConditionalAccessSettings</span></span>](../api/intune_onboarding_onpremisesconditionalaccesssettings_get.md)|[<span data-ttu-id="11c40-109">onpremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="11c40-109">onPremisesConditionalAccessSettings</span></span>](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|<span data-ttu-id="11c40-110">Lesen von Eigenschaften und Beziehungen des [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="11c40-110">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="11c40-111">onPremisesConditionalAccessSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="11c40-111">Update onPremisesConditionalAccessSettings</span></span>](../api/intune_onboarding_onpremisesconditionalaccesssettings_update.md)|[<span data-ttu-id="11c40-112">onpremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="11c40-112">onPremisesConditionalAccessSettings</span></span>](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|<span data-ttu-id="11c40-113">Aktualisieren der Eigenschaften eines [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="11c40-113">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="11c40-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="11c40-114">Properties</span></span>
|<span data-ttu-id="11c40-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="11c40-115">Property</span></span>|<span data-ttu-id="11c40-116">Typ</span><span class="sxs-lookup"><span data-stu-id="11c40-116">Type</span></span>|<span data-ttu-id="11c40-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11c40-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11c40-118">ID</span><span class="sxs-lookup"><span data-stu-id="11c40-118">id</span></span>|<span data-ttu-id="11c40-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="11c40-119">String</span></span>|<span data-ttu-id="11c40-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="11c40-120">Not yet documented</span></span>|
|<span data-ttu-id="11c40-121">aktiviert</span><span class="sxs-lookup"><span data-stu-id="11c40-121">enabled</span></span>|<span data-ttu-id="11c40-122">Boolesch</span><span class="sxs-lookup"><span data-stu-id="11c40-122">Boolean</span></span>|<span data-ttu-id="11c40-123">Gibt an, ob lokaler bedingter Zugriff für diese Organisation aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="11c40-123">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="11c40-124">includedGroups</span><span class="sxs-lookup"><span data-stu-id="11c40-124">includedGroups</span></span>|<span data-ttu-id="11c40-125">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="11c40-125">Guid collection</span></span>|<span data-ttu-id="11c40-126">Benutzergruppen, für die der lokale bedingte Zugriff gilt.</span><span class="sxs-lookup"><span data-stu-id="11c40-126">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="11c40-127">Alle Benutzer in diesen Gruppen müssen verwaltete und für den E-Mail-Zugriff kompatible Mobilgeräte verwenden.</span><span class="sxs-lookup"><span data-stu-id="11c40-127">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="11c40-128">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="11c40-128">excludedGroups</span></span>|<span data-ttu-id="11c40-129">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="11c40-129">Guid collection</span></span>|<span data-ttu-id="11c40-130">Benutzergruppen, die vom lokalen bedingten Zugriff ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="11c40-130">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="11c40-131">Alle Benutzer in diesen Gruppen werden von der Richtlinie zu bedingtem Zugriff ausgenommen.</span><span class="sxs-lookup"><span data-stu-id="11c40-131">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="11c40-132">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="11c40-132">overrideDefaultRule</span></span>|<span data-ttu-id="11c40-133">Boolesch</span><span class="sxs-lookup"><span data-stu-id="11c40-133">Boolean</span></span>|<span data-ttu-id="11c40-134">Überschreibt die Standardzugriffsregel, wenn zugelassen wird, dass einem Gerät Zugriff gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="11c40-134">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11c40-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="11c40-135">Relationships</span></span>
<span data-ttu-id="11c40-136">Keine</span><span class="sxs-lookup"><span data-stu-id="11c40-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="11c40-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="11c40-137">JSON Representation</span></span>
<span data-ttu-id="11c40-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="11c40-138">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```








