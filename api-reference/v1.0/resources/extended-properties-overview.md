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

In den meisten üblichen Szenarios sollten offene Erweiterungen verwendet werden können (dargestellt durch [openTypeExtension](../resources/opentypeextension.md) und bisher als Office 365-Datenerweiterungen bezeichnet), um benutzerdefinierte Daten für Ressourceninstanzen im Postfach eines Benutzers zu speichern oder darauf zuzugreifen. Verwenden Sie erweiterte Eigenschaften nur, wenn Sie auf benutzerdefinierte Daten für Outlook-MAPI-Eigenschaften zugreifen müssen, die nicht bereits in den [Microsoft Graph-API-Metadaten]((http://developer.microsoft.com/de-DE/graph/docs/overview/call_api)) verfügbar gemacht wurden. 

## <a name="types-of-extended-properties"></a>Typen erweiterter Eigenschaften

Je nachdem, ob Sie einen einzelnen oder mehrere Werte (vom gleichen Typ) in einer erweiterten Eigenschaft speichern möchten, können Sie eine erweiterte Eigenschaft als [SingleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) oder als [MultiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) erstellen.

Jeder dieser Typen identifiziert die Eigenschaft nach ihrer **ID** und speichert Daten als **Wert**. 

Sie können die **ID** verwenden, um eine spezifische Ressourceninstanz zusammen mit der erweiterten Eigenschaft abzurufen, oder sie können nach einer einwertigen erweiterten Eigenschaft filtern, um alle Instanzen mit dieser Eigenschaft abzurufen. 

**Hinweis** Sie können die REST API nicht dafür verwenden, alle erweiterten Eigenschaften einer spezifischen Instanz in einem Aufruf abzurufen.
  

### <a name="id-formats"></a>ID-Formate

Wenn Sie eine einwertige oder mehrwertige erweiterte Eigenschaft erstellen, können Sie die **id**-Eigenschaft in einem von zwei Formaten angeben, basierend auf einem Zeichenfolgennamen (**Name**) oder numerischen Bezeichner (**Id**) und auf dem tatsächlichen Typ des Werts bzw. der Werte der Eigenschaft. Die folgenden zwei Tabellen enthalten die unterstützten Formate zum Angeben von ein- oder mehrwertigen erweiterten Eigenschaften. {_type_} stellt den Typ des Werts bzw. der Werte für die Eigenschaft dar. In den Beispielen sind dies Zeichenfolgen, ganze Zahlen und Arrays dieser Typen.

Da erweiterte Eigenschaften in den meisten Fällen mit definierten MAPI-Eigenschaften zusammenarbeiten, die nicht in den Microsoft Graph-API-Metadaten verfügbar gemacht wurden, sollte das Format der Einfachheit halber angeben, ob die entsprechende MAPI-Eigenschaft eine Zeichenfolge aus Zeichen oder einen numerischen Wert in ihrem [MAPI-Eigenschaftsbezeichner]((https://msdn.microsoft.com/de-DE/library/office/cc815528.aspx)) verwendet.
Informationen zum Zuordnen einer erweiterten Eigenschaft zu einer vorhandenen MAPI-Eigenschaft wie dem Eigenschaftsbezeichner und der GUID finden Sie unter \[MS-OXPROPS\] Microsoft Corporation, [„Eigenschaften für Exchange Server-Protokolle“](https://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx).

**Hinweis** Nachdem Sie ein Format für die **ID** ausgewählt haben, sollten Sie nur mit diesem Format auf die betreffende erweiterte Eigenschaft zugreifen.


**Gültige ID-Formate für einwertige erweiterte Eigenschaften**

|**Format**|**Beispiel**|**Beschreibung**|
|:---------|:----------|:--------------|
| „{_type_} {_guid_} **Name** {_name_}“ | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | Identifiziert eine Eigenschaft nach dem Namespace (der GUID), zu dem sie gehört, und einem Namen.         |
| „{_type_} {_guid_} **Id** {_id_}“     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | Identifiziert eine Eigenschaft nach dem Namespace (der GUID), zu dem sie gehört, und einem Bezeichner.  |

**Gültige ID-Formate für mehrwertige erweiterte Eigenschaften**

|**Format**|**Beispiel**|**Beschreibung**|
|:---------|:----------|:--------------|
| „{_type_} {_guid_} **Name** {_name_}“ | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | Identifiziert eine Eigenschaft nach Namespace (der GUID) und Namen.         |
| „{_type_} {_guid_} **Id** {_id_}“     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | Identifiziert eine Eigenschaft nach Namespace (der GUID) und Bezeichner.   |

### <a name="rest-api-operations"></a>REST-API-Vorgänge
 
Vorgänge für erweiterte Eigenschaften mit einem einzelnen Wert:

- [Eine erweiterte Eigenschaft in einer neuen oder vorhandenen Ressourceninstanz erstellen](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md)
- [Eine oder eine Sammlung von Ressourceninstanzen mit einer erweiterten Eigenschaft mit `$expand` oder `$filter` abrufen](../api/singlevaluelegacyextendedproperty_get.md)

Vorgänge für erweiterte Eigenschaften mit mehreren Werten:

- [Eine erweiterte Eigenschaft in einer neuen oder vorhandenen Ressourceninstanz erstellen](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md)
- [Eine Ressourceninstanz mit einer erweiterten Eigenschaft mithilfe von `$expand` abrufen](../api/multivaluelegacyextendedproperty_get.md)

