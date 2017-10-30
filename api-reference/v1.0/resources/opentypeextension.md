# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="e6651-101">openTypeExtension-Ressourcentyp (offene Erweiterungen)</span><span class="sxs-lookup"><span data-stu-id="e6651-101">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="e6651-102">Offene Erweiterungen (bisher als Office 365-Datenerweiterungen bezeichnet) bieten Ihnen eine einfache Möglichkeit zum direkten Hinzufügen nicht typisierter Eigenschaften zu einer Ressource in Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e6651-102">Open extensions (formerly known as Office 365 data extensions) give you an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span> 

<span data-ttu-id="e6651-103">Offiene Erweiterungen werden mithilfe der **openTypeExtension**-Ressource dargestellt.</span><span class="sxs-lookup"><span data-stu-id="e6651-103">Office 365 data extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="e6651-104">Alle offenen Erweiterungen, die einer Ressource hinzugefügt wurden, werden in der **extensions**-Navigationseigenschaft angezeigt, die vom abstrakten Typ [extension](extension.md) abgeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="e6651-104">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span> <span data-ttu-id="e6651-105">Jede Erweiterung weist eine **extensionName**-Eigenschaft auf, die die einzige vordefinierte, schreibbare Eigenschaft für alle Erweiterungen zusammen mit ihren benutzerdefinierten Daten ist.</span><span class="sxs-lookup"><span data-stu-id="e6651-105">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span> 

<span data-ttu-id="e6651-106">Um sicherzustellen, dass Erweiterungsnamen eindeutig sind, können Sie eine umgekehrtes DNS-Format (Domain Name System) verwenden, das _von Ihrer eigenen Domäne_, z. B. `Com.Contoso.ContactInfo`, abhängig ist.</span><span class="sxs-lookup"><span data-stu-id="e6651-106">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="e6651-107">Verwenden Sie in Erweiterungsnamen auf keinen Fall die Microsoft-Domäne (`Com.Microsoft` oder `Com.OnMicrosoft`).</span><span class="sxs-lookup"><span data-stu-id="e6651-107">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="e6651-108">Beispiel für eine offene Erweiterung: [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](../../../concepts/extensibility_open_users.md)</span><span class="sxs-lookup"><span data-stu-id="e6651-108">Open extension example: [Add custom data to users using open extensions](../../../concepts/extensibility_open_users.md)</span></span>

<span data-ttu-id="e6651-109">Offene Erweiterungen werden von den folgenden Ressourcen in den entsprechenden Versionen unterstützt: - Allgemein verfügbar (GA: /v1.0 und /beta) oder Vorschau (/beta).</span><span class="sxs-lookup"><span data-stu-id="e6651-109">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

|<span data-ttu-id="e6651-110">Ressource</span><span class="sxs-lookup"><span data-stu-id="e6651-110">Resource</span></span> |<span data-ttu-id="e6651-111">Version</span><span class="sxs-lookup"><span data-stu-id="e6651-111">Version</span></span> |
|:---------------|:-------|
| [<span data-ttu-id="e6651-112">Administrative Einheit</span><span class="sxs-lookup"><span data-stu-id="e6651-112">Administrative unit</span></span>](../../beta/resources/administrativeunit.md)  | <span data-ttu-id="e6651-113">Nur Vorschau</span><span class="sxs-lookup"><span data-stu-id="e6651-113">Preview only</span></span> |
| [<span data-ttu-id="e6651-114">Kalenderereignis</span><span class="sxs-lookup"><span data-stu-id="e6651-114">Calendar event</span></span>](event.md) | <span data-ttu-id="e6651-115">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="e6651-115">GA</span></span> |
| <span data-ttu-id="e6651-116">[Kalenderereignis](event.md) für Gruppe</span><span class="sxs-lookup"><span data-stu-id="e6651-116">Group [calendar event](event.md)</span></span> | <span data-ttu-id="e6651-117">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="e6651-117">GA</span></span> |
| <span data-ttu-id="e6651-118">Unterhaltungsthread der Gruppe [posten](post.md)</span><span class="sxs-lookup"><span data-stu-id="e6651-118">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="e6651-119">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="e6651-119">GA</span></span> |
| [<span data-ttu-id="e6651-120">device</span><span class="sxs-lookup"><span data-stu-id="e6651-120">device</span></span>](device.md) | <span data-ttu-id="e6651-121">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="e6651-121">GA</span></span> |
| [<span data-ttu-id="e6651-122">group</span><span class="sxs-lookup"><span data-stu-id="e6651-122">group</span></span>](group.md) | <span data-ttu-id="e6651-123">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="e6651-123">GA</span></span> |
| [<span data-ttu-id="e6651-124">message</span><span class="sxs-lookup"><span data-stu-id="e6651-124">message</span></span>](message.md) | <span data-ttu-id="e6651-125">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="e6651-125">GA</span></span> |
| [<span data-ttu-id="e6651-126">organization</span><span class="sxs-lookup"><span data-stu-id="e6651-126">organization</span></span>](organization.md) | <span data-ttu-id="e6651-127">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="e6651-127">GA</span></span> |
| [<span data-ttu-id="e6651-128">Personal contact</span><span class="sxs-lookup"><span data-stu-id="e6651-128">Personal contact</span></span>](contact.md) | <span data-ttu-id="e6651-129">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="e6651-129">GA</span></span> |
| [<span data-ttu-id="e6651-130">user</span><span class="sxs-lookup"><span data-stu-id="e6651-130">user</span></span>](user.md) | <span data-ttu-id="e6651-131">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="e6651-131">GA</span></span> |

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="e6651-132">Sollen offene Erweiterungen (für Outlook-Ressourcen) oder erweiterte Eigenschaften verwendet werden?</span><span class="sxs-lookup"><span data-stu-id="e6651-132">Use open extensions (for Outlook resources) or extended properties?</span></span>

<span data-ttu-id="e6651-p103">Offene Erweiterungen sind die empfohlene Lösung für die meisten Szenarios, bei denen benutzerdefinierte Daten gespeichert und aufgerufen werden sollen. Wenn Sie auf benutzerdefinierte Daten für Outlook-MAPI-Eigenschaften zugreifen müssen, die nicht bereits in den [Microsoft Graph-API-Metadaten](http://developer.microsoft.com/en-us/graph/docs/overview/call_api) verfügbar gemacht wurden, können Sie [erweiterte Eigenschaften und deren REST-API](extended-properties-overview.md) verwenden. Unter https://graph.microsoft.com/v1.0/$metadata können Sie überprüfen, welche Eigenschaften die Metadaten verfügbar machen.</span><span class="sxs-lookup"><span data-stu-id="e6651-p103">Open extensions is the recommended solution for most scenarios involving storing and accessing custom data. If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](http://developer.microsoft.com/en-us/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md). You can verify which properties the metadata exposes at https://graph.microsoft.com/v1.0/$metadata.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e6651-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e6651-136">JSON representation</span></span>

<span data-ttu-id="e6651-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e6651-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.opentypeextension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

<br/>

## <a name="properties"></a><span data-ttu-id="e6651-138">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e6651-138">Properties</span></span>

|<span data-ttu-id="e6651-139">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e6651-139">Property</span></span>      |<span data-ttu-id="e6651-140">Typ</span><span class="sxs-lookup"><span data-stu-id="e6651-140">Type</span></span>    |<span data-ttu-id="e6651-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6651-141">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e6651-142">extensionName</span><span class="sxs-lookup"><span data-stu-id="e6651-142">extensionName</span></span>|<span data-ttu-id="e6651-143">String</span><span class="sxs-lookup"><span data-stu-id="e6651-143">String</span></span>|<span data-ttu-id="e6651-p104">Ein eindeutiger Textbezeichner für eine offene Erweiterung. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e6651-p104">A unique text identifier for an open type open extension. Required.</span></span>|
|<span data-ttu-id="e6651-146">id</span><span class="sxs-lookup"><span data-stu-id="e6651-146">id</span></span>|<span data-ttu-id="e6651-147">String</span><span class="sxs-lookup"><span data-stu-id="e6651-147">String</span></span>| <span data-ttu-id="e6651-p105">Eine vollqualifizierte ID, die den Erweiterungstyp mit dem **extensionName**-Element verkettet. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e6651-p105">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6651-150">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e6651-150">Relationships</span></span>

<span data-ttu-id="e6651-151">Keine</span><span class="sxs-lookup"><span data-stu-id="e6651-151">None</span></span>


## <a name="methods"></a><span data-ttu-id="e6651-152">Methoden</span><span class="sxs-lookup"><span data-stu-id="e6651-152">Methods</span></span>

|<span data-ttu-id="e6651-153">Methode</span><span class="sxs-lookup"><span data-stu-id="e6651-153">Method</span></span>        |<span data-ttu-id="e6651-154">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e6651-154">Return Type</span></span> |<span data-ttu-id="e6651-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6651-155">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="e6651-156">Post</span><span class="sxs-lookup"><span data-stu-id="e6651-156">Post</span></span>](../api/opentypeextension_post_opentypeextension.md) | <span data-ttu-id="e6651-157">[openTypeExtension](opentypeextension.md) (in einer vorhandenen Ressourceninstanz) oder ein neues [contact](../resources/contact.md)-, [event](../resources/event.md)- oder [message](../resources/message.md)-Objekt, das ein openTypeExtension-Objekt enthält.</span><span class="sxs-lookup"><span data-stu-id="e6651-157">[openTypeExtension](opentypeextension.md) (in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="e6651-158">Dient zum Erstellen eines openTypeExtension-Objekts in einer vorhandenen oder neuen Ressourceninstanz.</span><span class="sxs-lookup"><span data-stu-id="e6651-158">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="e6651-159">Get</span><span class="sxs-lookup"><span data-stu-id="e6651-159">Get</span></span>](../api/opentypeextension_get.md) | [<span data-ttu-id="e6651-160">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="e6651-160">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="e6651-161">Dient zum Lesen der Eigenschaften und der Beziehungen des openTypeExtension-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e6651-161">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="e6651-162">Update</span><span class="sxs-lookup"><span data-stu-id="e6651-162">Update</span></span>](../api/opentypeextension_update.md) | [<span data-ttu-id="e6651-163">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="e6651-163">openTypeExtension</span></span>](opentypeextension.md)   |<span data-ttu-id="e6651-164">Dient zum Aktualisieren des openTypeExtension-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e6651-164">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="e6651-165">Delete</span><span class="sxs-lookup"><span data-stu-id="e6651-165">Delete</span></span>](../api/opentypeextension_delete.md) | <span data-ttu-id="e6651-166">Keine</span><span class="sxs-lookup"><span data-stu-id="e6651-166">None</span></span> |<span data-ttu-id="e6651-167">Dient zum Löschen des openTypeExtension-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e6651-167">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
