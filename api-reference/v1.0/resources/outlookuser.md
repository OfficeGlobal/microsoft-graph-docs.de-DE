# <a name="outlookuser-resource-type"></a><span data-ttu-id="8c053-101">outlookUser-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8c053-101">outlookUser resource type</span></span>


<span data-ttu-id="8c053-102">Stellt die für einen Benutzer verfügbaren Outlook-Dienste dar.</span><span class="sxs-lookup"><span data-stu-id="8c053-102">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="8c053-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="8c053-103">Methods</span></span>

| <span data-ttu-id="8c053-104">Methode</span><span class="sxs-lookup"><span data-stu-id="8c053-104">Method</span></span>           | <span data-ttu-id="8c053-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8c053-105">Return Type</span></span>    |<span data-ttu-id="8c053-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c053-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8c053-107">Kategorie erstellen</span><span class="sxs-lookup"><span data-stu-id="8c053-107">Create category</span></span>](../api/outlookuser_post_mastercategories.md) | [<span data-ttu-id="8c053-108">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="8c053-108">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="8c053-109">Erstellen eines **outlookCategory**-Objekts in der Masterliste von Kategorien.</span><span class="sxs-lookup"><span data-stu-id="8c053-109">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="8c053-110">Kategorien auflisten</span><span class="sxs-lookup"><span data-stu-id="8c053-110">List categories</span></span>](../api/outlookuser_list_mastercategories.md) | <span data-ttu-id="8c053-111">[outlookCategory](outlookcategory.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8c053-111">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="8c053-112">Ruft alle Kategorien ab, die für den Benutzer definiert wurden.</span><span class="sxs-lookup"><span data-stu-id="8c053-112">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="8c053-113">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="8c053-113">supportedLanguages</span></span>](../api/outlookuser_supportedlanguages.md) | <span data-ttu-id="8c053-114">[localeInfo](localeinfo.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8c053-114">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="8c053-115">Abrufen der Liste von Gebietsschemas und Sprachen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="8c053-115">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="8c053-116">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="8c053-116">supportedTimeZones</span></span>](../api/outlookuser_supportedtimezones.md) | <span data-ttu-id="8c053-117">[timeZoneInformation](timezoneinformation.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8c053-117">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="8c053-118">Abrufen der Liste von Zeitzonen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="8c053-118">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="8c053-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8c053-119">Properties</span></span>
<span data-ttu-id="8c053-120">Keine</span><span class="sxs-lookup"><span data-stu-id="8c053-120">None</span></span>

## <a name="relationships"></a><span data-ttu-id="8c053-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8c053-121">Relationships</span></span>
| <span data-ttu-id="8c053-122">Beziehung</span><span class="sxs-lookup"><span data-stu-id="8c053-122">Relationship</span></span> | <span data-ttu-id="8c053-123">Typ</span><span class="sxs-lookup"><span data-stu-id="8c053-123">Type</span></span>   |<span data-ttu-id="8c053-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c053-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c053-125">masterCategories</span><span class="sxs-lookup"><span data-stu-id="8c053-125">masterCategories</span></span>|<span data-ttu-id="8c053-126">[outlookCategory](../resources/outlookCategory.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8c053-126">[outlookCategory](../resources/outlookCategory.md) collection</span></span>| <span data-ttu-id="8c053-127">Eine Liste von Kategorien, die für den Benutzer definiert sind.</span><span class="sxs-lookup"><span data-stu-id="8c053-127">A list of categories defined for the user.</span></span> | 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->