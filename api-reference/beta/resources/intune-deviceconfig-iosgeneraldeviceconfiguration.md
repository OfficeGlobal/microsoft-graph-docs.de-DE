---
title: iosGeneralDeviceConfiguration-Ressourcentyp
description: In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „ iosGeneralDeviceConfiguration“ verfügbar gemacht werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01ea145e90b2595035bbb49d02d14c285750e612
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175353"
---
# <a name="iosgeneraldeviceconfiguration-resource-type"></a>iosGeneralDeviceConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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
|id|string|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolescher Wert|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|accountBlockModification|Boolescher Wert|Gibt an, ob die Kontoänderung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.|
|activationLockAllowWhenSupervised|Boolescher Wert|Gibt an, ob die Aktivierungssperre zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.|
|airDropBlocked|Boolescher Wert|Gibt an, ob AirDrop zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.|
|airDropForceUnmanagedDropTarget|Boolescher Wert|Gibt an, ob AirDrop als nicht verwaltetes Drop-Ziel (iOS 9.0 oder höher) betrachtet werden soll.|
|airPlayForcePairingPasswordForOutgoingRequests|Boolescher Wert|Gibt an, ob erzwungen werden soll, dass alle Geräte, die AirPlay-Anforderungen von diesem Gerät erhalten, ein Kopplungskennwort verwenden.|
|appleWatchBlockPairing|Boolescher Wert|Gibt an, ob eine Apple Watch-Kopplung zulässig ist, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).|
|appleWatchForceWristDetection|Boolescher Wert|Gibt an, ob erzwungen werden soll, dass eine gekoppelte Apple Watch die Handgelenkerkennung (iOS 8.2 und höher) verwendet.|
|appleNewsBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer News verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).|
|appsSingleAppModeList|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Ruft die Liste von iOS-Apps ab, die autonom in den Einzelanwendungsmodus wechseln können, ab oder legt diese fest. Nur überwacht. iOS 7.0 oder höher. Diese Sammlung darf maximal 500 Elemente enthalten.|
|appsVisibilityList|[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung|Liste von Apps in der Sichtbarkeitsliste (entweder eine Liste sichtbarer/startbarer Apps oder eine Liste ausgeblendeter/nicht startbarer Apps, gesteuert von AppsVisibilityListType) (iOS 9.3 und höher). Diese Sammlung darf maximal 10.000 Elemente enthalten.|
|appsVisibilityListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Typ der in „AppsVisibilityList“ enthaltenen Liste. Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.|
|appStoreBlockAutomaticDownloads|Boolescher Wert|Gibt an, ob das automatische Herunterladen von Apps blockiert werden soll, die auf anderen Geräten gekauft wurden, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).|
|appStoreBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer den App Store verwendet.|
|appStoreBlockInAppPurchases|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer In-App-Käufe tätigt.|
|appStoreBlockUIAppInstallation|Boolescher Wert|Gibt an, ob die App Store-App blockiert werden soll, ohne die Installation über Host-Apps einzuschränken. Gilt nur für den überwachten Modus (iOS 9.0 und höher).|
|appStoreRequirePassword|Boolescher Wert|Gibt an, ob bei Verwendung des App Stores ein Kennwort erforderlich ist.|
|autoFillForceAuthentication|Boolescher Wert|Gibt an, ob die Benutzerauthentifizierung erzwungen werden soll, bevor Kennwörter und Kreditkarteninformationen in Safari und anderen apps auf überwachten Geräten automatisch gefüllt werden.|
|bluetoothBlockModification|Boolescher Wert|Gibt an, ob das Ändern von Bluetooth-Einstellungen zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 10.0 und höher).|
|cameraBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.|
|cellularBlockDataRoaming|Boolescher Wert|Gibt an, ob Datenroaming blockiert werden soll.|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Boolescher Wert|Gibt an, ob das globales Abrufen im Hintergrund beim Roaming blockiert werden soll.|
|cellularBlockPerAppDataModification|Boolescher Wert|Gibt an, ob Änderungen an den Mobil-App-Daten zulässig sind, wenn sich das Gerät im überwachten Modus befindet.|
|cellularBlockPersonalHotspot|Boolescher Wert|Gibt an, ob der privater Hotspot blockiert werden soll.|
|cellularBlockPlanModification|Boolescher Wert|Gibt an, ob Benutzer die Einstellungen des Mobil Funk Plans auf einem überwachten Gerät ändern dürfen.|
|cellularBlockVoiceRoaming|Boolescher Wert|Gibt an, ob Sprachroaming blockiert werden soll.|
|certificatesBlockUntrustedTlsCertificates|Boolescher Wert|Gibt an, ob nicht vertrauenswürdige TLS-Zertifikate blockiert werden sollen.|
|classroomAppBlockRemoteScreenObservation|Boolescher Wert|Gibt an, ob die Remotebildschirmüberwachung über die Classroom-App zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).|
|classroomAppForceUnpromptedScreenObservation|Boolescher Wert|Gibt an, ob dem Lehrer eines verwalteten Kurses in der Classroom-App automatisch die Berechtigung erteilt werden soll, den Bildschirm eines Kursteilnehmers ohne Aufforderung anzuzeigen, wenn sich das Gerät im überwachten Modus befindet.|
|classroomForceAutomaticallyJoinClasses|Boolescher Wert|Gibt an, ob die Berechtigung für die Anforderungen des Lehrers automatisch erteilt werden soll, ohne dass der Kursteilnehmer dazu aufgefordert wird, wenn sich das Gerät im überwachten Modus befindet.|
|classroomForceUnpromptedAppAndDeviceLock|Boolescher Wert|Gibt an, ob die Lehrerin Apps oder das Gerät Sperren soll, ohne dass der Kursteilnehmer dazu aufgefordert wird. Nur überwacht.|
|compliantAppsList|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“). Diese Collection darf maximal 10.000 Elemente enthalten.|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Typ der in „compliantAppsList“ definierten Liste. Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|configurationProfileBlockChanges|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Konfigurationsprofile und Zertifikate interaktiv installiert, wenn sich das Gerät im überwachten Modus befindet.|
|definitionLookupBlocked|Boolescher Wert|Gibt an, ob die Definitionssuche zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).|
|deviceBlockEnableRestrictions|Boolescher Wert|Gibt an, ob erlaubt werden soll, dass der Benutzer Einschränkungen in den Geräteeinstellungen aktiviert, wenn sich das Gerät im überwachten Modus befindet.|
|deviceBlockEraseContentAndSettings|Boolescher Wert|Gibt an, ob die Verwendung der Option zum Löschen aller Inhalte und Einstellungen auf dem Gerät zugelassen werden soll, wenn sich das Gerät im überwachten Modus befindet.|
|deviceBlockNameModification|Boolescher Wert|Gibt an, ob das Ändern des Gerätenamens zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).|
|diagnosticDataBlockSubmission|Boolean|Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.|
|diagnosticDataBlockSubmissionModification|Boolescher Wert|Gibt an, ob das Ändern der Einstellungen für die Diagnoseübermittlung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3.2 und höher).|
|documentsBlockManagedDocumentsInUnmanagedApps|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer verwaltete Dokumente in nicht verwalteten Apps anzeigt.|
|documentsBlockUnmanagedDocumentsInManagedApps|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer nicht verwaltete Dokumente in verwalteten Apps anzeigt.|
|emailInDomainSuffixes|String collection|E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.|
|enterpriseAppBlockTrust|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer einer Unternehmens-App vertraut.|
|enterpriseAppBlockTrustModification|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer die Vertrauensstellungseinstellungen der Unternehmens-App ändert.|
|esimBlockModification|Boolescher Wert|Gibt an, ob das Hinzufügen oder Entfernen von Zellen Plänen auf dem eSIM eines überwachten Geräts zugelassen werden soll.|
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
|kioskModeBlockVolumeButtons|Boolean|Gibt an, ob die Lautstärkeregler im Kioskmodus blockiert werden sollen.|
|kioskModeAllowZoomSettings|Boolescher Wert|Gibt ab, ob der Zugriff auf die Zoomeinstellungen im Kiosk-Modus erlaubt werden soll.|
|kioskModeAppStoreUrl|Zeichenfolge|URL im App Store zu der App, die für den Kiosk-Modus verwendet werden soll. Verwenden Sie diese, wenn „KioskModeManagedAppId“ nicht bekannt ist.|
|kioskModeBuiltInAppId|Zeichenfolge|ID für integrierte apps, die für den Kiosk-Modus verwendet werden sollen. Wird verwendet, wenn "Kioskmodemanagedappid" und KioskModeAppStoreUrl nicht festgelegt sind.|
|kioskModeRequireAssistiveTouch|Boolescher Wert|Gibt an, ob Touch-Unterstützung im Kiosk-Modus erforderlich ist.|
|kioskModeRequireColorInversion|Boolescher Wert|Gibt ab, ob die Farbinversion im Kiosk-Modus erforderlich ist.|
|kioskModeRequireMonoAudio|Boolescher Wert|Gibt ab, ob Mono-Audio im Kiosk-Modus erforderlich ist.|
|kioskModeRequireVoiceOver|Boolescher Wert|Gibt ab, ob Hintergrundkommentare im Kiosk-Modus erforderlich sind.|
|kioskModeRequireZoom|Boolean|Gibt ab, ob Zoom im Kiosk-Modus erforderlich ist.|
|kioskModeManagedAppId|Zeichenfolge|Verwaltete App-ID der App, die für den Kiosk-Modus verwendet werden soll. Wenn „KioskModeManagedAppId“ angegeben ist, wird „KioskModeAppStoreUrl“ ignoriert.|
|lockScreenBlockControlCenter|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer das Kontrollzentrum für den Sperrbildschirm verwendet.|
|lockScreenBlockNotificationView|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer die Benachrichtigungsansicht auf dem Sperrbildschirm verwendet.|
|lockScreenBlockPassbook|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Passbook verwendet, wenn das Gerät gesperrt ist.|
|lockScreenBlockTodayView|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer die Ansicht „Heute“ für den Sperrbildschirm verwendet.|
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
|mediaContentRatingApps|[ratingAppsType](../resources/intune-deviceconfig-ratingappstype.md)|Einstellungen für die Medieninhalts Bewertung für apps. Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12` und `agesAbove17`.|
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
|passcodeRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Geforderter Kennungstyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric`, `numeric`.|
|passcodeRequired|Boolescher Wert|Gibt an, ob eine Kennung erforderlich ist.|
|podcastsBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Podcasts auf dem überwachten Gerät verwendet (iOS 8.0 und höher).|
|proximityBlockSetupToNewDevice|Boolescher Wert|Gibt an, ob die Ansage zum Einrichten von benachbarten Geräten mit einem überwachten Gerät aktiviert werden soll.|
|safariBlockAutofill|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer AutoAusfüllen in Safari verwendet.|
|safariBlockJavaScript|Boolescher Wert|Gibt an, ob JavaScript in Safari blockiert werden soll.|
|safariBlockPopups|Boolescher Wert|Gibt an, ob Popups in Safari blockiert werden sollen.|
|safariBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Safari verwendet.|
|safariCookieSettings|[webBrowserCookieSettings](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|Cokkieeinstellungen für Safari. Mögliche Werte: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|safariManagedDomains|String collection|URLs, die mit den hier aufgeführten Mustern übereinstimmen, werden als verwaltet betrachtet.|
|safariPasswordAutoFillDomains|String collection|Benutzer können Kennwörter in Safari nur von URLs speichern, die mit den hier aufgeführten Mustern übereinstimmen. Gilt für Geräte im überwachten Modus (iOS 9.3 und höher).|
|safariRequireFraudWarning|Boolescher Wert|Gibt an, ob eine Betrugswarnung in Safari erforderlich ist.|
|screenCaptureBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Screenshots macht.|
|siriBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Siri verwendet.|
|siriBlockedWhenLocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Siri bei Sperrung verwendet.|
|siriBlockUserGeneratedContent|Boolescher Wert|Gibt an, ob Siri bei Verwendung auf einem überwachten Gerät davon abgehalten werden soll, benutzergenerierte Inhalte abzufragen.|
|siriRequireProfanityFilter|Boolean|Gibt an, ob verhindert werden soll, dass Siri anstößige Ausdrücke auf dem überwachten Gerät diktiert oder spricht.|
|softwareUpdatesEnforcedDelayInDays|Int32|Legt fest, wie viele Tage ein Software Update für ein überwachte Gerät delyed wird. Gültige Werte: 0 bis 90.|
|softwareUpdatesForceDelayed|Boolescher Wert|Gibt an, ob die Benutzersicht barkeit von Softwareupdates verzögert werden soll, wenn sich das Gerät im überwachten Modus befindet.|
|spotlightBlockInternetResults|Boolescher Wert|Gibt an, ob verhindert werden soll, dass die Spotlight-Suche Internetergebnisse auf dem überwachten Gerät zurückgibt.|
|voiceDialingBlocked|Boolescher Wert|Gibt an, ob das Sprachwahlverfahren blockiert werden soll.|
|wallpaperBlockModification|Boolescher Wert|Gibt an, ob das Ändern des Hintergrunds auf einem überwachten Gerät (iOS 9.0 und höher) zulässig ist.|
|wiFiConnectOnlyToConfiguredNetworks|Boolescher Wert|Gibt an, ob erzwungen werden soll, dass das Gerät nur WLAN-Netzwerke aus Konfigurationsprofilen verwendet, wenn sich das Gerät im überwachten Modus befindet.|
|classroomForceRequestPermissionToLeaveClasses|Boolescher Wert|Gibt an, ob ein Teilnehmer, der über das Klassenzimmer in einem nicht verwalteten Kurs angemeldet ist, beim Versuch, den Kurs zu verlassen (iOS 11,3 und höher) die Berechtigung des Lehrers anfordert.|
|keychainBlockCloudSync|Boolescher Wert|Gibt an, ob die iCloud-Schlüsselbund Synchronisierung blockiert ist.|
|pkiBlockOTAUpdates|Boolescher Wert|Gibt an, ob over-the-Air-PKI-Updates blockiert sind. Wenn Sie diese Einschränkung auf false festlegen, werden CRL-und OCSP-Prüfungen nicht deaktiviert (iOS 7,0 und höher).|
|privacyForceLimitAdTracking|Boolescher Wert|Gibt an, ob die AD-Verfolgung begrenzt ist. (iOS 7,0 und höher).|
|enterpriseBookBlockBackup|Boolescher Wert|Gibt an, ob Enterprise Book Back up gesperrt ist.|
|enterpriseBookBlockMetadataSync|Boolescher Wert|Gibt an, ob die Synchronisierung von Enterprise Book Notes und Highlights blockiert ist.|
|airPrintBlocked|Boolescher Wert|Gibt an, ob der druckDruck blockiert ist (iOS 11,0 und höher).|
|airPrintBlockCredentialsStorage|Boolescher Wert|Gibt an, ob die Schlüsselbund Speicherung von Benutzername und Kennwort für druckdruck blockiert ist (iOS 11,0 und höher).|
|airPrintForceTrustedTLS|Boolescher Wert|Gibt an, ob vertrauenswürdige Zertifikate für die TLS-Druckkommunikation erforderlich sind (iOS 11,0 und höher).|
|airPrintBlockiBeaconDiscovery|Boolescher Wert|Gibt an, ob die iBeacon-Erkennung von Druckern blockiert wird. Dadurch wird verhindert, dass gefälschte Bluetooth-Baken für den Netzwerkdatenverkehr aus dem Phishing entfernt werden (iOS 11,0 und höher).|
|blockSystemAppRemoval|Boolescher Wert|Gibt an, ob das Entfernen von System-apps vom Gerät auf einem überwachten Gerät (iOS 11,0 und höher) blockiert ist.|
|vpnBlockCreation|Boolescher Wert|Gibt an, ob die Erstellung von VPN-Konfigurationen blockiert ist (iOS 11,0 und höher).|
|appRemovalBlocked|Boolescher Wert|Gibt an, ob das Entfernen von apps zulässig ist.|
|usbRestrictedModeBlocked|Boolescher Wert|Gibt an, ob das Herstellen einer Verbindung mit USB-Zubehör während der Sperrung des Geräts zulässig ist (iOS 11.4.1 und höher).|
|passwordBlockAutoFill|Boolescher Wert|Gibt an, ob das Feature AutoFill passwords (iOS 12,0 und höher) zulässig ist.|
|passwordBlockProximityRequests|Boolescher Wert|Gibt an, ob das Anfordern von Kennwörtern von benachbarten Geräten (iOS 12,0 und höher) blockiert werden soll.|
|passwordBlockAirDropSharing|Boolescher Wert|Gibt an, ob das Freigeben von Kennwörtern für die Kennwörter von iOS 12,0 und höher blockiert werden soll.|
|dateAndTimeForceSetAutomatically|Boolescher Wert|Gibt an, ob die Funktion für Datum und Uhrzeit "automatisch festlegen" aktiviert ist und nicht vom Benutzer deaktiviert werden kann (iOS 12,0 und höher).|
|contactsAllowManagedToUnmanagedWrite|Boolescher Wert|Gibt an, ob verwaltete Apps Kontakte in nicht verwaltete Kontakte-Konten schreiben können (iOS 12,0 und höher).|
|contactsAllowUnmanagedToManagedRead|Boolescher Wert|Gibt an, ob nicht verwaltete Apps aus Konten für verwaltete Kontakte lesen können (iOS 12,0 oder höher).|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Sammlung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
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
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
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
  "esimBlockModification": true,
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
  "proximityBlockSetupToNewDevice": true,
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
  "softwareUpdatesEnforcedDelayInDays": 1024,
  "softwareUpdatesForceDelayed": true,
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




