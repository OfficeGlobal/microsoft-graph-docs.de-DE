---
title: openTypeExtension-Ressourcentyp (offene Erweiterungen)
description: Open-Erweiterungen (vormals Office 365 Daten Extensions) bieten eine einfache Möglichkeit nicht typisierte Eigenschaften auf eine Ressource in Microsoft Graph direkt hinzufügen.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 6a0be3c794fcfc880a99c5fd81e498b8121de68a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574908"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="fdb6f-103">openTypeExtension-Ressourcentyp (offene Erweiterungen)</span><span class="sxs-lookup"><span data-stu-id="fdb6f-103">openTypeExtension resource type (open extensions)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdb6f-104">Open-Erweiterungen (vormals Office 365 Daten Extensions) bieten eine einfache Möglichkeit nicht typisierte Eigenschaften auf eine Ressource in Microsoft Graph direkt hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-104">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>
<span data-ttu-id="fdb6f-105">Offiene Erweiterungen werden mithilfe der **openTypeExtension**-Ressource dargestellt.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-105">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="fdb6f-106">Alle offenen Erweiterungen, die einer Ressource hinzugefügt wurden, werden in der **extensions**-Navigationseigenschaft angezeigt, die vom abstrakten Typ [extension](extension.md) abgeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-106">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span>  <span data-ttu-id="fdb6f-107">Jede Erweiterung weist eine **extensionName**-Eigenschaft auf, die die einzige vordefinierte, schreibbare Eigenschaft für alle Erweiterungen zusammen mit ihren benutzerdefinierten Daten ist.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-107">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span> <span data-ttu-id="fdb6f-108">Um sicherzustellen, dass Erweiterungsnamen eindeutig sind, können Sie eine umgekehrtes DNS-Format (Domain Name System) verwenden, das _von Ihrer eigenen Domäne_, z. B. `Com.Contoso.ContactInfo`, abhängig ist.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-108">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="fdb6f-109">Verwenden Sie in Erweiterungsnamen auf keinen Fall die Microsoft-Domäne (`Com.Microsoft` oder `Com.OnMicrosoft`).</span><span class="sxs-lookup"><span data-stu-id="fdb6f-109">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="fdb6f-110">Beispiel für eine offene Erweiterung: [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](/graph/extensibility-open-users)</span><span class="sxs-lookup"><span data-stu-id="fdb6f-110">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="fdb6f-111">Offene Erweiterungen werden von den folgenden Ressourcen in den entsprechenden Versionen unterstützt: - Allgemein verfügbar (GA: /v1.0 und /beta) oder Vorschau (/beta).</span><span class="sxs-lookup"><span data-stu-id="fdb6f-111">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

| <span data-ttu-id="fdb6f-112">Ressource</span><span class="sxs-lookup"><span data-stu-id="fdb6f-112">Resource</span></span> | <span data-ttu-id="fdb6f-113">Version</span><span class="sxs-lookup"><span data-stu-id="fdb6f-113">Version</span></span> |
|---------------|-------|
| [<span data-ttu-id="fdb6f-114">Administrative Einheit</span><span class="sxs-lookup"><span data-stu-id="fdb6f-114">Administrative unit</span></span>](administrativeunit.md)  | <span data-ttu-id="fdb6f-115">Nur Vorschau</span><span class="sxs-lookup"><span data-stu-id="fdb6f-115">Preview only</span></span> |
| [<span data-ttu-id="fdb6f-116">Kalenderereignis</span><span class="sxs-lookup"><span data-stu-id="fdb6f-116">Calendar event</span></span>](event.md) | <span data-ttu-id="fdb6f-117">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="fdb6f-117">GA</span></span> |
| <span data-ttu-id="fdb6f-118">[Kalenderereignis](event.md) für Gruppe</span><span class="sxs-lookup"><span data-stu-id="fdb6f-118">Group [calendar event](event.md)</span></span> | <span data-ttu-id="fdb6f-119">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="fdb6f-119">GA</span></span> |
| <span data-ttu-id="fdb6f-120">Unterhaltungsthread der Gruppe [posten](post.md)</span><span class="sxs-lookup"><span data-stu-id="fdb6f-120">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="fdb6f-121">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="fdb6f-121">GA</span></span> |
| [<span data-ttu-id="fdb6f-122">device</span><span class="sxs-lookup"><span data-stu-id="fdb6f-122">device</span></span>](device.md) | <span data-ttu-id="fdb6f-123">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="fdb6f-123">GA</span></span> |
| [<span data-ttu-id="fdb6f-124">group</span><span class="sxs-lookup"><span data-stu-id="fdb6f-124">group</span></span>](group.md) | <span data-ttu-id="fdb6f-125">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="fdb6f-125">GA</span></span> |
| [<span data-ttu-id="fdb6f-126">message</span><span class="sxs-lookup"><span data-stu-id="fdb6f-126">message</span></span>](message.md) | <span data-ttu-id="fdb6f-127">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="fdb6f-127">GA</span></span> |
| [<span data-ttu-id="fdb6f-128">organization</span><span class="sxs-lookup"><span data-stu-id="fdb6f-128">organization</span></span>](organization.md) | <span data-ttu-id="fdb6f-129">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="fdb6f-129">GA</span></span> |
| [<span data-ttu-id="fdb6f-130">Privater Kontakt</span><span class="sxs-lookup"><span data-stu-id="fdb6f-130">Personal contact</span></span>](contact.md) | <span data-ttu-id="fdb6f-131">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="fdb6f-131">GA</span></span> |
| [<span data-ttu-id="fdb6f-132">user</span><span class="sxs-lookup"><span data-stu-id="fdb6f-132">user</span></span>](user.md) | <span data-ttu-id="fdb6f-133">Allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="fdb6f-133">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="fdb6f-134">Outlook-spezifische Aspekte</span><span class="sxs-lookup"><span data-stu-id="fdb6f-134">Outlook-specific considerations</span></span>

<span data-ttu-id="fdb6f-135">Jede open Erweiterung auf einer Outlook-Ressource (Ereignis, Nachricht oder persönlichen Kontakt) vorhanden ist in einem [MAPI benannte Eigenschaft](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx)gespeichert.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-135">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="fdb6f-136">Berücksichtigen Sie beim Erstellen von open-Erweiterungen für Outlook, dass MAPI benannte Eigenschaften sind eine begrenzte Ressource im Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-136">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="fdb6f-137">Wenn ein Benutzer benannte Eigenschaft Quota leer ist, können nicht Sie keine mehr benannten Eigenschaften für diesen Benutzer erstellen.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-137">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="fdb6f-138">Dies kann unerwartetes Verhalten von Clients führen, die benannte Eigenschaften-Funktion verwenden.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-138">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="fdb6f-139">Wenden Sie die folgenden Richtlinien beim Erstellen von open-Erweiterungen für Outlook-Ressourcen:</span><span class="sxs-lookup"><span data-stu-id="fdb6f-139">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="fdb6f-140">Erstellen Sie die minimale Anzahl von Erweiterungen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-140">Create the minimum number of extensions required.</span></span> <span data-ttu-id="fdb6f-141">Die meisten Clientanwendungen sollten nicht mehr als eine Erweiterung erfordern.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-141">Most applications should require no more than one extension.</span></span> <span data-ttu-id="fdb6f-142">Erweiterungen haben keine Eigenschaften festgelegt wird, oder die Struktur, damit Sie mehrere Werte in einer Erweiterung speichern können.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-142">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="fdb6f-143">Benennen Sie Erweiterungen in einer Variablen Weise (z. B. basierend auf Benutzereingaben usw..).</span><span class="sxs-lookup"><span data-stu-id="fdb6f-143">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="fdb6f-144">Jedes Mal, wenn eine open Erweiterung mit einem neuen Namen erstellt wird, die nicht im Postfach eines Benutzers vor, verwendet wurde, wird ein neues MAPI benannte Eigenschaft erstellt.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-144">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="fdb6f-145">Entfernen die Erweiterung, die benannte Eigenschaft nicht entfernt.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-145">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="fdb6f-146">Verwenden Sie open-Erweiterungen (für Outlook-Ressourcen) oder erweiterten Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fdb6f-146">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="fdb6f-147">Open Extensions ist die empfohlene Lösung für die meisten Szenarien im Zusammenhang mit Speichern von und Zugreifen auf benutzerdefinierte Daten.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-147">Open extensions is the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="fdb6f-148">Wenn Sie benutzerdefinierte Daten für Outlook-MAPI-Eigenschaften, die noch nicht verfügbar gemacht werden über die [Microsoft Graph-API-Metadaten](https://developer.microsoft.com/graph/docs/overview/call_api)zugreifen möchten, können Sie [Erweiterte Eigenschaften und der REST-API](extended-properties-overview.md)verwenden.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-148">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="fdb6f-149">Sie können überprüfen, welche Eigenschaften die Metadaten zur verfügbar gemacht [ https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span><span class="sxs-lookup"><span data-stu-id="fdb6f-149">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdb6f-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fdb6f-150">JSON representation</span></span>

<span data-ttu-id="fdb6f-151">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-151">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
       "companyName",
        "dealValue",
        "expirationDate"
  ],
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

## <a name="properties"></a><span data-ttu-id="fdb6f-152">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fdb6f-152">Properties</span></span>

| <span data-ttu-id="fdb6f-153">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fdb6f-153">Property</span></span> | <span data-ttu-id="fdb6f-154">Typ</span><span class="sxs-lookup"><span data-stu-id="fdb6f-154">Type</span></span> | <span data-ttu-id="fdb6f-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdb6f-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="fdb6f-156">extensionName</span><span class="sxs-lookup"><span data-stu-id="fdb6f-156">extensionName</span></span>|<span data-ttu-id="fdb6f-157">String</span><span class="sxs-lookup"><span data-stu-id="fdb6f-157">String</span></span>|<span data-ttu-id="fdb6f-p106">Ein eindeutiger Textbezeichner für eine OpenType-Datenerweiterung. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="fdb6f-p106">A unique text identifier for an open type data extension. Required.</span></span>|
|<span data-ttu-id="fdb6f-160">id</span><span class="sxs-lookup"><span data-stu-id="fdb6f-160">id</span></span>|<span data-ttu-id="fdb6f-161">String</span><span class="sxs-lookup"><span data-stu-id="fdb6f-161">String</span></span>| <span data-ttu-id="fdb6f-p107">Eine vollqualifizierte ID, die den Erweiterungstyp mit dem **extensionName**-Element verkettet. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-p107">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdb6f-164">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fdb6f-164">Relationships</span></span>

<span data-ttu-id="fdb6f-165">Keine</span><span class="sxs-lookup"><span data-stu-id="fdb6f-165">None</span></span>

## <a name="methods"></a><span data-ttu-id="fdb6f-166">Methoden</span><span class="sxs-lookup"><span data-stu-id="fdb6f-166">Methods</span></span>

| <span data-ttu-id="fdb6f-167">Methode</span><span class="sxs-lookup"><span data-stu-id="fdb6f-167">Method</span></span> | <span data-ttu-id="fdb6f-168">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="fdb6f-168">Return Type</span></span> | <span data-ttu-id="fdb6f-169">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdb6f-169">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="fdb6f-170">Post</span><span class="sxs-lookup"><span data-stu-id="fdb6f-170">Post</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="fdb6f-171">[openTypeExtension](opentypeextension.md) (in einer vorhandenen Ressource Instanz) oder ein neuer [Kontakt](../resources/contact.md), [Ereignis](../resources/event.md)oder [Nachricht](../resources/message.md) , die ein OpenTypeExtension-Objekt enthält.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-171">[openTypeExtension](opentypeextension.md)(in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="fdb6f-172">Dient zum Erstellen eines openTypeExtension-Objekts in einer vorhandenen oder neuen Ressourceninstanz.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-172">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="fdb6f-173">Get</span><span class="sxs-lookup"><span data-stu-id="fdb6f-173">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="fdb6f-174">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="fdb6f-174">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="fdb6f-175">Dient zum Lesen der Eigenschaften und der Beziehungen des openTypeExtension-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-175">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="fdb6f-176">Update</span><span class="sxs-lookup"><span data-stu-id="fdb6f-176">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="fdb6f-177">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="fdb6f-177">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="fdb6f-178">Dient zum Aktualisieren des openTypeExtension-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-178">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="fdb6f-179">Delete</span><span class="sxs-lookup"><span data-stu-id="fdb6f-179">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="fdb6f-180">Keine</span><span class="sxs-lookup"><span data-stu-id="fdb6f-180">None</span></span> |<span data-ttu-id="fdb6f-181">Dient zum Löschen des openTypeExtension-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fdb6f-181">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/opentypeextension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
