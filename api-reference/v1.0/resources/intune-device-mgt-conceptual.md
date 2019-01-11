---
title: Geräteverwaltung in Microsoft Intune
description: ''
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 72ff8234696c8a6d1f74bd7468d24e98c54e5052
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868362"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="be305-102">Geräteverwaltung in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="be305-102">Device management in Microsoft Intune</span></span>

> <span data-ttu-id="be305-103">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="be305-103">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="be305-104">Aktionszustand</span><span class="sxs-lookup"><span data-stu-id="be305-104">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="be305-105">Apple Push Notification-Zertifikat</span><span class="sxs-lookup"><span data-stu-id="be305-105">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="be305-106">Audit-Akteur</span><span class="sxs-lookup"><span data-stu-id="be305-106">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="be305-107">Audit-Ereignis</span><span class="sxs-lookup"><span data-stu-id="be305-107">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="be305-108">Audit-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="be305-108">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="be305-109">Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="be305-109">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="be305-110">Compliance-Status</span><span class="sxs-lookup"><span data-stu-id="be305-110">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="be305-111">In Konfigurations-Manager-Client aktivierte Features</span><span class="sxs-lookup"><span data-stu-id="be305-111">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="be305-112">Benutzer von freigegebenem Apple-Gerät löschen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="be305-112">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="be305-113">Erkannte App</span><span class="sxs-lookup"><span data-stu-id="be305-113">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="be305-114">Ergebnis von Geräteaktion</span><span class="sxs-lookup"><span data-stu-id="be305-114">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="be305-115">Gerät Registrierung Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="be305-115">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="be305-116">Registrierung Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="be305-116">Device enrollment type</span></span>](intune-devices-deviceenrollmenttype.md)
- [<span data-ttu-id="be305-117">Exchange-Zugriffsstatus für Geräte – Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="be305-117">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="be305-118">Geräte-Geolocation</span><span class="sxs-lookup"><span data-stu-id="be305-118">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="be305-119">Integritätsnachweis für Geräte – Status</span><span class="sxs-lookup"><span data-stu-id="be305-119">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="be305-120">Verwaltung von Exchange Zugriff Gerätestatus</span><span class="sxs-lookup"><span data-stu-id="be305-120">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="be305-121">Gerät Management Exchange Access Zustand Grund</span><span class="sxs-lookup"><span data-stu-id="be305-121">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="be305-122">Management Abonnement-Gerätestatus</span><span class="sxs-lookup"><span data-stu-id="be305-122">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="be305-123">Problembehandlung bei Geräteverwaltung</span><span class="sxs-lookup"><span data-stu-id="be305-123">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="be305-124">Betriebssystem des Geräts – Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="be305-124">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="be305-125">Die Registrierung des Geräts</span><span class="sxs-lookup"><span data-stu-id="be305-125">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="be305-126">Problembehandlung bei Registrierung</span><span class="sxs-lookup"><span data-stu-id="be305-126">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="be305-127">Lokalisierte Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="be305-127">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="be305-128">Gerät suchen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="be305-128">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="be305-129">Verwaltetes Gerät</span><span class="sxs-lookup"><span data-stu-id="be305-129">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="be305-130">Verwaltete Geräte – Übersicht</span><span class="sxs-lookup"><span data-stu-id="be305-130">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="be305-131">Verwaltete Eigentümer Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="be305-131">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="be305-132">Verwaltete Gerät Partner gemeldet Integritätsstatus</span><span class="sxs-lookup"><span data-stu-id="be305-132">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="be305-133">Management Agent-Typ</span><span class="sxs-lookup"><span data-stu-id="be305-133">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="be305-134">Benachrichtigungsvorlage</span><span class="sxs-lookup"><span data-stu-id="be305-134">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="be305-135">Benachrichtigungsvorlage branding-Optionen</span><span class="sxs-lookup"><span data-stu-id="be305-135">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="be305-136">Remoteunterstützung auf mittels Fingereingabe status</span><span class="sxs-lookup"><span data-stu-id="be305-136">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="be305-137">Partner für Remoteunterstützung</span><span class="sxs-lookup"><span data-stu-id="be305-137">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="be305-138">Remotesperren – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="be305-138">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="be305-139">Kennung zurücksetzen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="be305-139">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="be305-140">Aktualisieren von Windows-Gerätekonto – Aktionsparameter</span><span class="sxs-lookup"><span data-stu-id="be305-140">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="be305-141">Windows Defender-Überprüfung – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="be305-141">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="be305-142">Windows-Gerät – Konto</span><span class="sxs-lookup"><span data-stu-id="be305-142">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="be305-143">Windows-Gerät – AD-Konto</span><span class="sxs-lookup"><span data-stu-id="be305-143">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="be305-144">Windows-Gerät – Azure AD-Konto</span><span class="sxs-lookup"><span data-stu-id="be305-144">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)
