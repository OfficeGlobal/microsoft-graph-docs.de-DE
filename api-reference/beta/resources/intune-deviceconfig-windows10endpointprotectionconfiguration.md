---
title: windows10EndpointProtectionConfiguration-Ressourcentyp
description: In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „Windows10EndpointProtectionConfiguration“ verfügbar gemacht werden.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: b4f915db0fb6578779461dab0536354ee5f005da
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937593"
---
# <a name="windows10endpointprotectionconfiguration-resource-type"></a>windows10EndpointProtectionConfiguration-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „Windows10EndpointProtectionConfiguration“ verfügbar gemacht werden.

Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[windows10EndpointProtectionConfigurations auflisten](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-list.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)-Sammlung|Listet die Eigenschaften und Beziehungen der [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)-Objekte auf.|
|[windows10EndpointProtectionConfiguration abrufen](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-get.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|Liest die Eigenschaften und Beziehungen des [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)-Objekts auf.|
|[windows10EndpointProtectionConfiguration erstellen](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-create.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|Erstellen Sie ein neues [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)-Objekt.|
|[windows10EndpointProtectionConfiguration löschen](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-delete.md)|Keine|Löscht eine [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).|
|[windows10EndpointProtectionConfiguration aktualisieren](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-update.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|Aktualisieren Sie die Eigenschaften eines [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Collection von Objekten des Typs „String“|Liste der Bereich Tags für diese Instanz der Entität. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolescher Wert|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt. Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden. Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userRightsAccessCredentialManagerAsTrustedCaller|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Berechtigung wird während der Sicherung/Wiederherstellung von Anmeldeinformations-Manager verwendet. Gespeicherten Anmeldeinformationen der Benutzer können beeinträchtigt werden, wenn diese Berechtigung für die anderen Entitäten angegeben ist. Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsAllowAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Berechtigung bestimmt, welche Benutzer und Gruppen mit dem Computer über das Netzwerk herstellen dürfen. State zugelassen wird unterstützt.|
|userRightsBlockAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieser Benutzer Rechte bestimmt, welche Benutzer und Gruppen Block aus eine Verbindung mit dem Computer über das Netzwerk sind. State-Block wird unterstützt.|
|userRightsActAsPartOfTheOperatingSystem|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Berechtigung ermöglicht es einem Prozess zum Identitätswechsel für alle Benutzer ohne Authentifizierung. Der Prozess kann daher auf dieselben lokalen Ressourcen wie der Benutzer zugreifen. Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsLocalLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieser Benutzer Rechte bestimmt, welche Benutzer am Computer anmelden können. Status nicht konfiguriert, zugelassen und blockiert werden alle unterstützt. |
|userRightsBackupData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Rechte Benutzer bestimmt, welche Benutzer Datei-, Verzeichnis-, Registrierung und andere beständige Objekte Berechtigungen beim Sichern der Dateien und Verzeichnisse umgehen können. Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsChangeSystemTime|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieser Benutzer Rechte bestimmt, welche Benutzer und Gruppen Uhrzeit und Datum der internen Uhr des Computers ändern können. Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsCreateGlobalObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Einstellung bestimmt, ob Benutzer globale Objekte erstellen können, die alle Sitzungen zur Verfügung stehen. Benutzer, die globale Objekte erstellen können, können es sich um Prozesse auswirken, die unter anderer Benutzer Sitzungen, ausgeführt wird und zu Anwendung Fehler und Datenverlust führen kann. Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsCreatePageFile|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Berechtigung bestimmt, welche Benutzer und Gruppen können eine interne API zum Erstellen und Ändern der Größe der Auslagerungsdatei aufrufen. Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsCreatePermanentSharedObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Rechte Benutzer bestimmt, welche Konten von Prozessen verwendet werden können, um ein Verzeichnisobjekt mithilfe des Objekts-Manager erstellen. Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsCreateSymbolicLinks|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieser Benutzer Rechte bestimmt, ob der Benutzer eine symbolische Verbindung vom Computer erstellen kann, an dem sie angemeldet sind. Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsCreateToken|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Berechtigung bestimmt, welche Benutzer/Gruppen von Prozessen verwendet werden können, um ein Token erstellen, die Zugriff auf alle lokalen Ressourcen abrufen, wenn der Prozess eine interne API verwendet, um ein Zugriffstoken erstellen verwendet werden kann. Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsDebugPrograms|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Rechte Benutzer bestimmt, welche Benutzer einen Debugger an einen beliebigen Prozess oder an den Kernel anfügen können. Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsRemoteDesktopServicesLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Berechtigung bestimmt, welche Benutzer und Gruppen nicht zulässig sind, als Remote Desktop Services Client anmelden. Nur die Bundesländer nicht konfiguriert und blockiert werden unterstützt.|
|userRightsDelegation|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieser Benutzer Rechte bestimmt, welche Benutzer die vertrauenswürdige für Delegierung Einstellung für ein Benutzer- oder Computerkonto-Objekt festlegen können. Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsGenerateSecurityAudits|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieser Benutzer Rechte bestimmt, welche Konten von einem Prozess zum Hinzufügen von Einträgen im Sicherheitsprotokoll verwendet werden können. Sicherheitsprotokoll wird verwendet, um autorisierter Zugriff zu verfolgen.  Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsImpersonateClient|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Zuweisen von diesem Benutzerrecht keinem Benutzer kann für diesen Benutzer zum Annehmen der Clientidentität ausgeführte Programme. Voraussetzen dieses Benutzerrecht für diese Art des Identitätswechsels verhindert, dass einen nicht autorisierten Benutzer aus überzeugende einen Client eine Verbindung zu einem Dienst, die sie erstellt haben, und klicken Sie dann Identitätswechsel bei dieser Client, dem der nicht autorisierte Benutzer Berechtigungen zu erhöhen können Administrative oder Systemebenen. Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsIncreaseSchedulingPriority|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Rechte Benutzer bestimmt, welche Konten einen Prozess mit Schreibzugriff auf einen anderen Prozess verwenden können, um die Ausführungspriorität zugewiesen an den anderen Prozess zu erhöhen. Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsLoadUnloadDrivers|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieser Benutzer Rechte bestimmt, welche Benutzer können dynamisch laden und entladen Gerätetreiber oder anderen Code im Kernelmodus. Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsLockMemory|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieser Benutzer Rechte bestimmt, welche Konten einen Prozess Speichern von Daten im physikalischen Speicher, wodurch das System verhindert, dass die Daten in den virtuellen Speicher auf dem Datenträger paging verwenden können. Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsManageAuditingAndSecurityLogs|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Berechtigung bestimmt, welche Benutzer Objekt den Optionen für einzelne Ressourcen, wie Dateien, Active Directory-Objekte und Registrierungsschlüssel für die Überwachung angeben können. Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsManageVolumes|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Rechte Benutzer bestimmt der Benutzer und Gruppen auf einem Datenträger, wie remote Defragmentierung Wartungsaufgaben ausführen können. Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsModifyFirmwareEnvironment|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Berechtigung bestimmt, Firmware-Umgebungsvariablen geändert werden kann. Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsModifyObjectLabels|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieser Benutzer Rechte bestimmt, welche Benutzerkonten die Bezeichnung Integrität von Objekten, wie Dateien, Registrierungsschlüssel oder Prozesse, die im Besitz von anderen Benutzern ändern können. Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsProfileSingleProcess|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieser Benutzer Rechte bestimmt, welche Benutzer Tools zum Überwachen der Leistung verwenden können, zur Überwachung der Leistung der Systemprozesse. Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsRemoteShutdown|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieser Benutzer Rechte bestimmt, welche Benutzer dürfen Herunterfahren eines Computers von einem Remotestandort im Netzwerk. Missbrauch dieses Benutzerrechts kann ein Denial-of-Service führen. Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsRestoreData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Berechtigung bestimmt, welche Benutzer umgehen können Datei-, Verzeichnis-, Registrierung und andere beständige Objekte, die Berechtigungen, die beim Wiederherstellen von Dateien und Verzeichnisse gesichert und bestimmt, welche Benutzer einen beliebigen gültigen Sicherheitsprinzipal als Besitzer eines Objekts festlegen können. Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsTakeOwnership|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieser Benutzer Rechte bestimmt, welche Benutzer die Besitzrechte für ein beliebiges sicherungsfähiges Objekt in das System, einschließlich Active Directory-Objekte, Dateien und Ordner, Drucker, Registrierungsschlüssel, Prozesse und Threads übernehmen können. Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.|
|userRightsRegisterProcessAsService|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Einstellung legt fest, welche Dienstkonten für das Registrieren von eines Prozess als Dienst gehindert werden. Hinweis: Diese Einstellung gilt nicht für die Konten System, lokaler Dienst oder Netzwerkdienst. Nur Status blockiert wird unterstützt.|
|xboxServicesEnableXboxGameSaveTask|Boolescher Wert|Diese Einstellung bestimmt, ob Xbox Spiel speichern aktiviert (1) oder deaktiviert (0) ist.|
|xboxServicesAccessoryManagementServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Diese Einstellung bestimmt, ob der Verwaltungsdienst Zubehör Starttyp Automatic(2), Manual(3), Disabled(4) ist. Standard: manuell. Mögliche Werte sind: `manual`, `automatic` und `disabled`.|
|xboxServicesLiveAuthManagerServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Diese Einstellung bestimmt, ob Starttyp Live Auth-Manager-Dienst Automatic(2), Manual(3), Disabled(4) ist. Standard: manuell. Mögliche Werte sind: `manual`, `automatic` und `disabled`.|
|xboxServicesLiveGameSaveServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Diese Einstellung bestimmt, ob Live Spiel Speichern des Dienstes Starttyp Automatic(2), Manual(3), Disabled(4) ist. Standard: manuell. Mögliche Werte sind: `manual`, `automatic` und `disabled`.|
|xboxServicesLiveNetworkingServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Diese Einstellung bestimmt, ob Starttyp Networking-Dienst Automatic(2), Manual(3), Disabled(4) ist. Standard: manuell. Mögliche Werte sind: `manual`, `automatic` und `disabled`.|
|localSecurityOptionsBlockMicrosoftAccounts|Boolescher Wert|Hindert Benutzer am Hinzufügen von neuen Microsoft-Konten auf diesem Computer.|
|localSecurityOptionsBlockRemoteLogonWithBlankPassword|Boolescher Wert|Aktivieren Sie lokale Konten, die nicht von anderen Orten als physisches Gerät anmelden, um kennwortgeschützte sind. Standard ist aktiviert|
|localSecurityOptionsEnableAdministratorAccount|Boolescher Wert|Bestimmt, ob das lokale Administratorkonto aktiviert oder deaktiviert ist.|
|localSecurityOptionsAdministratorAccountName|Zeichenfolge|Definieren Sie einen anderen Kontonamen an, die Sicherheits-ID (SID) für das Konto "Administrator" zugeordnet werden soll.|
|localSecurityOptionsEnableGuestAccount|Boolescher Wert|Bestimmt, ob das Konto Gast aktiviert oder deaktiviert ist.|
|localSecurityOptionsGuestAccountName|Zeichenfolge|Definieren Sie einen anderen Kontonamen an, die Sicherheits-ID (SID) für das Konto "Gast" zugeordnet werden soll.|
|localSecurityOptionsAllowUndockWithoutHavingToLogon|Boolescher Wert|Verhindern Sie, dass eines portablen Computers ohne Anmeldung abgedockt werden.|
|localSecurityOptionsBlockUsersInstallingPrinterDrivers|Boolescher Wert|Installieren von Druckertreiber als Teil des Herstellens einer Verbindung zu einem freigegebenen Drucker Admins nur zu beschränken.|
|localSecurityOptionsBlockRemoteOpticalDriveAccess|Boolescher Wert|Aktivieren diese Einstellungen kann nur interaktiv angemeldeten Benutzer auf CD-ROM-Medien zugreifen.|
|localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser|[localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|Definieren Sie, wer berechtigt ist, zu formatieren und NTFS-Wechselmedium ausschließen. Mögliche Werte: sind `notConfigured`, `administrators`, `administratorsAndPowerUsers` und `administratorsAndInteractiveUsers`.|
|localSecurityOptionsMachineInactivityLimit|Int32|Definieren Sie maximale Minuten der Inaktivität auf dem interaktiven Desktop Anmeldebildschirm, bis der Bildschirmschoner ausgeführt wird. Gültige Werte von 0 bis 9999|
|localSecurityOptionsMachineInactivityLimitInMinutes|Int32|Definieren Sie maximale Minuten der Inaktivität auf dem interaktiven Desktop Anmeldebildschirm, bis der Bildschirmschoner ausgeführt wird. Gültige Werte von 0 bis 9999|
|localSecurityOptionsDoNotRequireCtrlAltDel|Boolescher Wert|Benötigen Sie STRG + ALT + ENTF gedrückt werden, bevor ein Benutzer anmelden kann.|
|localSecurityOptionsHideLastSignedInUser|Boolescher Wert|Der Benutzername der letzten Person ein, die Anmeldung auf dem Gerät nicht angezeigt.|
|localSecurityOptionsHideUsernameAtSignIn|Boolescher Wert|Der Benutzername der Person, die dieses Gerät anmelden, nachdem Anmeldeinformationen eingegeben wurden und bevor der Desktop des Geräts angezeigt wird nicht angezeigt.|
|localSecurityOptionsLogOnMessageTitle|Zeichenfolge|Festlegen Sie Titel der Nachricht für Benutzer, die versuchen, melden Sie sich bei.|
|localSecurityOptionsLogOnMessageText|Zeichenfolge|Festlegen des Nachrichtentexts für Benutzer, die sich anmelden.|
|localSecurityOptionsAllowPKU2UAuthenticationRequests|Boolescher Wert|Block PKU2U authentifizierungsanforderungen an dieses Gerät online-Identitäten zu verwenden.|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool|Boolescher Wert|UI-Hilfsprogramm für LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager Entität boolean|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager|Zeichenfolge|Bearbeiten Sie die Security Descriptor Definition Language Standardzeichenfolge zum gewähren oder verweigern, Benutzer und Gruppen, um die SAM remote anzurufen.|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|Diese Einstellung kann ein Client die Aushandlung von 128-Bit-Verschlüsselung und/oder sitzungssicherheit NTLMv2 erforderlich ist. Mögliche Werte: sind `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption` und `ntlmV2And128BitEncryption`.|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|Diese Einstellung kann ein Server die Aushandlung von 128-Bit-Verschlüsselung und/oder sitzungssicherheit NTLMv2 erforderlich ist. Mögliche Werte: sind `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption` und `ntlmV2And128BitEncryption`.|
|lanManagerAuthenticationLevel|[lanManagerAuthenticationLevel](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|Diese Einstellung bestimmt, welche Herausforderung/Antwort-Authentifizierungsprotokoll Netzwerk Anmeldungen verwendet wird. Mögliche Werte sind: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm` und `lmNtlmV2AndNotLmOrNtm`.|
|lanManagerWorkstationEnableInsecureGuestLogons|Boolescher Wert|Wenn aktiviert, wird der SMB-Client unsichere Gast Anmeldungen zulassen. Falls nicht konfiguriert, wird der SMB-Client unsichere Gast Anmeldungen abgelehnt.|
|localSecurityOptionsClearVirtualMemoryPageFile|Boolescher Wert|Diese Einstellung bestimmt, ob die Auslagerungsdatei beim Herunterfahren des Systems gelöscht wird.|
|localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn|Boolescher Wert|Diese Einstellung bestimmt, ob es sich bei ein Computer beendet werden kann, ohne bei Windows anmelden.|
|localSecurityOptionsAllowUIAccessApplicationElevation|Boolescher Wert|Ermöglichen Sie UIAccess apps Elevation einzugeben, mit dem sicheren Desktop.|
|localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations|Boolescher Wert|Virtualisieren von Datei- und -Schreibvorgänge mit Fehlern an pro Benutzer Speicherorte|
|localSecurityOptionsOnlyElevateSignedExecutables|Boolescher Wert|Erzwingen Sie PKI-Zertifizierung Pfad Überprüfung für eine bestimmte ausführbare Datei, bevor er ausführen kann.|
|localSecurityOptionsAdministratorElevationPromptBehavior|[localSecurityOptionsAdministratorElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|Definieren Sie das Verhalten der Aufforderung für Administratoren im Administratormodus Genehmigung. Mögliche Werte sind: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent` und `promptForConsentForNonWindowsBinaries`.|
|localSecurityOptionsStandardUserElevationPromptBehavior|[localSecurityOptionsStandardUserElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|Definieren Sie das Verhalten der Elevation Ansage für Standardbenutzer. Mögliche Werte: sind `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop` und `promptForCredentials`.|
|localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation|Boolescher Wert|Aktivieren Sie alle Elevation-Anforderungen, fahren Sie mit dem sicheren Desktop, sondern den interaktiven Desktop des Benutzers. Richtlinien für Administratoren und Standardbenutzer Prompt Verhalten dienen.|
|localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation|Boolescher Wert|App Installationen mit erhöhte Berechtigungen werden für die Administratoranmeldeinformationen aufgefordert. Standard ist aktiviert|
|localSecurityOptionsAllowUIAccessApplicationsForSecureLocations|Boolescher Wert|Ermöglichen Sie UIAccess apps Elevation einzugeben, mit dem sicheren Desktop. Standard ist aktiviert|
|localSecurityOptionsUseAdminApprovalMode|Boolescher Wert|Definiert, ob das integrierte Administratorkonto Administratormodus Genehmigung verwendet oder alle apps mit vollständigen Administratorberechtigungen ausgeführt wird. Standard ist aktiviert|
|localSecurityOptionsUseAdminApprovalModeForAdministrators|Boolescher Wert|Definieren Sie, ob Administratormodus Genehmigung und alle UAC-Richtlinieneinstellungen aktiviert sind, ist standardmäßig aktiviert.|
|localSecurityOptionsInformationShownOnLockScreen|[localSecurityOptionsInformationShownOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|Konfigurieren Sie die Benutzerinformationen, die angezeigt wird, wenn die Sitzung gesperrt ist. Falls nicht konfiguriert, werden Anzeigename des Benutzers, Domäne und Benutzername angezeigt. Mögliche Werte: sind `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly` und `doNotDisplayUser`.|
|localSecurityOptionsInformationDisplayedOnLockScreen|[localSecurityOptionsInformationDisplayedOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|Konfigurieren Sie die Benutzerinformationen, die angezeigt wird, wenn die Sitzung gesperrt ist. Falls nicht konfiguriert, werden Anzeigename des Benutzers, Domäne und Benutzername angezeigt. Mögliche Werte: sind `notConfigured`, `administrators`, `administratorsAndPowerUsers` und `administratorsAndInteractiveUsers`.|
|localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees|Boolescher Wert|Diese Einstellung bestimmt, ob der SMB-Client versucht, SMB-Paketsignatur aushandeln.|
|localSecurityOptionsClientDigitallySignCommunicationsAlways|Boolescher Wert|Diese Einstellung bestimmt, ob die Clientkomponente für SMB-Paketsignatur erforderlich ist.|
|localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers|Boolescher Wert|Wenn diese Einstellung aktiviert ist, kann der Server Message Block (SMB) Redirector nur-Text-Kennwörter an nicht - Microsoft SMB-Server zu senden, die keine für die Verschlüsselung von Kennwörtern während der Authentifizierung Unterstützung.|
|localSecurityOptionsDisableServerDigitallySignCommunicationsAlways|Boolescher Wert|Diese Einstellung bestimmt, ob die SMB-Server-Komponente Paketsignatur erforderlich ist.|
|localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees|Boolescher Wert|Diese Einstellung bestimmt, ob der SMB Server SMB-Paketsignatur mit Clients, die diese anfordern aushandeln kann.|
|localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares|Boolescher Wert|Diese Einstellung schränkt standardmäßig anonymen Zugriff auf Freigaben und Pipes an den Einstellungen für named Pipes, die anonym zugegriffen werden können und Freigaben, die anonym zugegriffen werden kann|
|localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts|Boolescher Wert|Diese Einstellung bestimmt, welche zusätzlichen Berechtigungen für anonyme Verbindungen mit dem Computer erteilt werden sollen.|
|localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares|Boolescher Wert|Diese Einstellung bestimmt, ob anonyme Benutzer zum Ausführen bestimmter Aktivitäten, beispielsweise die Namen von Domänenkonten und Netzwerkfreigaben auflisten können.|
|localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange|Boolescher Wert|Diese Einstellung bestimmt, ob, an die nächste Änderung des Kennworts, der Hashwert LAN Manager (LM) für das neue Kennwort gespeichert ist. Es wird nicht standardmäßig gespeichert.|
|localSecurityOptionsSmartCardRemovalBehavior|[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|Diese Einstellung bestimmt, was geschieht, wenn die Smartcard für einen angemeldeten Benutzer aus dem Smartcard-Leser entfernt wird. Mögliche Werte: sind `lockWorkstation`, `noAction`, `forceLogoff` und `disconnectRemoteDesktopSession`.|
|defenderSecurityCenterDisableAppBrowserUI|Boolescher Wert|So deaktivieren Sie die Anzeige des Bereichs Protection app und Browser verwendet.|
|defenderSecurityCenterDisableFamilyUI|Boolescher Wert|Verwendet, um die Anzeige des Bereichs-Optionen zu deaktivieren.|
|defenderSecurityCenterDisableHealthUI|Boolescher Wert|So deaktivieren Sie die Anzeige des Geräts Leistung und der Zustand Bereichs verwendet.|
|defenderSecurityCenterDisableNetworkUI|Boolescher Wert|So deaktivieren Sie die Anzeige des Bereichs Protection Firewall und Netzwerk verwendet.|
|defenderSecurityCenterDisableVirusUI|Boolescher Wert|So deaktivieren Sie die Anzeige des Bereichs Protection Viren und verwendet.|
|defenderSecurityCenterDisableAccountUI|Boolescher Wert|So deaktivieren Sie die Anzeige des Bereichs Protection Konto verwendet.|
|defenderSecurityCenterDisableHardwareUI|Boolescher Wert|Verwendet, um die Anzeige des Bereichs Protection Hardware zu deaktivieren.|
|defenderSecurityCenterDisableRansomwareUI|Boolescher Wert|So deaktivieren Sie die Anzeige des Bereichs Protection Ransomware verwendet. |
|defenderSecurityCenterDisableSecureBootUI|Boolescher Wert|So deaktivieren Sie die Anzeige des Bereichs sicheren Boot unter gerätesicherheit verwendet.|
|defenderSecurityCenterDisableTroubleshootingUI|Boolescher Wert|So deaktivieren Sie die Anzeige des Prozesses Sicherheit unter Sicherheit Gerät Problembehandlung verwendet.|
|defenderSecurityCenterOrganizationDisplayName|Zeichenfolge|Der Firmenname, der den Benutzern angezeigt wird.|
|defenderSecurityCenterHelpEmail|Zeichenfolge|Die e-Mail-Adresse, die Benutzern angezeigt wird.|
|defenderSecurityCenterHelpPhone|Zeichenfolge|Die angegebene Rufnummer oder Skype-ID, die Benutzern angezeigt wird.|
|defenderSecurityCenterHelpURL|Zeichenfolge|Das Hilfeportal URL dies für Benutzer angezeigt wird.|
|defenderSecurityCenterNotificationsFromApp|[defenderSecurityCenterNotificationsFromAppType](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|Benachrichtigungen über die angezeigte Bereiche der app angezeigt. Mögliche Werte sind: `notConfigured`, `blockNoncriticalNotifications` und `blockAllNotifications`.|
|defenderSecurityCenterITContactDisplay|[defenderSecurityCenterITContactDisplayType](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|Konfigurieren Sie, wie IT-Kontakt anzeigen Informationen für Endbenutzer. Mögliche Werte: sind `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp` und `displayOnlyInNotifications`.|
|firewallBlockStatefulFTP|Boolescher Wert|Blockiert statusbehaftete FTP-Verbindungen mit dem Gerät.|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|Konfiguriert das Leerlauftimeout für Sicherheitszuordnungen in Sekunden, von 300 bis einschließlich 3600. Dies ist der Zeitraum, nach dem Sicherheitszuordnungen ablaufen und gelöscht werden. Gültige Werte: 300 bis 3600.|
|firewallPreSharedKeyEncodingMethod|[firewallPreSharedKeyEncodingMethodType](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|Wählen Sie den vorinstallierten Schlüssel um zu verwendende Codierung. Mögliche Werte sind: `deviceDefault`, `none` und `utF8`.|
|firewallIPSecExemptionsAllowNeighborDiscovery|Boolescher Wert|Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Nachbarsuche zulässig sind.|
|firewallIPSecExemptionsAllowICMP|Boolescher Wert|Konfiguriert IPSec-Ausnahmen, sodass ICMP zulässig ist.|
|firewallIPSecExemptionsAllowRouterDiscovery|Boolescher Wert|Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Routersuche zulässig sind.|
|firewallIPSecExemptionsAllowDHCP|Boolescher Wert|Konfiguriert IPSec-Ausnahmen, sodass sowohl IPv4-basierter als auch IPv6-basierter DHC-Datenverkehr zulässig ist.|
|firewallCertificateRevocationListCheckMethod|[firewallCertificateRevocationListCheckMethodType](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|Geben Sie an, wie die Certificate Revocation List erzwungen werden. Mögliche Werte: sind `deviceDefault`, `none`, `attempt` und `require`.|
|firewallMergeKeyingModuleSettings|Boolescher Wert|Wenn ein Authentifizierungssatz nicht vollständig von einem Schlüsselerstellungsmodul unterstützt wird, weist diese Einstellung das Modul an, nur nicht unterstützte Authentifizierungssuites zu ignorieren und nicht den gesamten Satz.|
|firewallPacketQueueingMethod|[firewallPacketQueueingMethodType](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|Konfiguriert, wie vom Warteschlangensystem Paket im Szenario mit Tunnel Gateway angewendet werden soll. Mögliche Werte sind: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound` und `queueBoth`.|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Konfiguriert die Firewallprofileinstellungen für Domänennetzwerke.|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Konfiguriert die Firewallprofileinstellungen für öffentliche Netzwerke.|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Konfiguriert die Firewallprofileinstellungen für private Netzwerke.|
|defenderAttackSurfaceReductionExcludedPaths|Collection von Objekten des Typs „String“|Liste von EXE-Dateien und Ordnern, die von Regeln zur Verringerung der Angriffsfläche ausgenommen werden sollen.
|
|defenderOfficeAppsOtherProcessInjectionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der das Verhalten des Office-Clientanwendungen, die er in andere Prozesse einfügt. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderOfficeAppsOtherProcessInjection|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der das Verhalten des Office-Clientanwendungen, die er in andere Prozesse einfügt. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderOfficeAppsExecutableContentCreationOrLaunchType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der das Verhalten von Office-Anwendungen/Makros erstellen, oder starten die ausführbare Inhalte. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderOfficeAppsExecutableContentCreationOrLaunch|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der das Verhalten von Office-Anwendungen/Makros erstellen, oder starten die ausführbare Inhalte. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderOfficeAppsLaunchChildProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der das Verhalten des Office-Anwendung, die untergeordnete Prozesse starten. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderOfficeAppsLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der das Verhalten des Office-Anwendung, die untergeordnete Prozesse starten. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderOfficeMacroCodeAllowWin32ImportsType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Der Wert, der angibt, dass das Verhalten der Win32 aus Code der Makros in Office importiert. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderOfficeMacroCodeAllowWin32Imports|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Der Wert, der angibt, dass das Verhalten der Win32 aus Code der Makros in Office importiert. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderScriptObfuscatedMacroCodeType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der das Verhalten von verschleierte Js, Vbs/Ps-/ Makro Code. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderScriptObfuscatedMacroCode|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der das Verhalten von verschleierte Js, Vbs/Ps-/ Makro Code. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderScriptDownloadedPayloadExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der das Verhalten des Js/Vbs Nutzlast ausführen, die vom Internet heruntergeladen werden. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderScriptDownloadedPayloadExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der das Verhalten des Js/Vbs Nutzlast ausführen, die vom Internet heruntergeladen werden. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderPreventCredentialStealingType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Der Wert, der angibt, wenn die Anmeldeinformationen, die vom Windows lokalen Behörde Teilsystem stehlen zulässig ist. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderProcessCreationType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der angibt, Reaktion auf Prozess Kreationen PSExec und WMI-Befehle stammt. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderProcessCreation|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der angibt, Reaktion auf Prozess Kreationen PSExec und WMI-Befehle stammt. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderUntrustedUSBProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der als Antwort auf nicht vertrauenswürdigen und nicht signierte Prozesse, die über USB ausgeführt. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderUntrustedUSBProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der als Antwort auf nicht vertrauenswürdigen und nicht signierte Prozesse, die über USB ausgeführt. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderUntrustedExecutableType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der als Antwort auf ausführbare Dateien, die keiner Verbreitung, Alter oder Liste der vertrauenswürdigen erfüllen Kriterien. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderUntrustedExecutable|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der als Antwort auf ausführbare Dateien, die keiner Verbreitung, Alter oder Liste der vertrauenswürdigen erfüllen Kriterien. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderEmailContentExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Der Wert, der angibt, wenn die Ausführung der ausführbaren Inhalt (Exe, Dll, Ps, Js, Vbs usw.) aus e-Mail (Webmail/Mail-Client) gelöscht werden soll. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderEmailContentExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Der Wert, der angibt, wenn die Ausführung der ausführbaren Inhalt (Exe, Dll, Ps, Js, Vbs usw.) aus e-Mail (Webmail/Mail-Client) gelöscht werden soll. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderAdvancedRansomewareProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der Verwendung der erweiterte Schutz vor Ransomeware. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderGuardMyFoldersType|[folderProtectionType](../resources/intune-deviceconfig-folderprotectiontype.md)|Wert, der das Verhalten der geschützte Ordner. Mögliche Werte sind: `userDefined`, `enable`, `auditMode`, `blockDiskModification` und `auditDiskModification`.|
|defenderGuardedFoldersAllowedAppPaths|Collection von Objekten des Typs „String“|Liste von Pfaden zu EXE-Dateien, die auf geschützte Ordner zugreifen dürfen.
|
|defenderAdditionalGuardedFolders|Collection von Objekten des Typs „String“|Liste von Ordnerpfaden, die der Liste geschützter Ordner hinzugefügt werden sollen.
|
|defenderNetworkProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der das Verhalten des NetworkProtection. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderExploitProtectionXml|Binär|XML-Inhalte mit Details zum Exploit-Schutz.
|
|defenderExploitProtectionXmlFileName|Zeichenfolge|Name der Datei, aus der „DefenderExploitProtectionXml“ abgerufen wurde.
|
|defenderSecurityCenterBlockExploitProtectionOverride|Boolescher Wert|Gibt an, ob verhindert werden soll, dass Benutzer die Einstellungen für den Exploit-Schutz überschreiben.|
|appLockerApplicationControl|[appLockerApplicationControlType](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|Ermöglicht dem Administrator die Festlegung der auf Geräten zulässigen Typen von Apps. Mögliche Werte sind: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker` und `auditComponentsStoreAppsAndSmartlocker`.|
|deviceGuardLocalSystemAuthorityCredentialGuardSettings|[deviceGuardLocalSystemAuthorityCredentialGuardType](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|Anmeldeinformationen Guard aktivieren Sie, wenn Sicherheit Plattformebene mit Secure Boot und Virtualisierung Sicherheit sind beide aktiviert. Mögliche Werte sind: `notConfigured`, `enableWithUEFILock` und `enableWithoutUEFILock`.|
|deviceGuardEnableVirtualizationBasedSecurity|Boolescher Wert|Schaltet die Virtualisierung basierend Security(VBS).|
|deviceGuardEnableSecureBootWithDMA|Boolescher Wert|Gibt an, ob Sicherheit Plattformebene beim nächsten Neustart aktiviert ist.|
|smartScreenEnableInShell|Boolescher Wert|Ermöglicht IT-Administratoren die Konfiguration von SmartScreen für Windows.|
|smartScreenBlockOverrideForFiles|Boolescher Wert|Ermöglicht es IT-Administratoren, zu steuern, ob Benutzer SmartScreen-Warnungen ignorieren und Schaddateien ausführen dürfen.|
|applicationGuardEnabled|Boolescher Wert|Aktiviert Windows Defender Application Guard.|
|applicationGuardEnabledOptions|[applicationGuardEnabledOptions](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|Aktivieren Sie Windows Defender Anwendung Guard für neuere Versionen von Windows. Mögliche Werte: sind `notConfigured`, `enabledForEdge`, `enabledForOffice` und `enabledForEdgeAndOffice`.|
|applicationGuardBlockFileTransfer|[applicationGuardBlockFileTransferType](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|Block Zwischenablage Übertragung Bilddatei, Textdatei oder dürfen. Mögliche Werte sind: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone` und `blockTextFile`.|
|applicationGuardBlockNonEnterpriseContent|Boolescher Wert|Unterbindet, dass Unternehmenswebsites unternehmensfremde Inhalte laden, z. B. Plug-Ins von Drittanbietern.|
|applicationGuardAllowPersistence|Boolescher Wert|Erlaubt die dauerhafte Speicherung benutzergenerierter Daten im App Guard Container (Favoriten, Cookies, Webkennwörter usw.).|
|applicationGuardForceAuditing|Boolescher Wert|Erzwingt die dauerhafte Speicherung von Windows-Protokollen und -Ereignissen durch die Überwachung zwecks Erfüllung von Sicherheits- und Compliancevorgaben (Beispielereignisse sind Benutzeranmeldungen und -abmeldungen, die Verwendung von Berechtigungen, die Installation von Software und Änderungen am System).|
|applicationGuardBlockClipboardSharing|[applicationGuardBlockClipboardSharingType](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|Blockiert die Freigabe von Zwischenablagedaten zwischen Host und Container, zwischen Container und Host, in beide Richtungen oder in keine Richtung. Mögliche Werte sind: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost` und `blockNone`.|
|applicationGuardAllowPrintToPDF|Boolescher Wert|Erlaubt das Drucken im PDF-Format aus dem Container.
|
|applicationGuardAllowPrintToXPS|Boolescher Wert|Erlaubt das Drucken im XPS-Format aus dem Container.
|
|applicationGuardAllowPrintToLocalPrinters|Boolescher Wert|Erlaubt das Drucken auf lokalen Druckern aus dem Container.
|
|applicationGuardAllowPrintToNetworkPrinters|Boolescher Wert|Erlaubt das Drucken auf Netzwerkdruckern aus dem Container.
|
|applicationGuardAllowVirtualGPU|Boolescher Wert|Zulassen der Anwendung Guard virtuellen GPU verwenden|
|applicationGuardAllowFileSaveOnHost|Boolescher Wert|Zulassen, dass Benutzer Dateien vom Rand im Container Guard Anwendung herunterladen und speichern Sie sie auf dem Host Dateisystem|
|bitLockerDisableWarningForOtherDiskEncryption|Boolescher Wert|Ermöglicht es dem Administrator, den Warnhinweis bezüglich anderer Festplattenverschlüsselungslösungen auf Benutzer-PCs zu deaktivieren.|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolescher Wert|Ermöglicht es dem Administrator, eine Aktivierung der Verschlüsselung mittels BitLocker anzufordern.
 Diese Richtlinie gilt nur für Mobilgeräte-SKUs.|
|bitLockerEncryptDevice|Boolescher Wert|Ermöglicht es dem Administrator, eine Aktivierung der Verschlüsselung mittels BitLocker anzufordern.
|
|bitLockerSystemDrivePolicy|[bitLockerSystemDrivePolicy](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|System BitLocker Drive-Richtlinie.|
|bitLockerFixedDrivePolicy|[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|BitLocker feste Laufwerk Richtlinie.|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|BitLocker-Richtlinie für Wechseldatenträger.|

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
  "@odata.type": "microsoft.graph.windows10EndpointProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
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
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRegisterProcessAsService": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "String",
  "xboxServicesLiveAuthManagerServiceStartupMode": "String",
  "xboxServicesLiveGameSaveServiceStartupMode": "String",
  "xboxServicesLiveNetworkingServiceStartupMode": "String",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsEnableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "String",
  "localSecurityOptionsEnableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "String",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "String",
  "localSecurityOptionsMachineInactivityLimit": 1024,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 1024,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "String",
  "localSecurityOptionsLogOnMessageText": "String",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "String",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "String",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "String",
  "lanManagerAuthenticationLevel": "String",
  "lanManagerWorkstationEnableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "String",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "String",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "String",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "String",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "String",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "String",
  "defenderSecurityCenterHelpEmail": "String",
  "defenderSecurityCenterHelpPhone": "String",
  "defenderSecurityCenterHelpURL": "String",
  "defenderSecurityCenterNotificationsFromApp": "String",
  "defenderSecurityCenterITContactDisplay": "String",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 1024,
  "firewallPreSharedKeyEncodingMethod": "String",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "String",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "String",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "String"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "String",
  "defenderOfficeAppsOtherProcessInjection": "String",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "String",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "String",
  "defenderOfficeAppsLaunchChildProcessType": "String",
  "defenderOfficeAppsLaunchChildProcess": "String",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "String",
  "defenderOfficeMacroCodeAllowWin32Imports": "String",
  "defenderScriptObfuscatedMacroCodeType": "String",
  "defenderScriptObfuscatedMacroCode": "String",
  "defenderScriptDownloadedPayloadExecutionType": "String",
  "defenderScriptDownloadedPayloadExecution": "String",
  "defenderPreventCredentialStealingType": "String",
  "defenderProcessCreationType": "String",
  "defenderProcessCreation": "String",
  "defenderUntrustedUSBProcessType": "String",
  "defenderUntrustedUSBProcess": "String",
  "defenderUntrustedExecutableType": "String",
  "defenderUntrustedExecutable": "String",
  "defenderEmailContentExecutionType": "String",
  "defenderEmailContentExecution": "String",
  "defenderAdvancedRansomewareProtectionType": "String",
  "defenderGuardMyFoldersType": "String",
  "defenderGuardedFoldersAllowedAppPaths": [
    "String"
  ],
  "defenderAdditionalGuardedFolders": [
    "String"
  ],
  "defenderNetworkProtectionType": "String",
  "defenderExploitProtectionXml": "binary",
  "defenderExploitProtectionXmlFileName": "String",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "String",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "String",
  "applicationGuardBlockFileTransfer": "String",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "String",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "String",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "String",
    "startupAuthenticationTpmPinUsage": "String",
    "startupAuthenticationTpmKeyUsage": "String",
    "startupAuthenticationTpmPinAndKeyUsage": "String",
    "minimumPinLength": 1024,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "String",
      "recoveryKeyUsage": "String",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "String",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "String",
    "prebootRecoveryUrl": "String"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "String",
      "recoveryKeyUsage": "String",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "String",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```





