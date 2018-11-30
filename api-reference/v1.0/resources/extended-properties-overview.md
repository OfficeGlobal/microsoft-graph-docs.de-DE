---
title: Übersicht über erweiterte Outlook-Eigenschaften
description: 'Erweiterte Eigenschaften Speichern benutzerdefinierter Daten zulassen und insbesondere dienen als ein Sicherungsmechanismus für apps für den Zugriff auf '
ms.openlocfilehash: 062c39eca7a32f52f88334b43a79ad413b986ad7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016897"
---
# <a name="outlook-extended-properties-overview"></a>Übersicht über erweiterte Outlook-Eigenschaften

Erweiterte Eigenschaften ermöglichen das Speichern von benutzerdefinierten Daten und dienen insbesondere als Fallbackmechanismus, mit dem Apps auf benutzerdefinierte Daten für Outlook-MAPI-Eigenschaften zugreifen können, wenn diese Eigenschaften _noch nicht in den Microsoft Graph-API-Metadaten verfügbar gemacht wurden_. Sie können die REST-API für erweiterte Eigenschaften verwenden, um diese benutzerdefinierten Daten in folgenden Benutzerressourcen zu speichern oder abzurufen:

- [message](../resources/message.md)
- [mailFolder](../resources/mailfolder.md)
- [event](../resources/event.md)
- [calendar](../resources/calendar.md)
- [contact](../resources/contact.md)
- [contactFolder](../resources/contactfolder.md) 

Möglich sind auch die folgenden Office 365-Gruppenressourcen:

- [event](../resources/event.md)-Ressourcen für Gruppen
- [calendar](../resources/calendar.md)-Ressourcen für Gruppen
- [post](../resources/post.md)-Ressourcen für Gruppen 

## <a name="use-extended-properties-or-open-extensions"></a>Sollten erweiterte Eigenschaften oder offene Erweiterungen verwendet werden?

In den meisten üblichen Szenarios sollten offene Erweiterungen verwendet werden können (dargestellt durch [openTypeExtension](../resources/opentypeextension.md) und bisher als Office 365-Datenerweiterungen bezeichnet), um benutzerdefinierte Daten für Ressourceninstanzen im Postfach eines Benutzers zu speichern oder darauf zuzugreifen. Verwenden Sie erweiterte Eigenschaften nur, wenn Sie auf benutzerdefinierte Daten für Outlook-MAPI-Eigenschaften zugreifen müssen, die nicht bereits in den [Microsoft Graph-API-Metadaten](https://developer.microsoft.com/graph/docs/overview/call_api) verfügbar gemacht wurden. 

## <a name="types-of-extended-properties"></a>Typen erweiterter Eigenschaften

Je nachdem, ob Sie einen einzelnen oder mehrere Werte (vom gleichen Typ) in einer erweiterten Eigenschaft speichern möchten, können Sie eine erweiterte Eigenschaft als [SingleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) oder als [MultiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) erstellen.

Jeder dieser Typen identifiziert die Eigenschaft nach ihrer **ID** und speichert Daten als **Wert**. 

Sie können die **ID** verwenden, um eine spezifische Ressourceninstanz zusammen mit der erweiterten Eigenschaft abzurufen, oder sie können nach einer einwertigen erweiterten Eigenschaft filtern, um alle Instanzen mit dieser Eigenschaft abzurufen. 

**Hinweis** Sie können die REST API nicht dafür verwenden, alle erweiterten Eigenschaften einer spezifischen Instanz in einem Aufruf abzurufen.
  

### <a name="id-formats"></a>ID-Formate

Sie können in drei Formaten **Id** einer erweiterten Eigenschaft angeben:

- Als eine benannte Eigenschaft, durch die erweiterte Eigenschaftentyp, Namespace und eines Zeichenfolgennamens identifiziert.
- Als eine benannte Eigenschaft, durch die erweiterte Eigenschaftentyp, Namespace und einen numerischen Bezeichner identifiziert.
- Format Proptag, identifiziert den Typ der erweiterten Eigenschaft sowie ein [MAPI-Eigenschaftentag](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags).

Die nächsten 2 Tabellen beschreiben diese Formate als erweiterte Eigenschaften auf einzelne und mit mehreren Werten angewendet. {_Typ_} stellt den Typ des den oder die Werte der erweiterten Eigenschaft dar. In den Beispielen sind dies Zeichenfolgen, ganze Zahlen und Arrays dieser Typen.

**Gültige ID-Formate für einwertige erweiterte Eigenschaften**

|**Format**|**Beispiel**|**Beschreibung**|
|:---------|:----------|:--------------|
| „{_type_} {_guid_} **Name** {_name_}“ | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | Identifiziert eine Eigenschaft, indem Sie den Namespace (die GUID), zu der sie gehört, und eines Zeichenfolgennamens.         |
| „{_type_} {_guid_} **Id** {_id_}“     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | Identifiziert eine Eigenschaft durch den Namespace (die GUID), zu der sie gehört, und einen numerischen Bezeichner.  |
| "{_Typ_} {_Proptag_}"                    | ```"String 0x4001001E"```                                           | Identifiziert eine vordefinierte Eigenschaft von der Eigenschaftentag. |

**Gültige ID-Formate für mehrwertige erweiterte Eigenschaften**

|**Format**|**Beispiel**|**Beschreibung**|
|:---------|:----------|:--------------|
| „{_type_} {_guid_} **Name** {_name_}“ | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | Identifiziert eine Eigenschaft durch den Namespace (die GUID) und eines Zeichenfolgennamens.         |
| „{_type_} {_guid_} **Id** {_id_}“     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | Identifiziert eine Eigenschaft durch den Namespace (die GUID) und einen numerischen Bezeichner.   |
| "{_Typ_} {_Proptag_}"                    | ```"StringArray 0x4002101E"```                                           | Identifiziert eine vordefinierte Eigenschaft von der Eigenschaftentag. |


Verwenden Sie eines der Formate für die benannte Eigenschaft, um eine erweiterte Eigenschaft einwertig oder mit mehreren Werten als benutzerdefinierte Eigenschaft zu definieren. Zwischen den beiden Formaten ist das erste aus, das eine Zeichenfolge (**Name**) übernimmt das bevorzugte Format Bezug zu erleichtern. Benannte Eigenschaften verfügen über ihre [Eigenschaftenbezeichner](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview) in der 0 x 8000-0xfffe Bereich.

Verwenden Sie das Format Proptag Zugriff auf Eigenschaften, die vordefinierte MAPI oder von einem Client oder Server, und, haben nicht bereits verfügbar gemacht wurde in Microsoft Graph. Diese Eigenschaften haben Eigenschaftenbezeichner in der 0 x 0001-0x7fff Bereich. Versuchen Sie nicht, um eine benutzerdefinierte Eigenschaft mit dem Format Proptag zu definieren. 

Informationen zum Zuordnen einer erweiterten Eigenschaft zu einer vorhandenen MAPI-Eigenschaft wie dem Eigenschaftsbezeichner und der GUID finden Sie unter \[MS-OXPROPS\] Microsoft Corporation, [„Eigenschaften für Exchange Server-Protokolle“](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).

**Hinweis** Nachdem Sie ein Format für die **ID** ausgewählt haben, sollten Sie nur mit diesem Format auf die betreffende erweiterte Eigenschaft zugreifen.

### <a name="rest-api-operations"></a>REST-API-Vorgänge
 
Vorgänge für erweiterte Eigenschaften mit einem einzelnen Wert:

- [Eine erweiterte Eigenschaft in einer neuen oder vorhandenen Ressourceninstanz erstellen](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [Eine oder eine Sammlung von Ressourceninstanzen mit einer erweiterten Eigenschaft mit `$expand` oder `$filter` abrufen](../api/singlevaluelegacyextendedproperty-get.md)

Vorgänge für erweiterte Eigenschaften mit mehreren Werten:

- [Eine erweiterte Eigenschaft in einer neuen oder vorhandenen Ressourceninstanz erstellen](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [Eine Ressourceninstanz mit einer erweiterten Eigenschaft mithilfe von `$expand` abrufen](../api/multivaluelegacyextendedproperty-get.md)

