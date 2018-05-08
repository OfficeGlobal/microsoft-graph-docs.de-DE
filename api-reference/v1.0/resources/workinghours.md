# <a name="workinghours-resource-type"></a><span data-ttu-id="95244-101">workingHours-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="95244-101">workingHours resource type</span></span>

<span data-ttu-id="95244-102">Stellt die Wochentage und Zeiten in einer bestimmten Zeitzone dar, an bzw. zu denen der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="95244-102">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="95244-103">Zugriff auf die Arbeitszeiten eines Benutzers ist bei der Aktivitäts- oder Ressourcenplanung hilfreich.</span><span class="sxs-lookup"><span data-stu-id="95244-103">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="95244-104">Sie können die Arbeitszeiten eines Benutzers als Teil der [Postfacheinstellungen](mailboxSettings.md) des Benutzers [abrufen](../api/user_get_mailboxsettings.md#request-3) und [festlegen](../api/user_update_mailboxsettings.md#request-2) .</span><span class="sxs-lookup"><span data-stu-id="95244-104">You can [get](../api/user_get_mailboxsettings.md#request-3) and [set](../api/user_update_mailboxsettings.md#request-2) the working hours of a user as part of the user's [mailbox settings](mailboxSettings.md).</span></span> 

<span data-ttu-id="95244-105">Sie können für die Arbeitszeiten auch eine andere Zeitzone als die für Ihren Outlook-Client festgelegte Zeitzone festlegen.</span><span class="sxs-lookup"><span data-stu-id="95244-105">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="95244-106">Dies kann zum Beispiel hilfreich sein, wenn Sie in eine andere Zeitzone reisen.</span><span class="sxs-lookup"><span data-stu-id="95244-106">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="95244-107">Sie können den Outlook-Client auf</span><span class="sxs-lookup"><span data-stu-id="95244-107">You can set the Outlook client</span></span>  
<span data-ttu-id="95244-108">die Zielzeitzone festlegen, sodass die Outlook-Zeitwerte in der lokalen Zeit angezeigt werden, solange Sie sich in dieser Zeitzone befinden.</span><span class="sxs-lookup"><span data-stu-id="95244-108">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="95244-109">Wenn andere Personen Arbeitsbesprechungen mit Ihnen an Ihrem üblichen Arbeitsplatz anfordern, können sie sich an Ihre Arbeitszeiten in der jeweiligen Zeitzone halten.</span><span class="sxs-lookup"><span data-stu-id="95244-109">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="95244-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="95244-110">Properties</span></span>
| <span data-ttu-id="95244-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="95244-111">Property</span></span>     | <span data-ttu-id="95244-112">Typ</span><span class="sxs-lookup"><span data-stu-id="95244-112">Type</span></span>   |<span data-ttu-id="95244-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95244-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="95244-114">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="95244-114">daysOfWeek</span></span> | <span data-ttu-id="95244-115">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="95244-115">String collection</span></span> | <span data-ttu-id="95244-116">Die Wochentage, an denen der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="95244-116">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="95244-117">startTime</span><span class="sxs-lookup"><span data-stu-id="95244-117"><starttime></span></span> | <span data-ttu-id="95244-118">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="95244-118">Edm.TimeOfDay</span></span> | <span data-ttu-id="95244-119">Die Tageszeit, zu der der Benutzer zu arbeiten beginnt.</span><span class="sxs-lookup"><span data-stu-id="95244-119">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="95244-120">endTime</span><span class="sxs-lookup"><span data-stu-id="95244-120"><endtime></span></span> | <span data-ttu-id="95244-121">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="95244-121">Edm.TimeOfDay</span></span> | <span data-ttu-id="95244-122">Die Tageszeit, zu der der Benutzer zu arbeiten aufhört.</span><span class="sxs-lookup"><span data-stu-id="95244-122">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="95244-123">timeZone</span><span class="sxs-lookup"><span data-stu-id="95244-123">timeZone</span></span> | [<span data-ttu-id="95244-124">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="95244-124">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="95244-125">Die Zeitzone, für die die Arbeitszeiten gelten.</span><span class="sxs-lookup"><span data-stu-id="95244-125">The time zone to which the working hours apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="95244-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="95244-126">JSON representation</span></span>

<span data-ttu-id="95244-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="95244-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "TimeOfDay",
  "endTime": "TimeOfDay",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->