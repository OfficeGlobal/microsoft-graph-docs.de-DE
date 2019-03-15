---
title: windows10EndpointProtectionConfiguration-Ressourcentyp
description: In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „Windows10EndpointProtectionConfiguration“ verfügbar gemacht werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4f034a6b35c1ae8bd8172a20c5da0ee2e818623
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571704"
---
# <a name="windows10endpointprotectionconfiguration-resource-type"></a>windows10EndpointProtectionConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolesch|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|dmaGuardDeviceEnumerationPolicy|[dmaGuardDeviceEnumerationPolicyType](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|Diese Richtlinie soll zusätzliche Sicherheit für externe DMA-fähige Geräte bieten. Es ermöglicht eine bessere Kontrolle über die Enumeration externer DMA-Geräte, die mit der DMA-Neuzuordnung/Gerätespeicher Isolierung und Sandkasten nicht kompatibel sind. Diese Richtlinie wird nur wirksam, wenn der Kernel DMA-Schutz von der System Firmware unterstützt und aktiviert wird. Der Kernel DMA Protection ist eine Plattformfunktion, die nicht über Richtlinien oder Endbenutzer gesteuert werden kann. Sie muss zum Zeitpunkt der Fertigung vom System unterstützt werden. Um zu überprüfen, ob das System den Kernel DMA-Schutz unterstützt, aktivieren Sie auf der Zusammenfassungsseite von MSINFO32. exe das Feld Kernel DMA Protection. Mögliche Werte sind: `deviceDefault`, `blockAll` und `allowAll`.|
|firewallRules|[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) -Sammlung|Konfiguriert die Firewall-Regeleinstellungen. Diese Auflistung kann maximal 150 Elemente enthalten.|
|userRightsAccessCredentialManagerAsTrustedCaller|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht wird von Credential Manager während der Sicherung/Wiederherstellung verwendet. Die gespeicherten Anmeldeinformationen der Benutzer werden möglicherweise kompromittiert, wenn diese Berechtigung anderen Entitäten erteilt wird. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsAllowAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen über das Netzwerk eine Verbindung mit dem Computer herstellen dürfen. Der Status Allowed wird unterstützt.|
|userRightsBlockAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen blockieren, eine Verbindung mit dem Computer über das Netzwerk herzustellen. Status Block wird unterstützt.|
|userRightsActAsPartOfTheOperatingSystem|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht ermöglicht es einem Prozess, einen beliebigen Benutzer ohne Authentifizierung zu imitieren. Der Prozess kann daher Zugriff auf die gleichen lokalen Ressourcen wie diesen Benutzer erlangen. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsLocalLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer sich am Computer anmelden können. Status NotConfigured, zulässig und blockiert werden alle unterstützt. |
|userRightsBackupData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer beim Sichern von Dateien und Verzeichnissen Datei-, Verzeichnis-, Registrierungs-und andere persistent Objects-Berechtigungen umgehen können. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsChangeSystemTime|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen die Uhrzeit und das Datum für die interne Uhr des Computers ändern können. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsCreateGlobalObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Sicherheitseinstellung bestimmt, ob Benutzer globale Objekte erstellen können, die für alle Sitzungen zur Verfügung stehen. Benutzer, die globale Objekte erstellen können, könnten sich auf Prozesse auswirken, die in Sitzungen anderer Benutzer ausgeführt werden, was zu Anwendungsfehlern oder Datenbeschädigungen führen kann. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsCreatePageFile|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen eine interne API aufrufen können, um die Größe einer Auslagerungsdatei zu erstellen und zu ändern. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsCreatePermanentSharedObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Konten von Prozessen verwendet werden können, um mithilfe des Objekt-Managers ein Verzeichnisobjekt zu erstellen. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsCreateSymbolicLinks|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, ob der Benutzer einen symbolischen Link von dem Computer aus erstellen kann, auf dem Sie angemeldet sind. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsCreateToken|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer/Gruppen von Prozessen verwendet werden können, um ein Token zu erstellen, das dann verwendet werden kann, um Zugriff auf lokale Ressourcen zu erhalten, wenn der Prozess eine interne API zum Erstellen eines Zugriffstokens verwendet. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsDebugPrograms|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer einen Debugger an einen beliebigen Prozess oder an den Kernel anfügen können. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsRemoteDesktopServicesLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen nicht als Remote Desktop Dienste-Client angemeldet werden dürfen. Nur Status NotConfigured und blockiert werden unterstützt.|
|userRightsDelegation|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer die Einstellung für die vertrauenswürdige deLegierung für ein Benutzer-oder Computerobjekt festlegen können. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsGenerateSecurityAudits|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Konten von einem Prozess zum Hinzufügen von Einträgen zum Sicherheitsprotokoll verwendet werden können. Das Sicherheitsprotokoll wird verwendet, um nicht autorisierten Systemzugriff nachzuverfolgen.  Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsImpersonateClient|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Durch das Zuweisen dieses Benutzerrechts zu einem Benutzer können Programme, die im Auftrag dieses Benutzers laufen, die Identität eines Clients annehmen. Wenn Sie dieses Benutzerrecht für diese Art von Identitätswechsel benötigen, wird verhindert, dass ein nicht autorisierter Benutzer einen Client dazu überzeugt, eine Verbindung mit einem Dienst herzustellen, den er erstellt hat, und dann die Identität dieses Clients annehmen, wodurch die Berechtigungen des nicht autorisierten Benutzers erhöht werden können administrative oder Systemebenen. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsIncreaseSchedulingPriority|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Konten einen Prozess mit Schreibeigenschaften Zugriff auf einen anderen Prozess verwenden können, um die dem anderen Prozess zugewiesene Ausführungspriorität zu verlängern. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsLoadUnloadDrivers|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer Gerätetreiber oder anderen Code im Kernelmodus dynamisch laden und entladen können. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsLockMemory|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Konten einen Prozess verwenden können, um Daten im physischen Arbeitsspeicher zu speichern, wodurch verhindert wird, dass das System die Daten auf dem Datenträger in den virtuellen Arbeitsspeicher eingibt. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsManageAuditingAndSecurityLogs|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer die Objektzugriffs-Überwachungsoptionen für einzelne Ressourcen wie Dateien, Active Directory-Objekte und Registrierungsschlüssel angeben können. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsManageVolumes|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen Wartungsaufgaben auf einem Volume ausführen können, beispielsweise die Remote Defragmentierung. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsModifyFirmwareEnvironment|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, wer die Werte der Firmware-Umgebung ändern kann. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsModifyObjectLabels|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzerkonten die Integritäts Bezeichnung von Objekten wie Dateien, Registrierungsschlüssel oder Prozesse ändern können, die anderen Benutzern gehören. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsProfileSingleProcess|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer Leistungsüberwachungstools verwenden können, um die Leistung von Systemprozessen zu überwachen. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsRemoteShutdown|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer einen Computer von einem Remotestandort im Netzwerk Herunterfahren dürfen. Missbrauch dieses Benutzerrechts kann zu einem Denial-of-Service führen. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsRestoreData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer bei der Wiederherstellung gesicherter Dateien und Verzeichnisse Datei-, Verzeichnis-, Registrierungs-und andere persistent Objects-Berechtigungen umgehen können, und bestimmt, welche Benutzer einen gültigen Sicherheitsprinzipal als Besitzer eines Objekts festlegen können. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsTakeOwnership|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Dieses Benutzerrecht bestimmt, welche Benutzer den Besitz eines sicherungsfähigen Objekts im System übernehmen können, einschließlich Active Directory-Objekte, Dateien und Ordner, Drucker, Registrierungsschlüssel, Prozesse und Threads. Nur Status NotConfigured und Allowed werden unterstützt.|
|userRightsRegisterProcessAsService|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Diese Sicherheitseinstellung bestimmt, welche Dienstkonten verhindert werden, einen Prozess als Dienst zu registrieren. Hinweis: Diese Sicherheitseinstellung gilt nicht für die System-, lokalen Dienst-oder Netzwerkdienstkonten. Nur Status blockiert wird unterstützt.|
|xboxServicesEnableXboxGameSaveTask|Boolesch|Diese Einstellung bestimmt, ob Xbox Game Save (1) oder Disabled (0) aktiviert ist.|
|xboxServicesAccessoryManagementServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Diese Einstellung bestimmt, ob der Starttyp des Zubehör Verwaltungsdiensts automatisch (2), manuell (3), deaktiviert (4) ist. Standard: manual. Mögliche Werte sind: `manual`, `automatic` und `disabled`.|
|xboxServicesLiveAuthManagerServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Diese Einstellung bestimmt, ob der Starttyp des Live auth Manager-Diensts automatisch (2), manuell (3), deaktiviert (4) ist. Standard: manual. Mögliche Werte sind: `manual`, `automatic` und `disabled`.|
|xboxServicesLiveGameSaveServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Diese Einstellung bestimmt, ob der Starttyp des Live Spiel-Diensts automatisch ist (2), manuell (3), deaktiviert (4). Standard: manual. Mögliche Werte sind: `manual`, `automatic` und `disabled`.|
|xboxServicesLiveNetworkingServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Diese Einstellung bestimmt, ob der Starttyp des Netzwerkdiensts automatisch (2), manuell (3), deaktiviert (4) ist. Standard: manual. Mögliche Werte sind: `manual`, `automatic` und `disabled`.|
|localSecurityOptionsBlockMicrosoftAccounts|Boolesch|Verhindern, dass Benutzer neue Microsoft-Konten zu diesem Computer hinzufügen.|
|localSecurityOptionsBlockRemoteLogonWithBlankPassword|Boolesch|Aktivieren Sie lokale Konten, die nicht kennwortgeschützt sind, um sich an anderen Speicherorten als dem physischen Gerät anzumelden. Standard ist aktiviert|
|localSecurityOptionsDisableAdministratorAccount|Boolesch|Bestimmt, ob das lokale Administrator Konto aktiviert oder deaktiviert ist.|
|localSecurityOptionsAdministratorAccountName|String|Definieren Sie einen anderen Kontonamen, der der Sicherheits-ID (SID) für das Konto "Administrator" zugeordnet werden soll.|
|localSecurityOptionsDisableGuestAccount|Boolesch|Bestimmt, ob das Gastkonto aktiviert oder deaktiviert ist.|
|localSecurityOptionsGuestAccountName|String|Definieren Sie einen anderen Kontonamen, der der Sicherheits-ID (SID) für das Konto "Guest" zugeordnet werden soll.|
|localSecurityOptionsAllowUndockWithoutHavingToLogon|Boolesch|Verhindern, dass ein tragbarer Computer ohne Anmeldung abdockt.|
|localSecurityOptionsBlockUsersInstallingPrinterDrivers|Boolesch|Beschränken Sie die Installation von Druckertreibern im Rahmen der Verbindung zu einem freigegebenen Drucker nur mit Administratoren.|
|localSecurityOptionsBlockRemoteOpticalDriveAccess|Boolesch|Wenn Sie diese Einstellung aktivieren, kann nur interaktiv auf CD-ROM-Medien zugegriffen werden.|
|localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser|[localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|Legen Sie fest, wer Wechseldatenträger formatieren und Auswerfen darf. Mögliche Werte sind: `notConfigured`, `administrators`, `administratorsAndPowerUsers` und `administratorsAndInteractiveUsers`.|
|localSecurityOptionsMachineInactivityLimit|Int32|Definieren Sie maximale Minuten der Inaktivität auf dem Anmeldebildschirm des interaktiven Desktops, bis der Bildschirmschoner ausgeführt wird. Gültige Werte 0 bis 9999|
|localSecurityOptionsMachineInactivityLimitInMinutes|Int32|Definieren Sie maximale Minuten der Inaktivität auf dem Anmeldebildschirm des interaktiven Desktops, bis der Bildschirmschoner ausgeführt wird. Gültige Werte 0 bis 9999|
|localSecurityOptionsDoNotRequireCtrlAltDel|Boolesch|Die Tastenkombination STRG + ALT + ENTF muss gedrückt werden, bevor sich ein Benutzer anmelden kann.|
|localSecurityOptionsHideLastSignedInUser|Boolesch|Zeigen Sie nicht den Benutzernamen der letzten Person an, die sich auf diesem Gerät angemeldet hat.|
|localSecurityOptionsHideUsernameAtSignIn|Boolesch|Zeigen Sie nicht den Benutzernamen der Person an, die sich bei diesem Gerät anmeldet, nachdem Sie die Anmeldeinformationen eingegeben haben, und bevor der Desktop des Geräts angezeigt wird.|
|localSecurityOptionsLogOnMessageTitle|String|Festlegen des Nachrichten Titels für Benutzer, die sich anmelden möchten.|
|localSecurityOptionsLogOnMessageText|String|Festlegen des Nachrichtentexts für Benutzer, die sich anmelden möchten.|
|localSecurityOptionsAllowPKU2UAuthenticationRequests|Boolesch|Blockieren Sie PKU2U-Authentifizierungsanforderungen für dieses Gerät, um Online Identitäten zu verwenden.|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool|Boolesch|UI Helper Boolean für LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager-Entität|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager|String|Bearbeiten Sie die standardmäßige Zeichenfolge für die Sicherheitsdeskriptor-Definition, um Benutzern und Gruppen das Ausführen von Remote anrufen für SAM zu erlauben oder zu verweigern.|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|Mit dieser Sicherheitseinstellung kann ein Client die 128-Bit-Verschlüsselung und/oder die NTLMv2-Sitzungssicherheit aushandeln. Mögliche Werte sind: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption` und `ntlmV2And128BitEncryption`.|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|Mit dieser Sicherheitseinstellung kann ein Server die Aushandlung der 128-Bit-Verschlüsselung und/oder der NTLMv2-Sitzungssicherheit erfordern. Mögliche Werte sind: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption` und `ntlmV2And128BitEncryption`.|
|lanManagerAuthenticationLevel|[lanManagerAuthenticationLevel](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|Diese Sicherheitseinstellung bestimmt, welches Abfrage-/Antwort Authentifizierungsprotokoll für Netzwerkanmeldungen verwendet wird. Mögliche Werte sind: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm` und `lmNtlmV2AndNotLmOrNtm`.|
|lanManagerWorkstationDisableInsecureGuestLogons|Boolesch|Wenn diese Option aktiviert ist, erlaubt der SMB-Client unsichere Gastanmeldungen. Wenn nicht konfiguriert, lehnt der SMB-Client unsichere Gastanmeldungen ab.|
|localSecurityOptionsClearVirtualMemoryPageFile|Boolesch|Diese Sicherheitseinstellung bestimmt, ob die Auslagerungsdatei des virtuellen Speichers gelöscht wird, wenn das System heruntergefahren wird.|
|localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn|Boolesch|Diese Sicherheitseinstellung bestimmt, ob ein Computer heruntergefahren werden kann, ohne sich bei Windows anmelden zu müssen.|
|localSecurityOptionsAllowUIAccessApplicationElevation|Boolesch|Zulassen, dass UIAccess-apps ohne Verwendung des sicheren Desktops zur Eingabe aufgefordert werden.|
|localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations|Boolesch|Virtualisieren von Datei-und Registrierungs Schreibfehlern pro Benutzerspeicherorte|
|localSecurityOptionsOnlyElevateSignedExecutables|Boolesch|Erzwingen Sie die Validierung des PKI-Zertifizierungspfads für eine bestimmte ausführbare Datei, bevor Sie ausgeführt werden kann.|
|localSecurityOptionsAdministratorElevationPromptBehavior|[localSecurityOptionsAdministratorElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|Definieren Sie das Verhalten der Eingabeaufforderung für Administratoren im AdministratorgenehmigungsModus. Mögliche Werte: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.|
|localSecurityOptionsStandardUserElevationPromptBehavior|[localSecurityOptionsStandardUserElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|Definieren Sie das Verhalten der Eingabeaufforderung für Standardbenutzer. Mögliche Werte sind: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop` und `promptForCredentials`.|
|localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation|Boolesch|Aktivieren Sie alle Elevation-Anforderungen, um anstelle des sicheren Desktops zum Desktop des interaktiven Benutzers zu wechseln. Richtlinieneinstellungen für das Ansage Verhalten für Administratoren und Standardbenutzer werden verwendet.|
|localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation|Boolesch|App-Installationen, die erhöhte Rechte erfordern, werden zur Eingabe von Administratoranmeldeinformationen aufgefordert. Standard ist aktiviert|
|localSecurityOptionsAllowUIAccessApplicationsForSecureLocations|Boolesch|Zulassen, dass UIAccess-apps ohne Verwendung des sicheren Desktops zur Eingabe aufgefordert werden. Standard ist aktiviert|
|localSecurityOptionsUseAdminApprovalMode|Boolesch|Definiert, ob das integrierte Administratorkonto den AdministratorgenehmigungsModus verwendet oder alle apps mit vollständigen Administratorrechten ausführt. Standard ist aktiviert|
|localSecurityOptionsUseAdminApprovalModeForAdministrators|Boolesch|Legen Sie fest, ob der AdministratorgenehmigungsModus und alle UAC-Richtlinieneinstellungen aktiviert sind, Standard ist aktiviert.|
|localSecurityOptionsInformationShownOnLockScreen|[localSecurityOptionsInformationShownOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|Konfigurieren Sie die Benutzerinformationen, die angezeigt werden, wenn die Sitzung gesperrt ist. Wenn nicht konfiguriert, werden Benutzeranzeigename, Domäne und Benutzername angezeigt. Mögliche Werte sind: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly` und `doNotDisplayUser`.|
|localSecurityOptionsInformationDisplayedOnLockScreen|[localSecurityOptionsInformationDisplayedOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|Konfigurieren Sie die Benutzerinformationen, die angezeigt werden, wenn die Sitzung gesperrt ist. Wenn nicht konfiguriert, werden Benutzeranzeigename, Domäne und Benutzername angezeigt. Mögliche Werte sind: `notConfigured`, `administrators`, `administratorsAndPowerUsers` und `administratorsAndInteractiveUsers`.|
|localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees|Boolesch|Diese Sicherheitseinstellung bestimmt, ob der SMB-Client versucht, die SMB-Paketsignierung auszuhandeln.|
|localSecurityOptionsClientDigitallySignCommunicationsAlways|Boolesch|Diese Sicherheitseinstellung bestimmt, ob die Paketsignierung für die SMB-Clientkomponente erforderlich ist.|
|localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers|Boolesch|Wenn diese Sicherheitseinstellung aktiviert ist, kann der SMB-Redirector (Server Message Block) Klartext-Kennwörter an nicht-Microsoft SMB-Server senden, die die Kennwortverschlüsselung während der Authentifizierung nicht unterstützen.|
|localSecurityOptionsDisableServerDigitallySignCommunicationsAlways|Boolesch|Diese Sicherheitseinstellung bestimmt, ob für die SMB-Serverkomponente eine Paketsignierung erforderlich ist.|
|localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees|Boolesch|Diese Sicherheitseinstellung bestimmt, ob der SMB-Server die SMB-Paketsignierung mit Clients aushandelt, die ihn anfordern.|
|localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares|Boolesch|Diese Sicherheitseinstellung beschränkt den anonymen Zugriff auf Freigaben und Pipes standardmäßig auf die Einstellungen für Named Pipes, auf die anonym zugegriffen werden kann, und auf Freigaben, auf die anonym zugegriffen werden kann.|
|localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts|Boolesch|Diese Sicherheitseinstellung bestimmt, welche zusätzlichen Berechtigungen für anonyme Verbindungen mit dem Computer erteilt werden.|
|localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares|Boolesch|Diese Sicherheitseinstellung bestimmt, ob anonyme Benutzer bestimmte Aktivitäten ausführen können, beispielsweise das Aufzählen der Namen von Domänenkonten und Netzwerkfreigaben.|
|localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange|Boolesch|Diese Sicherheitseinstellung bestimmt, ob bei der nächsten Kennwortänderung der LAN-Manager (LM)-Hashwert für das neue Kennwort gespeichert wird. Sie wird nicht standardmäßig gespeichert.|
|localSecurityOptionsSmartCardRemovalBehavior|[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|Diese Sicherheitseinstellung bestimmt, was geschieht, wenn die Smartcard für einen angemeldeten Benutzer aus dem Smartcard-Lesegerät entfernt wird. Mögliche Werte sind: `lockWorkstation`, `noAction`, `forceLogoff` und `disconnectRemoteDesktopSession`.|
|defenderSecurityCenterDisableAppBrowserUI|Boolesch|Wird verwendet, um die Anzeige des App-und Browser Schutzbereichs zu deaktivieren.|
|defenderSecurityCenterDisableFamilyUI|Boolesch|Wird verwendet, um die Anzeige des Bereichs Familienoptionen zu deaktivieren.|
|defenderSecurityCenterDisableHealthUI|Boolesch|Wird verwendet, um die Anzeige der Geräteleistung und des Integritäts Bereichs zu deaktivieren.|
|defenderSecurityCenterDisableNetworkUI|Boolesch|Wird verwendet, um die Anzeige des Firewall-und Netzwerkschutz Bereichs zu deaktivieren.|
|defenderSecurityCenterDisableVirusUI|Boolesch|Wird verwendet, um die Anzeige des Viren-und Bedrohungsschutz Bereichs zu deaktivieren.|
|defenderSecurityCenterDisableAccountUI|Boolesch|Wird verwendet, um die Anzeige des Kontoschutz Bereichs zu deaktivieren.|
|defenderSecurityCenterDisableClearTpmUI|Boolesch|Wird verwendet, um die Anzeige der Schaltfläche TPM löschen zu deaktivieren.|
|defenderSecurityCenterDisableHardwareUI|Boolesch|Wird verwendet, um die Anzeige des Hardwareschutz Bereichs zu deaktivieren.|
|defenderSecurityCenterDisableNotificationAreaUI|Boolesch|Wird verwendet, um die Anzeige des Benachrichtigungsbereichs-Steuerelements zu deaktivieren. Der Benutzer muss sich abmelden und sich anmelden oder den Computer neu starten, damit diese Einstellung wirksam wird.|
|defenderSecurityCenterDisableRansomwareUI|Boolesch|Wird verwendet, um die Anzeige des Ransomware-Schutzbereichs zu deaktivieren. |
|defenderSecurityCenterDisableSecureBootUI|Boolesch|Wird verwendet, um die Anzeige des sicheren Startbereichs unter Gerätesicherheit zu deaktivieren.|
|defenderSecurityCenterDisableTroubleshootingUI|Boolesch|Wird verwendet, um die Anzeige der Sicherheitsprozess-Problembehandlung unter Gerätesicherheit zu deaktivieren.|
|defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI|Boolesch|Wird verwendet, um die Anzeige der TPM-Update-Firmware zu deaktivieren, wenn eine Sicherheitsanfälligkeit erkannt wird.|
|defenderSecurityCenterOrganizationDisplayName|String|Der Name des Unternehmens, der den Benutzern angezeigt wird.|
|defenderSecurityCenterHelpEmail|String|Die e-Mail-Adresse, die Benutzern angezeigt wird.|
|defenderSecurityCenterHelpPhone|String|Die Telefonnummer oder die Skype-ID, die Benutzern angezeigt wird.|
|defenderSecurityCenterHelpURL|String|Die URL des Hilfe Portals, die für Benutzer angezeigt wird.|
|defenderSecurityCenterNotificationsFromApp|[defenderSecurityCenterNotificationsFromAppType](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|Benachrichtigungen, die aus den angezeigten Bereichen der App angezeigt werden sollen. Mögliche Werte sind: `notConfigured`, `blockNoncriticalNotifications` und `blockAllNotifications`.|
|defenderSecurityCenterITContactDisplay|[defenderSecurityCenterITContactDisplayType](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|Konfigurieren Sie, wo die IT-Kontaktinformationen Endbenutzern angezeigt werden sollen. Mögliche Werte sind: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp` und `displayOnlyInNotifications`.|
|firewallBlockStatefulFTP|Boolesch|Blockiert statusbehaftete FTP-Verbindungen mit dem Gerät.|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|Konfiguriert das Leerlauftimeout für Sicherheitszuordnungen in Sekunden, von 300 bis einschließlich 3600. Dies ist der Zeitraum, nach dem Sicherheitszuordnungen ablaufen und gelöscht werden. Gültige Werte: 300 bis 3600.|
|firewallPreSharedKeyEncodingMethod|[firewallPreSharedKeyEncodingMethodType](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|Wählen Sie die zu verwendende vorinstallierte Tasten Codierung aus. Mögliche Werte sind: `deviceDefault`, `none` und `utF8`.|
|firewallIPSecExemptionsAllowNeighborDiscovery|Boolesch|Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Nachbarsuche zulässig sind.|
|firewallIPSecExemptionsAllowICMP|Boolesch|Konfiguriert IPSec-Ausnahmen, sodass ICMP zulässig ist.|
|firewallIPSecExemptionsAllowRouterDiscovery|Boolesch|Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Routersuche zulässig sind.|
|firewallIPSecExemptionsAllowDHCP|Boolesch|Konfiguriert IPSec-Ausnahmen, sodass sowohl IPv4-basierter als auch IPv6-basierter DHC-Datenverkehr zulässig ist.|
|firewallCertificateRevocationListCheckMethod|[firewallCertificateRevocationListCheckMethodType](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|Geben Sie an, wie die Zertifikatssperrliste erzwungen werden soll. Mögliche Werte sind: `deviceDefault`, `none`, `attempt` und `require`.|
|firewallMergeKeyingModuleSettings|Boolean|Wenn ein Authentifizierungssatz nicht vollständig von einem Schlüsselerstellungsmodul unterstützt wird, weist diese Einstellung das Modul an, nur nicht unterstützte Authentifizierungssuites zu ignorieren und nicht den gesamten Satz.|
|firewallPacketQueueingMethod|[firewallPacketQueueingMethodType](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|Konfiguriert, wie Paketwarteschlangen im Tunnel Gateway-Szenario angewendet werden sollen. Mögliche Werte: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Konfiguriert die Firewallprofileinstellungen für Domänennetzwerke.|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Konfiguriert die Firewallprofileinstellungen für öffentliche Netzwerke.|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Konfiguriert die Firewallprofileinstellungen für private Netzwerke.|
|defenderAdobeReaderLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der das Verhalten von Adobe Reader beim Erstellen von untergeordneten Prozessen angibt. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderAttackSurfaceReductionExcludedPaths|Zeichenfolgenauflistung|Liste von EXE-Dateien und Ordnern, die von Regeln zur Verringerung der Angriffsfläche ausgenommen werden sollen|
|defenderOfficeAppsOtherProcessInjectionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der das Verhalten von Office-Anwendungen angibt, das in andere Prozesse einfügt. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderOfficeAppsOtherProcessInjection|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der das Verhalten von Office-Anwendungen angibt, das in andere Prozesse einfügt. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderOfficeCommunicationAppsLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der das Verhalten von Office-Kommunikationsanwendungen, einschließlich Microsoft Outlook, zum Erstellen von untergeordneten Prozessen angibt. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderOfficeAppsExecutableContentCreationOrLaunchType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der das Verhalten von Office-Anwendungen/-Makros angibt, die ausführbare Inhalte erstellen oder starten. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderOfficeAppsExecutableContentCreationOrLaunch|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der das Verhalten von Office-Anwendungen/-Makros angibt, die ausführbare Inhalte erstellen oder starten. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderOfficeAppsLaunchChildProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der das Verhalten der Office-Anwendung startet untergeordnete Prozesse. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderOfficeAppsLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der das Verhalten der Office-Anwendung startet untergeordnete Prozesse. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderOfficeMacroCodeAllowWin32ImportsType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der das Verhalten von Win32-Importen aus Makrocode in Office angibt. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderOfficeMacroCodeAllowWin32Imports|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der das Verhalten von Win32-Importen aus Makrocode in Office angibt. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderScriptObfuscatedMacroCodeType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der das Verhalten von verschleierten js/VBS/PS/Macro-Code angibt. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderScriptObfuscatedMacroCode|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der das Verhalten von verschleierten js/VBS/PS/Macro-Code angibt. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderScriptDownloadedPayloadExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der das Verhalten von JS/VBS ausführt, das aus dem Internet heruntergeladen wird. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderScriptDownloadedPayloadExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der das Verhalten von JS/VBS ausführt, das aus dem Internet heruntergeladen wird. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderPreventCredentialStealingType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der angibt, ob das unter System für die Windows Local Security Authority gestohlen werden darf. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderProcessCreationType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der die Antwort auf Prozess Kreationen aus PSExec und WMI-Befehlen angibt. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderProcessCreation|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der die Antwort auf Prozess Kreationen aus PSExec und WMI-Befehlen angibt. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderUntrustedUSBProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der die Antwort auf nicht vertrauenswürdige und nicht signierte Prozesse angibt, die von USB ausgeführt werden. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderUntrustedUSBProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der die Antwort auf nicht vertrauenswürdige und nicht signierte Prozesse angibt, die von USB ausgeführt werden. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderUntrustedExecutableType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der die Antwort auf ausführbare Dateien angibt, die den Kriterien Prävalenz, Alter oder Vertrauenswürdige Listen nicht entsprechen. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderUntrustedExecutable|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der die Antwort auf ausführbare Dateien angibt, die den Kriterien Prävalenz, Alter oder Vertrauenswürdige Listen nicht entsprechen. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderEmailContentExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Wert, der angibt, ob die Ausführung von ausführbaren Inhalten (exe, dll, PS, JS, VBS usw.) aus e-Mail (Webmail/Mail-Client) gelöscht werden soll. Mögliche Werte sind: `userDefined`, `block` und `auditMode`.|
|defenderEmailContentExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der angibt, ob die Ausführung von ausführbaren Inhalten (exe, dll, PS, JS, VBS usw.) aus e-Mail (Webmail/Mail-Client) gelöscht werden soll. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderAdvancedRansomewareProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der die Verwendung von erweitertem Schutz gegen ransomeware angibt. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderGuardMyFoldersType|[folderProtectionType](../resources/intune-deviceconfig-folderprotectiontype.md)|Wert, der das Verhalten von geschützten Ordnern angibt. Mögliche Werte: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.|
|defenderGuardedFoldersAllowedAppPaths|String collection|Liste von Pfaden zu EXE-Dateien, die auf geschützte Ordner zugreifen dürfen|
|defenderAdditionalGuardedFolders|Zeichenfolgenauflistung|Liste von Ordnerpfaden, die der Liste der geschützter Ordner hinzugefügt werden sollen|
|defenderNetworkProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Wert, der das Verhalten von NetworkProtection angibt. Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.|
|defenderExploitProtectionXml|Binär|XML-Inhalte mit Details zum Exploit-Schutz|
|defenderExploitProtectionXmlFileName|String|Name der Datei, aus der „DefenderExploitProtectionXml“ abgerufen wurde|
|defenderSecurityCenterBlockExploitProtectionOverride|Boolean|Gibt an, ob verhindert werden soll, dass Benutzer die Einstellungen für den Exploit-Schutz überschreiben.|
|appLockerApplicationControl|[appLockerApplicationControlType](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|Ermöglicht dem Administrator die Festlegung der auf Geräten zulässigen Typen von Apps. Mögliche Werte sind: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker` und `auditComponentsStoreAppsAndSmartlocker`.|
|deviceGuardLocalSystemAuthorityCredentialGuardSettings|[deviceGuardLocalSystemAuthorityCredentialGuardType](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|Aktivieren Sie die Aktivierung der Anmeldeinformationen, wenn die Platt Form sicherheitsStufe mit Secure Boot-und Virtualisierungs-basierter Sicherheit aktiviert ist. Mögliche Werte sind: `notConfigured`, `enableWithUEFILock` und `enableWithoutUEFILock`.|
|deviceGuardEnableVirtualizationBasedSecurity|Boolesch|Aktiviert die Virtualisierungs-basierte Sicherheit (VBS).|
|deviceGuardEnableSecureBootWithDMA|Boolesch|Gibt an, ob die Platt Form sicherheitsStufe beim nächsten Neustart aktiviert ist.|
|deviceGuardLaunchSystemGuard|[Aktivierung](../resources/intune-shared-enablement.md)|Ermöglicht es dem IT-Administrator, den Start von System Guard zu konfigurieren. Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.|
|smartScreenEnableInShell|Boolesch|Ermöglicht IT-Administratoren die Konfiguration von SmartScreen für Windows.|
|smartScreenBlockOverrideForFiles|Boolesch|Ermöglicht es IT-Administratoren, zu steuern, ob Benutzer SmartScreen-Warnungen ignorieren und Schaddateien ausführen dürfen.|
|applicationGuardEnabled|Boolesch|Aktiviert Windows Defender Application Guard.|
|applicationGuardEnabledOptions|[applicationGuardEnabledOptions](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|Aktivieren Sie Windows Defender Application Guard für neuere Windows-Builds. Mögliche Werte sind: `notConfigured`, `enabledForEdge`, `enabledForOffice` und `enabledForEdgeAndOffice`.|
|applicationGuardBlockFileTransfer|[applicationGuardBlockFileTransferType](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|Zwischenablage zum Übertragen der Bilddatei, Textdatei oder keiner dieser Dateien blockieren. Mögliche Werte: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.|
|applicationGuardBlockNonEnterpriseContent|Boolesch|Unterbindet, dass Unternehmenswebsites unternehmensfremde Inhalte laden, z. B. Plug-Ins von Drittanbietern.|
|applicationGuardAllowPersistence|Boolesch|Erlaubt die dauerhafte Speicherung benutzergenerierter Daten im App Guard Container (Favoriten, Cookies, Webkennwörter usw.).|
|applicationGuardForceAuditing|Boolesch|Erzwingt die dauerhafte Speicherung von Windows-Protokollen und -Ereignissen durch die Überwachung zwecks Erfüllung von Sicherheits- und Compliancevorgaben (Beispielereignisse sind Benutzeranmeldungen und -abmeldungen, die Verwendung von Berechtigungen, die Installation von Software und Änderungen am System).|
|applicationGuardBlockClipboardSharing|[applicationGuardBlockClipboardSharingType](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|Blockiert die Freigabe von Zwischenablagedaten zwischen Host und Container, zwischen Container und Host, in beide Richtungen oder in keine Richtung. Mögliche Werte sind: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost` und `blockNone`.|
|applicationGuardAllowPrintToPDF|Boolesch|Erlaubt das Drucken im PDF-Format über Container.|
|applicationGuardAllowPrintToXPS|Boolesch|Erlaubt das Drucken im XPS-Format über Container.|
|applicationGuardAllowPrintToLocalPrinters|Boolesch|Erlaubt das Drucken mit lokalen Druckern über Container.|
|applicationGuardAllowPrintToNetworkPrinters|Boolesch|Erlaubt das Drucken mit Netzwerkdruckern über Container.|
|applicationGuardAllowVirtualGPU|Boolesch|Anwendungsschutz für die Verwendung virtueller GPU zulassen|
|applicationGuardAllowFileSaveOnHost|Boolesch|Benutzer können Dateien von Edge im Application Guard-Container herunterladen und im Hostdateisystem speichern.|
|bitLockerAllowStandardUserEncryption|Boolesch|Ermöglicht es dem Administrator, Standardbenutzern das Aktivieren von encrpytion während des Azure AD-Joins zu ermöglichen.|
|bitLockerDisableWarningForOtherDiskEncryption|Boolesch|Ermöglicht es dem Administrator, den Warnhinweis bezüglich anderer Festplattenverschlüsselungslösungen auf Benutzer-PCs zu deaktivieren.|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolean|Ermöglicht, dass der Administrator die Aktivierung der Verschlüsselung mittels BitLocker fordert. Diese Richtlinie gilt nur für Mobilgeräte-SKUs.|
|bitLockerEncryptDevice|Boolean|Ermöglicht, dass der Administrator die Aktivierung der Verschlüsselung mittels BitLocker fordert.|
|bitLockerSystemDrivePolicy|[bitLockerSystemDrivePolicy](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|BitLocker-System Laufwerk Richtlinie.|
|bitLockerFixedDrivePolicy|[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|BitLocker-Richtlinie für feste Laufwerke.|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|BitLocker-Richtlinie für Wechseldatenträger.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Sammlung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries|Sammlung von Objekten des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

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
  "dmaGuardDeviceEnumerationPolicy": "String",
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "String",
      "description": "String",
      "packageFamilyName": "String",
      "filePath": "String",
      "serviceName": "String",
      "protocol": 1024,
      "localPortRanges": [
        "String"
      ],
      "remotePortRanges": [
        "String"
      ],
      "localAddressRanges": [
        "String"
      ],
      "remoteAddressRanges": [
        "String"
      ],
      "profileTypes": "String",
      "action": "String",
      "trafficDirection": "String",
      "interfaceTypes": "String",
      "localUserAuthorizations": "String"
    }
  ],
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
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "String",
  "localSecurityOptionsDisableGuestAccount": true,
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
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
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
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
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
  "defenderAdobeReaderLaunchChildProcess": "String",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "String"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "String",
  "defenderOfficeAppsOtherProcessInjection": "String",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "String",
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
  "deviceGuardLaunchSystemGuard": "String",
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
  "bitLockerAllowStandardUserEncryption": true,
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




