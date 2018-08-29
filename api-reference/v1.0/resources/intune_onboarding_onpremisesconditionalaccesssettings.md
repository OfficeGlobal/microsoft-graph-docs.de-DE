# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="49197-101">onPremisesConditionalAccessSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="49197-101">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="49197-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="49197-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49197-103">Einzelne Entität, die die Exchange-Einstellungen für lokalen bedingten Zugriff für einen Mandanten darstellt.</span><span class="sxs-lookup"><span data-stu-id="49197-103">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="49197-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="49197-104">Methods</span></span>
|<span data-ttu-id="49197-105">Methode</span><span class="sxs-lookup"><span data-stu-id="49197-105">Method</span></span>|<span data-ttu-id="49197-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="49197-106">Return Type</span></span>|<span data-ttu-id="49197-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49197-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="49197-108">onpremisesConditionalAccessSettings abrufen</span><span class="sxs-lookup"><span data-stu-id="49197-108">Get onPremisesConditionalAccessSettings</span></span>](../api/intune_onboarding_onpremisesconditionalaccesssettings_get.md)|[<span data-ttu-id="49197-109">onpremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="49197-109">onPremisesConditionalAccessSettings</span></span>](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|<span data-ttu-id="49197-110">Lesen von Eigenschaften und Beziehungen des [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="49197-110">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="49197-111">onPremisesConditionalAccessSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="49197-111">Update onPremisesConditionalAccessSettings</span></span>](../api/intune_onboarding_onpremisesconditionalaccesssettings_update.md)|[<span data-ttu-id="49197-112">onpremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="49197-112">onPremisesConditionalAccessSettings</span></span>](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|<span data-ttu-id="49197-113">Aktualisieren der Eigenschaften eines [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="49197-113">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="49197-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="49197-114">Properties</span></span>
|<span data-ttu-id="49197-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="49197-115">Property</span></span>|<span data-ttu-id="49197-116">Typ</span><span class="sxs-lookup"><span data-stu-id="49197-116">Type</span></span>|<span data-ttu-id="49197-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49197-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49197-118">id</span><span class="sxs-lookup"><span data-stu-id="49197-118">id</span></span>|<span data-ttu-id="49197-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49197-119">String</span></span>|<span data-ttu-id="49197-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="49197-120">Not yet documented</span></span>|
|<span data-ttu-id="49197-121">enabled</span><span class="sxs-lookup"><span data-stu-id="49197-121">enabled</span></span>|<span data-ttu-id="49197-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="49197-122">Boolean</span></span>|<span data-ttu-id="49197-123">Gibt an, ob lokaler bedingter Zugriff für diese Organisation aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="49197-123">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="49197-124">includedGroups</span><span class="sxs-lookup"><span data-stu-id="49197-124">includedGroups</span></span>|<span data-ttu-id="49197-125">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="49197-125">Guid collection</span></span>|<span data-ttu-id="49197-126">Benutzergruppen, für die der lokale bedingte Zugriff gilt.</span><span class="sxs-lookup"><span data-stu-id="49197-126">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="49197-127">Alle Benutzer in diesen Gruppen müssen verwaltete und für den E-Mail-Zugriff kompatible Mobilgeräte verwenden.</span><span class="sxs-lookup"><span data-stu-id="49197-127">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="49197-128">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="49197-128">excludedGroups</span></span>|<span data-ttu-id="49197-129">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="49197-129">Guid collection</span></span>|<span data-ttu-id="49197-130">Benutzergruppen, die vom lokalen bedingten Zugriff ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="49197-130">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="49197-131">Alle Benutzer in diesen Gruppen werden von der Richtlinie zu bedingtem Zugriff ausgenommen.</span><span class="sxs-lookup"><span data-stu-id="49197-131">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="49197-132">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="49197-132">overrideDefaultRule</span></span>|<span data-ttu-id="49197-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="49197-133">Boolean</span></span>|<span data-ttu-id="49197-134">Überschreibt die Standardzugriffsregel, wenn zugelassen wird, dass einem Gerät Zugriff gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="49197-134">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49197-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="49197-135">Relationships</span></span>
<span data-ttu-id="49197-136">Keine</span><span class="sxs-lookup"><span data-stu-id="49197-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="49197-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="49197-137">JSON Representation</span></span>
<span data-ttu-id="49197-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="49197-138">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "fe4d7f2b-e7b8-4276-9976-7a3fc83edbbc"
  ],
  "excludedGroups": [
    "79199ed9-e50b-4257-8de4-70b9c8685061"
  ],
  "overrideDefaultRule": true
}
```



