---
title: iosGeneralDeviceConfiguration-Ressourcentyp
description: In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „ iosGeneralDeviceConfiguration“ verfügbar gemacht werden.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 055abce38989d5d49f1f009ac38b6a5aac548ac2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410889"
---
# <a name="iosgeneraldeviceconfiguration-resource-type"></a>iosGeneralDeviceConfiguration-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „ iosGeneralDeviceConfiguration“ verfügbar gemacht werden.


Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[iosGeneralDeviceConfigurations auflisten](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-list.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)-Sammlung|Listet die Eigenschaften und Beziehungen der [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)-Objekte auf.|
|[iosGeneralDeviceConfiguration abrufen](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-get.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)|Liest die Eigenschaften und Beziehungen des [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)-Objekts.|
|[iosGeneralDeviceConfiguration erstellen](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-create.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)|Erstellen Sie ein neues [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)-Objekt.|
|[iosGeneralDeviceConfiguration löschen](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-delete.md)|Keine|Löscht eine [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)|
|[iosGeneralDeviceConfiguration aktualisieren](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-update.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)|Aktualisiert die Eigenschaften eines [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Zeichenfolgenauflistung|Liste der Bereich Tags für diese Instanz der Entität. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt. Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden. Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|accountBlockModification|Boolean|Gibt an, ob die Kontoänderung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.|
|activationLockAllowWhenSupervised|Boolean|Gibt an, ob die Aktivierungssperre zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.|
|airDropBlocked|Boolean|Gibt an, ob AirDrop zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.|
|airDropForceUnmanagedDropTarget|Boolean|Gibt an, ob AirDrop als nicht verwaltetes Drop-Ziel (iOS 9.0 oder höher) betrachtet werden soll.|
|airPlayForcePairingPasswordForOutgoingRequests|Boolean|Gibt an, ob erzwungen werden soll, dass alle Geräte, die AirPlay-Anforderungen von diesem Gerät erhalten, ein Kopplungskennwort verwenden.|
|appleWatchBlockPairing|Boolean|Gibt an, ob eine Apple Watch-Kopplung zulässig ist, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).|
|appleWatchForceWristDetection|Boolean|Gibt an, ob erzwungen werden soll, dass eine gekoppelte Apple Watch die Handgelenkerkennung (iOS 8.2 und höher) verwendet.|
|appleNewsBlocked|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer News verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).|
|appsSingleAppModeList|[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung|Ruft die Liste von iOS-Apps ab, die autonom in den Einzelanwendungsmodus wechseln können, ab oder legt diese fest. Nur überwacht. iOS 7.0 oder höher. Diese Sammlung darf maximal 500 Elemente enthalten.|
|appsVisibilityList|[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung|Liste von Apps in der Sichtbarkeitsliste (entweder eine Liste sichtbarer/startbarer Apps oder eine Liste ausgeblendeter/nicht startbarer Apps, gesteuert von AppsVisibilityListType) (iOS 9.3 und höher). Diese Sammlung darf maximal 10.000 Elemente enthalten.|
|appsVisibilityListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Typ der in „AppsVisibilityList“ enthaltenen Liste. Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|appStoreBlockAutomaticDownloads|Boolean|Gibt an, ob das automatische Herunterladen von Apps blockiert werden soll, die auf anderen Geräten gekauft wurden, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).|
|appStoreBlocked|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer den App Store verwendet.|
|appStoreBlockInAppPurchases|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer In-App-Käufe tätigt.|
|appStoreBlockUIAppInstallation|Boolean|Gibt an, ob die App Store-App blockiert werden soll, ohne die Installation über Host-Apps einzuschränken. Gilt nur für den überwachten Modus (iOS 9.0 und höher).|
|appStoreRequirePassword|Boolean|Gibt an, ob bei Verwendung des App Stores ein Kennwort erforderlich ist.|
|bluetoothBlockModification|Boolean|Gibt an, ob das Ändern von Bluetooth-Einstellungen zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 10.0 und höher).|
|cameraBlocked|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.|
|cellularBlockDataRoaming|Boolean|Gibt an, ob Datenroaming blockiert werden soll.|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Boolean|Gibt an, ob das globales Abrufen im Hintergrund beim Roaming blockiert werden soll.|
|cellularBlockPerAppDataModification|Boolean|Gibt an, ob Änderungen an den Mobil-App-Daten zulässig sind, wenn sich das Gerät im überwachten Modus befindet.|
|cellularBlockPersonalHotspot|Boolean|Gibt an, ob der privater Hotspot blockiert werden soll.|
|cellularBlockVoiceRoaming|Boolean|Gibt an, ob Sprachroaming blockiert werden soll.|
|certificatesBlockUntrustedTlsCertificates|Boolean|Gibt an, ob nicht vertrauenswürdige TLS-Zertifikate blockiert werden sollen.|
|classroomAppBlockRemoteScreenObservation|Boolean|Gibt an, ob die Remotebildschirmüberwachung über die Classroom-App zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).|
|classroomAppForceUnpromptedScreenObservation|Boolean|Gibt an, ob dem Lehrer eines verwalteten Kurses in der Classroom-App automatisch die Berechtigung erteilt werden soll, den Bildschirm eines Kursteilnehmers ohne Aufforderung anzuzeigen, wenn sich das Gerät im überwachten Modus befindet.|
|compliantAppsList|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“). Diese Collection darf maximal 10.000 Elemente enthalten.|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Typ der in „compliantAppsList“ definierten Liste. Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|configurationProfileBlockChanges|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer Konfigurationsprofile und Zertifikate interaktiv installiert, wenn sich das Gerät im überwachten Modus befindet.|
|definitionLookupBlocked|Boolean|Gibt an, ob die Definitionssuche zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).|
|deviceBlockEnableRestrictions|Boolean|Gibt an, ob erlaubt werden soll, dass der Benutzer Einschränkungen in den Geräteeinstellungen aktiviert, wenn sich das Gerät im überwachten Modus befindet.|
|deviceBlockEraseContentAndSettings|Boolean|Gibt an, ob die Verwendung der Option zum Löschen aller Inhalte und Einstellungen auf dem Gerät zugelassen werden soll, wenn sich das Gerät im überwachten Modus befindet.|
|deviceBlockNameModification|Boolean|Gibt an, ob das Ändern des Gerätenamens zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).|
|diagnosticDataBlockSubmission|Boolean|Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.|
|diagnosticDataBlockSubmissionModification|Boolean|Gibt an, ob das Ändern der Einstellungen für die Diagnoseübermittlung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3.2 und höher).|
|documentsBlockManagedDocumentsInUnmanagedApps|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer verwaltete Dokumente in nicht verwalteten Apps anzeigt.|
|documentsBlockUnmanagedDocumentsInManagedApps|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer nicht verwaltete Dokumente in verwalteten Apps anzeigt.|
|emailInDomainSuffixes|Zeichenfolgenauflistung|E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.|
|enterpriseAppBlockTrust|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer einer Unternehmens-App vertraut.|
|enterpriseAppBlockTrustModification|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer die Vertrauensstellungseinstellungen der Unternehmens-App ändert.|
|faceTimeBlocked|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer FaceTime verwendet.|
|findMyFriendsBlocked|Boolean|Gibt an, ob „Freunde suchen“ blockiert wird, wenn sich das Gerät im überwachten Modus befindet.|
|gamingBlockGameCenterFriends|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer Freunde im Game Center hat.|
|gamingBlockMultiplayer|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer Multiplayerspiele verwendet.|
|gameCenterBlocked|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer Game Center verwendet, wenn sich das Gerät im überwachten Modus befindet.|
|hostPairingBlocked|Boolean|Gibt an, ob die Hostkopplung blockiert werden soll, um zu steuern, mit welchen Geräten ein iOS-Gerät gekoppelt werden kann,wenn sich das iOS-Gerät im überwachten Modus befindet.|
|iBooksStoreBlocked|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer den iBooks Store verwendet, wenn sich das Gerät im überwachten Modus befindet.|
|iBooksStoreBlockErotica|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer Medien aus dem iBook Store herunterlädt, die als Erotik gekennzeichnet sind.|
|iCloudBlockActivityContinuation|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer eine Aufgabe, die er auf dem iOS-Gerät begonnen hat, auf einem anderen iOS- oder macOS-Gerät fortsetzt.|
|iCloudBlockBackup|Boolean|Gibt an, ob die iCloud-Sicherung blockiert werden soll.|
|iCloudBlockDocumentSync|Boolean|Gibt an, ob die iCloud-Dokumentsynchronisierung blockiert werden soll.|
|iCloudBlockManagedAppsSync|Boolean|Gibt an, ob die Cloudsynchronisierung für verwaltete Apps blockiert werden soll.|
|iCloudBlockPhotoLibrary|Boolean|Gibt an, ob die iCloud-Fotomediathek blockiert werden soll.|
|iCloudBlockPhotoStreamSync|Boolean|Gibt an, ob die Fotostream-Synchronisierung in iCloud blockiert werden soll.|
|iCloudBlockSharedPhotoStream|Boolean|Gibt an, ob die Fotofreigabe blockiert werden soll.|
|iCloudRequireEncryptedBackup|Boolean|Gibt an, ob Sicherungen in iCloud verschlüsselt sein müssen.|
|iTunesBlockExplicitContent|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer auf anstößige Inhalte in iTunes und im App Store zugreift. |
|iTunesBlockMusicService|Boolean|Gibt an, ob der Music-Dienst blockiert und die Music-App in den klassischen Modus zurückgesetzt werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher und Mac OS 10.12 und höher).|
|iTunesBlockRadio|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer iTunes Radio verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).|
|keyboardBlockAutoCorrect|Boolean|Gibt an, ob die Autokorrektur der Tastatur blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).|
|keyboardBlockDictation|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer die Diktatfunktion verwendet, wenn sich das Gerät im überwachten Modus befindet.|
|keyboardBlockPredictive|Boolean|Gibt an, ob Tastaturwortvorschläge blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).|
|keyboardBlockShortcuts|Boolean|Gibt an, ob Tastenkombinationen blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).|
|keyboardBlockSpellCheck|Boolean|Gibt an, ob die Rechtschreibprüfung blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).|
|kioskModeAllowAssistiveSpeak|Boolean|Gibt an, ob Sprachunterstützung im Kiosk-Modus zulässig ist.|
|kioskModeAllowAssistiveTouchSettings|Boolean|Gibt an, ob Zugriff auf die Einstellungen der Touch-Unterstützung im Kiosk-Modus gewährt werden soll.|
|kioskModeAllowAutoLock|Boolean|Gibt an, ob die automatische Gerätesperre im Kiosk-Modus zulässig ist.|
|kioskModeAllowColorInversionSettings|Boolean|Gibt ab, ob der Zugriff auf die Farbinversionseinstellungen im Kiosk-Modus erlaubt werden soll.|
|kioskModeAllowRingerSwitch|Boolean|Gibt ab, ob die Verwendung des Ruftonschalters im Kiosk-Modus erlaubt werden soll.|
|kioskModeAllowScreenRotation|Boolean|Gibt ab, ob die Bildschirmdrehung im Kiosk-Modus erlaubt werden soll.|
|kioskModeAllowSleepButton|Boolean|Gibt ab, ob die Verwendung der Energiespartaste im Kiosk-Modus erlaubt werden soll.|
|kioskModeAllowTouchscreen|Boolean|Gibt ab, ob die Verwendung des Touchscreens im Kiosk-Modus erlaubt werden soll.|
|kioskModeAllowVoiceOverSettings|Boolean|Gibt ab, ob der Zugriff auf die Einstellungen für Hintergrundkommentare im Kiosk-Modus erlaubt werden soll.|
|kioskModeAllowVolumeButtons|Boolean|Gibt ab, ob die Verwendung der Lautstärketasten im Kiosk-Modus erlaubt werden soll.|
|kioskModeBlockVolumeButtons|Boolean|Gibt an, ob die Lautstärkeregler im Kioskmodus blockiert werden sollen.|
|kioskModeAllowZoomSettings|Boolean|Gibt ab, ob der Zugriff auf die Zoomeinstellungen im Kiosk-Modus erlaubt werden soll.|
|kioskModeAppStoreUrl|Zeichenfolge|URL im App Store zu der App, die für den Kiosk-Modus verwendet werden soll. Verwenden Sie diese, wenn „KioskModeManagedAppId“ nicht bekannt ist.|
|kioskModeBuiltInAppId|Zeichenfolge|ID für integrierte apps im Kioskmodus verwenden. Verwendet, wenn KioskModeManagedAppId und KioskModeAppStoreUrl nicht festgelegt werden.|
|kioskModeRequireAssistiveTouch|Boolean|Gibt an, ob Touch-Unterstützung im Kiosk-Modus erforderlich ist.|
|kioskModeRequireColorInversion|Boolean|Gibt ab, ob die Farbinversion im Kiosk-Modus erforderlich ist.|
|kioskModeRequireMonoAudio|Boolean|Gibt ab, ob Mono-Audio im Kiosk-Modus erforderlich ist.|
|kioskModeRequireVoiceOver|Boolean|Gibt ab, ob Hintergrundkommentare im Kiosk-Modus erforderlich sind.|
|kioskModeRequireZoom|Boolean|Gibt ab, ob Zoom im Kiosk-Modus erforderlich ist.|
|kioskModeManagedAppId|Zeichenfolge|Verwaltete App-ID der App, die für den Kiosk-Modus verwendet werden soll. Wenn „KioskModeManagedAppId“ angegeben ist, wird „KioskModeAppStoreUrl“ ignoriert.|
|lockScreenBlockControlCenter|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer das Kontrollzentrum für den Sperrbildschirm verwendet.|
|lockScreenBlockNotificationView|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer die Benachrichtigungsansicht auf dem Sperrbildschirm verwendet.|
|lockScreenBlockPassbook|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer Passbook verwendet, wenn das Gerät gesperrt ist.|
|lockScreenBlockTodayView|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer die Ansicht „Heute“ für den Sperrbildschirm verwendet.|
|mediaContentRatingAustralia|[mediaContentRatingAustralia](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|Einstellungen für Medieninhalte für Australien|
|mediaContentRatingCanada|[mediaContentRatingCanada](../resources/intune-deviceconfig-mediacontentratingcanada.md)|Einstellungen für Medieninhalte für Kanada|
|mediaContentRatingFrance|[mediaContentRatingFrance](../resources/intune-deviceconfig-mediacontentratingfrance.md)|Einstellungen für Medieninhalte für Frankreich|
|mediaContentRatingGermany|[mediaContentRatingGermany](../resources/intune-deviceconfig-mediacontentratinggermany.md)|Einstellungen für Medieninhalte für Deutschland|
|mediaContentRatingIreland|[mediaContentRatingIreland](../resources/intune-deviceconfig-mediacontentratingireland.md)|Einstellungen für Medieninhalte für Irland|
|mediaContentRatingJapan|[mediaContentRatingJapan](../resources/intune-deviceconfig-mediacontentratingjapan.md)|Einstellungen für Medieninhalte für Japan|
|mediaContentRatingNewZealand|[mediaContentRatingNewZealand](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|Einstellungen für Medieninhalte für Neuseeland|
|mediaContentRatingUnitedKingdom|[mediaContentRatingUnitedKingdom](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|Einstellungen für Medieninhalte für das Vereinigte Königreich|
|mediaContentRatingUnitedStates|[mediaContentRatingUnitedStates](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|Einstellungen für Medieninhalte für die USA|
|networkUsageRules|[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)-Sammlung|Liste verwalteter Apps und die Netzwerkregeln, die darauf angewendet werden. Diese Sammlung kann bis zu 1000 Elemente enthalten.|
|mediaContentRatingApps|[ratingAppsType](../resources/intune-deviceconfig-ratingappstype.md)|Media content Bewertung Einstellungen für Apps. Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12` und `agesAbove17`.|
|messagesBlocked|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer die Nachrichten-App auf dem überwachten Gerät verwendet.|
|notificationsBlockSettingsModification|Boolean|Gibt an, ob die Änderung von Benachrichtigungseinstellungen zugelassen wird (iOS 9.3 und höher).|
|passcodeBlockFingerprintUnlock|Boolean|Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.|
|passcodeBlockFingerprintModification|Boolean|Blockiert das Ändern registrierter Touch ID-Fingerabdrücke im überwachten Modus.|
|passcodeBlockModification|Boolean|Gibt an, ob das Ändern der Kennung auf dem überwachten Gerät (iOS 9.0 und höher) zulässig ist.|
|passcodeBlockSimple|Boolean|Gibt an, ob einfache Kennungen erlaubt sind.|
|passcodeExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen der Kennung. Gültige Werte: 1 bis 65535.|
|passcodeMinimumLength|Int32|Mindestlänge von Kennungen. Gültige Werte: 4 bis 14.|
|passcodeMinutesOfInactivityBeforeLock|Int32|Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.|
|passcodeMinimumCharacterSetCount|Int32|Anzahl von Zeichensätzen, die eine Kennung enthalten muss Gültige Werte: 0 bis 4.|
|passcodePreviousPasscodeBlockCount|Int32|Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen. Gültige Werte: 1 bis 24.|
|passcodeSignInFailureCountBeforeWipe|Int32|Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung des Geräts durchgeführt wird. Gültige Werte: 4 bis 11.|
|passcodeRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Geforderter Kennungstyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric`, `numeric`.|
|passcodeRequired|Boolean|Gibt an, ob eine Kennung erforderlich ist.|
|podcastsBlocked|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer Podcasts auf dem überwachten Gerät verwendet (iOS 8.0 und höher).|
|safariBlockAutofill|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer AutoAusfüllen in Safari verwendet.|
|safariBlockJavaScript|Boolean|Gibt an, ob JavaScript in Safari blockiert werden soll.|
|safariBlockPopups|Boolean|Gibt an, ob Popups in Safari blockiert werden sollen.|
|safariBlocked|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer Safari verwendet.|
|safariCookieSettings|[webBrowserCookieSettings](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|Cokkieeinstellungen für Safari. Mögliche Werte: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|safariManagedDomains|Zeichenfolgenauflistung|URLs, die mit den hier aufgeführten Mustern übereinstimmen, werden als verwaltet betrachtet.|
|safariPasswordAutoFillDomains|Zeichenfolgenauflistung|Benutzer können Kennwörter in Safari nur von URLs speichern, die mit den hier aufgeführten Mustern übereinstimmen. Gilt für Geräte im überwachten Modus (iOS 9.3 und höher).|
|safariRequireFraudWarning|Boolean|Gibt an, ob eine Betrugswarnung in Safari erforderlich ist.|
|screenCaptureBlocked|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer Screenshots macht.|
|siriBlocked|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer Siri verwendet.|
|siriBlockedWhenLocked|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer Siri bei Sperrung verwendet.|
|siriBlockUserGeneratedContent|Boolean|Gibt an, ob Siri bei Verwendung auf einem überwachten Gerät davon abgehalten werden soll, benutzergenerierte Inhalte abzufragen.|
|siriRequireProfanityFilter|Boolean|Gibt an, ob verhindert werden soll, dass Siri anstößige Ausdrücke auf dem überwachten Gerät diktiert oder spricht.|
|spotlightBlockInternetResults|Boolean|Gibt an, ob verhindert werden soll, dass die Spotlight-Suche Internetergebnisse auf dem überwachten Gerät zurückgibt.|
|voiceDialingBlocked|Boolean|Gibt an, ob das Sprachwahlverfahren blockiert werden soll.|
|wallpaperBlockModification|Boolean|Gibt an, ob das Ändern des Hintergrunds auf einem überwachten Gerät (iOS 9.0 und höher) zulässig ist.|
|wiFiConnectOnlyToConfiguredNetworks|Boolean|Gibt an, ob erzwungen werden soll, dass das Gerät nur WLAN-Netzwerke aus Konfigurationsprofilen verwendet, wenn sich das Gerät im überwachten Modus befindet.|
|classroomForceRequestPermissionToLeaveClasses|Boolean|Gibt an, ob in einer nicht verwalteten Kurs über vor Ort registriert Student Berechtigung aus der Schulungsleiter anfordern soll, bei dem Versuch, lassen Sie den Kurs (iOS 11.3 und höher).|
|keychainBlockCloudSync|Boolean|Gibt an, ob iCloud Schlüsselsammlung Synchronisierung ausgeschlossen wird.|
|pkiBlockOTAUpdates|Boolean|Gibt an, ob over-the PKI-Updates blockiert sind. Wenn Sie diese Einschränkung deaktivieren false nicht Zertifikatsperrlisten und OCSP-Prüfungen (iOS 7.0 und höher) festlegen.|
|privacyForceLimitAdTracking|Boolean|Gibt an, ob Ad nachverfolgen beschränkt ist. (iOS 7.0 und höher).|
|enterpriseBookBlockBackup|Boolean|Gibt an, dass unabhängig davon, ob Enterprise zum Sichern von Buch ausgeschlossen werden.|
|enterpriseBookBlockMetadataSync|Boolean|Gibt an, ob Enterprise Adressbuch Notizen und highlights zur Synchronisierung ausgeschlossen wird.|
|airPrintBlocked|Boolean|Gibt an, ob AirPrint blockierte (iOS 11.0 und höher) ist.|
|airPrintBlockCredentialsStorage|Boolean|Gibt an, ob Schlüsselsammlung Speicherung von Benutzername und Kennwort für Airprint blockierte (iOS 11.0 und höher) ist.|
|airPrintForceTrustedTLS|Boolean|Gibt an, ob vertrauenswürdige Zertifikate für Drucken TLS-Kommunikation (iOS 11.0 und höher) erforderlich sind.|
|airPrintBlockiBeaconDiscovery|Boolean|Gibt an, ob iBeacon Ermittlung von AirPrint Drucker ausgeschlossen wird. Dies verhindert, dass falsche AirPrint Bluetooth Beacons vor Phishing für den Netzwerkdatenverkehr (iOS 11.0 und höher).|
|blockSystemAppRemoval|Boolean|Gibt an, ob das Entfernen der System apps aus dem Gerät auf einem überwachten Gerät (iOS 11.0 und höher) ausgeschlossen wird.|
|vpnBlockCreation|Boolean|Gibt an, ob die Erstellung des VPN-Konfigurationen blockierte (iOS 11.0 und höher) ist.|
|appRemovalBlocked|Boolean|Gibt an, ob das Entfernen von apps zulässig ist.|
|usbRestrictedModeBlocked|Boolean|Gibt an, ob das Herstellen einer Verbindung mit USB-Zubehör, während das Gerät gesperrt ist zulässig ist (iOS 11.4.1 und höher).|
|passwordBlockAutoFill|Boolean|Gibt an, ob das Feature der AutoFill-Kennwörter (iOS 12.0 und höher) zulässig ist.|
|passwordBlockProximityRequests|Boolean|Gibt an, ob anfordernde Kennwörter von benachbarten Geräten (iOS 12.0 oder höher) blockieren.|
|passwordBlockAirDropSharing|Boolean|Gibt an, ob blockierende sharing Kennwörter mit AirDrop Kennwörter Feature iOS 12.0 oder höher).|
|dateAndTimeForceSetAutomatically|Boolean|Gibt an, ob Datum und Uhrzeit "Festlegen automatisch" Feature aktiviert ist und nicht durch den Benutzer (iOS 12.0 oder höher) deaktiviert.|
|contactsAllowManagedToUnmanagedWrite|Boolean|Gibt an, ob verwaltet, dass apps Kontakte auf Kontakte nicht verwalteten Konten (iOS 12.0 oder höher) schreiben können.|
|contactsAllowUnmanagedToManagedRead|Boolean|Gibt an, ob nicht verwaltete apps Kontakte verwalteten Konten (iOS 12.0 oder höher) lesen können.|

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
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
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
  "kioskModeBlockVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "String",
  "kioskModeBuiltInAppId": "String",
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
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true
}
```




