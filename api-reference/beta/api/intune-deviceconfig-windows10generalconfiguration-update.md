---
title: windows10GeneralConfiguration aktualisieren
description: Aktualisiert die Eigenschaften eines windows10GeneralConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae6479f0d4d422a29ddff741e1f8a2368f1a50ce
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572383"
---
# <a name="update-windows10generalconfiguration"></a>windows10GeneralConfiguration aktualisieren

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisiert die Eigenschaften eines [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)-Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).

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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie als Anforderungstext eine JSON-Darstellung des  [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)-Objekts an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie das [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)-Objekt erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolesch|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|taskManagerBlockEndTask|Boolesch|Geben Sie an, ob nicht-Administratoren Aufgaben mithilfe des Task-Managers beenden können.|
|windows10AppsForceUpdateSchedule|[windows10AppsForceUpdateSchedule](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|Windows 10 Erzwingen des Aktualisierungszeitplans für apps.|
|enableAutomaticRedeployment|Boolesch|Benutzern mit Administratorrechten das Löschen aller Benutzerdaten und-Einstellungen mithilfe von STRG + Win + R auf dem Bildschirm "Gerätesperre" geStatten, damit das Gerät automatisch neu konfiguriert und für die Verwaltung erneut registriert werden kann.|
|microsoftAccountSignInAssistantSettings|[signInAssistantOptions](../resources/intune-deviceconfig-signinassistantoptions.md)|Steuert den Microsoft-Konto-Anmelde-Assistenten (wlidsvc) NT-Dienst. Mögliche Werte sind: `notConfigured` und `disabled`.|
|authenticationAllowSecondaryDevice|Boolesch|Ermöglicht die Verwendung sekundärer Authentifizierungsgeräte mit Windows.|
|authenticationWebSignIn|[Aktivierung](../resources/intune-shared-enablement.md)|Gibt an, ob der webAnmelder-Anbieter aktiviert wird. Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.|
|authenticationPreferredAzureADTenantDomainName|Zeichenfolge|Gibt die bevorzugte Domäne unter den verfügbaren Domänen im Azure AD-Mandanten an.|
|cryptographyAllowFipsAlgorithmPolicy|Boolesch|Geben Sie an, ob die FIPS-Richtlinie (Federal Information Processing Standard) zugelassen oder verweigert werden soll.|
|displayAppListWithGdiDPIScalingTurnedOn|String collection|Liste der Legacyanwendungen, für die die GDI-DPI-Skalierung aktiviert ist.|
|displayAppListWithGdiDPIScalingTurnedOff|String collection|Liste der Legacyanwendungen, für die die GDI-DPI-Skalierung deaktiviert ist.|
|enterpriseCloudPrintDiscoveryEndPoint|Zeichenfolge|Der Endpunkt zur Ermittlung von Clouddruckern.|
|enterpriseCloudPrintOAuthAuthority|Zeichenfolge|Authentifizierungsendpunkt zum Abrufen von OAuth-Token.|
|enterpriseCloudPrintOAuthClientIdentifier|Zeichenfolge|GUID einer Clientanwendung, die berechtigt ist, OAuth-Token von der OAuth Authority.|
|enterpriseCloudPrintResourceIdentifier|Zeichenfolge|OAuth-Ressourcen-URI für den Druckdienst, wie im Azure-Portal konfiguriert.|
|enterpriseCloudPrintDiscoveryMaxLimit|Int32|Maximale Anzahl von Druckern, die von einem Ermittlungsendpunkt abgefragt werden sollen. Dies ist nur eine Mobileinstellung. Gültige Werte: 1 bis 65535.|
|enterpriseCloudPrintMopriaDiscoveryResourceIdentifier|String|OAuth-Ressourcen-URI für Druckerermittlungsdienst, wie im Azure-Portal konfiguriert.|
|experienceDoNotSyncBrowserSettings|[browserSyncSetting](../resources/intune-deviceconfig-browsersyncsetting.md)|Zulassen oder verhindern der Synchronisierung von Einstellungen des Microsoft-Edge-Browsers. Option für IT-Administratoren, um die Synchronisierung über Geräte hinweg zu verhindern, aber die Benutzer außer Kraft zu setzen. Mögliche Werte sind: `notConfigured`, `blockedWithUserOverride` und `blocked`.|
|messagingBlockSync|Boolesch|Gibt an, ob das Sichern und Wiederherstellen und Nachrichten von Textnachrichten überall blockiert werden soll.|
|messagingBlockMMS|Boolesch|Gibt an, ob die MMS-Sende-/Empfangsfunktionalität auf dem Gerät blockiert werden soll.|
|messagingBlockRichCommunicationServices|Boolesch|Gibt an, ob die RCS-Sende-und-Empfangsfunktionalität auf dem Gerät blockiert werden soll.|
|Eigenschaften printernames|String collection|Automatische Bereitstellung von Druckern basierend auf Ihren Namen (Netzwerk Host Namen)|
|printerDefaultName|Zeichenfolge|Name (Netzwerk Hostname) eines installierten Druckers.|
|printerBlockAddition|Boolesch|Verhindern der Benutzerinstallation zusätzlicher Drucker aus den Druckereinstellungen.|
|searchBlockDiacritics|Boolesch|Gibt an, ob die Suche diakritische Zeichen verwenden kann.|
|searchDisableAutoLanguageDetection|Boolesch|Gibt an, ob die automatische Spracherkennung bei der Indizierung von Inhalten und Eigenschaften verwendet werden soll.|
|searchDisableIndexingEncryptedItems|Boolesch|Gibt an, ob die Indizierung WIP-geschützter Elemente blockiert werden soll, um zu verhindern, dass diese in Suchergebnissen für Cortana oder Explorer angezeigt werden.|
|searchEnableRemoteQueries|Boolesch|Gibt an, ob Remoteabfragen des Indexes dieses Computers blockiert werden sollen.|
|searchDisableUseLocation|Boolesch|Gibt an, ob die Suche Standortinformationen verwenden kann.|
|searchDisableLocation|Boolesch|Gibt an, ob die Suche Standortinformationen verwenden kann.|
|searchDisableIndexerBackoff|Boolesch|Gibt an, ob die Sicherungsfunktion der Suchindizierung deaktiviert werden soll.|
|searchDisableIndexingRemovableDrive|Boolesch|Gibt an, ob zugelassen werden soll, dass Benutzer Speicherorte auf Wechseldatenträgern hinzufügen, die indiziert werden sollen.|
|searchEnableAutomaticIndexSizeManangement|Boolesch|Gibt die Mindestmenge an Festplattenspeicherplatz auf demselben Laufwerk wie der Indexspeicherort an, bevor die Indizierung beendet wird.|
|searchBlockWebResults|Boolesch|Gibt an, ob die Websuche blockiert werden soll.|
|securityBlockAzureADJoinedDevicesAutoEncryption|Boolesch|Geben Sie an, ob die automatische Geräteverschlüsselung während OOBE zugelassen werden soll, wenn das Gerät mit Azure AD verbunden ist (nur Desktop).|
|diagnosticsDataSubmissionMode|[diagnosticDataSubmissionMode](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|Ruft einen Wert ab, der es dem Gerät ermöglicht, Diagnose- und Nutzungstelemetriedaten zu senden, oder ruft diesen ab (z. B. Watson). Mögliche Werte: `userDefined`, `none`, `basic`, `enhanced`, `full`.|
|oneDriveDisableFileSync|Boolesch|Ruft einen Wert ab, der es IT-Administratoren ermöglicht, zu verhindern, dass Apps und Features mit Dateien auf OneDrive arbeiten.|
|systemTelemetryProxyServer|Zeichenfolge|Ruft den vollqualifizierten Domänennamen (FQDN) oder die IP-Adresse eines Proxyservers ab, um verbundene Benutzererlebnisse und teleMetrie-Anforderungen weiterzuleiten, oder legt diesen fest.|
|edgeTelemetryForMicrosoft365Analytics|[edgeTelemetryMode](../resources/intune-deviceconfig-edgetelemetrymode.md)|Gibt an, welcher Typ von Telemetrie-Daten (keine, Intranet, Internet, beides) an Microsoft 365 Analytics gesendet wird. Mögliche Werte sind: `notConfigured`, `intranet`, `internet` und `intranetAndInternet`.|
|inkWorkspaceAccess|[inkAccessSetting](../resources/intune-deviceconfig-inkaccesssetting.md)|Steuert den Benutzer Zugriff auf den frei Hand Arbeitsbereich vom Desktop und über den Sperrbildschirm. Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.|
|inkWorkspaceAccessState|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Steuert den Benutzer Zugriff auf den frei Hand Arbeitsbereich vom Desktop und über den Sperrbildschirm. Mögliche Werte sind: `notConfigured`, `blocked` und `allowed`.|
|inkWorkspaceBlockSuggestedApps|Boolesch|Geben Sie an, ob Empfohlene App-Vorschläge im frei Hand Arbeitsbereich angezeigt werden sollen.|
|smartScreenEnableAppInstallControl|Boolesch|Ermöglicht IT-Administratoren, zu steuern, ob Benutzer Apps von anderen Orten als dem Store installieren können.|
|personalizationDesktopImageUrl|Zeichenfolge|Eine http- oder https-URL zu einem JPG-, JPEG- oder PNP-Bild, das heruntergeladen und als Desktopbild verwendet werden muss, oder eine Datei-URL zu einem lokalen Bild in dem Dateisystem, das als Desktopbild verwendet werden muss.|
|personalizationLockScreenImageUrl|String|Eine http- oder https-URL zu einem JPG-, JPEG- oder PNP-Bild, das heruntergeladen und als Sperrbildschirmbild verwendet werden muss, oder eine Datei-URL zu einem lokalen Bild in dem Dateisystem, das als Sperrbildschirmbild verwendet werden muss.|
|bluetoothAllowedServices|String collection|Gibt eine Liste zulässiger Bluetooth-Dienste und -Profile in Zeichenfolgen im Hexadezimalformat an.|
|bluetoothBlockAdvertising|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer Bluetooth-Werbung verwendet.|
|bluetoothBlockPromptedProximalConnections|Boolesch|Gibt an, ob die Benutzer mit SWIFT-Paaren und anderen Näherungs basierten Szenarien blockiert werden sollen.|
|bluetoothBlockDiscoverableMode|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer den sichtbaren Bluetoothmodus verwendet.|
|bluetoothBlockPrePairing|Boolean|Gibt an, ob bestimmte gebündelte Bluetooth-Peripheriegeräte automatisch mit dem Hostgerät gekoppelt werden.|
|edgeBlockAutofill|Boolesch|Gibt an, ob AutoAusfüllen blockiert werden soll.|
|edgeBlocked|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer den Edge-Browser verwendet.|
|edgeCookiePolicy|[edgeCookiePolicy](../resources/intune-deviceconfig-edgecookiepolicy.md)|Gibt an, welche Cookies im Edge-Browsers blockiert werden sollen. Mögliche Werte: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.|
|edgeBlockDeveloperTools|Boolesch|Gibt an, ob Entwicklertools im Edge-Browser blockiert werden sollen.|
|edgeBlockSendingDoNotTrackHeader|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer die Kopfzeile „Do Not Track“ (nicht verfolgen) sendet.|
|edgeBlockExtensions|Boolesch|Gibt an, ob Erweiterungen im Edge-Browser blockiert werden sollen.|
|edgeBlockInPrivateBrowsing|Boolesch|Gibt an, ob InPrivate-Browsen in Firmennetzwerken im Edge-Browser blockiert werden soll.|
|edgeBlockJavaScript|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer JavaScript verwendet.|
|edgeBlockPasswordManager|Boolesch|Gibt an, ob der Kennwort-Manager blockiert werden soll.|
|edgeBlockAddressBarDropdown|Boolesch|Blockiert die Dropdownfunktionalität der Adressleiste in Microsoft Edge. Deaktivieren Sie diese Einstellung, um Netzwerkverbindungen zu Microsoft-Diensten zu minimieren.|
|edgeBlockCompatibilityList|Boolesch|Blockiert die Microsoft-Kompatibilitätsliste in Microsoft Edge. Diese Liste von Microsoft hilft Edge beim korrekten Anzeigen von Websites mit bekannten Kompatibilitätsproblemen.|
|edgeClearBrowsingDataOnExit|Boolesch|Löscht Browserdaten beim Beenden von Microsoft Edge.|
|edgeAllowStartPagesModification|Boolesch|Lässt zu, dass Benutzer Startseiten in Edge ändern. Verwenden Sie „EdgeHomepageUrls“, um Startseiten anzugeben, die dem Benutzer standardmäßig angezeigt werden, wenn er Edge öffnet.|
|edgeDisableFirstRunPage|Boolesch|Blockiert die Microsoft-Webseite, die bei der ersten Verwendung von Microsoft Edge geöffnet wird. Mithilfe dieser Richtlinie können Unternehmen diese Seite blockieren, z. B. in Umgebungen mit Nullemissionskonfiguration.|
|edgeBlockLiveTileDataCollection|Boolescher Wert|Hiermit wird die Erfassung von Informationen durch Microsoft für die Erstellung von Livekacheln blockiert, wenn Benutzer über Microsoft Edge eine Website an das Startmenü anheften.|
|edgeSyncFavoritesWithInternetExplorer|Boolean|Hiermit wird die Synchronisierung von Favoriten zwischen Internet Explorer und Microsoft Edge aktiviert. Hinzufügungen, Löschungen, Änderungen und Reihenfolgenänderungen bei Favoriten werden zwischen Browsern beibehalten.|
|edgeFavoritesListLocation|Zeichenfolge|Der Speicherort der Favoritenliste, die festgestellt werden soll. Dies kann eine lokale Datei, ein lokales Netzwerk oder ein http-Speicherort sein.|
|edgeBlockEditFavorites|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer Änderungen an den Favoriten vornimmt.|
|edgeNewTabPageURL|Zeichenfolge|Geben Sie die Seite an, die beim Erstellen neuer Registerkarten geöffnet wird.|
|edgeHomeButtonConfiguration|[edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)|Bewirkt, dass die Schaltfläche "Start" entweder ausgeblendet wird, die Standard Startseite laden, eine neue Registerkarte Laden oder eine benutzerdefinierte URL|
|edgeHomeButtonConfigurationEnabled|Boolesch|Aktivieren Sie die Schaltfläche Konfiguration der Startseite.|
|edgeOpensWith|[edgeOpenOptions](../resources/intune-deviceconfig-edgeopenoptions.md)|Geben Sie an, welche Art von Seiten am Anfang geöffnet sind. Mögliche Werte: `notConfigured`, `startPage`, `newTabPage`, `previousPages`, `specificPages`.|
|edgeBlockSideloadingExtensions|Boolesch|Gibt an, ob der Benutzer Erweiterungen querladen kann.|
|edgeRequiredExtensionPackageFamilyNames|String collection|Geben Sie die Liste der Paket Familiennamen von Browsererweiterungen an, die erforderlich sind und nicht vom Benutzer deaktiviert werden können.|
|edgeBlockPrinting|Boolesch|Konfigurieren von Edge zum Zulassen oder Blockieren des Druckens.|
|edgeFavoritesBarVisibility|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Dient zum Abrufen oder Festlegen eines Werts, der angibt, ob die Favoritenleiste so festgelegt werden soll, dass Sie auf einer Seite immer sichtbar oder ausgeblendet ist. Mögliche Werte sind: `notConfigured`, `hide` und `show`.|
|edgeBlockSavingHistory|Boolesch|Konfigurieren Sie Edge so, dass der Browserverlauf gespeichert oder der Browserverlauf nie gespeichert wird.|
|edgeBlockFullScreenMode|Boolesch|Zulassen oder verhindern, dass Edge in den Vollbildmodus wechselt.|
|edgeBlockWebContentOnNewTabPage|Boolesch|Konfigurieren Sie, um eine leere Seite in Edge anstelle der standardmäßigen neuen Registerkarte zu laden und zu verhindern, dass Benutzer Sie ändern.|
|edgeBlockTabPreloading|Boolesch|Konfigurieren Sie, ob Edge die neue Registerkarte beim Windows-Start vorlädt.|
|edgeBlockPrelaunch|Boolesch|Entscheiden Sie, ob Microsoft Edge beim Windows-Start vorgestartet wird.|
|edgeShowMessageWhenOpeningInternetExplorerSites|[internetExplorerMessageSetting](../resources/intune-deviceconfig-internetexplorermessagesetting.md)|Steuert die von Edge angezeigte Nachricht vor dem Wechsel zu Internet Explorer. Mögliche Werte sind: `notConfigured`, `disabled`, `enabled` und `keepGoing`.|
|edgePreventCertificateErrorOverride|Boolesch|Zulassen oder verhindern, dass Benutzerzertifikat Fehler überschreiben.|
|edgeKioskModeRestriction|[edgeKioskModeRestrictionType](../resources/intune-deviceconfig-edgekioskmoderestrictiontype.md)|Steuert, wie die Microsoft-Edgeeinstellungen basierend auf dem Konfigurations-Kiosk-Modus eingeschränkt werden. Mögliche Werte: `notConfigured`, `digitalSignage`, `normalMode`, `publicBrowsingSingleApp`, `publicBrowsingMultiApp`.|
|edgeKioskResetAfterIdleTimeInMinutes|Int32|Gibt die Zeit in Minuten der letzten Benutzeraktivität an, bevor Microsoft Edge Kiosk zurückgesetzt wird.  Gültige Werte sind 0-1440. Die möglichen Werte liegen in einem Bereich von 1 bis 998, der Standardwert ist 5. 0 gibt keine Zurücksetzung an. Gültige Werte 0 bis 1440|
|cellularBlockDataWhenRoaming|Boolesch|Gibt an, ob verhindert wird, dass der Benutzer beim Roaming Daten über Mobilfunk verwendet.|
|cellularBlockVpn|Boolesch|Gibt an, ob verhindert wird, dass der Benutzer beim Roaming VPN über Mobilfunk verwendet.|
|cellularBlockVpnWhenRoaming|Boolesch|Gibt an, ob verhindert wird, dass der Benutzer beim Roaming über Mobilfunk VPN verwendet.|
|cellularData|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob der Mobilfunkdaten Kanal auf dem Gerät zugelassen werden soll. Wenn dieser nicht konfiguriert ist, wird der zelluläre Datenkanal zugelassen, und der Benutzer kann ihn deaktivieren. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|defenderBlockEndUserAccess|Boolesch|Gibt ab, ob der Endbenutzerzugriff auf Defender blockiert wird.|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Anzahl von Tagen, bevor Schadsoftware in Quarantäne gelöscht werden. Gültige Werte: 0 bis 90.|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|Ruft Defender-Aktionen für erkannte Schadsoftware pro Bedrohungsstufe an. oder legt diese fest.|
|defenderSystemScanSchedule|[weeklySchedule](../resources/intune-deviceconfig-weeklyschedule.md)|Wochentag für die Systemüberprüfung. Mögliche Werte: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|defenderFilesAndFoldersToExclude|String collection|Dateien und Ordner, die von Überprüfungen und Echtzeitschutz ausgenommen werden sollen.|
|defenderFileExtensionsToExclude|String collection|Dateierweiterungen, die von Überprüfungen und Echtzeitschutz ausgenommen werden sollen.|
|defenderScanMaxCpu|Int32|Prozentsatz der maximalen CPU-Auslastung während der Überprüfung. Gültige Werte: 0 bis 100.|
|defenderMonitorFileActivity|[defenderMonitorFileActivity](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|Wert für die Überwachung der Dateiaktivität. Mögliche Werte: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|defenderPotentiallyUnwantedAppAction|[defenderPotentiallyUnwantedAppAction](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|Ruft die Aktion des Verteidigers ab oder legt Sie fest, die auf potenziell unerwünschte Anwendung (PUA) übertragen werden soll, einschließlich Software mit Verhaltensweisen von AD-Injection, Software Bündelung, dauerhafte Aufforderung zur Zahlung oder zum Abonnement usw. Defender warnt Benutzer, wenn PUA heruntergeladen wird, oder versucht, sich selbst zu installieren. HinzugeFügt in Windows 10 für Desktop. Mögliche Werte sind: `deviceDefault`, `block` und `audit`.|
|defenderPotentiallyUnwantedAppActionSetting|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Ruft die Aktion des Verteidigers ab oder legt Sie fest, die auf potenziell unerwünschte Anwendung (PUA) übertragen werden soll, einschließlich Software mit Verhaltensweisen von AD-Injection, Software Bündelung, dauerhafte Aufforderung zur Zahlung oder zum Abonnement usw. Defender warnt Benutzer, wenn PUA heruntergeladen wird, oder versucht, sich selbst zu installieren. HinzugeFügt in Windows 10 für Desktop. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderProcessesToExclude|String collection|Prozesse, die von Überprüfungen und Echtzeitschutz ausgenommen werden sollen.|
|defenderPromptForSampleSubmission|[defenderPromptForSampleSubmission](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|Die Konfiguration zur Aufforderung des Benutzers, ein Beispiel zu übermitteln. Mögliche Werte: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.|
|defenderRequireBehaviorMonitoring|Boolesch|Gibt an, ob eine Verhaltensüberwachung erforderlich ist.|
|defenderRequireCloudProtection|Boolesch|Gibt an, ob Cloudschutz erforderlich ist.|
|defenderRequireNetworkInspectionSystem|Boolesch|Gibt an, ob ein Netzwerkinspektionssystem erforderlich ist.|
|defenderRequireRealTimeMonitoring|Boolesch|Gibt an, ob eine Echtzeitüberwachung erforderlich ist.|
|defenderScanArchiveFiles|Boolescher Wert|Gibt an, ob Archivdateien gescannt werden sollen.|
|defenderScanDownloads|Boolean|Gibt an, ob Downloads gescannt werden sollen.|
|defenderScheduleScanEnableLowCpuPriority|Boolesch|Wenn diese Option aktiviert ist, wird bei geplanten Scans eine niedrige CPU-Priorität verwendet.|
|defenderDisableCatchupQuickScan|Boolesch|Nach der Blockierung werden die Catch-up-Scans für geplante Schnellscans deaktiviert.|
|defenderDisableCatchupFullScan|Boolesch|Nach der Blockierung werden die Catch-up-Scans für geplante vollständige Scans deaktiviert.|
|defenderScanNetworkFiles|Boolesch|Gibt an, ob in einem Netzwerkordner geöffnete Dateien gescannt werden sollen.|
|defenderScanIncomingMail|Boolesch|Gibt an, ob eingehende E-Mail-Nachrichten gescannt werden sollen.|
|defenderScanMappedNetworkDrivesDuringFullScan|Boolesch|Gibt an, ob zugeordnete Netzwerklaufwerke bei der vollständigen Überprüfung gescannt werden sollen.|
|defenderScanRemovableDrivesDuringFullScan|Boolesch|Gibt an, ob Wechseldatenträger bei der vollständigen Überprüfung gescannt werden sollen.|
|defenderScanScriptsLoadedInInternetExplorer|Boolesch|Gibt an, ob Skripts, die in Internet Explorer geladen sind, gescannt werden sollen.|
|defenderSignatureUpdateIntervalInHours|Int32|Das Aktualisierungsintervall der Signatur in Stunden. Geben Sie 0, wenn keine Überprüfung ausgeführt werden soll. Gültige Werte: 0 bis 24.|
|defenderScanType|[defenderScanType](../resources/intune-deviceconfig-defenderscantype.md)|Der Überprüfungstyp des Defender-Systems. Mögliche Werte sind: `userDefined`, `disabled`, `quick` und `full`.|
|defenderScheduledScanTime|TimeOfDay|Die Defender-Uhrzeit für die Systemüberprüfung.|
|defenderScheduledQuickScanTime|TimeOfDay|Die Zeit, zu der eine tägliche Schnellüberprüfung durchgeführt werden soll.|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|Gibt die Ebene für Schutz in der Cloud an. Mögliche Werte: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|defenderCloudExtendedTimeout|Int32|Timeout Erweiterung für die Dateiüberprüfung durch die Cloud. Gültige Werte: 0 bis 50.|
|defenderCloudExtendedTimeoutInSeconds|Int32|Timeout Erweiterung für die Dateiüberprüfung durch die Cloud. Gültige Werte: 0 bis 50.|
|defenderBlockOnAccessProtection|Boolesch|Ermöglicht oder deaktiviert Windows Defender bei Zugriffsschutzfunktionen.|
|defenderSubmitSamplesConsentType|[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|Überprüft die Benutzer Zustimmungs Stufe in Windows Defender zum Senden von Daten. Mögliche Werte: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.|
|lockScreenAllowTimeoutConfiguration|Boolesch|Gibt an, ob eine vom Benutzer konfigurierbare Einstellung zum Steuern des Bildschirmtimeouts auf dem Sperrbildschirm von Windows 10 Mobile-Geräten angezeigt werden soll. Wenn diese Richtlinie auf „Zulassen“ festgelegt ist, wird der von „lockScreenTimeoutInSeconds“ Wert ignoriert.|
|lockScreenBlockActionCenterNotifications|Boolesch|Gibt an, ob Benachrichtigungen des Info-Centers über den Sperrbildschirm blockiert werden sollen.|
|lockScreenBlockCortana|Boolesch|Gibt an, ob der Benutzer über die Spracherkennung mit Cortana interagieren kann, solange das System gesperrt ist.|
|lockScreenBlockToastNotifications|Boolesch|Gibt an, ob Popupbenachrichtigungen über dem Sperrbildschirm des Geräts zulässig sind.|
|lockScreenTimeoutInSeconds|Int32|Legt die Dauer (in Sekunden) vom Sperren des Bildschirms bis zum Abschalten des Bildschirms für Windows 10 Mobile-Geräte fest. Unterstützte Werte: 11 bis 1800. Gültige Werte: 11 bis 1800.|
|passwordBlockSimple|Boolesch|Geben Sie an, ob PINs oder Kennwörter wie „1111“ oder „1234“ zulässig sind. Für Windows 10-Desktops wird dadurch auch die Verwendung von Bildkennwörtern gesteuert.|
|passwordExpirationDays|Int32|Zeitraum in Tagen bis zum Ablaufen des Kennworts Gültige Werte: 0 bis 730.|
|passwordMinimumLength|Int32|Mindestlänge des Kennworts Gültige Werte: 4 bis 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.|
|passwordMinimumCharacterSetCount|Int32|Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen.|
|passwordPreviousPasswordBlockCount|Int32|Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss. Gültige Werte: 0 bis 50.|
|passwordRequired|Boolescher Wert|Gibt an, ob der Benutzer ein Kennwort benötigt.|
|passwordRequireWhenResumeFromIdleState|Boolean|Gibt an, ob zum Fortsetzen aus einem Leerlaufstatus ein Kennwort erforderlich ist.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Die Anzahl von fehlgeschlagenen Anmeldeversuchen, bevor eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird. Gültige Werte: 0 bis 999.|
|passwordMinimumAgeInDays|Int32|Diese Sicherheitseinstellung bestimmt den Zeitraum (in Tagen), für den ein Kennwort verwendet werden muss, bevor der Benutzer es ändern kann. Gültige Werte 0 bis 998|
|privacyAdvertisingId|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Aktiviert oder deaktiviert die Verwendung einer Werbe-ID. Dies wurde in Windows 10, Version 1607, hinzugefügt. Mögliche Werte sind: `notConfigured`, `blocked` und `allowed`.|
|privacyAutoAcceptPairingAndConsentPrompts|Boolesch|Gibt an, ob beim Starten von Apps das automatische Akzeptieren der Dialogfelder für die Benutzerzustimmung zur Kopplung und zum Datenschutz zulässig ist.|
|privacyDisableLaunchExperience|Boolesch|Diese Richtlinie verhindert, dass die Datenschutzumgebung während der Benutzeranmeldung für neue und aktualisierte Benutzer gestartet wird.|
|privacyBlockInputPersonalization|Boolesch|Gibt an, ob die Nutzung cloudbasierter Sprachdienste für Cortana, Diktat oder Store-Apps blockiert wird.|
|privacyBlockPublishUserActivities|Boolesch|Blockiert die gemeinsamen Erfahrungen/Ermittlung von zuletzt verwendeten Ressourcen in Task Switcher usw.|
|privacyBlockActivityFeed|Boolesch|Blockiert die Verwendung von Cloud-basierten Sprachdiensten für Cortana-, Diktat-oder Store-Anwendungen.|
|startBlockUnpinningAppsFromTaskbar|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer Apps aus der Taskleiste loslöst.|
|startMenuAppListVisibility|[windowsStartMenuAppListVisibilityType](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|Durch Festlegen dieses Werts wird die App-Liste reduziert oder vollständig entfernt bzw. die entsprechende Option in der App „Einstellungen“ deaktiviert. Mögliche Werte: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.|
|startMenuHideChangeAccountSettings|Boolesch|Durch Aktivieren dieser Richtlinie wird die Einstellung zur Kontoänderung in der Benutzerkachel im Startmenü ausgeblendet.|
|startMenuHideFrequentlyUsedApps|Boolesch|Durch Aktivieren dieser Richtlinie werden die meistverwendeten Apps aus dem Startmenü ausgeblendet, und die entsprechende Option wird in der App „Einstellungen“ deaktiviert.|
|startMenuHideHibernate|Boolesch|Durch Aktivieren dieser Richtlinie wird die Option „Ruhezustand“ nicht mehr im Netzschaltersymbol im Startmenü angezeigt.|
|startMenuHideLock|Boolesch|Durch Aktivieren dieser Richtlinie wird die Sperre aus der Benutzerkachel im Startmenü ausgeblendet.|
|startMenuHidePowerButton|Boolesch|Durch Aktivieren dieser Richtlinie wird das Netzschaltersymbol aus dem Startmenü ausgeblendet.|
|startMenuHideRecentJumpLists|Boolesch|Durch Aktivieren dieser Richtlinie werden die letzten Sprunglisten aus dem Startmenü/der Taskleiste ausgeblendet, und die entsprechende Option wird in der App „Einstellungen“ deaktiviert.|
|startMenuHideRecentlyAddedApps|Boolesch|Durch Aktivieren dieser Richtlinie werden zuletzt hinzugefügte Apps aus dem Startmenü ausgeblendet, und die entsprechende Option wird in der App „Einstellungen“ deaktiviert.|
|startMenuHideRestartOptions|Boolesch|Durch Aktivieren dieser Richtlinie werden die Optionen „Neu starten“und „Aktualisieren und neu starten“ nicht mehr im Netzschaltersymbol im Startmenü angezeigt.|
|startMenuHideShutDown|Boolesch|Durch Aktivieren dieser Richtlinie wird „Herunterfahren/Aktualisieren“ und „Herunterfahren“ aus dem Netzschaltersymbol im Startmenü ausgeblendet.|
|startMenuHideSignOut|Boolesch|Durch Aktivieren dieser Richtlinie wird „Abmelden“ aus der Benutzerkachel im Startmenü ausgeblendet.|
|startMenuHideSleep|Boolesch|Durch Aktivieren dieser Richtlinie wird „Standbymodus“ aus dem Netzschaltersymbol im Startmenü ausgeblendet|
|startMenuHideSwitchAccount|Boolescher Wert|Durch Aktivieren dieser Richtlinie wird „Konto wechseln“ aus der Benutzerkachel im Startmenü ausgeblendet.|
|startMenuHideUserTile|Boolean|Durch Aktivieren dieser Richtlinie wird die Benutzerkachel aus dem Startmenü ausgeblendet.|
|startMenuLayoutEdgeAssetsXml|Binär|Diese Richtlinieneinstellung ermöglicht Ihnen das Importieren von Microsoft Edge-Assets zur Verwendung mit der Richtlinie „startMenuLayoutXml“. Das Startlayout kann eine sekundäre Kachel aus der Edge-App enthalten, die nach der lokalen Edge-Assetdatei sucht. Das lokale Edge-Asset ist in diesem Fall nicht vorhanden und führt dazu, dass die sekundäre Edge-Kachel leer angezeigt wird.  Diese Richtlinie wird nur angewendet, wenn die Richtlinie „startMenuLayoutXml“ geändert wird. Der Wert sollte ein UTF-8-Base64-codiertes Bytearray sein.|
|startMenuLayoutXml|Binär|Ermöglicht Administratoren das Außerkraftsetzen des Startmenü-Standardlayouts und verhindert Änderungen durch den Benutzer. Das Layout wird durch Angabe einer XML-Datei geändert, die auf einem Layoutänderungsschema basiert. XML muss ein UTF8-codiertes Bytearrayformat aufweisen.|
|startMenuMode|[windowsStartMenuModeType](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|Ermöglicht Administratoren zu entscheiden, wie das Startmenü angezeigt wird. Mögliche Werte sind: `userDefined`, `fullScreen` und `nonFullScreen`.|
|startMenuPinnedFolderDocuments|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Dokumente“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderDownloads|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Downloads“ im Startmenü. Mögliche Werte sind: `notConfigured`, `hide` und `show`.|
|startMenuPinnedFolderFileExplorer|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung „FileExplorer“ im Startmenü Mögliche Werte sind: `notConfigured`, `hide` und `show`.|
|startMenuPinnedFolderHomeGroup|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „ Heimnetzgruppe“ im Startmenü. Mögliche Werte sind: `notConfigured`, `hide` und `show`.|
|startMenuPinnedFolderMusic|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Musik“ im Startmenü. Mögliche Werte sind: `notConfigured`, `hide` und `show`.|
|startMenuPinnedFolderNetwork|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Netzwerk“ im Startmenü. Mögliche Werte sind: `notConfigured`, `hide` und `show`.|
|startMenuPinnedFolderPersonalFolder|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem persönlichen Ordner im Startmenü. Mögliche Werte sind: `notConfigured`, `hide` und `show`.|
|startMenuPinnedFolderPictures|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Bilder“ im Startmenü. Mögliche Werte sind: `notConfigured`, `hide` und `show`.|
|startMenuPinnedFolderSettings|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Einstellungen“ im Startmenü. Mögliche Werte sind: `notConfigured`, `hide` und `show`.|
|startMenuPinnedFolderVideos|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Erzwingt die Sichtbarkeit (Anzeigen/Ausblenden) der Verknüpfung mit dem Ordner „Videos“ im Startmenü. Mögliche Werte: `notConfigured`, `hide`, `show`.|
|settingsBlockSettingsApp|Boolesch|Gibt an, ob der Zugriff auf die App „Einstellungen“ blockiert werden soll.|
|settingsBlockSystemPage|Boolesch|Gibt an, ob der Zugriff auf „System“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockDevicesPage|Boolesch|Gibt an, ob der Zugriff auf „Geräte“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockNetworkInternetPage|Boolesch|Gibt an, ob der Zugriff auf „Netzwerk und Internet“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockPersonalizationPage|Boolesch|Gibt an, ob der Zugriff auf „Personalisierung“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockAccountsPage|Boolesch|Gibt an, ob der Zugriff auf „Konten“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockTimeLanguagePage|Boolesch|Gibt an, ob der Zugriff auf „Zeit und Sprache“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockEaseOfAccessPage|Boolesch|Gibt an, ob der Zugriff auf „Erleichterte Bedienung“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockPrivacyPage|Boolesch|Gibt an, ob der Zugriff auf „Datenschutz“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockUpdateSecurityPage|Boolesch|Gibt an, ob der Zugriff auf „Update und Sicherheit“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockAppsPage|Boolesch|Gibt an, ob der Zugriff auf „Apps“ in der App „Einstellungen“ blockiert werden soll.|
|settingsBlockGamingPage|Boolesch|Gibt an, ob der Zugriff auf „Gaming“ in der App „Einstellungen“ blockiert werden soll.|
|windowsSpotlightBlockConsumerSpecificFeatures|Boolesch|Ermöglicht IT-Administratoren das Blockieren von Funktionen, die normalerweise nur für Endbenutzer bestimmt sind, beispielsweise Startvorschläge, Mitgliedschaftsbenachrichtigungen, App-Installation nach Anzeige der Windows-Willkommensseite und Kachelumleitungen.|
|windowsSpotlightBlocked|Boolesch|Ermöglicht IT-Administratoren das Deaktivieren aller Features von Windows-Blickpunkt.|
|windowsSpotlightBlockOnActionCenter|Boolesch|Blockiert Vorschläge von Microsoft, die nach jeder Neuinstallation des Betriebssytem, nach jedem Upgrade oder auf fortlaufender Basis angezeigt werden, um Benutzern Neuigkeiten oder Änderungen vorzustellen.|
|windowsSpotlightBlockTailoredExperiences|Boolesch|Blockiert personalisierte Inhalte in Windows-Blickpunkt basierend auf dem Gerät, das der Benutzer verwendet.|
|windowsSpotlightBlockThirdPartyNotifications|Boolesch|Blockiert Inhalte von Drittanbietern, die über Windows-Blickpunkt übermittelt werden.|
|windowsSpotlightBlockWelcomeExperience|Boolesch|Windows-Begrüßungsseite zur Vorstellung neuer oder aktualisierter Features blockieren|
|windowsSpotlightBlockWindowsTips|Boolescher Wert|Ermöglicht IT-Administratoren das Deaktivieren des Popups von Windows-Tipps.|
|windowsSpotlightConfigureOnLockScreen|[windowsSpotlightEnablementSettings](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|Gibt den Typ des Spotlight an. Mögliche Werte sind: `notConfigured`, `disabled` und `enabled`.|
|networkProxyApplySettingsDeviceWide|Boolean|Wenn dieser Wert festgelegt ist, werden Proxyeinstellungen auf alle Prozesse und Konten in dem Gerät angewendet. Andernfalls wird er auf das Benutzerkonto angewendet, das bei MDM registriert ist.|
|networkProxyDisableAutoDetect|Boolesch|Deaktiviert die automatische Erkennung von Einstellungen. Wenn diese Option aktiviert ist, versucht das System, den Pfad zu einem PAC-Skript (automatische Proxykonfiguration) zu suchen.|
|networkProxyAutomaticConfigurationUrl|Zeichenfolge|Adresse zu dem PAC-Skript, das Sie verwenden möchten.|
|networkProxyServer|[windows10NetworkProxyServer](../resources/intune-deviceconfig-windows10networkproxyserver.md)|Gibt manuelle Proxyservereinstellungen an.|
|accountsBlockAddingNonMicrosoftAccountEmail|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer E-Mail-Konten zu Geräten hinzufügt, die keinem Microsoft-Konto zugeordnet sind.|
|antiTheftModeBlocked|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer eine Einstellung für den AntiTheft-Modus auswählt (nur Windows 10 Mobile).|
|bluetoothBlocked|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer Bluetooth verwendet.|
|cameraBlocked|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.|
|connectedDevicesServiceBlocked|Boolesch|Gibt an, ob der Dienst für verbundene Geräte blockiert werden soll, der die Ermittlung anderer Geräte und eine Verbindungsherstellung zu anderen Geräten, Remotmessaging, Remote-App-Sitzungen und anderen geräteübergreifenden Oberflächen ermöglicht.|
|certificatesBlockManualRootCertificateInstallation|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer eine manuelle Stammzertifikatinstallation ausführt.|
|copyPasteBlocked|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer Kopieren/Einfügen verwendet.|
|cortanaBlocked|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer Cortana verwendet.|
|deviceManagementBlockFactoryResetOnMobile|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer sein Telefon zurücksetzt.|
|deviceManagementBlockManualUnenroll|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer eine manuelle Aufhebung der Registrierung von der Geräteverwaltung vornimmt.|
|safeSearchFilter|[safeSearchFilterType](../resources/intune-deviceconfig-safesearchfiltertype.md)|Gibt an, welche Filterebene von SafeSearch erforderlich ist. Mögliche Werte: `userDefined`, `strict`, `moderate`.|
|edgeBlockPopups|Boolesch|Gibt an, ob Popups blockiert werden sollen.|
|edgeBlockSearchSuggestions|Boolesch|Gibt an, ob die Verwendung der Suchvorschläge in der Adressleiste verhindert werden soll.|
|edgeBlockSearchEngineCustomization|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer neue Suchmaschine hinzufügt oder die Standardsuchmaschine ändert.|
|edgeBlockSendingIntranetTrafficToInternetExplorer|Boolesch|Gibt an, ob der Intranet-Datenverkehr von Edge zu Internet Explorer gewechselt werden soll. Hinweis: der Name dieser Eigenschaft ist irreführend; die Eigenschaft ist veraltet, verwenden Sie stattdessen EdgeSendIntranetTrafficToInternetExplorer.|
|edgeSendIntranetTrafficToInternetExplorer|Boolesch|Gibt an, ob der Intranet-Datenverkehr von Edge zu Internet Explorer gewechselt werden soll.|
|edgeRequireSmartScreen|Boolesch|Gibt an, ob der Benutzer aufgefordert werden soll, den Smartscreenfilter zu verwenden.|
|edgeEnterpriseModeSiteListLocation|Zeichenfolge|Gibt den Speicherort der Siteliste für den Unternehmensmodus an. Dies kann eine lokale Datei, ein lokales Netzwerk oder ein http-Speicherort sein.|
|edgeFirstRunUrl|String|Die URL für erste Ausführung, wenn der Edge-Browser das erste Mal geöffnet wird.|
|edgeSearchEngine|[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)|Ermöglicht es IT-Administratoren, eine standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen. Benutzer können dies außer Kraft setzen und die standardmäßige Suchmaschine ändern, sofern die Richtlinie „AllowSearchEngineCustomization“ nicht festgelegt ist.|
|edgeHomepageUrls|String collection|Die Liste von URLs für Startseiten, die auf bei MDM-registrierten Geräten im Edge-Browser angezeigt werden.|
|edgeBlockAccessToAboutFlags|Boolesch|Gibt an, ob Zugriff auf Info-Flags im Edge-Browser verhindert werden soll.|
|smartScreenBlockPromptOverride|Boolesch|Gibt an, ob Benutzer SmartScreenFilter-Warnungen zu potenziell bösartigen Websites außer Kraft setzen können.|
|smartScreenBlockPromptOverrideForFiles|Boolesch|Gibt an, ob Benutzer die SmartScreenFilter-Warnungen zum Herunterladen nicht überprüfter Dateien außer Kraft setzen können.|
|webRtcBlockLocalhostIpAddress|Boolesch|Gibt an, ob die LocalHost-IP-Adresse des Benutzers angezeigt wird, während Telefonanrufe über WebRTC getätigt werden.|
|internetSharingBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Internetfreigabe verwendet.|
|settingsBlockAddProvisioningPackage|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Bereitstellungspakete installiert.|
|settingsBlockRemoveProvisioningPackage|Boolesch|Gibt an, ob verhindert werden soll, dass der Laufzeitkonfigurations-Agent Bereitstellungspakete entfernt.|
|settingsBlockChangeSystemTime|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer die Einstellungen für Datum und Uhrzeit ändert.|
|settingsBlockEditDeviceName|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer den Gerätenamen bearbeitet.|
|settingsBlockChangeRegion|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer Regionseinstellungen ändert.|
|settingsBlockChangeLanguage|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer Spracheinstellungen ändert.|
|settingsBlockChangePowerSleep|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer Energie- und Energiesparmoduseinstellungen ändert.|
|locationServicesBlocked|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer Ortungsdienste verwendet.|
|microsoftAccountBlocked|Boolesch|Gibt an, ob ein Microsoft-Konto blockiert werden soll.|
|microsoftAccountBlockSettingsSync|Boolesch|Gibt an, ob die Synchronisierung von Einstellungen eines Microsoft-Kontos blockiert werden soll.|
|nfcBlocked|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer Near Field Communication verwendet.|
|resetProtectionModeBlocked|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer den Schutzmodus zurücksetzt.|
|screenCaptureBlocked|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer Screenshots macht.|
|storageBlockRemovableStorage|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer Wechselmedien verwendet.|
|storageRequireMobileDeviceEncryption|Boolesch|Gibt an, ob für ein mobiles Gerät eine Verschlüsselung erforderlich ist.|
|usbBlocked|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer eine USB-Verbindung verwendet.|
|voiceRecordingBlocked|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer die Sprachaufzeichnung verwendet.|
|wiFiBlockAutomaticConnectHotspots|Boolesch|Gibt an, ob die automatische Herstellung einer Verbindung zu WLAN-Hotspots blockiert werden soll. Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.|
|wiFiBlocked|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer WLAN verwendet.|
|wiFiBlockManualConfiguration|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer eine manuelle WLAN-Konfiguration verwendet.|
|wiFiScanInterval|Int32|Gibt an, wie häufig Geräte nach WLAN-Netzwerken suchen. Unterstützte Werte sind 1 bis 500, wobei 100 der Standardwert ist und 500 eine niedrige Häufigkeit bedeutet. Gültige Werte: 1 bis 500.|
|wirelessDisplayBlockProjectionToThisDevice|Boolesch|Gibt an, ob erlaubt werden soll, dass andere Geräte diesen Computer für die Projektion ermitteln.|
|wirelessDisplayBlockUserInputFromReceiver|Boolesch|Gibt an, ob Benutzereingaben von drahtlosen Anzeigeempfängern erlaubt sind.|
|wirelessDisplayRequirePinForPairing|Boolesch|Gibt an, ob eine PIN für neue Geräte zum Initiieren der Kopplung erforderlich ist.|
|windowsStoreBlocked|Boolesch|Gibt an, ob verhindert werden soll, dass der Benutzer den Windows Store verwendet.|
|appsAllowTrustedAppsSideloading|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Gibt an, ob Apps aus AppX-Paketen, die mit einem vertrauenswürdigen Zertifikat signiert sind, quergeladen werden können. Mögliche Werte sind: `notConfigured`, `blocked` und `allowed`.|
|windowsStoreBlockAutoUpdate|Boolesch|Gibt an, ob automatische Updates von Apps aus dem Windows Store blockiert werden sollen.|
|developerUnlockSetting|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Gibt an, ob die Entwicklersperre zulässig ist. Mögliche Werte: `notConfigured`, `blocked`, `allowed`.|
|sharedUserAppDataAllowed|Boolesch|Gibt an, ob verhindert werden soll, dass mehrere Benutzer derselben App Daten austauschen.|
|appsBlockWindowsStoreOriginatedApps|Boolesch|Gibt an, ob das Starten aller Apps aus dem Windows Store deaktiviert werden soll, die vorinstalliert waren oder heruntergeladen wurden.|
|windowsStoreEnablePrivateStoreOnly|Boolesch|Gibt an, ob nur der private Store aktiviert werden soll.|
|storageRestrictAppDataToSystemVolume|Boolesch|Gibt an, ob Anwendungsdaten auf das Systemlaufwerk beschränkt sind.|
|storageRestrictAppInstallToSystemVolume|Boolescher Wert|Gibt an, ob die Installation von Anwendungen auf das Systemlaufwerk beschränkt ist.|
|gameDvrBlocked|Boolean|Gibt an, ob DVR und Broadcasting blockiert werden soll.|
|experienceBlockDeviceDiscovery|Boolesch|Gibt an, ob die Geräteerkennungs-UX aktiviert werden soll.|
|experienceBlockErrorDialogWhenNoSIM|Boolesch|Gibt an, ob das Fehlerdialogfeld angezeigt werden soll, wenn keine SIM-Karte erkannt wird.|
|experienceBlockTaskSwitcher|Boolescher Wert|Gibt an, ob die Programmumschaltung auf dem Gerät aktiviert werden soll.|
|logonBlockFastUserSwitching|Boolean|Verhindert, dass schnell zwischen Benutzern umgeschaltet werden kann, die gleichzeitig ohne Abmelden angemeldet sind.|
|tenantLockdownRequireNetworkDuringOutOfBoxExperience|Boolesch|Gibt an, ob das Gerät zum Herstellen einer Verbindung mit dem Netzwerk erforderlich ist.|
|appManagementMSIAllowUserControlOverInstall|Boolesch|Mit dieser Richtlinieneinstellung können Benutzer Installationsoptionen ändern, die normalerweise nur Systemadministratoren zur Verfügung stehen.|
|appManagementMSIAlwaysInstallWithElevatedPrivileges|Boolesch|Diese Richtlinieneinstellung weist Windows Installer an, bei der Installation von Programmen auf dem System erhöhte Berechtigungen zu verwenden.|
|dataProtectionBlockDirectMemoryAccess|Boolesch|Mit dieser Richtlinieneinstellung können Sie DMA (Direct Memory Access) für alle Hot-Plug-fähigen PCI Downstream-Ports blockieren, bis sich ein Benutzer an Windows anmeldet.|
|appManagementPackageFamilyNamesToLaunchAfterLogOn|String collection|Liste der mit Trennzeichen getrennten Doppelpunkt-Paket Familiennamen von Windows-apps. Aufgelistete Windows-apps sollen nach der Anmeldung gestartet werden.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 13518

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "taskManagerBlockEndTask": true,
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "microsoftAccountSignInAssistantSettings": "disabled",
  "authenticationAllowSecondaryDevice": true,
  "authenticationWebSignIn": "enabled",
  "authenticationPreferredAzureADTenantDomainName": "Authentication Preferred Azure ADTenant Domain Name value",
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "Display App List With Gdi DPIScaling Turned On value"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "Display App List With Gdi DPIScaling Turned Off value"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "experienceDoNotSyncBrowserSettings": "blockedWithUserOverride",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "Printer Names value"
  ],
  "printerDefaultName": "Printer Default Name value",
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
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
  "edgeTelemetryForMicrosoft365Analytics": "intranet",
  "inkWorkspaceAccess": "enabled",
  "inkWorkspaceAccessState": "blocked",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockPromptedProximalConnections": true,
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
  "edgeFavoritesListLocation": "Edge Favorites List Location value",
  "edgeBlockEditFavorites": true,
  "edgeNewTabPageURL": "Edge New Tab Page URL value",
  "edgeHomeButtonConfiguration": {
    "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
  },
  "edgeHomeButtonConfigurationEnabled": true,
  "edgeOpensWith": "startPage",
  "edgeBlockSideloadingExtensions": true,
  "edgeRequiredExtensionPackageFamilyNames": [
    "Edge Required Extension Package Family Names value"
  ],
  "edgeBlockPrinting": true,
  "edgeFavoritesBarVisibility": "hide",
  "edgeBlockSavingHistory": true,
  "edgeBlockFullScreenMode": true,
  "edgeBlockWebContentOnNewTabPage": true,
  "edgeBlockTabPreloading": true,
  "edgeBlockPrelaunch": true,
  "edgeShowMessageWhenOpeningInternetExplorerSites": "disabled",
  "edgePreventCertificateErrorOverride": true,
  "edgeKioskModeRestriction": "digitalSignage",
  "edgeKioskResetAfterIdleTimeInMinutes": 4,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "required",
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
  "defenderPotentiallyUnwantedAppAction": "block",
  "defenderPotentiallyUnwantedAppActionSetting": "enable",
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
  "defenderScheduleScanEnableLowCpuPriority": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderDisableCatchupFullScan": true,
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
  "defenderCloudExtendedTimeout": 12,
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderBlockOnAccessProtection": true,
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
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
  "passwordMinimumAgeInDays": 8,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyDisableLaunchExperience": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
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
  "edgeBlockSearchEngineCustomization": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeSendIntranetTrafficToInternetExplorer": true,
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
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true,
  "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
    "App Management Package Family Names To Launch After Log On value"
  ]
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 13690

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "taskManagerBlockEndTask": true,
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "microsoftAccountSignInAssistantSettings": "disabled",
  "authenticationAllowSecondaryDevice": true,
  "authenticationWebSignIn": "enabled",
  "authenticationPreferredAzureADTenantDomainName": "Authentication Preferred Azure ADTenant Domain Name value",
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "Display App List With Gdi DPIScaling Turned On value"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "Display App List With Gdi DPIScaling Turned Off value"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "experienceDoNotSyncBrowserSettings": "blockedWithUserOverride",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "Printer Names value"
  ],
  "printerDefaultName": "Printer Default Name value",
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
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
  "edgeTelemetryForMicrosoft365Analytics": "intranet",
  "inkWorkspaceAccess": "enabled",
  "inkWorkspaceAccessState": "blocked",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockPromptedProximalConnections": true,
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
  "edgeFavoritesListLocation": "Edge Favorites List Location value",
  "edgeBlockEditFavorites": true,
  "edgeNewTabPageURL": "Edge New Tab Page URL value",
  "edgeHomeButtonConfiguration": {
    "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
  },
  "edgeHomeButtonConfigurationEnabled": true,
  "edgeOpensWith": "startPage",
  "edgeBlockSideloadingExtensions": true,
  "edgeRequiredExtensionPackageFamilyNames": [
    "Edge Required Extension Package Family Names value"
  ],
  "edgeBlockPrinting": true,
  "edgeFavoritesBarVisibility": "hide",
  "edgeBlockSavingHistory": true,
  "edgeBlockFullScreenMode": true,
  "edgeBlockWebContentOnNewTabPage": true,
  "edgeBlockTabPreloading": true,
  "edgeBlockPrelaunch": true,
  "edgeShowMessageWhenOpeningInternetExplorerSites": "disabled",
  "edgePreventCertificateErrorOverride": true,
  "edgeKioskModeRestriction": "digitalSignage",
  "edgeKioskResetAfterIdleTimeInMinutes": 4,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "required",
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
  "defenderPotentiallyUnwantedAppAction": "block",
  "defenderPotentiallyUnwantedAppActionSetting": "enable",
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
  "defenderScheduleScanEnableLowCpuPriority": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderDisableCatchupFullScan": true,
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
  "defenderCloudExtendedTimeout": 12,
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderBlockOnAccessProtection": true,
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
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
  "passwordMinimumAgeInDays": 8,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyDisableLaunchExperience": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
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
  "edgeBlockSearchEngineCustomization": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeSendIntranetTrafficToInternetExplorer": true,
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
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true,
  "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
    "App Management Package Family Names To Launch After Log On value"
  ]
}
```




