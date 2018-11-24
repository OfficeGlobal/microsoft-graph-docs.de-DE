# <a name="create-windows10generalconfiguration"></a>windows10GeneralConfiguration erstellen

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Erstellt ein neues [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md)-Objekt.
## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementConfiguration.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Autorisierung|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie als Anforderungstext eine JSON-Darstellung des windows10GeneralConfiguration-Objekts an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie das windows10GeneralConfiguration-Objekt erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|enterpriseCloudPrintDiscoveryEndPoint|Zeichenfolge|Der Endpunkt zur Ermittlung von Clouddruckern.|
|enterpriseCloudPrintOAuthAuthority|Zeichenfolge|Authentifizierungsendpunkt zum Abrufen von OAuth-Token.|
|enterpriseCloudPrintOAuthClientIdentifier|Zeichenfolge|GUID einer Clientanwendung, die berechtigt ist, OAuth-Token von der OAuth Authority.|
|enterpriseCloudPrintResourceIdentifier|Zeichenfolge|OAuth-Ressourcen-URI für den Druckdienst, wie im Azure-Portal konfiguriert.|
|enterpriseCloudPrintDiscoveryMaxLimit|Int32|Maximale Anzahl von Druckern, die von einem Ermittlungsendpunkt abgefragt werden sollen. Dies ist nur eine Mobileinstellung. Gültige Werte: 1 bis 65535.|
|enterpriseCloudPrintMopriaDiscoveryResourceIdentifier|Zeichenfolge|OAuth-Ressourcen-URI für Druckerermittlungsdienst, wie im Azure-Portal konfiguriert.|
|searchBlockDiacritics|Boolean|Gibt an, ob die Suche diakritische Zeichen verwenden kann.|
|searchDisableAutoLanguageDetection|Boolean|Gibt an, ob die automatische Spracherkennung bei der Indizierung von Inhalten und Eigenschaften verwendet werden soll.|
|searchDisableIndexingEncryptedItems|Boolean|Gibt an, ob die Indizierung WIP-geschützter Elemente blockiert werden soll, um zu verhindern, dass diese in Suchergebnissen für Cortana oder Explorer angezeigt werden.|
|searchEnableRemoteQueries|Boolean|Gibt an, ob Remoteabfragen des Indexes dieses Computers blockiert werden sollen.|
|searchDisableIndexerBackoff|Boolean|Gibt an, ob die Sicherungsfunktion der Suchindizierung deaktiviert werden soll.|
|searchDisableIndexingRemovableDrive|Boolean|Gibt an, ob zugelassen werden soll, dass Benutzer Speicherorte auf Wechseldatenträgern hinzufügen, die indiziert werden sollen.|
|searchEnableAutomaticIndexSizeManangement|Boolean|Gibt die Mindestmenge an Festplattenspeicherplatz auf demselben Laufwerk wie der Indexspeicherort an, bevor die Indizierung beendet wird.|
|diagnosticsDataSubmissionMode|[diagnosticDataSubmissionMode](../resources/intune_deviceconfig_diagnosticdatasubmissionmode.md)|Ruft einen Wert ab, der es dem Gerät ermöglicht, Diagnose- und Nutzungstelemetriedaten zu senden, oder ruft diesen ab (z. B. Watson). Mögliche Werte: `userDefined`, `none`, `basic`, `enhanced`, `full`.|
|oneDriveDisableFileSync|Boolean|Ruft einen Wert ab, der es IT-Administratoren ermöglicht, zu verhindern, dass Apps und Features mit Dateien auf OneDrive arbeiten.|
|smartScreenEnableAppInstallControl|Boolean|Ermöglicht IT-Administratoren, zu steuern, ob Benutzer Apps von anderen Orten als dem Store installieren können.|
|personalizationDesktopImageUrl|Zeichenfolge|Eine http- oder https-URL zu einem JPG-, JPEG- oder PNP-Bild, das heruntergeladen und als Desktopbild verwendet werden muss, oder eine Datei-URL zu einem lokalen Bild in dem Dateisystem, das als Desktopbild verwendet werden muss.|
|personalizationLockScreenImageUrl|Zeichenfolge|Eine http- oder https-URL zu einem JPG-, JPEG- oder PNP-Bild, das heruntergeladen und als Sperrbildschirmbild verwendet werden muss, oder eine Datei-URL zu einem lokalen Bild in dem Dateisystem, das als Sperrbildschirmbild verwendet werden muss.|
|bluetoothAllowedServices|String collection|Gibt eine Liste zulässiger Bluetooth-Dienste und -Profile in Zeichenfolgen im Hexadezimalformat an.|
|bluetoothBlockAdvertising|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer Bluetooth-Werbung verwendet.|
|bluetoothBlockDiscoverableMode|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer den sichtbaren Bluetoothmodus verwendet.|
|bluetoothBlockPrePairing|Boolean|Gibt an, ob bestimmte gebündelte Bluetooth-Peripheriegeräte automatisch mit dem Hostgerät gekoppelt werden.|
|edgeBlockAutofill|Boolean|Gibt an, ob AutoAusfüllen blockiert werden soll.|
|edgeBlocked|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer den Edge-Browser verwendet.|
|edgeCookiePolicy|[edgeCookiePolicy](../resources/intune_deviceconfig_edgecookiepolicy.md)|Gibt an, welche Cookies im Edge-Browsers blockiert werden sollen. Mögliche Werte: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.|
|edgeBlockDeveloperTools|Boolean|Gibt an, ob Entwicklertools im Edge-Browser blockiert werden sollen.|
|edgeBlockSendingDoNotTrackHeader|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer die Kopfzeile „Do Not Track“ (nicht verfolgen) sendet.|
|edgeBlockExtensions|Boolean|Gibt an, ob Erweiterungen im Edge-Browser blockiert werden sollen.|
|edgeBlockInPrivateBrowsing|Boolean|Gibt an, ob InPrivate-Browsen in Firmennetzwerken im Edge-Browser blockiert werden soll.|
|edgeBlockJavaScript|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer JavaScript verwendet.|
|edgeBlockPasswordManager|Boolean|Gibt an, ob der Kennwort-Manager blockiert werden soll.|
|edgeBlockAddressBarDropdown|Boolean|Blockiert die Dropdownfunktionalität der Adressleiste in Microsoft Edge. Deaktivieren Sie diese Einstellung, um Netzwerkverbindungen zu Microsoft-Diensten zu minimieren.|
|edgeBlockCompatibilityList|Boolean|Blockiert die Microsoft-Kompatibilitätsliste in Microsoft Edge. Diese Liste von Microsoft hilft Edge beim korrekten Anzeigen von Websites mit bekannten Kompatibilitätsproblemen.|
|edgeClearBrowsingDataOnExit|Boolean|Löscht Browserdaten beim Beenden von Microsoft Edge.|
|edgeAllowStartPagesModification|Boolean|Lässt zu, dass Benutzer Startseiten in Edge ändern. Verwenden Sie „EdgeHomepageUrls“, um Startseiten anzugeben, die dem Benutzer standardmäßig angezeigt werden, wenn er Edge öffnet.|
|edgeDisableFirstRunPage|Boolean|Blockiert die Microsoft-Webseite, die bei der ersten Verwendung von Microsoft Edge geöffnet wird. Mithilfe dieser Richtlinie können Unternehmen diese Seite blockieren, z. B. in Umgebungen mit Nullemissionskonfiguration.|
|edgeBlockLiveTileDataCollection|Boolean|Hiermit wird die Erfassung von Informationen durch Microsoft für die Erstellung von Livekacheln blockiert, wenn Benutzer über Microsoft Edge eine Website an das Startmenü anheften.|
|edgeSyncFavoritesWithInternetExplorer|Boolean|Hiermit wird die Synchronisierung von Favoriten zwischen Internet Explorer und Microsoft Edge aktiviert. Hinzufügungen, Löschungen, Änderungen und Reihenfolgenänderungen bei Favoriten werden zwischen Browsern beibehalten.|
|cellularBlockDataWhenRoaming|Boolean|Gibt an, ob verhindert wird, dass der Benutzer beim Roaming Daten über Mobilfunk verwendet.|
|cellularBlockVpn|Boolean|Gibt an, ob verhindert wird, dass der Benutzer beim Roaming VPN über Mobilfunk verwendet.|
|cellularBlockVpnWhenRoaming|Boolean|Gibt an, ob verhindert wird, dass der Benutzer beim Roaming über Mobilfunk VPN verwendet.|
|defenderBlockEndUserAccess|Boolean|Gibt ab, ob der Endbenutzerzugriff auf Defender blockiert wird.|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Anzahl von Tagen, bevor Schadsoftware in Quarantäne gelöscht werden. Gültige Werte: 0 bis 90.|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune_deviceconfig_defenderdetectedmalwareactions.md)|Ruft Defender-Aktionen für erkannte Schadsoftware pro Bedrohungsstufe an. oder legt diese fest.|
|defenderSystemScanSchedule|[weeklySchedule](../resources/intune_deviceconfig_weeklyschedule.md)|Wochentag für die Systemüberprüfung. Mögliche Werte: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|defenderFilesAndFoldersToExclude|String collection|Dateien und Ordner, die von Überprüfungen und Echtzeitschutz ausgenommen werden sollen.|
|defenderFileExtensionsToExclude|String collection|Dateierweiterungen, die von Überprüfungen und Echtzeitschutz ausgenommen werden sollen.|
|defenderScanMaxCpu|Int32|Prozentsatz der maximalen CPU-Auslastung während der Überprüfung. Gültige Werte: 0 bis 100.|
|defenderMonitorFileActivity|[defenderMonitorFileActivity](../resources/intune_deviceconfig_defendermonitorfileactivity.md)|Wert für die Überwachung der Dateiaktivität. Mögliche Werte: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|defenderProcessesToExclude|String collection|Prozesse, die von Überprüfungen und Echtzeitschutz ausgenommen werden sollen.|
|defenderPromptForSampleSubmission|[defenderPromptForSampleSubmission](../resources/intune_deviceconfig_defenderpromptforsamplesubmission.md)|Die Konfiguration zur Aufforderung des Benutzers, ein Beispiel zu übermitteln. Mögliche Werte: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.|
|defenderRequireBehaviorMonitoring|Boolean|Gibt an, ob eine Verhaltensüberwachung erforderlich ist.|
|defenderRequireCloudProtection|Boolean|Gibt an, ob Cloudschutz erforderlich ist.|
|defenderRequireNetworkInspectionSystem|Boolean|Gibt an, ob ein Netzwerkinspektionssystem erforderlich ist.|
|defenderRequireRealTimeMonitoring|Boolean|Gibt an, ob eine Echtzeitüberwachung erforderlich ist.|
|defenderScanArchiveFiles|Boolean|Gibt an, ob Archivdateien gescannt werden sollen.|
|defenderScanDownloads|Boolean|Gibt an, ob Downloads gescannt werden sollen.|
|defenderScanNetworkFiles|Boolean|Gibt an, ob in einem Netzwerkordner geöffnete Dateien gescannt werden sollen.|
|defenderScanIncomingMail|Boolean|Gibt an, ob eingehende E-Mail-Nachrichten gescannt werden sollen.|
|defenderScanMappedNetworkDrivesDuringFullScan|Boolean|Gibt an, ob zugeordnete Netzwerklaufwerke bei der vollständigen Überprüfung gescannt werden sollen.|
|defenderScanRemovableDrivesDuringFullScan|Boolean|Gibt an, ob Wechseldatenträger bei der vollständigen Überprüfung gescannt werden sollen.|
|defenderScanScriptsLoadedInInternetExplorer|Boolean|Gibt an, ob Skripts, die in Internet Explorer geladen sind, gescannt werden sollen.|
|defenderSignatureUpdateIntervalInHours|Int32|Das Aktualisierungsintervall der Signatur in Stunden. Geben Sie 0, wenn keine Überprüfung ausgeführt werden soll. Gültige Werte: 0 bis 24.|
|defenderScanType|[defenderScanType](../resources/intune_deviceconfig_defenderscantype.md)|Der Überprüfungstyp des Defender-Systems. Mögliche Werte: `userDefined`, `disabled`, `quick`, `full`.|
|defenderScheduledScanTime|TimeOfDay|Die Defender-Uhrzeit für die Systemüberprüfung.|
|defenderScheduledQuickScanTime|TimeOfDay|Die Zeit, zu der eine tägliche Schnellüberprüfung durchgeführt werden soll.|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune_deviceconfig_defendercloudblockleveltype.md)|Gibt die Ebene für Schutz in der Cloud an. Mögliche Werte: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|lockScreenAllowTimeoutConfiguration|Boolean|Gibt an, ob eine vom Benutzer konfigurierbare Einstellung zum Steuern des Bildschirmtimeouts auf dem Sperrbildschirm von Windows 10 Mobile-Geräten angezeigt werden soll. Wenn diese Richtlinie auf „Zulassen“ festgelegt ist, wird der von „lockScreenTimeoutInSeconds“ Wert ignoriert.|
|lockScreenBlockActionCenterNotifications|Boolean|Gibt an, ob Benachrichtigungen des Info-Centers über den Sperrbildschirm blockiert werden sollen.|
|lockScreenBlockCortana|Boolean|Gibt an, ob der Benutzer über die Spracherkennung mit Cortana interagieren kann, solange das System gesperrt ist.|
|lockScreenBlockToastNotifications|Boolean|Gibt an, ob Popupbenachrichtigungen über dem Sperrbildschirm des Geräts zulässig sind.|
|lockScreenTimeoutInSeconds|Int32|Legt die Dauer (in Sekunden) vom Sperren des Bildschirms bis zum Abschalten des Bildschirms für Windows 10 Mobile-Geräte fest. Unterstützte Werte: 11 bis 1800. Gültige Werte: 11 bis 1800.|
|passwordBlockSimple|Boolean|Geben Sie an, ob PINs oder Kennwörter wie „1111“ oder „1234“ zulässig sind. Für Windows 10-Desktops wird dadurch auch die Verwendung von Bildkennwörtern gesteuert.|
|passwordExpirationDays|Int32|Zeitraum in Tagen bis zum Ablaufen des Kennworts Gültige Werte: 0 bis 730.|
|passwordMinimumLength|Int32|Mindestlänge des Kennworts Gültige Werte: 4 bis 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.|
|passwordMinimumCharacterSetCount|Int32|Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen.|
|passwordPreviousPasswordBlockCount|Int32|Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss. Gültige Werte: 0 bis 50.|
|passwordRequired|Boolean|Gibt an, ob der Benutzer ein Kennwort benötigt.|
|passwordRequireWhenResumeFromIdleState|Boolean|Gibt an, ob zum Fortsetzen aus einem Leerlaufstatus ein Kennwort erforderlich ist.|
|passwordRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|Geforderter Kennworttyp. Mögliche Werte: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Die Anzahl von fehlgeschlagenen Anmeldeversuchen, bevor eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird. Gültige Werte: 0 bis 999.|
|privacyAdvertisingId|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|Aktiviert oder deaktiviert die Verwendung einer Werbe-ID. Dies wurde in Windows 10, Version 1607, hinzugefügt. Mögliche Werte: `notConfigured`, `blocked`, `allowed`.|
|privacyAutoAcceptPairingAndConsentPrompts|Boolean|Gibt an, ob beim Starten von Apps das automatische Akzeptieren der Dialogfelder für die Benutzerzustimmung zur Kopplung und zum Datenschutz zulässig ist.|
|privacyBlockInputPersonalization|Boolean|Gibt an, ob die Nutzung cloudbasierter Sprachdienste für Cortana, Diktat oder Store-Apps blockiert wird.|
|startBlockUnpinningAppsFromTaskbar|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer Apps aus der Taskleiste loslöst.|
|startMenuAppListVisibility|[windowsStartMenuAppListVisibilityType](../resources/intune_deviceconfig_windowsstartmenuapplistvisibilitytype.md)|Durch Festlegen dieses Werts wird die App-Liste reduziert oder vollständig entfernt bzw. die entsprechende Option in der App „Einstellungen“ deaktiviert. Mögliche Werte: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.|
|startMenuHideChangeAccountSettings|Boolean|Durch Aktivieren dieser Richtlinie wird die Einstellung zur Kontoänderung in der Benutzerkachel im Startmenü ausgeblendet.|
|startMenuHideFrequentlyUsedApps|Boolean|Durch Aktivieren dieser Richtlinie werden die meistverwendeten Apps aus dem Startmenü ausgeblendet, und die entsprechende Option wird in der App „Einstellungen“ deaktiviert.|
|startMenuHideHibernate|Boolean|Durch Aktivieren dieser Richtlinie wird die Option „Ruhezustand“ nicht mehr im Netzschaltersymbol im Startmenü angezeigt.|
|startMenuHideLock|Boolean|Durch Aktivieren dieser Richtlinie wird die Sperre aus der Benutzerkachel im Startmenü ausgeblendet.|
|startMenuHidePowerButton|Boolean|Durch Aktivieren dieser Richtlinie wird das Netzschaltersymbol aus dem Startmenü ausgeblendet.|
|startMenuHideRecentJumpLists|Boolean|Durch Aktivieren dieser Richtlinie werden die letzten Sprunglisten aus dem Startmenü/der Taskleiste ausgeblendet, und die entsprechende Option wird in der App „Einstellungen“ deaktiviert.|
|startMenuHideRecentlyAddedApps|Boolean|Durch Aktivieren dieser Richtlinie werden zuletzt hinzugefügte Apps aus dem Startmenü ausgeblendet, und die entsprechende Option wird in der App „Einstellungen“ deaktiviert.|
|startMenuHideRestartOptions|Boolean|Durch Aktivieren dieser Richtlinie werden die Optionen „Neu starten“und „Aktualisieren und neu starten“ nicht mehr im Netzschaltersymbol im Startmenü angezeigt.|
|startMenuHideShutDown|Boolean|Durch Aktivieren dieser Richtlinie wird „Herunterfahren/Aktualisieren“ und „Herunterfahren“ aus dem Netzschaltersymbol im Startmenü ausgeblendet.|
|startMenuHideSignOut|Boolean|Durch Aktivieren dieser Richtlinie wird „Abmelden“ aus der Benutzerkachel im Startmenü ausgeblendet.|
|startMenuHideSleep|Boolean|Durch Aktivieren dieser Richtlinie wird „Standbymodus“ aus dem Netzschaltersymbol im Startmenü ausgeblendet|
|startMenuHideSwitchAccount|Boolean|Durch Aktivieren dieser Richtlinie wird „Konto wechseln“ aus der Benutzerkachel im Startmenü ausgeblendet.|
|startMenuHideUserTile|Boolean|Durch Aktivieren dieser Richtlinie wird die Benutzerkachel aus dem Startmenü ausgeblendet.|
|startMenuLayoutEdgeAssetsXml|Binär|Diese Richtlinieneinstellung ermöglicht Ihnen das Importieren von Microsoft Edge-Assets zur Verwendung mit der Richtlinie „startMenuLayoutXml“. Das Startlayout kann eine sekundäre Kachel aus der Edge-App enthalten, die nach der lokalen Edge-Assetdatei sucht. Das lokale Edge-Asset ist in diesem Fall nicht vorhanden und führt dazu, dass die sekundäre Edge-Kachel leer angezeigt wird.  Diese Richtlinie wird nur angewendet, wenn die Richtlinie „startMenuLayoutXml“ geändert wird. Der Wert sollte ein UTF-8-Base64-codiertes Bytearray sein.|
|startMenuLayoutXml|Binär|Ermöglicht Administratoren das Außerkraftsetzen des Startmenü-Standardlayouts und verhindert Änderungen durch den Benutzer. Das Layout wird durch Angabe einer XML-Datei geändert, die auf einem Layoutänderungsschema basiert. XML muss ein UTF8-codiertes Bytearrayformat aufweisen.|
|startMenuMode|[windowsStartMenuModeType](../resources/intune_deviceconfig_windowsstartmenumodetype.md)|Ermöglicht Administratoren zu entscheiden, wie das Startmenü angezeigt wird. Mögliche Werte: `userDefined`, `fullScreen`, `nonFullScreen`.|
|startMenuPinnedFolderDocuments|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Dokumente“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderDownloads|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Downloads“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderFileExplorer|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung „FileExplorer“ im Startmenü Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderHomeGroup|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „ Heimnetzgruppe“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderMusic|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Musik“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderNetwork|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Netzwerk“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPersonalFolder|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem persönlichen Ordner im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPictures|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Bilder“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderSettings|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Einstellungen“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderVideos|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Videos“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|settingsBlockSettingsApp|Boolean|Gibt an, ob der Zugriff auf die App „Einstellungen“ blockiert werden soll.|
|settingsBlockSystemPage|Boolean|Gibt an, ob der Zugriff auf „System“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockDevicesPage|Boolean|Gibt an, ob der Zugriff auf „Geräte“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockNetworkInternetPage|Boolean|Gibt an, ob der Zugriff auf „Netzwerk und Internet“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockPersonalizationPage|Boolean|Gibt an, ob der Zugriff auf „Personalisierung“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockAccountsPage|Boolean|Gibt an, ob der Zugriff auf „Konten“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockTimeLanguagePage|Boolean|Gibt an, ob der Zugriff auf „Zeit und Sprache“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockEaseOfAccessPage|Boolean|Gibt an, ob der Zugriff auf „Erleichterte Bedienung“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockPrivacyPage|Boolean|Gibt an, ob der Zugriff auf „Datenschutz“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockUpdateSecurityPage|Boolean|Gibt an, ob der Zugriff auf „Update und Sicherheit“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockAppsPage|Boolean|Gibt an, ob der Zugriff auf „Apps“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockGamingPage|Boolean|Gibt an, ob der Zugriff auf „Gaming“ in der App „Einstellungen“ blockiert werden soll.|
|windowsSpotlightBlockConsumerSpecificFeatures|Boolean|Ermöglicht IT-Administratoren das Blockieren von Funktionen, die normalerweise nur für Endbenutzer bestimmt sind, beispielsweise Startvorschläge, Mitgliedschaftsbenachrichtigungen, App-Installation nach Anzeige der Windows-Willkommensseite und Kachelumleitungen.|
|windowsSpotlightBlocked|Boolean|Ermöglicht IT-Administratoren das Deaktivieren aller Features von Windows-Blickpunkt.|
|windowsSpotlightBlockOnActionCenter|Boolean|Blockiert Vorschläge von Microsoft, die nach jeder Neuinstallation des Betriebssytem, nach jedem Upgrade oder auf fortlaufender Basis angezeigt werden, um Benutzern Neuigkeiten oder Änderungen vorzustellen.|
|windowsSpotlightBlockTailoredExperiences|Boolean|Blockiert personalisierte Inhalte in Windows-Blickpunkt basierend auf dem Gerät, das der Benutzer verwendet.|
|windowsSpotlightBlockThirdPartyNotifications|Boolean|Blockiert Inhalte von Drittanbietern, die über Windows-Blickpunkt übermittelt werden.|
|windowsSpotlightBlockWelcomeExperience|Boolean|Windows-Begrüßungsseite zur Vorstellung neuer oder aktualisierter Features blockieren|
|windowsSpotlightBlockWindowsTips|Boolean|Ermöglicht IT-Administratoren das Deaktivieren des Popups von Windows-Tipps.|
|windowsSpotlightConfigureOnLockScreen|[windowsSpotlightEnablementSettings](../resources/intune_deviceconfig_windowsspotlightenablementsettings.md)|Gibt den Typ des Spotlight. Mögliche Werte sind: `notConfigured`, `disabled` und `enabled`.|
|networkProxyApplySettingsDeviceWide|Boolescher Wert|Wenn dieser Wert festgelegt ist, werden Proxyeinstellungen auf alle Prozesse und Konten in dem Gerät angewendet. Andernfalls wird er auf das Benutzerkonto angewendet, das bei MDM registriert ist.|
|networkProxyDisableAutoDetect|Boolescher Wert|Deaktiviert die automatische Erkennung von Einstellungen. Wenn diese Option aktiviert ist, versucht das System, den Pfad zu einem PAC-Skript (automatische Proxykonfiguration) zu suchen.|
|networkProxyAutomaticConfigurationUrl|Zeichenfolge|Adresse zu dem PAC-Skript, das Sie verwenden möchten.|
|networkProxyServer|[windows10NetworkProxyServer](../resources/intune_deviceconfig_windows10networkproxyserver.md)|Gibt manuelle Proxyservereinstellungen an.|
|accountsBlockAddingNonMicrosoftAccountEmail|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer E-Mail-Konten zu Geräten hinzufügt, die keinem Microsoft-Konto zugeordnet sind.|
|antiTheftModeBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer eine Einstellung für den AntiTheft-Modus auswählt (nur Windows 10 Mobile).|
|bluetoothBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Bluetooth verwendet.|
|cameraBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.|
|connectedDevicesServiceBlocked|Boolescher Wert|Gibt an, ob der Dienst für verbundene Geräte blockiert werden soll, der die Ermittlung anderer Geräte und eine Verbindungsherstellung zu anderen Geräten, Remotmessaging, Remote-App-Sitzungen und anderen geräteübergreifenden Oberflächen ermöglicht.|
|certificatesBlockManualRootCertificateInstallation|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer eine manuelle Stammzertifikatinstallation ausführt.|
|copyPasteBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Kopieren/Einfügen verwendet.|
|cortanaBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Cortana verwendet.|
|deviceManagementBlockFactoryResetOnMobile|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer sein Telefon zurücksetzt.|
|deviceManagementBlockManualUnenroll|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer eine manuelle Aufhebung der Registrierung von der Geräteverwaltung vornimmt.|
|safeSearchFilter|[safeSearchFilterType](../resources/intune_deviceconfig_safesearchfiltertype.md)|Gibt an, welche Filterebene von SafeSearch erforderlich ist. Mögliche Werte: `userDefined`, `strict`, `moderate`.|
|edgeBlockPopups|Boolescher Wert|Gibt an, ob Popups blockiert werden sollen.|
|edgeBlockSearchSuggestions|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Suchvorschläge in der Adressleiste verwendet.|
|edgeBlockSendingIntranetTrafficToInternetExplorer|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Intranetverkehr aus Edge an Internet Explorer sendet.|
|edgeRequireSmartScreen|Boolescher Wert|Gibt an, ob der Benutzer aufgefordert werden soll, den Smartscreenfilter zu verwenden.|
|edgeEnterpriseModeSiteListLocation|Zeichenfolge|Gibt den Speicherort der Siteliste für den Unternehmensmodus an. Dies kann eine lokale Datei, ein lokales Netzwerk oder ein http-Speicherort sein.|
|edgeFirstRunUrl|Zeichenfolge|Die URL für erste Ausführung, wenn der Edge-Browser das erste Mal geöffnet wird.|
|edgeSearchEngine|[edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)|Ermöglicht es IT-Administratoren, eine standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen. Benutzer können dies außer Kraft setzen und die standardmäßige Suchmaschine ändern, sofern die Richtlinie „AllowSearchEngineCustomization“ nicht festgelegt ist.|
|edgeHomepageUrls|Zeichenfolgenauflistung|Die Liste von URLs für Startseiten, die auf bei MDM-registrierten Geräten im Edge-Browser angezeigt werden.|
|edgeBlockAccessToAboutFlags|Boolescher Wert|Gibt an, ob Zugriff auf Info-Flags im Edge-Browser verhindert werden soll.|
|smartScreenBlockPromptOverride|Boolescher Wert|Gibt an, ob Benutzer SmartScreenFilter-Warnungen zu potenziell bösartigen Websites außer Kraft setzen können.|
|smartScreenBlockPromptOverrideForFiles|Boolescher Wert|Gibt an, ob Benutzer die SmartScreenFilter-Warnungen zum Herunterladen nicht überprüfter Dateien außer Kraft setzen können.|
|webRtcBlockLocalhostIpAddress|Boolescher Wert|Gibt an, ob die LocalHost-IP-Adresse des Benutzers angezeigt wird, während Telefonanrufe über WebRTC getätigt werden.|
|internetSharingBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Internetfreigabe verwendet.|
|settingsBlockAddProvisioningPackage|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Bereitstellungspakete installiert.|
|settingsBlockRemoveProvisioningPackage|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Laufzeitkonfigurations-Agent Bereitstellungspakete entfernt.|
|settingsBlockChangeSystemTime|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer die Einstellungen für Datum und Uhrzeit ändert.|
|settingsBlockEditDeviceName|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer den Gerätenamen bearbeitet.|
|settingsBlockChangeRegion|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Regionseinstellungen ändert.|
|settingsBlockChangeLanguage|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Spracheinstellungen ändert.|
|settingsBlockChangePowerSleep|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Energie- und Energiesparmoduseinstellungen ändert.|
|locationServicesBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Ortungsdienste verwendet.|
|microsoftAccountBlocked|Boolescher Wert|Gibt an, ob ein Microsoft-Konto blockiert werden soll.|
|microsoftAccountBlockSettingsSync|Boolescher Wert|Gibt an, ob die Synchronisierung von Einstellungen eines Microsoft-Kontos blockiert werden soll.|
|nfcBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Near Field Communication verwendet.|
|resetProtectionModeBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer den Schutzmodus zurücksetzt.|
|screenCaptureBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Screenshots macht.|
|storageBlockRemovableStorage|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Wechselmedien verwendet.|
|storageRequireMobileDeviceEncryption|Boolescher Wert|Gibt an, ob für ein mobiles Gerät eine Verschlüsselung erforderlich ist.|
|usbBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer eine USB-Verbindung verwendet.|
|voiceRecordingBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer die Sprachaufzeichnung verwendet.|
|wiFiBlockAutomaticConnectHotspots|Boolescher Wert|Gibt an, ob die automatische Herstellung einer Verbindung zu WLAN-Hotspots blockiert werden soll. Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.|
|wiFiBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer WLAN verwendet.|
|wiFiBlockManualConfiguration|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer eine manuelle WLAN-Konfiguration verwendet.|
|wiFiScanInterval|Int32|Gibt an, wie häufig Geräte nach WLAN-Netzwerken suchen. Unterstützte Werte sind 1 bis 500, wobei 100 der Standardwert ist und 500 eine niedrige Häufigkeit bedeutet. Gültige Werte: 1 bis 500.|
|wirelessDisplayBlockProjectionToThisDevice|Boolescher Wert|Gibt an, ob erlaubt werden soll, dass andere Geräte diesen Computer für die Projektion ermitteln.|
|wirelessDisplayBlockUserInputFromReceiver|Boolescher Wert|Gibt an, ob Benutzereingaben von drahtlosen Anzeigeempfängern erlaubt sind.|
|wirelessDisplayRequirePinForPairing|Boolescher Wert|Gibt an, ob eine PIN für neue Geräte zum Initiieren der Kopplung erforderlich ist.|
|windowsStoreBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer den Windows Store verwendet.|
|appsAllowTrustedAppsSideloading|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|Gibt an, ob Apps aus AppX-Paketen, die mit einem vertrauenswürdigen Zertifikat signiert sind, quergeladen werden können. Mögliche Werte: `notConfigured`, `blocked`, `allowed`.|
|windowsStoreBlockAutoUpdate|Boolescher Wert|Gibt an, ob automatische Updates von Apps aus dem Windows Store blockiert werden sollen.|
|developerUnlockSetting|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|Gibt an, ob die Entwicklersperre zulässig ist. Mögliche Werte: `notConfigured`, `blocked`, `allowed`.|
|sharedUserAppDataAllowed|Boolescher Wert|Gibt an, ob verhindert werden soll, dass mehrere Benutzer derselben App Daten austauschen.|
|appsBlockWindowsStoreOriginatedApps|Boolescher Wert|Gibt an, ob das Starten aller Apps aus dem Windows Store deaktiviert werden soll, die vorinstalliert waren oder heruntergeladen wurden.|
|windowsStoreEnablePrivateStoreOnly|Boolescher Wert|Gibt an, ob nur der private Store aktiviert werden soll.|
|storageRestrictAppDataToSystemVolume|Boolescher Wert|Gibt an, ob Anwendungsdaten auf das Systemlaufwerk beschränkt sind.|
|storageRestrictAppInstallToSystemVolume|Boolescher Wert|Gibt an, ob die Installation von Anwendungen auf das Systemlaufwerk beschränkt ist.|
|gameDvrBlocked|Boolescher Wert|Gibt an, ob DVR und Broadcasting blockiert werden soll.|
|experienceBlockDeviceDiscovery|Boolescher Wert|Gibt an, ob die Geräteerkennungs-UX aktiviert werden soll.|
|experienceBlockErrorDialogWhenNoSIM|Boolescher Wert|Gibt an, ob das Fehlerdialogfeld angezeigt werden soll, wenn keine SIM-Karte erkannt wird.|
|experienceBlockTaskSwitcher|Boolescher Wert|Gibt an, ob die Programmumschaltung auf dem Gerät aktiviert werden soll.|
|logonBlockFastUserSwitching|Boolescher Wert|Verhindert, dass schnell zwischen Benutzern umgeschaltet werden kann, die gleichzeitig ohne Abmelden angemeldet sind.|
|tenantLockdownRequireNetworkDuringOutOfBoxExperience|Boolescher Wert|Gibt an, ob das Gerät für die Verbindung mit dem Netzwerk erforderlich ist.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) im Antworttext zurück.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 9768

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9940

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true
}
```



