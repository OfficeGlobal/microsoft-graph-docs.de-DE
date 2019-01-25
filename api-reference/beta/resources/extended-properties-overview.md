---
title: Übersicht über erweiterte Outlook-Eigenschaften
description: 'Erweiterte Eigenschaften Speichern benutzerdefinierter Daten zulassen und insbesondere dienen als ein Sicherungsmechanismus für apps für den Zugriff auf '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ead40279547fa838b7224a25c3605d0825c3f797
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517995"
---
# <a name="outlook-extended-properties-overview"></a><span data-ttu-id="1fb4b-103">Übersicht über erweiterte Outlook-Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1fb4b-103">Outlook extended properties overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fb4b-p101">Erweiterte Eigenschaften ermöglichen das Speichern von benutzerdefinierten Daten und dienen insbesondere als Fallbackmechanismus, mit dem Apps auf benutzerdefinierte Daten für Outlook-MAPI-Eigenschaften zugreifen können, wenn diese Eigenschaften _noch nicht in den Microsoft Graph-API-Metadaten verfügbar gemacht wurden_. Sie können die REST-API für erweiterte Eigenschaften verwenden, um diese benutzerdefinierten Daten in folgenden Benutzerressourcen zu speichern oder abzurufen:</span><span class="sxs-lookup"><span data-stu-id="1fb4b-p101">Extended properties allow storing custom data and specifically serve as a fallback mechanism for apps to access custom data for Outlook MAPI properties when these properties are _not already exposed in the Microsoft Graph API metadata_. You can use extended properties REST API to store or get such custom data in the following user resources:</span></span>

- [<span data-ttu-id="1fb4b-106">message</span><span class="sxs-lookup"><span data-stu-id="1fb4b-106">message</span></span>](../resources/message.md)
- [<span data-ttu-id="1fb4b-107">mailFolder</span><span class="sxs-lookup"><span data-stu-id="1fb4b-107">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="1fb4b-108">event</span><span class="sxs-lookup"><span data-stu-id="1fb4b-108">event</span></span>](../resources/event.md)
- [<span data-ttu-id="1fb4b-109">calendar</span><span class="sxs-lookup"><span data-stu-id="1fb4b-109">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="1fb4b-110">contact</span><span class="sxs-lookup"><span data-stu-id="1fb4b-110">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="1fb4b-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="1fb4b-111">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="1fb4b-112">Outlook-Aufgabe</span><span class="sxs-lookup"><span data-stu-id="1fb4b-112">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="1fb4b-113">Outlook-Ordner "Aufgaben"</span><span class="sxs-lookup"><span data-stu-id="1fb4b-113">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) 

<span data-ttu-id="1fb4b-114">Möglich sind auch die folgenden Office 365-Gruppenressourcen:</span><span class="sxs-lookup"><span data-stu-id="1fb4b-114">Or, in the following Office 365 group resources:</span></span>

- <span data-ttu-id="1fb4b-115">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="1fb4b-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="1fb4b-116">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="1fb4b-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="1fb4b-117">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="1fb4b-117">group [post](../resources/post.md)</span></span> 

## <a name="use-extended-properties-or-open-extensions"></a><span data-ttu-id="1fb4b-118">Sollten erweiterte Eigenschaften oder offene Erweiterungen verwendet werden?</span><span class="sxs-lookup"><span data-stu-id="1fb4b-118">Use extended properties or open extensions?</span></span>

<span data-ttu-id="1fb4b-p102">In den meisten üblichen Szenarios sollten offene Erweiterungen verwendet werden können (dargestellt durch [openTypeExtension](../resources/opentypeextension.md) und bisher als Office 365-Datenerweiterungen bezeichnet), um benutzerdefinierte Daten für Ressourceninstanzen im Postfach eines Benutzers zu speichern oder darauf zuzugreifen. Verwenden Sie erweiterte Eigenschaften nur, wenn Sie auf benutzerdefinierte Daten für Outlook-MAPI-Eigenschaften zugreifen müssen, die nicht bereits in den [Microsoft Graph-API-Metadaten](https://developer.microsoft.com/graph/docs/overview/call_api) verfügbar gemacht wurden.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-p102">In most common scenarios, you should be able to use open extensions (represented by [openTypeExtension](../resources/opentypeextension.md), formerly known as Office 365 data extensions) to store and access custom data for resource instances in a user's mailbox. Use extended properties only if you need to access custom data for Outlook MAPI properties that are not already exposed in the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api).</span></span>

## <a name="types-of-extended-properties"></a><span data-ttu-id="1fb4b-121">Typen erweiterter Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1fb4b-121">Types of extended properties</span></span>

<span data-ttu-id="1fb4b-122">Je nachdem, ob Sie einen einzelnen oder mehrere Werte (vom gleichen Typ) in einer erweiterten Eigenschaft speichern möchten, können Sie eine erweiterte Eigenschaft als [SingleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) oder als [MultiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-122">Depending on whether you intend to store a single or multiple values (of the same type) in an extended property, you can create an extended property as a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), or [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span></span>

<span data-ttu-id="1fb4b-123">Jeder dieser Typen identifiziert die Eigenschaft nach ihrer **ID** und speichert Daten als **Wert**.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-123">Each of these types identifies the property by its **id** and stores data in **value**.</span></span> 

<span data-ttu-id="1fb4b-124">Sie können die **ID** verwenden, um eine spezifische Ressourceninstanz zusammen mit der erweiterten Eigenschaft abzurufen, oder sie können nach einer einwertigen erweiterten Eigenschaft filtern, um alle Instanzen mit dieser Eigenschaft abzurufen.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-124">You can use **id** to get a specific resource instance together with that extended property, or filter on a single-value extended property to get all the instances that have that property.</span></span> 

<span data-ttu-id="1fb4b-125">**Hinweis** Sie können die REST API nicht dafür verwenden, alle erweiterten Eigenschaften einer spezifischen Instanz in einem Aufruf abzurufen.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-125">**Note** You cannot use the REST API to get all the extended properties of a specific instance in one call.</span></span>
  

### <a name="id-formats"></a><span data-ttu-id="1fb4b-126">ID-Formate</span><span class="sxs-lookup"><span data-stu-id="1fb4b-126">id formats</span></span>

<span data-ttu-id="1fb4b-127">Sie können in drei Formaten **Id** einer erweiterten Eigenschaft angeben:</span><span class="sxs-lookup"><span data-stu-id="1fb4b-127">You can specify **id** of an extended property in one of three formats:</span></span>

- <span data-ttu-id="1fb4b-128">Als eine benannte Eigenschaft, durch die erweiterte Eigenschaftentyp, Namespace und eines Zeichenfolgennamens identifiziert.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-128">As a named property, identified by the extended property type, namespace, and a string name.</span></span>
- <span data-ttu-id="1fb4b-129">Als eine benannte Eigenschaft, durch die erweiterte Eigenschaftentyp, Namespace und einen numerischen Bezeichner identifiziert.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-129">As a named property, identified by the extended property type, namespace, and a numeric identifier.</span></span>
- <span data-ttu-id="1fb4b-130">Format Proptag, identifiziert den Typ der erweiterten Eigenschaft sowie ein [MAPI-Eigenschaftentag](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags).</span><span class="sxs-lookup"><span data-stu-id="1fb4b-130">In a proptag format, identified by the extended property type and a [MAPI property tag](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags).</span></span>

<span data-ttu-id="1fb4b-131">Die nächsten 2 Tabellen beschreiben diese Formate als erweiterte Eigenschaften auf einzelne und mit mehreren Werten angewendet.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-131">The next 2 tables describe these formats as applied to single and multi-value extended properties.</span></span> <span data-ttu-id="1fb4b-132">{_Typ_} stellt den Typ des den oder die Werte der erweiterten Eigenschaft dar.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-132">{_type_} represents the type of the value or values of the extended property.</span></span> <span data-ttu-id="1fb4b-133">In den Beispielen sind dies Zeichenfolgen, ganze Zahlen und Arrays dieser Typen.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-133">Shown in the examples are string, integer, and arrays of these types.</span></span>

<span data-ttu-id="1fb4b-134">**Gültige ID-Formate für einwertige erweiterte Eigenschaften**</span><span class="sxs-lookup"><span data-stu-id="1fb4b-134">**Valid id formats for single-value extended properties**</span></span>

|<span data-ttu-id="1fb4b-135">**Format**</span><span class="sxs-lookup"><span data-stu-id="1fb4b-135">**Format**</span></span>|<span data-ttu-id="1fb4b-136">**Beispiel**</span><span class="sxs-lookup"><span data-stu-id="1fb4b-136">**Example**</span></span>|<span data-ttu-id="1fb4b-137">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="1fb4b-137">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="1fb4b-138">„{_type_} {_guid_} **Name** {_name_}“</span><span class="sxs-lookup"><span data-stu-id="1fb4b-138">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="1fb4b-139">Identifiziert eine Eigenschaft, indem Sie den Namespace (die GUID), zu der sie gehört, und eines Zeichenfolgennamens.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-139">Identifies a property by the namespace (the GUID) it belongs to, and a string name.</span></span>         |
| <span data-ttu-id="1fb4b-140">„{_type_} {_guid_} **Id** {_id_}“</span><span class="sxs-lookup"><span data-stu-id="1fb4b-140">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | <span data-ttu-id="1fb4b-141">Identifiziert eine Eigenschaft durch den Namespace (die GUID), zu der sie gehört, und einen numerischen Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-141">Identifies a property by the namespace (the GUID) it belongs to, and a numeric identifier.</span></span>  |
| <span data-ttu-id="1fb4b-142">"{_Typ_} {_Proptag_}"</span><span class="sxs-lookup"><span data-stu-id="1fb4b-142">"{_type_} {_proptag_}"</span></span>                    | ```"String 0x4001001E"```                                           | <span data-ttu-id="1fb4b-143">Identifiziert eine vordefinierte Eigenschaft von der Eigenschaftentag.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-143">Identifies a pre-defined property by its property tag.</span></span> |

<span data-ttu-id="1fb4b-144">**Gültige ID-Formate für mehrwertige erweiterte Eigenschaften**</span><span class="sxs-lookup"><span data-stu-id="1fb4b-144">**Valid id formats for multi-value extended properties**</span></span>

|<span data-ttu-id="1fb4b-145">**Format**</span><span class="sxs-lookup"><span data-stu-id="1fb4b-145">**Format**</span></span>|<span data-ttu-id="1fb4b-146">**Beispiel**</span><span class="sxs-lookup"><span data-stu-id="1fb4b-146">**Example**</span></span>|<span data-ttu-id="1fb4b-147">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="1fb4b-147">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="1fb4b-148">„{_type_} {_guid_} **Name** {_name_}“</span><span class="sxs-lookup"><span data-stu-id="1fb4b-148">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="1fb4b-149">Identifiziert eine Eigenschaft durch den Namespace (die GUID) und eines Zeichenfolgennamens.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-149">Identifies a property by the namespace (the GUID) and a string name.</span></span>         |
| <span data-ttu-id="1fb4b-150">„{_type_} {_guid_} **Id** {_id_}“</span><span class="sxs-lookup"><span data-stu-id="1fb4b-150">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | <span data-ttu-id="1fb4b-151">Identifiziert eine Eigenschaft durch den Namespace (die GUID) und einen numerischen Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-151">Identifies a property by the namespace (the GUID) and a numeric identifier.</span></span>   |
| <span data-ttu-id="1fb4b-152">"{_Typ_} {_Proptag_}"</span><span class="sxs-lookup"><span data-stu-id="1fb4b-152">"{_type_} {_proptag_}"</span></span>                    | ```"StringArray 0x4002101E"```                                           | <span data-ttu-id="1fb4b-153">Identifiziert eine vordefinierte Eigenschaft von der Eigenschaftentag.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-153">Identifies a pre-defined property by its property tag.</span></span> |


<span data-ttu-id="1fb4b-154">Verwenden Sie eines der Formate für die benannte Eigenschaft, um eine erweiterte Eigenschaft einwertig oder mit mehreren Werten als benutzerdefinierte Eigenschaft zu definieren.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-154">Use either of the named property formats to define a single-value or multi-value extended property as a custom property.</span></span> <span data-ttu-id="1fb4b-155">Zwischen den beiden Formaten ist das erste aus, das eine Zeichenfolge (**Name**) übernimmt das bevorzugte Format Bezug zu erleichtern.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-155">Among the two formats, the first one that takes a string name (**Name**) is the preferred format for ease of reference.</span></span> <span data-ttu-id="1fb4b-156">Benannte Eigenschaften verfügen über ihre [Eigenschaftenbezeichner](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview) in der 0 x 8000-0xfffe Bereich.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-156">Named properties have their [property identifiers](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview) in the 0x8000-0xfffe range.</span></span>

<span data-ttu-id="1fb4b-157">Verwenden Sie das Format Proptag Zugriff auf Eigenschaften, die vordefinierte MAPI oder von einem Client oder Server, und, haben nicht bereits verfügbar gemacht wurde in Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-157">Use the proptag format to access properties predefined by MAPI, or by a client or server, and that have not already been exposed in Microsoft Graph.</span></span> <span data-ttu-id="1fb4b-158">Diese Eigenschaften haben Eigenschaftenbezeichner in der 0 x 0001-0x7fff Bereich.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-158">These properties have property identifiers in the 0x0001-0x7fff range.</span></span> <span data-ttu-id="1fb4b-159">Versuchen Sie nicht, um eine benutzerdefinierte Eigenschaft mit dem Format Proptag zu definieren.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-159">Do not try to define a custom property using the proptag format.</span></span> 

<span data-ttu-id="1fb4b-160">Informationen zum Zuordnen einer erweiterten Eigenschaft zu einer vorhandenen MAPI-Eigenschaft wie dem Eigenschaftsbezeichner und der GUID finden Sie unter \[MS-OXPROPS\] Microsoft Corporation, [„Eigenschaften für Exchange Server-Protokolle“](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="1fb4b-160">You can find information about mapping an extended property to an existing MAPI property, such as the property identifier and GUID, in \[MS-OXPROPS\] Microsoft Corporation, ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span></span>

<span data-ttu-id="1fb4b-161">**Hinweis** Nachdem Sie ein Format für die **ID** ausgewählt haben, sollten Sie nur mit diesem Format auf die betreffende erweiterte Eigenschaft zugreifen.</span><span class="sxs-lookup"><span data-stu-id="1fb4b-161">**Note** After you have chosen one format for the **id**, you should access that extended property by only that format.</span></span>

## <a name="rest-api-operations"></a><span data-ttu-id="1fb4b-162">REST-API-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="1fb4b-162">REST API operations</span></span>
 
<span data-ttu-id="1fb4b-163">Vorgänge für erweiterte Eigenschaften mit einem einzelnen Wert:</span><span class="sxs-lookup"><span data-stu-id="1fb4b-163">Single-value extended property operations:</span></span>

- [<span data-ttu-id="1fb4b-164">Eine erweiterte Eigenschaft in einer neuen oder vorhandenen Ressourceninstanz erstellen</span><span class="sxs-lookup"><span data-stu-id="1fb4b-164">Create an extended property in a new or existing resource instance</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [<span data-ttu-id="1fb4b-165">Eine oder eine Sammlung von Ressourceninstanzen mit einer erweiterten Eigenschaft mit `$expand` oder `$filter` abrufen</span><span class="sxs-lookup"><span data-stu-id="1fb4b-165">Get one or a collection of resource instances with an extended property using `$expand` or `$filter`</span></span>](../api/singlevaluelegacyextendedproperty-get.md)

<span data-ttu-id="1fb4b-166">Vorgänge für erweiterte Eigenschaften mit mehreren Werten:</span><span class="sxs-lookup"><span data-stu-id="1fb4b-166">Multi-value extended property operations:</span></span>

- [<span data-ttu-id="1fb4b-167">Eine erweiterte Eigenschaft in einer neuen oder vorhandenen Ressourceninstanz erstellen</span><span class="sxs-lookup"><span data-stu-id="1fb4b-167">Create an extended property in a new or existing resource instance</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [<span data-ttu-id="1fb4b-168">Eine Ressourceninstanz mit einer erweiterten Eigenschaft mithilfe von `$expand` abrufen</span><span class="sxs-lookup"><span data-stu-id="1fb4b-168">Get a resource instance with an extended property using `$expand`</span></span>](../api/multivaluelegacyextendedproperty-get.md)

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/extended-properties-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
