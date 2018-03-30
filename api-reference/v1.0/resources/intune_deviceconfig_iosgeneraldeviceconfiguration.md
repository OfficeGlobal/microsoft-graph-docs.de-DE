# <a name="iosgeneraldeviceconfiguration-resource-type"></a>iosGeneralDeviceConfiguration-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „ iosGeneralDeviceConfiguration“ verfügbar gemacht werden.

Sie erbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[iosGeneralDeviceConfigurations auflisten](../api/intune_deviceconfig_iosgeneraldeviceconfiguration_list.md)|[iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)-Sammlung|Listet die Eigenschaften und Beziehungen der [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)-Objekte auf.|
|[iosGeneralDeviceConfiguration abrufen](../api/intune_deviceconfig_iosgeneraldeviceconfiguration_get.md)|[iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)|Liest die Eigenschaften und Beziehungen des [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)-Objekts.|
|[iosGeneralDeviceConfiguration erstellen](../api/intune_deviceconfig_iosgeneraldeviceconfiguration_create.md)|[iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)|Erstellen Sie ein neues [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)-Objekt.|
|[iosGeneralDeviceConfiguration löschen](../api/intune_deviceconfig_iosgeneraldeviceconfiguration_delete.md)|Keine|Löscht eine [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)|
|[iosGeneralDeviceConfiguration aktualisieren](../api/intune_deviceconfig_iosgeneraldeviceconfiguration_update.md)|[iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)|Aktualisiert die Eigenschaften eines [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Beschreibung|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|accountBlockModification|Boolescher Wert|Gibt an, ob die Kontoänderung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.|
|activationLockAllowWhenSupervised|Boolescher Wert|Gibt an, ob die Aktivierungssperre zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.|
|airDropBlocked|Boolescher Wert|Gibt an, ob AirDrop zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.|
|airDropForceUnmanagedDropTarget|Boolescher Wert|Gibt an, ob AirDrop als nicht verwaltetes Drop-Ziel (iOS 9.0 oder höher) betrachtet werden soll.|
|airPlayForcePairingPasswordForOutgoingRequests|Boolescher Wert|Gibt an, ob erzwungen werden soll, dass alle Geräte, die AirPlay-Anforderungen von diesem Gerät erhalten, ein Kopplungskennwort verwenden.|
|appleWatchBlockPairing|Boolescher Wert|Gibt an, ob eine Apple Watch-Kopplung zulässig ist, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).|
|appleWatchForceWristDetection|Boolescher Wert|Gibt an, ob erzwungen werden soll, dass eine gekoppelte Apple Watch die Handgelenkerkennung (iOS 8.2 und höher) verwendet.|
|appleNewsBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer News verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).|
|appsSingleAppModeList|[appListItem](../resources/intune_deviceconfig_applistitem.md)-Sammlung|Ruft die Liste von iOS-Apps ab, die autonom in den Einzelanwendungsmodus wechseln können, ab oder legt diese fest. Nur überwacht. iOS 7.0 oder höher. Diese Sammlung darf maximal 500 Elemente enthalten.|
|appsVisibilityList|[appListItem](../resources/intune_deviceconfig_applistitem.md)-Sammlung|Liste von Apps in der Sichtbarkeitsliste (entweder eine Liste sichtbarer/startbarer Apps oder eine Liste ausgeblendeter/nicht startbarer Apps, gesteuert von AppsVisibilityListType) (iOS 9.3 und höher). Diese Sammlung darf maximal 10.000 Elemente enthalten.|
|appsVisibilityListType|Zeichenfolge|Typ der in „AppsVisibilityList“ enthaltenen Liste. Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|appStoreBlockAutomaticDownloads|Boolescher Wert|Gibt an, ob das automatische Herunterladen von Apps blockiert werden soll, die auf anderen Geräten gekauft wurden, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).|
|appStoreBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer den App Store verwendet.|
|appStoreBlockInAppPurchases|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer In-App-Käufe tätigt.|
|appStoreBlockUIAppInstallation|Boolescher Wert|Gibt an, ob die App Store-App blockiert werden soll, ohne die Installation über Host-Apps einzuschränken. Gilt nur für den überwachten Modus (iOS 9.0 und höher).|
|appStoreRequirePassword|Boolescher Wert|Gibt an, ob bei Verwendung des App Stores ein Kennwort erforderlich ist.|
|bluetoothBlockModification|Boolescher Wert|Gibt an, ob das Ändern von Bluetooth-Einstellungen zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 10.0 und höher).|
|cameraBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.|
|cellularBlockDataRoaming|Boolescher Wert|Gibt an, ob Datenroaming blockiert werden soll.|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Boolescher Wert|Gibt an, ob das globales Abrufen im Hintergrund beim Roaming blockiert werden soll.|
|cellularBlockPerAppDataModification|Boolescher Wert|Gibt an, ob Änderungen an den Mobil-App-Daten zulässig sind, wenn sich das Gerät im überwachten Modus befindet.|
|cellularBlockPersonalHotspot|Boolescher Wert|Gibt an, ob der privater Hotspot blockiert werden soll.|
|cellularBlockVoiceRoaming|Boolescher Wert|Gibt an, ob Sprachroaming blockiert werden soll.|
|certificatesBlockUntrustedTlsCertificates|Boolescher Wert|Gibt an, ob nicht vertrauenswürdige TLS-Zertifikate blockiert werden sollen.|
|classroomAppBlockRemoteScreenObservation|Boolescher Wert|Gibt an, ob die Remotebildschirmüberwachung über die Classroom-App zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).|
|classroomAppForceUnpromptedScreenObservation|Boolescher Wert|Gibt an, ob dem Lehrer eines verwalteten Kurses in der Classroom-App automatisch die Berechtigung erteilt werden soll, den Bildschirm eines Kursteilnehmers ohne Aufforderung anzuzeigen, wenn sich das Gerät im überwachten Modus befindet.|
|compliantAppsList|[appListItem](../resources/intune_deviceconfig_applistitem.md)-Sammlung|Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“). Diese Sammlung darf maximal 10.000 Elemente enthalten.|
|compliantAppListType|Zeichenfolge|Typ der in „compliantAppsList“ definierten Liste. Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|configurationProfileBlockChanges|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Konfigurationsprofile und Zertifikate interaktiv installiert, wenn sich das Gerät im überwachten Modus befindet.|
|definitionLookupBlocked|Boolescher Wert|Gibt an, ob die Definitionssuche zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).|
|deviceBlockEnableRestrictions|Boolescher Wert|Gibt an, ob erlaubt werden soll, dass der Benutzer Einschränkungen in den Geräteeinstellungen aktiviert, wenn sich das Gerät im überwachten Modus befindet.|
|deviceBlockEraseContentAndSettings|Boolescher Wert|Gibt an, ob die Verwendung der Option zum Löschen aller Inhalte und Einstellungen auf dem Gerät zugelassen werden soll, wenn sich das Gerät im überwachten Modus befindet.|
|deviceBlockNameModification|Boolescher Wert|Gibt an, ob das Ändern des Gerätenamens zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).|
|diagnosticDataBlockSubmission|Boolescher Wert|Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.|
|diagnosticDataBlockSubmissionModification|Boolescher Wert|Gibt an, ob das Ändern der Einstellungen für die Diagnoseübermittlung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3.2 und höher).|
|documentsBlockManagedDocumentsInUnmanagedApps|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer verwaltete Dokumente in nicht verwalteten Apps anzeigt.|
|documentsBlockUnmanagedDocumentsInManagedApps|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer nicht verwaltete Dokumente in verwalteten Apps anzeigt.|
|emailInDomainSuffixes|Zeichenfolgenauflistung|E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.|
|enterpriseAppBlockTrust|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer einer Unternehmens-App vertraut.|
|enterpriseAppBlockTrustModification|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer die Vertrauensstellungseinstellungen der Unternehmens-App ändert.|
|faceTimeBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer FaceTime verwendet.|
|findMyFriendsBlocked|Boolescher Wert|Gibt an, ob „Freunde suchen“ blockiert wird, wenn sich das Gerät im überwachten Modus befindet.|
|gamingBlockGameCenterFriends|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Freunde im Game Center hat.|
|gamingBlockMultiplayer|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Multiplayerspiele verwendet.|
|gameCenterBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Game Center verwendet, wenn sich das Gerät im überwachten Modus befindet.|
|hostPairingBlocked|Boolescher Wert|Gibt an, ob die Hostkopplung blockiert werden soll, um zu steuern, mit welchen Geräten ein iOS-Gerät gekoppelt werden kann,wenn sich das iOS-Gerät im überwachten Modus befindet.|
|iBooksStoreBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer den iBooks Store verwendet, wenn sich das Gerät im überwachten Modus befindet.|
|iBooksStoreBlockErotica|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Medien aus dem iBook Store herunterlädt, die als Erotik gekennzeichnet sind.|
|iCloudBlockActivityContinuation|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer eine Aufgabe, die er auf dem iOS-Gerät begonnen hat, auf einem anderen iOS- oder macOS-Gerät fortsetzt.|
|iCloudBlockBackup|Boolescher Wert|Gibt an, ob die iCloud-Sicherung blockiert werden soll.|
|iCloudBlockDocumentSync|Boolescher Wert|Gibt an, ob die iCloud-Dokumentsynchronisierung blockiert werden soll.|
|iCloudBlockManagedAppsSync|Boolescher Wert|Gibt an, ob die Cloudsynchronisierung für verwaltete Apps blockiert werden soll.|
|iCloudBlockPhotoLibrary|Boolescher Wert|Gibt an, ob die iCloud-Fotomediathek blockiert werden soll.|
|iCloudBlockPhotoStreamSync|Boolescher Wert|Gibt an, ob die Fotostream-Synchronisierung in iCloud blockiert werden soll.|
|iCloudBlockSharedPhotoStream|Boolescher Wert|Gibt an, ob die Fotofreigabe blockiert werden soll.|
|iCloudRequireEncryptedBackup|Boolescher Wert|Gibt an, ob Sicherungen in iCloud verschlüsselt sein müssen.|
|iTunesBlockExplicitContent|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer auf anstößige Inhalte in iTunes und im App Store zugreift. |
|iTunesBlockMusicService|Boolescher Wert|Gibt an, ob der Music-Dienst blockiert und die Music-App in den klassischen Modus zurückgesetzt werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher und Mac OS 10.12 und höher).|
|iTunesBlockRadio|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer iTunes Radio verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).|
|keyboardBlockAutoCorrect|Boolescher Wert|Gibt an, ob die Autokorrektur der Tastatur blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).|
|keyboardBlockDictation|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer die Diktatfunktion verwendet, wenn sich das Gerät im überwachten Modus befindet.|
|keyboardBlockPredictive|Boolescher Wert|Gibt an, ob Tastaturwortvorschläge blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).|
|keyboardBlockShortcuts|Boolescher Wert|Gibt an, ob Tastenkombinationen blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).|
|keyboardBlockSpellCheck|Boolescher Wert|Gibt an, ob die Rechtschreibprüfung blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).|
|kioskModeAllowAssistiveSpeak|Boolescher Wert|Gibt an, ob Sprachunterstützung im Kiosk-Modus zulässig ist.|
|kioskModeAllowAssistiveTouchSettings|Boolescher Wert|Gibt an, ob Zugriff auf die Einstellungen der Touch-Unterstützung im Kiosk-Modus gewährt werden soll.|
|kioskModeAllowAutoLock|Boolescher Wert|Gibt an, ob die automatische Gerätesperre im Kiosk-Modus zulässig ist.|
|kioskModeAllowColorInversionSettings|Boolescher Wert|Gibt ab, ob der Zugriff auf die Farbinversionseinstellungen im Kiosk-Modus erlaubt werden soll.|
|kioskModeAllowRingerSwitch|Boolescher Wert|Gibt ab, ob die Verwendung des Ruftonschalters im Kiosk-Modus erlaubt werden soll.|
|kioskModeAllowScreenRotation|Boolescher Wert|Gibt ab, ob die Bildschirmdrehung im Kiosk-Modus erlaubt werden soll.|
|kioskModeAllowSleepButton|Boolescher Wert|Gibt ab, ob die Verwendung der Energiespartaste im Kiosk-Modus erlaubt werden soll.|
|kioskModeAllowTouchscreen|Boolescher Wert|Gibt ab, ob die Verwendung des Touchscreens im Kiosk-Modus erlaubt werden soll.|
|kioskModeAllowVoiceOverSettings|Boolescher Wert|Gibt ab, ob der Zugriff auf die Einstellungen für Hintergrundkommentare im Kiosk-Modus erlaubt werden soll.|
|kioskModeAllowVolumeButtons|Boolescher Wert|Gibt ab, ob die Verwendung der Lautstärketasten im Kiosk-Modus erlaubt werden soll.|
|kioskModeAllowZoomSettings|Boolescher Wert|Gibt ab, ob der Zugriff auf die Zoomeinstellungen im Kiosk-Modus erlaubt werden soll.|
|kioskModeAppStoreUrl|Zeichenfolge|URL im App Store zu der App, die für den Kiosk-Modus verwendet werden soll. Verwenden Sie diese, wenn „KioskModeManagedAppId“ nicht bekannt ist.|
|kioskModeRequireAssistiveTouch|Boolescher Wert|Gibt an, ob Touch-Unterstützung im Kiosk-Modus erforderlich ist.|
|kioskModeRequireColorInversion|Boolescher Wert|Gibt ab, ob die Farbinversion im Kiosk-Modus erforderlich ist.|
|kioskModeRequireMonoAudio|Boolescher Wert|Gibt ab, ob Mono-Audio im Kiosk-Modus erforderlich ist.|
|kioskModeRequireVoiceOver|Boolescher Wert|Gibt ab, ob Hintergrundkommentare im Kiosk-Modus erforderlich sind.|
|kioskModeRequireZoom|Boolescher Wert|Gibt ab, ob Zoom im Kiosk-Modus erforderlich ist.|
|kioskModeManagedAppId|Zeichenfolge|Verwaltete App-ID der App, die für den Kiosk-Modus verwendet werden soll. Wenn „KioskModeManagedAppId“ angegeben ist, wird „KioskModeAppStoreUrl“ ignoriert.|
|lockScreenBlockControlCenter|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer das Kontrollzentrum für den Sperrbildschirm verwendet.|
|lockScreenBlockNotificationView|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer die Benachrichtigungsansicht auf dem Sperrbildschirm verwendet.|
|lockScreenBlockPassbook|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Passbook verwendet, wenn das Gerät gesperrt ist.|
|lockScreenBlockTodayView|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer die Ansicht „Heute“ für den Sperrbildschirm verwendet.|
|mediaContentRatingAustralia|[mediaContentRatingAustralia](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|Einstellungen für Medieninhalte für Australien|
|mediaContentRatingCanada|[mediaContentRatingCanada](../resources/intune_deviceconfig_mediacontentratingcanada.md)|Einstellungen für Medieninhalte für Kanada|
|mediaContentRatingFrance|[mediaContentRatingFrance](../resources/intune_deviceconfig_mediacontentratingfrance.md)|Einstellungen für Medieninhalte für Frankreich|
|mediaContentRatingGermany|[mediaContentRatingGermany](../resources/intune_deviceconfig_mediacontentratinggermany.md)|Einstellungen für Medieninhalte für Deutschland|
|mediaContentRatingIreland|[mediaContentRatingIreland](../resources/intune_deviceconfig_mediacontentratingireland.md)|Einstellungen für Medieninhalte für Irland|
|mediaContentRatingJapan|[mediaContentRatingJapan](../resources/intune_deviceconfig_mediacontentratingjapan.md)|Einstellungen für Medieninhalte für Japan|
|mediaContentRatingNewZealand|[mediaContentRatingNewZealand](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|Einstellungen für Medieninhalte für Neuseeland|
|mediaContentRatingUnitedKingdom|[mediaContentRatingUnitedKingdom](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|Einstellungen für Medieninhalte für das Vereinigte Königreich|
|mediaContentRatingUnitedStates|[mediaContentRatingUnitedStates](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|Einstellungen für Medieninhalte für die USA|
|networkUsageRules|[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md)-Sammlung|Liste verwalteter Apps und die Netzwerkregeln, die darauf angewendet werden. Diese Sammlung kann bis zu 1000 Elemente enthalten.|
|mediaContentRatingApps|Zeichenfolge|Bewertungseinstellungen für Medieninhalte für Apps. Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.|
|messagesBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer die Nachrichten-App auf dem überwachten Gerät verwendet.|
|notificationsBlockSettingsModification|Boolescher Wert|Gibt an, ob die Änderung von Benachrichtigungseinstellungen zugelassen wird (iOS 9.3 und höher).|
|passcodeBlockFingerprintUnlock|Boolescher Wert|Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.|
|passcodeBlockFingerprintModification|Boolescher Wert|Blockiert das Ändern registrierter Touch ID-Fingerabdrücke im überwachten Modus.|
|passcodeBlockModification|Boolescher Wert|Gibt an, ob das Ändern der Kennung auf dem überwachten Gerät (iOS 9.0 und höher) zulässig ist.|
|passcodeBlockSimple|Boolescher Wert|Gibt an, ob einfache Kennungen erlaubt sind.|
|passcodeExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen der Kennung. Gültige Werte: 1 bis 65535.|
|passcodeMinimumLength|Int32|Mindestlänge von Kennungen. Gültige Werte: 4 bis 14.|
|passcodeMinutesOfInactivityBeforeLock|Int32|Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.|
|passcodeMinimumCharacterSetCount|Int32|Anzahl von Zeichensätzen, die eine Kennung enthalten muss Gültige Werte: 0 bis 4.|
|passcodePreviousPasscodeBlockCount|Int32|Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen. Gültige Werte: 1 bis 24.|
|passcodeSignInFailureCountBeforeWipe|Int32|Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung des Geräts durchgeführt wird. Gültige Werte: 4 bis 11.|
|passcodeRequiredType|Zeichenfolge|Geforderter Kennungstyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric`, `numeric`.|
|passcodeRequired|Boolescher Wert|Gibt an, ob eine Kennung erforderlich ist.|
|podcastsBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Podcasts auf dem überwachten Gerät verwendet (iOS 8.0 und höher).|
|safariBlockAutofill|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer AutoAusfüllen in Safari verwendet.|
|safariBlockJavaScript|Boolescher Wert|Gibt an, ob JavaScript in Safari blockiert werden soll.|
|safariBlockPopups|Boolescher Wert|Gibt an, ob Popups in Safari blockiert werden sollen.|
|safariBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Safari verwendet.|
|safariCookieSettings|Zeichenfolge|Cokkieeinstellungen für Safari. Mögliche Werte: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|safariManagedDomains|Zeichenfolgenauflistung|URLs, die mit den hier aufgeführten Mustern übereinstimmen, werden als verwaltet betrachtet.|
|safariPasswordAutoFillDomains|Zeichenfolgenauflistung|Benutzer können Kennwörter in Safari nur von URLs speichern, die mit den hier aufgeführten Mustern übereinstimmen. Gilt für Geräte im überwachten Modus (iOS 9.3 und höher).|
|safariRequireFraudWarning|Boolescher Wert|Gibt an, ob eine Betrugswarnung in Safari erforderlich ist.|
|screenCaptureBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Screenshots macht.|
|siriBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Siri verwendet.|
|siriBlockedWhenLocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Siri bei Sperrung verwendet.|
|siriBlockUserGeneratedContent|Boolescher Wert|Gibt an, ob Siri bei Verwendung auf einem überwachten Gerät davon abgehalten werden soll, benutzergenerierte Inhalte abzufragen.|
|siriRequireProfanityFilter|Boolescher Wert|Gibt an, ob verhindert werden soll, dass Siri anstößige Ausdrücke auf dem überwachten Gerät diktiert oder spricht.|
|spotlightBlockInternetResults|Boolescher Wert|Gibt an, ob verhindert werden soll, dass die Spotlight-Suche Internetergebnisse auf dem überwachten Gerät zurückgibt.|
|voiceDialingBlocked|Boolescher Wert|Gibt an, ob das Sprachwahlverfahren blockiert werden soll.|
|wallpaperBlockModification|Boolescher Wert|Gibt an, ob das Ändern des Hintergrunds auf einem überwachten Gerät (iOS 9.0 und höher) zulässig ist.|
|wiFiConnectOnlyToConfiguredNetworks|Boolescher Wert|Gibt an, ob erzwungen werden soll, dass das Gerät nur WLAN-Netzwerke aus Konfigurationsprofilen verwendet, wenn sich das Gerät im überwachten Modus befindet.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|Zuweisungen|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsVisibilityListType": "String",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "String"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "String",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "String",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "String",
    "tvRating": "String"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "String",
          "publisher": "String",
          "appStoreUrl": "String",
          "appId": "String"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "String",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 1024,
  "passcodeMinimumLength": 1024,
  "passcodeMinutesOfInactivityBeforeLock": 1024,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passcodeMinimumCharacterSetCount": 1024,
  "passcodePreviousPasscodeBlockCount": 1024,
  "passcodeSignInFailureCountBeforeWipe": 1024,
  "passcodeRequiredType": "String",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "String",
  "safariManagedDomains": [
    "String"
  ],
  "safariPasswordAutoFillDomains": [
    "String"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```



