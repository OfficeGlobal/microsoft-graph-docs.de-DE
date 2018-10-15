# <a name="outlook-extended-properties-overview"></a>Übersicht über erweiterte Outlook-Eigenschaften

Erweiterte Eigenschaften ermöglichen das Speichern von benutzerdefinierten Daten und dienen insbesondere als Fallbackmechanismus, mit dem Apps auf benutzerdefinierte Daten für Outlook-MAPI-Eigenschaften zugreifen können, wenn diese Eigenschaften _noch nicht in den Microsoft Graph-API-Metadaten verfügbar gemacht wurden_. Sie können die REST-API für erweiterte Eigenschaften verwenden, um diese benutzerdefinierten Daten in folgenden Benutzerressourcen zu speichern oder abzurufen:

- [message](../resources/message.md)
- [mailFolder](../resources/mailfolder.md)
- [Ereignis](../resources/event.md)
- [Kalender](../resources/calendar.md)
- [Kontakt](../resources/contact.md)
- [contactFolder](../resources/contactfolder.md) 

Möglich sind auch die folgenden Office 365-Gruppenressourcen:

- [event](../resources/event.md)-Ressourcen für Gruppen
- [calendar](../resources/calendar.md)-Ressourcen für Gruppen
- [post](../resources/post.md)-Ressourcen für Gruppen 

## <a name="use-extended-properties-or-open-extensions"></a>Sollten erweiterte Eigenschaften oder offene Erweiterungen verwendet werden?

In den meisten üblichen Szenarios sollten offene Erweiterungen verwendet werden können (dargestellt durch [openTypeExtension](../resources/opentypeextension.md) und bisher als Office 365-Datenerweiterungen bezeichnet), um benutzerdefinierte Daten für Ressourceninstanzen im Postfach eines Benutzers zu speichern oder darauf zuzugreifen. Verwenden Sie erweiterte Eigenschaften nur, wenn Sie auf benutzerdefinierte Daten für Outlook-MAPI-Eigenschaften zugreifen müssen, die nicht bereits in den [Microsoft Graph-API-Metadaten](http://developer.microsoft.com/en-us/graph/docs/overview/call_api) verfügbar gemacht wurden. 

## <a name="types-of-extended-properties"></a>Typen erweiterter Eigenschaften

Je nachdem, ob Sie einen einzelnen oder mehrere Werte (vom gleichen Typ) in einer erweiterten Eigenschaft speichern möchten, können Sie eine erweiterte Eigenschaft als [SingleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) oder als [MultiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) erstellen.

Jeder dieser Typen identifiziert die Eigenschaft nach ihrer **ID** und speichert Daten als **Wert**. 

Sie können die **ID** verwenden, um eine spezifische Ressourceninstanz zusammen mit der erweiterten Eigenschaft abzurufen, oder sie können nach einer einwertigen erweiterten Eigenschaft filtern, um alle Instanzen mit dieser Eigenschaft abzurufen. 

**Hinweis** Sie können die REST API nicht dafür verwenden, alle erweiterten Eigenschaften einer spezifischen Instanz in einem Aufruf abzurufen.
  

### <a name="id-formats"></a>id formats

Sie können die **id** einer erweiterten Eigenschaft in drei Formaten angeben:

- Als eine benannte Eigenschaft, identifiziert durch den erweiterten Eigenschaftentyp, als Namespace und als einen Zeichenfolgennamen.
- Als eine benannte Eigenschaft, identifiziert durch den erweiterten Eigenschaftentyp, als Namespace und als einen numerischen Bezeichner.
- Im Format Proptag, identifiziert durch den erweiterten Eigenschaftentyp sowie ein [MAPI-Eigenschaftentag](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags).

Die nächsten 2 Tabellen beschreiben diese Formate als erweiterte Eigenschaften, angewendet auf einzelne und mehrere Werten. {_type_} stellt den Typ des Werts bzw. der Werte für die erweiterte Eigenschaft dar. In den Beispielen sind dies Zeichenfolgen, ganze Zahlen und Arrays dieser Typen.

**Gültige ID-Formate für einwertige erweiterte Eigenschaften**

|**Format**|**Beispiel**|**Beschreibung**|
|:---------|:----------|:--------------|
| „{_type_} {_guid_} **Name** {_name_}“ | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | Identifiziert eine Eigenschaft nach dem Namespace (der GUID), zu dem sie gehört, und einem Zeichenfolgenamen.         |
| „{_type_} {_guid_} **Id** {_id_}“     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | Identifiziert eine Eigenschaft nach dem Namespace (der GUID), zu dem sie gehört, und einem numerischen Bezeichner.  |
| "{_type_} {_proptag_}"                    | ```"String 0x4001001E"```                                           | Identifiziert eine vordefinierte Eigenschaft über ihren Eigenschaftentag. |

**Gültige ID-Formate für mehrwertige erweiterte Eigenschaften**

|**Format**|**Beispiel**|**Beschreibung**|
|:---------|:----------|:--------------|
| „{_type_} {_guid_} **Name** {_name_}“ | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | Identifiziert eine Eigenschaft nach dem Namespace (der GUID) und einem Zeichenfolgenamen.         |
| „{_type_} {_guid_} **Id** {_id_}“     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | Identifiziert eine Eigenschaft nach dem Namespace (der GUID) und einem numerischen Bezeichner.   |
| "{_type_} {_proptag_}"                    | ```"StringArray 0x4002101E"```                                           | Identifiziert eine vordefinierte Eigenschaft über ihren Eigenschaftentag. |


Verwenden Sie eines der Formate für die benannte Eigenschaft, um eine erweiterte Eigenschaft mit einem oder mit mehreren Werten als benutzerdefinierte Eigenschaft zu definieren. Bei den beiden Formaten bezieht das erste einen Zeichenfolgenamen (**Name**) und ist der Einfachheit halber das bevorzugte Format. Benannte Eigenschaften verfügen über ihre [Eigenschaftenbezeichner](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview) in der Spanne 0x8000-0xfffe.

Verwenden Sie das Format Proptag um auf Eigenschaften zuzugreifen, die mit MAPI oder von einem Client oder Server vordefiniert wurden und nicht die noch nicht in Microsoft Graph verfügbar gemacht wurden. Diese Eigenschaften haben Eigenschaftenbezeichner in der Spanne 0x0001-0x7fff. Versuchen Sie nicht, eine benutzerdefinierte Eigenschaft mit dem Format Proptag zu definieren. 

Informationen zum Zuordnen einer erweiterten Eigenschaft zu einer vorhandenen MAPI-Eigenschaft wie dem Eigenschaftsbezeichner und der GUID finden Sie unter \[MS-OXPROPS\] Microsoft Corporation, [„Eigenschaften für Exchange Server-Protokolle“](https://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx).

**Hinweis** Nachdem Sie ein Format für die **ID** ausgewählt haben, sollten Sie nur mit diesem Format auf die betreffende erweiterte Eigenschaft zugreifen.

### <a name="rest-api-operations"></a>REST-API-Vorgänge
 
Vorgänge für erweiterte Eigenschaften mit einem einzelnen Wert:

- [Eine erweiterte Eigenschaft in einer neuen oder vorhandenen Ressourceninstanz erstellen](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md)
- [Eine oder eine Sammlung von Ressourceninstanzen mit einer erweiterten Eigenschaft mit `$expand` oder `$filter` abrufen `$filter`](../api/singlevaluelegacyextendedproperty_get.md)

Vorgänge für erweiterte Eigenschaften mit mehreren Werten:

- [Eine erweiterte Eigenschaft in einer neuen oder vorhandenen Ressourceninstanz erstellen](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md)
- [Eine Ressourceninstanz mit einer erweiterten Eigenschaft mithilfe von `$expand` abrufen `$expand`](../api/multivaluelegacyextendedproperty_get.md)

