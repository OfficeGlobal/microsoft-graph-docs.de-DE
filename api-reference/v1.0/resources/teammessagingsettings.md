# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="b9980-101">Ressourcentyp teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="b9980-101">teamMessagingSettings resource type</span></span>



<span data-ttu-id="b9980-102">So konfigurieren Sie die messaging-Einstellungen und erwähnungen im [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="b9980-102">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b9980-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b9980-103">Properties</span></span>
| <span data-ttu-id="b9980-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b9980-104">Property</span></span>     | <span data-ttu-id="b9980-105">Typ</span><span class="sxs-lookup"><span data-stu-id="b9980-105">Type</span></span>   |<span data-ttu-id="b9980-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9980-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9980-107">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="b9980-107">allowUserEditMessages</span></span>|<span data-ttu-id="b9980-108">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9980-108">Boolean</span></span>|<span data-ttu-id="b9980-109">Wenn es sich bei Festlegung auf true können Benutzer ihre Nachrichten bearbeiten kann.</span><span class="sxs-lookup"><span data-stu-id="b9980-109">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="b9980-110">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="b9980-110">allowUserDeleteMessages</span></span>|<span data-ttu-id="b9980-111">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9980-111">Boolean</span></span>|<span data-ttu-id="b9980-112">Bei Festlegung auf true können Benutzer ihre Nachrichten löschen kann.</span><span class="sxs-lookup"><span data-stu-id="b9980-112">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="b9980-113">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="b9980-113">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="b9980-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9980-114">Boolean</span></span>|<span data-ttu-id="b9980-115">Bei Festlegung auf "true" Websitebesitzer eine beliebige Nachricht löschen kann.</span><span class="sxs-lookup"><span data-stu-id="b9980-115">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="b9980-116">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="b9980-116">allowTeamMentions</span></span>|<span data-ttu-id="b9980-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9980-117">Boolean</span></span>|<span data-ttu-id="b9980-118">Wenn Festlegung auf "true", "@team erwähnungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="b9980-118">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="b9980-119">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="b9980-119">allowChannelMentions</span></span>|<span data-ttu-id="b9980-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9980-120">Boolean</span></span>|<span data-ttu-id="b9980-121">Wenn Festlegung auf "true", "@channel erwähnungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="b9980-121">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9980-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b9980-122">JSON representation</span></span>

<span data-ttu-id="b9980-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b9980-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
