---
title: Abrufen von „windows10EndpointProtectionConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs windows10EndpointProtectionConfiguration.
ms.openlocfilehash: 21e8dc71524f32317fd2e89f8bfd78d2271e83d9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059201"
---
# <a name="get-windows10endpointprotectionconfiguration"></a>Abrufen von „windows10EndpointProtectionConfiguration“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).
## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.
## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Accept|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) im Antworttext zurück.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 27756

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
    "id": "09709403-9403-0970-0394-700903947009",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "userRightsAccessCredentialManagerAsTrustedCaller": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsAllowAccessFromNetwork": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsBlockAccessFromNetwork": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsActAsPartOfTheOperatingSystem": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsLocalLogOn": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsBackupData": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsChangeSystemTime": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsCreateGlobalObjects": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsCreatePageFile": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsCreatePermanentSharedObjects": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsCreateSymbolicLinks": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsCreateToken": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsDebugPrograms": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsRemoteDesktopServicesLogOn": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsDelegation": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsGenerateSecurityAudits": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsImpersonateClient": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsIncreaseSchedulingPriority": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsLoadUnloadDrivers": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsLockMemory": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsManageAuditingAndSecurityLogs": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsManageVolumes": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsModifyFirmwareEnvironment": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsModifyObjectLabels": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsProfileSingleProcess": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsRemoteShutdown": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsRestoreData": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsTakeOwnership": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsRegisterProcessAsService": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "xboxServicesEnableXboxGameSaveTask": true,
    "xboxServicesAccessoryManagementServiceStartupMode": "automatic",
    "xboxServicesLiveAuthManagerServiceStartupMode": "automatic",
    "xboxServicesLiveGameSaveServiceStartupMode": "automatic",
    "xboxServicesLiveNetworkingServiceStartupMode": "automatic",
    "localSecurityOptionsBlockMicrosoftAccounts": true,
    "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
    "localSecurityOptionsEnableAdministratorAccount": true,
    "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
    "localSecurityOptionsEnableGuestAccount": true,
    "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
    "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
    "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
    "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
    "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "administrators",
    "localSecurityOptionsMachineInactivityLimit": 10,
    "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
    "localSecurityOptionsDoNotRequireCtrlAltDel": true,
    "localSecurityOptionsHideLastSignedInUser": true,
    "localSecurityOptionsHideUsernameAtSignIn": true,
    "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
    "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
    "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
    "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
    "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
    "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "requireNtmlV2SessionSecurity",
    "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "requireNtmlV2SessionSecurity",
    "lanManagerAuthenticationLevel": "lmNtlmAndNtlmV2",
    "lanManagerWorkstationEnableInsecureGuestLogons": true,
    "localSecurityOptionsClearVirtualMemoryPageFile": true,
    "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
    "localSecurityOptionsAllowUIAccessApplicationElevation": true,
    "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
    "localSecurityOptionsOnlyElevateSignedExecutables": true,
    "localSecurityOptionsAdministratorElevationPromptBehavior": "elevateWithoutPrompting",
    "localSecurityOptionsStandardUserElevationPromptBehavior": "automaticallyDenyElevationRequests",
    "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
    "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
    "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
    "localSecurityOptionsUseAdminApprovalMode": true,
    "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
    "localSecurityOptionsInformationShownOnLockScreen": "userDisplayNameDomainUser",
    "localSecurityOptionsInformationDisplayedOnLockScreen": "administrators",
    "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
    "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
    "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
    "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
    "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
    "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
    "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
    "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
    "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
    "localSecurityOptionsSmartCardRemovalBehavior": "noAction",
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
    "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
    "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
    "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
    "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
    "defenderSecurityCenterNotificationsFromApp": "blockNoncriticalNotifications",
    "defenderSecurityCenterITContactDisplay": "displayInAppAndInNotifications",
    "firewallBlockStatefulFTP": true,
    "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
    "firewallPreSharedKeyEncodingMethod": "none",
    "firewallIPSecExemptionsAllowNeighborDiscovery": true,
    "firewallIPSecExemptionsAllowICMP": true,
    "firewallIPSecExemptionsAllowRouterDiscovery": true,
    "firewallIPSecExemptionsAllowDHCP": true,
    "firewallCertificateRevocationListCheckMethod": "none",
    "firewallMergeKeyingModuleSettings": true,
    "firewallPacketQueueingMethod": "disabled",
    "firewallProfileDomain": {
      "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
      "firewallEnabled": "blocked",
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
      "firewallEnabled": "blocked",
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
      "firewallEnabled": "blocked",
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
      "Defender Attack Surface Reduction Excluded Paths value"
    ],
    "defenderOfficeAppsOtherProcessInjectionType": "block",
    "defenderOfficeAppsOtherProcessInjection": "enable",
    "defenderOfficeAppsExecutableContentCreationOrLaunchType": "block",
    "defenderOfficeAppsExecutableContentCreationOrLaunch": "enable",
    "defenderOfficeAppsLaunchChildProcessType": "block",
    "defenderOfficeAppsLaunchChildProcess": "enable",
    "defenderOfficeMacroCodeAllowWin32ImportsType": "block",
    "defenderOfficeMacroCodeAllowWin32Imports": "enable",
    "defenderScriptObfuscatedMacroCodeType": "block",
    "defenderScriptObfuscatedMacroCode": "enable",
    "defenderScriptDownloadedPayloadExecutionType": "block",
    "defenderScriptDownloadedPayloadExecution": "enable",
    "defenderPreventCredentialStealingType": "enable",
    "defenderProcessCreationType": "block",
    "defenderProcessCreation": "enable",
    "defenderUntrustedUSBProcessType": "block",
    "defenderUntrustedUSBProcess": "enable",
    "defenderUntrustedExecutableType": "block",
    "defenderUntrustedExecutable": "enable",
    "defenderEmailContentExecutionType": "block",
    "defenderEmailContentExecution": "enable",
    "defenderAdvancedRansomewareProtectionType": "enable",
    "defenderGuardMyFoldersType": "enable",
    "defenderGuardedFoldersAllowedAppPaths": [
      "Defender Guarded Folders Allowed App Paths value"
    ],
    "defenderAdditionalGuardedFolders": [
      "Defender Additional Guarded Folders value"
    ],
    "defenderNetworkProtectionType": "enable",
    "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
    "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
    "defenderSecurityCenterBlockExploitProtectionOverride": true,
    "appLockerApplicationControl": "enforceComponentsAndStoreApps",
    "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "enableWithUEFILock",
    "deviceGuardEnableVirtualizationBasedSecurity": true,
    "deviceGuardEnableSecureBootWithDMA": true,
    "smartScreenEnableInShell": true,
    "smartScreenBlockOverrideForFiles": true,
    "applicationGuardEnabled": true,
    "applicationGuardEnabledOptions": "enabledForEdge",
    "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
    "applicationGuardBlockNonEnterpriseContent": true,
    "applicationGuardAllowPersistence": true,
    "applicationGuardForceAuditing": true,
    "applicationGuardBlockClipboardSharing": "blockBoth",
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
      "encryptionMethod": "aesCbc256",
      "startupAuthenticationRequired": true,
      "startupAuthenticationBlockWithoutTpmChip": true,
      "startupAuthenticationTpmUsage": "required",
      "startupAuthenticationTpmPinUsage": "required",
      "startupAuthenticationTpmKeyUsage": "required",
      "startupAuthenticationTpmPinAndKeyUsage": "required",
      "minimumPinLength": 0,
      "recoveryOptions": {
        "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
        "blockDataRecoveryAgent": true,
        "recoveryPasswordUsage": "required",
        "recoveryKeyUsage": "required",
        "hideRecoveryOptions": true,
        "enableRecoveryInformationSaveToStore": true,
        "recoveryInformationToStore": "passwordOnly",
        "enableBitLockerAfterRecoveryInformationToStore": true
      },
      "prebootRecoveryEnableMessageAndUrl": true,
      "prebootRecoveryMessage": "Preboot Recovery Message value",
      "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
    },
    "bitLockerFixedDrivePolicy": {
      "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
      "encryptionMethod": "aesCbc256",
      "requireEncryptionForWriteAccess": true,
      "recoveryOptions": {
        "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
        "blockDataRecoveryAgent": true,
        "recoveryPasswordUsage": "required",
        "recoveryKeyUsage": "required",
        "hideRecoveryOptions": true,
        "enableRecoveryInformationSaveToStore": true,
        "recoveryInformationToStore": "passwordOnly",
        "enableBitLockerAfterRecoveryInformationToStore": true
      }
    },
    "bitLockerRemovableDrivePolicy": {
      "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
      "encryptionMethod": "aesCbc256",
      "requireEncryptionForWriteAccess": true,
      "blockCrossOrganizationWriteAccess": true
    }
  }
}
```




