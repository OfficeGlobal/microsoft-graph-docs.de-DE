# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="59b9c-101">mailboxSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="59b9c-101">mailboxSettings resource type</span></span>

<span data-ttu-id="59b9c-102">Einstellungen für das primäre Postfach des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="59b9c-102">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="59b9c-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="59b9c-103">Properties</span></span>
| <span data-ttu-id="59b9c-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="59b9c-104">Property</span></span>     | <span data-ttu-id="59b9c-105">Typ</span><span class="sxs-lookup"><span data-stu-id="59b9c-105">Type</span></span>   |<span data-ttu-id="59b9c-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59b9c-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59b9c-107">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="59b9c-107">archiveFolder</span></span>|<span data-ttu-id="59b9c-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="59b9c-108">string</span></span>|<span data-ttu-id="59b9c-109">Ordner-ID eines Archivordners für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="59b9c-109">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="59b9c-110">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="59b9c-110">automaticRepliesSetting</span></span>|[<span data-ttu-id="59b9c-111">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="59b9c-111">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="59b9c-112">Konfigurationseinstellungen zum automatischen Benachrichtigen des Absenders bei eingehenden E-Mails mit einer Nachricht vom angemeldeten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="59b9c-112">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="59b9c-113">language</span><span class="sxs-lookup"><span data-stu-id="59b9c-113">language</span></span>|[<span data-ttu-id="59b9c-114">localeInfo</span><span class="sxs-lookup"><span data-stu-id="59b9c-114">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="59b9c-115">Die Gebietsschemainformationen des Benutzers, einschließlich der bevorzugten Sprache und Land/Region.</span><span class="sxs-lookup"><span data-stu-id="59b9c-115">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="59b9c-116">timeZone</span><span class="sxs-lookup"><span data-stu-id="59b9c-116">timeZone</span></span>|<span data-ttu-id="59b9c-117">string</span><span class="sxs-lookup"><span data-stu-id="59b9c-117">string</span></span>|<span data-ttu-id="59b9c-118">Die Standardzeitzone für das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="59b9c-118">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="59b9c-119">workingHours</span><span class="sxs-lookup"><span data-stu-id="59b9c-119">workingHours</span></span>|[<span data-ttu-id="59b9c-120">workingHours</span><span class="sxs-lookup"><span data-stu-id="59b9c-120">workingHours</span></span>](workinghours.md)|<span data-ttu-id="59b9c-121">Die Wochentage und Zeiten in einer bestimmten Zeitzone, an bzw. zu denen der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="59b9c-121">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59b9c-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="59b9c-122">JSON representation</span></span>

<span data-ttu-id="59b9c-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="59b9c-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "archiveFolder"
  ],
  "@odata.type": "microsoft.graph.mailboxSettings"
}-->

```json
{
  "archiveFolder": "string",
  "automaticRepliesSetting": {"@odata.type": "microsoft.graph.automaticRepliesSetting"},
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->