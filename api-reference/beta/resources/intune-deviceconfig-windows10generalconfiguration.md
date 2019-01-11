---
title: windows10GeneralConfiguration-Ressourcentyp
description: In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „windows10GeneralConfiguration“ verfügbar gemacht werden.
localization_priority: Normal
ms.openlocfilehash: a4fa24d6ef11608d19649925debf3a4855b61e98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845507"
---
# <a name="windows10generalconfiguration-resource-type"></a>windows10GeneralConfiguration-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „windows10GeneralConfiguration“ verfügbar gemacht werden.

Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[windows10GeneralConfigurations auflisten](../api/intune-deviceconfig-windows10generalconfiguration-list.md)|[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)-Sammlung|Listet die Eigenschaften und Beziehungen der [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)-Objekte auf.|
|[windows10GeneralConfigurations abrufen](../api/intune-deviceconfig-windows10generalconfiguration-get.md)|[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)|Liest die Eigenschaften und Beziehungen des [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)-Objekts.|
|[windows10GeneralConfiguration erstellen](../api/intune-deviceconfig-windows10generalconfiguration-create.md)|[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)|Erstellt ein neues [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)-Objekt.|
|[windows10GeneralConfiguration löschen](../api/intune-deviceconfig-windows10generalconfiguration-delete.md)|Keine|Löscht eine [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)|
|[windows10GeneralConfiguration aktualisieren](../api/intune-deviceconfig-windows10generalconfiguration-update.md)|[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)|Aktualisiert die Eigenschaften eines [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Collection von Objekten des Typs „String“|Liste der Bereich Tags für diese Instanz der Entität. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt. Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden. Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|windows10AppsForceUpdateSchedule|[windows10AppsForceUpdateSchedule](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|Windows 10 Force Zeitplan für die Aktualisierung für Apps.|
|enableAutomaticRedeployment|Boolean|Zulassen Sie Benutzer mit Administratorrechten für alle Benutzerdaten und Einstellungen mithilfe von STRG + Win + R auf dem Sperrbildschirm, damit das Gerät werden automatisch so neu konfiguriert und kann in Management basierendes löschen.|
|assignedAccessSingleModeUserName|String|Diese Richtlinie ermöglicht das Benutzerkonto, mit das gesperrt wird auf den einzelnen App Kiosk-Modus definieren.|
|assignedAccessSingleModeAppUserModelId|String|Diese Richtlinie ermöglicht so definieren Sie die Anwendung Benutzer Modell ID (AUMID), die gesperrt wird auf den einzelnen App Kiosk-Modus.|
|microsoftAccountSignInAssistantSettings|[signInAssistantOptions](../resources/intune-deviceconfig-signinassistantoptions.md)|Steuert den Microsoft-Konto Anmelde-Assistent (Wlidsvc) NT-Dienst. Mögliche Werte sind: `notConfigured` und `disabled`.|
|authenticationAllowSecondaryDevice|Boolean|Ermöglicht sekundäre Authentifizierung Geräten Windows entwickelt.|
|authenticationAllowFIDODevice|Boolean|Gibt an, ob Authentifizierung mithilfe von Fido kommt die Nachricht zulassen Gerät)https://fidoalliance.org/)|
|cryptographyAllowFipsAlgorithmPolicy|Boolean|Gibt an, ob zulassen oder verweigern die Richtlinie Federal Information Processing Standard (FIPS).|
|displayAppListWithGdiDPIScalingTurnedOn|Collection von Objekten des Typs „String“|Liste der Legacyanwendungen, die GDI DPI-Skalierung aktiviert haben.|
|displayAppListWithGdiDPIScalingTurnedOff|Collection von Objekten des Typs „String“|Liste der Legacyanwendungen, die GDI DPI-Skalierung deaktiviert haben.|
|enterpriseCloudPrintDiscoveryEndPoint|String|Der Endpunkt zur Ermittlung von Clouddruckern.|
|enterpriseCloudPrintOAuthAuthority|String|Authentifizierungsendpunkt zum Abrufen von OAuth-Token.|
|enterpriseCloudPrintOAuthClientIdentifier|String|GUID einer Clientanwendung, die berechtigt ist, OAuth-Token von der OAuth Authority.|
|enterpriseCloudPrintResourceIdentifier|String|OAuth-Ressourcen-URI für den Druckdienst, wie im Azure-Portal konfiguriert.|
|enterpriseCloudPrintDiscoveryMaxLimit|Int32|Maximale Anzahl von Druckern, die von einem Ermittlungsendpunkt abgefragt werden sollen. Dies ist nur eine Mobileinstellung. Gültige Werte: 1 bis 65535.|
|enterpriseCloudPrintMopriaDiscoveryResourceIdentifier|Zeichenfolge|OAuth-Ressourcen-URI für Druckerermittlungsdienst, wie im Azure-Portal konfiguriert.|
|messagingBlockSync|Boolean|Gibt an, ob Textnachricht blockieren, Sichern und Wiederherstellen und Messaging überall.|
|messagingBlockMMS|Boolean|Gibt an, ob Blockieren der MMS senden/empfangen Funktionalität auf dem Gerät.|
|messagingBlockRichCommunicationServices|Boolean|Gibt an, ob blockieren die RCS senden/empfangen Funktionalität auf dem Gerät.|
|printerNames|Collection von Objekten des Typs „String“|Drucker basierend auf ihren Namen (Hostnamen Netzwerk) automatisch bereitgestellt.|
|printerDefaultName|String|Name (Hostname Netzwerk) eines installierten Druckers.|
|printerBlockAddition|Boolean|Verhindern, dass Benutzerinstallation von zusätzlichen Druckern von Druckern Einstellungen.|
|searchBlockDiacritics|Boolean|Gibt an, ob die Suche diakritische Zeichen verwenden kann.|
|searchDisableAutoLanguageDetection|Boolean|Gibt an, ob die automatische Spracherkennung bei der Indizierung von Inhalten und Eigenschaften verwendet werden soll.|
|searchDisableIndexingEncryptedItems|Boolean|Gibt an, ob die Indizierung WIP-geschützter Elemente blockiert werden soll, um zu verhindern, dass diese in Suchergebnissen für Cortana oder Explorer angezeigt werden.|
|searchEnableRemoteQueries|Boolean|Gibt an, ob Remoteabfragen des Indexes dieses Computers blockiert werden sollen.|
|searchDisableUseLocation|Boolean|Gibt an, ob die Suche Standortinformationen nutzen kann.|
|searchDisableLocation|Boolean|Gibt an, ob die Suche Standortinformationen nutzen kann.|
|searchDisableIndexerBackoff|Boolean|Gibt an, ob die Sicherungsfunktion der Suchindizierung deaktiviert werden soll.|
|searchDisableIndexingRemovableDrive|Boolean|Gibt an, ob zugelassen werden soll, dass Benutzer Speicherorte auf Wechseldatenträgern hinzufügen, die indiziert werden sollen.|
|searchEnableAutomaticIndexSizeManangement|Boolean|Gibt die Mindestmenge an Festplattenspeicherplatz auf demselben Laufwerk wie der Indexspeicherort an, bevor die Indizierung beendet wird.|
|searchBlockWebResults|Boolean|Gibt an, ob die Websuche zu blockieren.|
|securityBlockAzureADJoinedDevicesAutoEncryption|Boolean|Gibt an, ob automatische geräteverschlüsselung während OOBE zulassen, wenn das Gerät Azure AD verbunden (nur Desktop) ist.|
|diagnosticsDataSubmissionMode|[diagnosticDataSubmissionMode](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|Ruft einen Wert ab, der es dem Gerät ermöglicht, Diagnose- und Nutzungstelemetriedaten zu senden, oder ruft diesen ab (z. B. Watson). Mögliche Werte: `userDefined`, `none`, `basic`, `enhanced`, `full`.|
|oneDriveDisableFileSync|Boolean|Ruft einen Wert ab, der es IT-Administratoren ermöglicht, zu verhindern, dass Apps und Features mit Dateien auf OneDrive arbeiten.|
|systemTelemetryProxyServer|Zeichenfolge|Ruft ab, oder legt diesen fest, den vollqualifizierten Domänennamen (FQDN) oder die IP-Adresse eines Proxyservers Benutzererlebnis verbunden und Telemetrie Anforderungen weiterleiten.|
|inkWorkspaceAccess|[inkAccessSetting](../resources/intune-deviceconfig-inkaccesssetting.md)|Steuert den Zugriff auf den Arbeitsbereich Freihand vom Desktop und aus dem Sperrbildschirm einer. Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.|
|inkWorkspaceAccessState|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Steuert den Zugriff auf den Arbeitsbereich Freihand vom Desktop und aus dem Sperrbildschirm einer. Mögliche Werte sind: `notConfigured`, `blocked` und `allowed`.|
|inkWorkspaceBlockSuggestedApps|Boolean|Gibt an, ob im Arbeitsbereich Freihand empfohlene app Vorschläge anzeigen.|
|smartScreenEnableAppInstallControl|Boolean|Ermöglicht IT-Administratoren, zu steuern, ob Benutzer Apps von anderen Orten als dem Store installieren können.|
|personalizationDesktopImageUrl|Zeichenfolge|Eine http- oder https-URL zu einem JPG-, JPEG- oder PNP-Bild, das heruntergeladen und als Desktopbild verwendet werden muss, oder eine Datei-URL zu einem lokalen Bild in dem Dateisystem, das als Desktopbild verwendet werden muss.|
|personalizationLockScreenImageUrl|Zeichenfolge|Eine http- oder https-URL zu einem JPG-, JPEG- oder PNP-Bild, das heruntergeladen und als Sperrbildschirmbild verwendet werden muss, oder eine Datei-URL zu einem lokalen Bild in dem Dateisystem, das als Sperrbildschirmbild verwendet werden muss.|
|bluetoothAllowedServices|Zeichenfolgenauflistung|Gibt eine Liste zulässiger Bluetooth-Dienste und -Profile in Zeichenfolgen im Hexadezimalformat an.|
|bluetoothBlockAdvertising|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer Bluetooth-Werbung verwendet.|
|bluetoothBlockDiscoverableMode|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer den sichtbaren Bluetoothmodus verwendet.|
|bluetoothBlockPrePairing|Boolean|Gibt an, ob bestimmte gebündelte Bluetooth-Peripheriegeräte automatisch mit dem Hostgerät gekoppelt werden.|
|edgeBlockAutofill|Boolean|Gibt an, ob AutoAusfüllen blockiert werden soll.|
|edgeBlocked|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer den Edge-Browser verwendet.|
|edgeCookiePolicy|[edgeCookiePolicy](../resources/intune-deviceconfig-edgecookiepolicy.md)|Gibt an, welche Cookies im Edge-Browsers blockiert werden sollen. Mögliche Werte: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.|
|edgeBlockDeveloperTools|Boolean|Gibt an, ob Entwicklertools im Edge-Browser blockiert werden sollen.|
|edgeBlockSendingDoNotTrackHeader|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer die Kopfzeile „Do Not Track“ (nicht verfolgen) sendet.|
|edgeBlockExtensions|Boolean|Gibt an, ob Erweiterungen im Edge-Browser blockiert werden sollen.|
|edgeBlockInPrivateBrowsing|Boolean|Gibt an, ob InPrivate-Browsen in Firmennetzwerken im Edge-Browser blockiert werden soll.|
|edgeBlockJavaScript|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer JavaScript verwendet.|
|edgeBlockPasswordManager|Boolean|Gibt an, ob der Kennwort-Manager blockiert werden soll.|
|edgeBlockAddressBarDropdown|Boolean|Blockiert die Dropdownfunktionalität der Adressleiste in Microsoft Edge. Deaktivieren Sie diese Einstellung, um Netzwerkverbindungen zu Microsoft-Diensten zu minimieren.|
|edgeBlockCompatibilityList|Boolescher Wert|Blockiert die Microsoft-Kompatibilitätsliste in Microsoft Edge. Diese Liste von Microsoft hilft Edge beim korrekten Anzeigen von Websites mit bekannten Kompatibilitätsproblemen.|
|edgeClearBrowsingDataOnExit|Boolean|Löscht Browserdaten beim Beenden von Microsoft Edge.|
|edgeAllowStartPagesModification|Boolean|Lässt zu, dass Benutzer Startseiten in Edge ändern. Verwenden Sie „EdgeHomepageUrls“, um Startseiten anzugeben, die dem Benutzer standardmäßig angezeigt werden, wenn er Edge öffnet.|
|edgeDisableFirstRunPage|Boolean|Blockiert die Microsoft-Webseite, die bei der ersten Verwendung von Microsoft Edge geöffnet wird. Mithilfe dieser Richtlinie können Unternehmen diese Seite blockieren, z. B. in Umgebungen mit Nullemissionskonfiguration.|
|edgeBlockLiveTileDataCollection|Boolescher Wert|Hiermit wird die Erfassung von Informationen durch Microsoft für die Erstellung von Livekacheln blockiert, wenn Benutzer über Microsoft Edge eine Website an das Startmenü anheften.|
|edgeSyncFavoritesWithInternetExplorer|Boolescher Wert|Hiermit wird die Synchronisierung von Favoriten zwischen Internet Explorer und Microsoft Edge aktiviert. Hinzufügungen, Löschungen, Änderungen und Reihenfolgenänderungen bei Favoriten werden zwischen Browsern beibehalten.|
|edgeFavoritesListLocation|Zeichenfolge|Der Speicherort der Favoritenliste bereitstellen. Dies kann eine lokale Datei, ein lokales Netzwerk oder ein HTTP-Speicherort sein.|
|edgeBlockEditFavorites|Boolean|Gibt an, ob die Benutzer Datensätze ändert Favoriten blockieren.|
|cellularBlockDataWhenRoaming|Boolean|Gibt an, ob verhindert wird, dass der Benutzer beim Roaming Daten über Mobilfunk verwendet.|
|cellularBlockVpn|Boolean|Gibt an, ob verhindert wird, dass der Benutzer beim Roaming VPN über Mobilfunk verwendet.|
|cellularBlockVpnWhenRoaming|Boolean|Gibt an, ob verhindert wird, dass der Benutzer beim Roaming über Mobilfunk VPN verwendet.|
|cellularData|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Ob Sie den Kanal Mobilfunk-Daten auf dem Gerät zulassen. Wenn nicht konfiguriert, der Channel Mobilfunk-Daten ist zulässig, der Benutzer kann aktivieren oder deaktivieren. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|defenderBlockEndUserAccess|Boolean|Gibt ab, ob der Endbenutzerzugriff auf Defender blockiert wird.|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Anzahl von Tagen, bevor Schadsoftware in Quarantäne gelöscht werden. Gültige Werte: 0 bis 90.|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|Ruft Defender-Aktionen für erkannte Schadsoftware pro Bedrohungsstufe an. oder legt diese fest.|
|defenderSystemScanSchedule|[weeklySchedule](../resources/intune-deviceconfig-weeklyschedule.md)|Wochentag für die Systemüberprüfung. Mögliche Werte: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|defenderFilesAndFoldersToExclude|Zeichenfolgenauflistung|Dateien und Ordner, die von Überprüfungen und Echtzeitschutz ausgenommen werden sollen.|
|defenderFileExtensionsToExclude|Zeichenfolgenauflistung|Dateierweiterungen, die von Überprüfungen und Echtzeitschutz ausgenommen werden sollen.|
|defenderScanMaxCpu|Int32|Prozentsatz der maximalen CPU-Auslastung während der Überprüfung. Gültige Werte: 0 bis 100.|
|defenderMonitorFileActivity|[defenderMonitorFileActivity](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|Wert für die Überwachung der Dateiaktivität. Mögliche Werte: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|defenderPotentiallyUnwantedAppAction|[defenderPotentiallyUnwantedAppAction](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|Ruft ab oder legt diesen fest Defender Aktion, die auf potenziell unerwünschte Anwendung (PUA), die Software mit Verhaltensweisen der Ad-Einfügung, Software Bündeln von, permanente erneute Zahlung oder Abonnement usw. enthält. Defender Benachrichtigungsbenutzer beim PUA heruntergeladen wird oder versucht, sich selbst zu installieren. In Windows-10 hinzugefügt für Desktop. Mögliche Werte sind: `deviceDefault`, `block` und `audit`.|
|defenderPotentiallyUnwantedAppActionSetting|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Ruft ab oder legt diesen fest Defender Aktion, die auf potenziell unerwünschte Anwendung (PUA), die Software mit Verhaltensweisen der Ad-Einfügung, Software Bündeln von, permanente erneute Zahlung oder Abonnement usw. enthält. Defender Benachrichtigungsbenutzer beim PUA heruntergeladen wird oder versucht, sich selbst zu installieren. In Windows-10 hinzugefügt für Desktop. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderProcessesToExclude|Zeichenfolgenauflistung|Prozesse, die von Überprüfungen und Echtzeitschutz ausgenommen werden sollen.|
|defenderPromptForSampleSubmission|[defenderPromptForSampleSubmission](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|Die Konfiguration zur Aufforderung des Benutzers, ein Beispiel zu übermitteln. Mögliche Werte: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.|
|defenderRequireBehaviorMonitoring|Boolean|Gibt an, ob eine Verhaltensüberwachung erforderlich ist.|
|defenderRequireCloudProtection|Boolean|Gibt an, ob Cloudschutz erforderlich ist.|
|defenderRequireNetworkInspectionSystem|Boolean|Gibt an, ob ein Netzwerkinspektionssystem erforderlich ist.|
|defenderRequireRealTimeMonitoring|Boolean|Gibt an, ob eine Echtzeitüberwachung erforderlich ist.|
|defenderScanArchiveFiles|Boolescher Wert|Gibt an, ob Archivdateien gescannt werden sollen.|
|defenderScanDownloads|Boolescher Wert|Gibt an, ob Downloads gescannt werden sollen.|
|defenderScanNetworkFiles|Boolean|Gibt an, ob in einem Netzwerkordner geöffnete Dateien gescannt werden sollen.|
|defenderScanIncomingMail|Boolean|Gibt an, ob eingehende E-Mail-Nachrichten gescannt werden sollen.|
|defenderScanMappedNetworkDrivesDuringFullScan|Boolescher Wert|Gibt an, ob zugeordnete Netzwerklaufwerke bei der vollständigen Überprüfung gescannt werden sollen.|
|defenderScanRemovableDrivesDuringFullScan|Boolescher Wert|Gibt an, ob Wechseldatenträger bei der vollständigen Überprüfung gescannt werden sollen.|
|defenderScanScriptsLoadedInInternetExplorer|Boolescher Wert|Gibt an, ob Skripts, die in Internet Explorer geladen sind, gescannt werden sollen.|
|defenderSignatureUpdateIntervalInHours|Int32|Das Aktualisierungsintervall der Signatur in Stunden. Geben Sie 0, wenn keine Überprüfung ausgeführt werden soll. Gültige Werte: 0 bis 24.|
|defenderScanType|[defenderScanType](../resources/intune-deviceconfig-defenderscantype.md)|Der Überprüfungstyp des Defender-Systems. Mögliche Werte: `userDefined`, `disabled`, `quick`, `full`.|
|defenderScheduledScanTime|TimeOfDay|Die Defender-Uhrzeit für die Systemüberprüfung.|
|defenderScheduledQuickScanTime|TimeOfDay|Die Zeit, zu der eine tägliche Schnellüberprüfung durchgeführt werden soll.|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|Gibt die Ebene für Schutz in der Cloud an. Mögliche Werte: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|defenderCloudExtendedTimeout|Int32|Timeout-Erweiterung für die Datei scannen, indem Sie die Cloud. Gültige Werte: 0 bis 50.|
|defenderCloudExtendedTimeoutInSeconds|Int32|Timeout-Erweiterung für die Datei scannen, indem Sie die Cloud. Gültige Werte: 0 bis 50.|
|defenderBlockOnAccessProtection|Boolescher Wert|Zugelassen oder verweigert Windows Defender für den Zugriffsschutz-Funktionalität.|
|defenderScheduleScanDay|[defenderScheduleScanDay](../resources/intune-deviceconfig-defenderschedulescanday.md)|Wählt den Tag, den die Überprüfung Windows Defender ausgeführt werden soll. Mögliche Werte: `everyday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`, `noScheduledScan`.|
|defenderSubmitSamplesConsentType|[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|Überprüft, ob der Benutzer stimmen Ebene in Windows Defender zum Senden von Daten. Mögliche Werte: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.|
|lockScreenAllowTimeoutConfiguration|Boolescher Wert|Gibt an, ob eine vom Benutzer konfigurierbare Einstellung zum Steuern des Bildschirmtimeouts auf dem Sperrbildschirm von Windows 10 Mobile-Geräten angezeigt werden soll. Wenn diese Richtlinie auf „Zulassen“ festgelegt ist, wird der von „lockScreenTimeoutInSeconds“ Wert ignoriert.|
|lockScreenBlockActionCenterNotifications|Boolescher Wert|Gibt an, ob Benachrichtigungen des Info-Centers über den Sperrbildschirm blockiert werden sollen.|
|lockScreenBlockCortana|Boolescher Wert|Gibt an, ob der Benutzer über die Spracherkennung mit Cortana interagieren kann, solange das System gesperrt ist.|
|lockScreenBlockToastNotifications|Boolescher Wert|Gibt an, ob Popupbenachrichtigungen über dem Sperrbildschirm des Geräts zulässig sind.|
|lockScreenTimeoutInSeconds|Int32|Legt die Dauer (in Sekunden) vom Sperren des Bildschirms bis zum Abschalten des Bildschirms für Windows 10 Mobile-Geräte fest. Unterstützte Werte: 11 bis 1800. Gültige Werte: 11 bis 1800.|
|passwordBlockSimple|Boolescher Wert|Geben Sie an, ob PINs oder Kennwörter wie „1111“ oder „1234“ zulässig sind. Für Windows 10-Desktops wird dadurch auch die Verwendung von Bildkennwörtern gesteuert.|
|passwordExpirationDays|Int32|Zeitraum in Tagen bis zum Ablaufen des Kennworts Gültige Werte: 0 bis 730.|
|passwordMinimumLength|Int32|Mindestlänge des Kennworts Gültige Werte: 4 bis 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt|
|passwordMinimumCharacterSetCount|Int32|Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen|
|passwordPreviousPasswordBlockCount|Int32|Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss. Gültige Werte: 0 bis 50.|
|passwordRequired|Boolescher Wert|Gibt an, ob der Benutzer ein Kennwort benötigt.|
|passwordRequireWhenResumeFromIdleState|Boolescher Wert|Gibt an, ob zum Fortsetzen aus einem Leerlaufstatus ein Kennwort erforderlich ist.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Die Anzahl von fehlgeschlagenen Anmeldeversuchen, bevor eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird. Gültige Werte: 0 bis 999.|
|passwordMinimumAgeInDays|Int32|Diese Einstellung bestimmt den Zeitraum (in Tagen), der ein Kennwort sein muss verwendet werden, bevor der Benutzer geändert werden kann. Gültige Werte 0 zu 998|
|privacyAdvertisingId|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Aktiviert oder deaktiviert die Verwendung einer Werbe-ID. Dies wurde in Windows 10, Version 1607, hinzugefügt. Mögliche Werte: `notConfigured`, `blocked`, `allowed`.|
|privacyAutoAcceptPairingAndConsentPrompts|Boolescher Wert|Gibt an, ob beim Starten von Apps das automatische Akzeptieren der Dialogfelder für die Benutzerzustimmung zur Kopplung und zum Datenschutz zulässig ist.|
|privacyBlockInputPersonalization|Boolescher Wert|Gibt an, ob die Nutzung cloudbasierter Sprachdienste für Cortana, Diktat oder Store-Apps blockiert wird.|
|privacyBlockPublishUserActivities|Boolescher Wert|Die freigegebene Erfahrungen/Ermittlung der zuletzt verwendeten Ressourcen im Aufgabenbereich wechseln usw. blockiert.|
|privacyBlockActivityFeed|Boolescher Wert|Die Verwendung von Cloud-basierten Sprachdienste für Cortana, Dictation oder Store Applikationen blockiert.|
|startBlockUnpinningAppsFromTaskbar|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Apps aus der Taskleiste loslöst.|
|startMenuAppListVisibility|[windowsStartMenuAppListVisibilityType](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|Durch Festlegen dieses Werts wird die App-Liste reduziert oder vollständig entfernt bzw. die entsprechende Option in der App „Einstellungen“ deaktiviert. Mögliche Werte: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.|
|startMenuHideChangeAccountSettings|Boolescher Wert|Durch Aktivieren dieser Richtlinie wird die Einstellung zur Kontoänderung in der Benutzerkachel im Startmenü ausgeblendet.|
|startMenuHideFrequentlyUsedApps|Boolescher Wert|Durch Aktivieren dieser Richtlinie werden die meistverwendeten Apps aus dem Startmenü ausgeblendet, und die entsprechende Option wird in der App „Einstellungen“ deaktiviert.|
|startMenuHideHibernate|Boolescher Wert|Durch Aktivieren dieser Richtlinie wird die Option „Ruhezustand“ nicht mehr im Netzschaltersymbol im Startmenü angezeigt.|
|startMenuHideLock|Boolescher Wert|Durch Aktivieren dieser Richtlinie wird die Sperre aus der Benutzerkachel im Startmenü ausgeblendet.|
|startMenuHidePowerButton|Boolescher Wert|Durch Aktivieren dieser Richtlinie wird das Netzschaltersymbol aus dem Startmenü ausgeblendet.|
|startMenuHideRecentJumpLists|Boolescher Wert|Durch Aktivieren dieser Richtlinie werden die letzten Sprunglisten aus dem Startmenü/der Taskleiste ausgeblendet, und die entsprechende Option wird in der App „Einstellungen“ deaktiviert.|
|startMenuHideRecentlyAddedApps|Boolescher Wert|Durch Aktivieren dieser Richtlinie werden zuletzt hinzugefügte Apps aus dem Startmenü ausgeblendet, und die entsprechende Option wird in der App „Einstellungen“ deaktiviert.|
|startMenuHideRestartOptions|Boolescher Wert|Durch Aktivieren dieser Richtlinie werden die Optionen „Neu starten“und „Aktualisieren und neu starten“ nicht mehr im Netzschaltersymbol im Startmenü angezeigt.|
|startMenuHideShutDown|Boolescher Wert|Durch Aktivieren dieser Richtlinie wird „Herunterfahren/Aktualisieren“ und „Herunterfahren“ aus dem Netzschaltersymbol im Startmenü ausgeblendet.|
|startMenuHideSignOut|Boolescher Wert|Durch Aktivieren dieser Richtlinie wird „Abmelden“ aus der Benutzerkachel im Startmenü ausgeblendet.|
|startMenuHideSleep|Boolescher Wert|Durch Aktivieren dieser Richtlinie wird „Standbymodus“ aus dem Netzschaltersymbol im Startmenü ausgeblendet|
|startMenuHideSwitchAccount|Boolescher Wert|Durch Aktivieren dieser Richtlinie wird „Konto wechseln“ aus der Benutzerkachel im Startmenü ausgeblendet.|
|startMenuHideUserTile|Boolescher Wert|Durch Aktivieren dieser Richtlinie wird die Benutzerkachel aus dem Startmenü ausgeblendet.|
|startMenuLayoutEdgeAssetsXml|Binär|Diese Richtlinieneinstellung ermöglicht Ihnen das Importieren von Microsoft Edge-Assets zur Verwendung mit der Richtlinie „startMenuLayoutXml“. Das Startlayout kann eine sekundäre Kachel aus der Edge-App enthalten, die nach der lokalen Edge-Assetdatei sucht. Das lokale Edge-Asset ist in diesem Fall nicht vorhanden und führt dazu, dass die sekundäre Edge-Kachel leer angezeigt wird.  Diese Richtlinie wird nur angewendet, wenn die Richtlinie „startMenuLayoutXml“ geändert wird. Der Wert sollte ein UTF-8-Base64-codiertes Bytearray sein.|
|startMenuLayoutXml|Binär|Ermöglicht Administratoren das Außerkraftsetzen des Startmenü-Standardlayouts und verhindert Änderungen durch den Benutzer. Das Layout wird durch Angabe einer XML-Datei geändert, die auf einem Layoutänderungsschema basiert. XML muss ein UTF8-codiertes Bytearrayformat aufweisen.|
|startMenuMode|[windowsStartMenuModeType](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|Ermöglicht Administratoren zu entscheiden, wie das Startmenü angezeigt wird. Mögliche Werte: `userDefined`, `fullScreen`, `nonFullScreen`.|
|startMenuPinnedFolderDocuments|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Dokumente“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderDownloads|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Downloads“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderFileExplorer|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung „FileExplorer“ im Startmenü Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderHomeGroup|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „ Heimnetzgruppe“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderMusic|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Musik“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderNetwork|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Netzwerk“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPersonalFolder|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem persönlichen Ordner im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPictures|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Bilder“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderSettings|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Einstellungen“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderVideos|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Videos“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|settingsBlockSettingsApp|Boolescher Wert|Gibt an, ob der Zugriff auf die App „Einstellungen“ blockiert werden soll.|
|settingsBlockSystemPage|Boolescher Wert|Gibt an, ob der Zugriff auf „System“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockDevicesPage|Boolescher Wert|Gibt an, ob der Zugriff auf „Geräte“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockNetworkInternetPage|Boolescher Wert|Gibt an, ob der Zugriff auf „Netzwerk und Internet“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockPersonalizationPage|Boolescher Wert|Gibt an, ob der Zugriff auf „Personalisierung“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockAccountsPage|Boolescher Wert|Gibt an, ob der Zugriff auf „Konten“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockTimeLanguagePage|Boolescher Wert|Gibt an, ob der Zugriff auf „Zeit und Sprache“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockEaseOfAccessPage|Boolescher Wert|Gibt an, ob der Zugriff auf „Erleichterte Bedienung“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockPrivacyPage|Boolescher Wert|Gibt an, ob der Zugriff auf „Datenschutz“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockUpdateSecurityPage|Boolescher Wert|Gibt an, ob der Zugriff auf „Update und Sicherheit“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockAppsPage|Boolescher Wert|Gibt an, ob der Zugriff auf „Apps“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockGamingPage|Boolescher Wert|Gibt an, ob der Zugriff auf „Gaming“ in der App „Einstellungen“ blockiert werden soll.|
|windowsSpotlightBlockConsumerSpecificFeatures|Boolescher Wert|Ermöglicht IT-Administratoren das Blockieren von Funktionen, die normalerweise nur für Endbenutzer bestimmt sind, beispielsweise Startvorschläge, Mitgliedschaftsbenachrichtigungen, App-Installation nach Anzeige der Windows-Willkommensseite und Kachelumleitungen.|
|windowsSpotlightBlocked|Boolescher Wert|Ermöglicht IT-Administratoren das Deaktivieren aller Features von Windows-Blickpunkt.|
|windowsSpotlightBlockOnActionCenter|Boolescher Wert|Blockiert Vorschläge von Microsoft, die nach jeder Neuinstallation des Betriebssytem, nach jedem Upgrade oder auf fortlaufender Basis angezeigt werden, um Benutzern Neuigkeiten oder Änderungen vorzustellen.|
|windowsSpotlightBlockTailoredExperiences|Boolescher Wert|Blockiert personalisierte Inhalte in Windows-Blickpunkt basierend auf dem Gerät, das der Benutzer verwendet.|
|windowsSpotlightBlockThirdPartyNotifications|Boolescher Wert|Blockiert Inhalte von Drittanbietern, die über Windows-Blickpunkt übermittelt werden.|
|windowsSpotlightBlockWelcomeExperience|Boolescher Wert|Windows-Begrüßungsseite zur Vorstellung neuer oder aktualisierter Features blockieren|
|windowsSpotlightBlockWindowsTips|Boolescher Wert|Ermöglicht IT-Administratoren das Deaktivieren des Popups von Windows-Tipps.|
|windowsSpotlightConfigureOnLockScreen|[windowsSpotlightEnablementSettings](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|Gibt den Typ des Spotlight. Mögliche Werte sind: `notConfigured`, `disabled` und `enabled`.|
|networkProxyApplySettingsDeviceWide|Boolescher Wert|Wenn dieser Wert festgelegt ist, werden Proxyeinstellungen auf alle Prozesse und Konten in dem Gerät angewendet. Andernfalls wird er auf das Benutzerkonto angewendet, das bei MDM registriert ist.|
|networkProxyDisableAutoDetect|Boolescher Wert|Deaktiviert die automatische Erkennung von Einstellungen. Wenn diese Option aktiviert ist, versucht das System, den Pfad zu einem PAC-Skript (automatische Proxykonfiguration) zu suchen.|
|networkProxyAutomaticConfigurationUrl|Zeichenfolge|Adresse zu dem PAC-Skript, das Sie verwenden möchten.|
|networkProxyServer|[windows10NetworkProxyServer](../resources/intune-deviceconfig-windows10networkproxyserver.md)|Gibt manuelle Proxyservereinstellungen an.|
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
|safeSearchFilter|[safeSearchFilterType](../resources/intune-deviceconfig-safesearchfiltertype.md)|Gibt an, welche Filterebene von SafeSearch erforderlich ist. Mögliche Werte: `userDefined`, `strict`, `moderate`.|
|edgeBlockPopups|Boolescher Wert|Gibt an, ob Popups blockiert werden sollen.|
|edgeBlockSearchSuggestions|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Suchvorschläge in der Adressleiste verwendet.|
|edgeBlockSendingIntranetTrafficToInternetExplorer|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Intranetverkehr aus Edge an Internet Explorer sendet.|
|edgeRequireSmartScreen|Boolescher Wert|Gibt an, ob der Benutzer aufgefordert werden soll, den Smartscreenfilter zu verwenden.|
|edgeEnterpriseModeSiteListLocation|Zeichenfolge|Gibt den Speicherort der Siteliste für den Unternehmensmodus an. Dies kann eine lokale Datei, ein lokales Netzwerk oder ein http-Speicherort sein.|
|edgeFirstRunUrl|Zeichenfolge|Die URL für erste Ausführung, wenn der Edge-Browser das erste Mal geöffnet wird.|
|edgeSearchEngine|[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)|Ermöglicht es IT-Administratoren, eine standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen. Benutzer können dies außer Kraft setzen und die standardmäßige Suchmaschine ändern, sofern die Richtlinie „AllowSearchEngineCustomization“ nicht festgelegt ist.|
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
|appsAllowTrustedAppsSideloading|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Gibt an, ob Apps aus AppX-Paketen, die mit einem vertrauenswürdigen Zertifikat signiert sind, quergeladen werden können. Mögliche Werte: `notConfigured`, `blocked`, `allowed`.|
|windowsStoreBlockAutoUpdate|Boolescher Wert|Gibt an, ob automatische Updates von Apps aus dem Windows Store blockiert werden sollen.|
|developerUnlockSetting|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Gibt an, ob die Entwicklersperre zulässig ist. Mögliche Werte: `notConfigured`, `blocked`, `allowed`.|
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
|appManagementMSIAllowUserControlOverInstall|Boolescher Wert|Diese Einstellung ermöglicht Benutzern Installationsoptionen zu ändern, die in der Regel nur für Systemadministratoren verfügbar sind.|
|appManagementMSIAlwaysInstallWithElevatedPrivileges|Boolescher Wert|Diese Einstellung veranlasst Windows Installer, mit erhöhten Berechtigungen verwenden, wenn es Anwendung auf dem System installiert.|
|dataProtectionBlockDirectMemoryAccess|Boolescher Wert|Mithilfe dieser richtlinieneinstellung können Sie direkter Speicherzugriff (DMA) blockieren für alle hot austauschbaren PCI downstream-Ports, bis ein Benutzer in Windows anmeldet.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Auflistung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Gerät Konfiguration Installationsstatus durch Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignedAccessMultiModeProfiles|[WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) -Auflistung|Dieser Richtlinie können Sie eine Liste der zugewiesenen Zugriffsrechten Profile für Multi-app-Modus definieren.|
|privacyAccessControls|[WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Auflistung|Gibt eine Liste von Anwendungen mit ihrer Zugriffsebenen Steuerelement über private Datenschutzkategorien und/oder die Standardzugriffsebenen pro Kategorie an.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10GeneralConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "String (timestamp)",
    "recurrence": "String",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "assignedAccessSingleModeUserName": "String",
  "assignedAccessSingleModeAppUserModelId": "String",
  "microsoftAccountSignInAssistantSettings": "String",
  "authenticationAllowSecondaryDevice": true,
  "authenticationAllowFIDODevice": true,
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "String"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "String"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "String",
  "enterpriseCloudPrintOAuthAuthority": "String",
  "enterpriseCloudPrintOAuthClientIdentifier": "String",
  "enterpriseCloudPrintResourceIdentifier": "String",
  "enterpriseCloudPrintDiscoveryMaxLimit": 1024,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "String",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "String"
  ],
  "printerDefaultName": "String",
  "printerBlockAddition": true,
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableUseLocation": true,
  "searchDisableLocation": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "searchBlockWebResults": true,
  "securityBlockAzureADJoinedDevicesAutoEncryption": true,
  "diagnosticsDataSubmissionMode": "String",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "String",
  "inkWorkspaceAccess": "String",
  "inkWorkspaceAccessState": "String",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "String",
  "personalizationLockScreenImageUrl": "String",
  "bluetoothAllowedServices": [
    "String"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "String",
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
  "edgeFavoritesListLocation": "String",
  "edgeBlockEditFavorites": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "String",
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 1024,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "String",
    "moderateSeverity": "String",
    "highSeverity": "String",
    "severeSeverity": "String"
  },
  "defenderSystemScanSchedule": "String",
  "defenderFilesAndFoldersToExclude": [
    "String"
  ],
  "defenderFileExtensionsToExclude": [
    "String"
  ],
  "defenderScanMaxCpu": 1024,
  "defenderMonitorFileActivity": "String",
  "defenderPotentiallyUnwantedAppAction": "String",
  "defenderPotentiallyUnwantedAppActionSetting": "String",
  "defenderProcessesToExclude": [
    "String"
  ],
  "defenderPromptForSampleSubmission": "String",
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
  "defenderSignatureUpdateIntervalInHours": 1024,
  "defenderScanType": "String",
  "defenderScheduledScanTime": "String (time of day)",
  "defenderScheduledQuickScanTime": "String (time of day)",
  "defenderCloudBlockLevel": "String",
  "defenderCloudExtendedTimeout": 1024,
  "defenderCloudExtendedTimeoutInSeconds": 1024,
  "defenderBlockOnAccessProtection": true,
  "defenderScheduleScanDay": "String",
  "defenderSubmitSamplesConsentType": "String",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 1024,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordMinimumAgeInDays": 1024,
  "privacyAdvertisingId": "String",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "String",
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
  "startMenuLayoutEdgeAssetsXml": "binary",
  "startMenuLayoutXml": "binary",
  "startMenuMode": "String",
  "startMenuPinnedFolderDocuments": "String",
  "startMenuPinnedFolderDownloads": "String",
  "startMenuPinnedFolderFileExplorer": "String",
  "startMenuPinnedFolderHomeGroup": "String",
  "startMenuPinnedFolderMusic": "String",
  "startMenuPinnedFolderNetwork": "String",
  "startMenuPinnedFolderPersonalFolder": "String",
  "startMenuPinnedFolderPictures": "String",
  "startMenuPinnedFolderSettings": "String",
  "startMenuPinnedFolderVideos": "String",
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
  "windowsSpotlightConfigureOnLockScreen": "String",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "String",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "String",
    "exceptions": [
      "String"
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
  "safeSearchFilter": "String",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "String",
  "edgeFirstRunUrl": "String",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "String"
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
  "wiFiScanInterval": 1024,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "String",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "String",
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
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true
}
```





