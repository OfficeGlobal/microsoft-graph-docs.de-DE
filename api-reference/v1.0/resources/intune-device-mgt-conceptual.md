---
title: Geräteverwaltung in Microsoft Intune
description: ''
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4c8f6676647405e8186e9d27466266f6690e2cd1
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250068"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="938c5-102">Geräteverwaltung in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="938c5-102">Device management in Microsoft Intune</span></span>

> <span data-ttu-id="938c5-103">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="938c5-103">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="938c5-104">Aktionszustand</span><span class="sxs-lookup"><span data-stu-id="938c5-104">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="938c5-105">Apple Push Notification-Zertifikat</span><span class="sxs-lookup"><span data-stu-id="938c5-105">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="938c5-106">Audit-Akteur</span><span class="sxs-lookup"><span data-stu-id="938c5-106">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="938c5-107">Audit-Ereignis</span><span class="sxs-lookup"><span data-stu-id="938c5-107">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="938c5-108">Audit-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="938c5-108">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="938c5-109">Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="938c5-109">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="938c5-110">Compliance-Status</span><span class="sxs-lookup"><span data-stu-id="938c5-110">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="938c5-111">In Konfigurations-Manager-Client aktivierte Features</span><span class="sxs-lookup"><span data-stu-id="938c5-111">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="938c5-112">Benutzer von freigegebenem Apple-Gerät löschen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="938c5-112">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="938c5-113">Erkannte App</span><span class="sxs-lookup"><span data-stu-id="938c5-113">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="938c5-114">Ergebnis von Geräteaktion</span><span class="sxs-lookup"><span data-stu-id="938c5-114">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="938c5-115">Grund des Geräteregistrierungsfehlers</span><span class="sxs-lookup"><span data-stu-id="938c5-115">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="938c5-116">Exchange-Zugriffsstatus für Geräte – Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="938c5-116">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="938c5-117">Geräte-Geolocation</span><span class="sxs-lookup"><span data-stu-id="938c5-117">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="938c5-118">Integritätsnachweis für Geräte – Status</span><span class="sxs-lookup"><span data-stu-id="938c5-118">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="938c5-119">Exchange-Zugriffsstatus für Geräteverwaltung</span><span class="sxs-lookup"><span data-stu-id="938c5-119">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="938c5-120">Exchange-Zugriffsstatusgrund für Geräteverwaltung</span><span class="sxs-lookup"><span data-stu-id="938c5-120">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="938c5-121">Status des Abonnements der Geräteverwaltung</span><span class="sxs-lookup"><span data-stu-id="938c5-121">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="938c5-122">Problembehandlung bei Geräteverwaltung</span><span class="sxs-lookup"><span data-stu-id="938c5-122">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="938c5-123">Betriebssystem des Geräts – Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="938c5-123">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="938c5-124">Status der Geräteregistrierung</span><span class="sxs-lookup"><span data-stu-id="938c5-124">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="938c5-125">Problembehandlung bei Registrierung</span><span class="sxs-lookup"><span data-stu-id="938c5-125">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="938c5-126">Lokalisierte Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="938c5-126">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="938c5-127">Gerät suchen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="938c5-127">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="938c5-128">Verwaltetes Gerät</span><span class="sxs-lookup"><span data-stu-id="938c5-128">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="938c5-129">Verwaltete Geräte – Übersicht</span><span class="sxs-lookup"><span data-stu-id="938c5-129">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="938c5-130">Besitzertyp für verwaltetes Gerät</span><span class="sxs-lookup"><span data-stu-id="938c5-130">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="938c5-131">Vom Partner gemeldeter Integritätsstatus für verwaltetes Gerät</span><span class="sxs-lookup"><span data-stu-id="938c5-131">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="938c5-132">Verwaltungs-Agenttyp</span><span class="sxs-lookup"><span data-stu-id="938c5-132">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="938c5-133">Benachrichtigungsvorlage</span><span class="sxs-lookup"><span data-stu-id="938c5-133">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="938c5-134">Brandingoptionen der Nachrichtenvorlage</span><span class="sxs-lookup"><span data-stu-id="938c5-134">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="938c5-135">Onboardingstatus für Remoteunterstützung</span><span class="sxs-lookup"><span data-stu-id="938c5-135">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="938c5-136">Partner für Remoteunterstützung</span><span class="sxs-lookup"><span data-stu-id="938c5-136">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="938c5-137">Remotesperren – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="938c5-137">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="938c5-138">Kennung zurücksetzen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="938c5-138">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="938c5-139">Aktualisieren von Windows-Gerätekonto – Aktionsparameter</span><span class="sxs-lookup"><span data-stu-id="938c5-139">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="938c5-140">Windows Defender-Überprüfung – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="938c5-140">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="938c5-141">Windows-Gerät – Konto</span><span class="sxs-lookup"><span data-stu-id="938c5-141">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="938c5-142">Windows-Gerät – AD-Konto</span><span class="sxs-lookup"><span data-stu-id="938c5-142">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="938c5-143">Windows-Gerät – Azure AD-Konto</span><span class="sxs-lookup"><span data-stu-id="938c5-143">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)
