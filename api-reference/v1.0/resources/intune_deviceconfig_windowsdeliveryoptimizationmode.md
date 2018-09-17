# <a name="windowsdeliveryoptimizationmode-enum-type"></a>WindowsDeliveryOptimizationMode Enumerationstyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Zustellungsoptimierungsmodus für Peer-Zustellung
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|userDefined|0|Dem Benutzer ermöglichen, Folgendes festzulegen.|
|httpOnly|1|Nur HTTP, kein Peering|
|httpWithPeeringNat|2|OS-Standard – Http gemischt mit Peering hinter dem gleichen Nezwerkadressen-Konvertierungsprogramm|
|httpWithPeeringPrivateGroup|3|HTTP gemischt mit Peering über eine private Gruppe|
|httpWithInternetPeering|4|HTTP gemischt mit Internet-Peering|
|simpleDownload|99|Einfacher Downloadmodus ohne Peering|
|bypassMode|100|Umgehungsmodus Keine Zustellungsoptimierung verwenden, sondern BITS|








