---
title: Zuordnen des Office 365-Kontos zu Azure AD zum Erstellen und Verwalten von Apps
description: 'Um die Anwendung zu authentifizieren, müssen Sie diese in Microsoft Azure Active Directory (Azure AD) registrieren. Hier werden die Office 365-Benutzerkonto- und Anwendungsinformationen gespeichert. Zum Verwalten von Azure AD über das Azure-Portal benötigen Sie ein Microsoft Azure-Abonnement. Sie können das Portal in Microsoft Azure zum Verwalten von Benutzern, Rollen und Apps verwenden.. '
localization_priority: Normal
ms.openlocfilehash: 815cc80fa8d25f52ac05a1bf80f9e9dfa89b9b4d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880157"
---
# <a name="associate-your-office-365-account-with-azure-ad-to-create-and-manage-apps"></a>Zuordnen des Office 365-Kontos zu Azure AD zum Erstellen und Verwalten von Apps

Um die Anwendung zu authentifizieren, müssen Sie diese in Microsoft Azure Active Directory (Azure AD) registrieren. Hier werden die Office 365-Benutzerkonto- und Anwendungsinformationen gespeichert. Zum Verwalten von Azure AD über das Azure-Portal benötigen Sie ein Microsoft Azure-Abonnement. Sie können das Portal in Microsoft Azure zum Verwalten von Benutzern, Rollen und Apps verwenden.. 

In diesem Artikel wird gezeigt, wie Sie Ihr Office 365-Konto zu Azure AD zuordnen, um Apps zu erstellen und zu verwalten.

 >**Hinweis:** In diesem Artikel wird Azure AD als Authentifizierungsanbieter für Ihre App verwendet. Wenn Sie den Azure AD v2.0-Endpunkt verwenden, müssen Sie diesen Schritt nicht durchführen. Weitere Informationen finden Sie unter [App-Authentifizierung mit Microsoft Graph](auth-overview.md).

## <a name="prerequisites"></a>Voraussetzungen

**Office 365 for Business-Konten**

Wenn Sie über kein Office 365 for Business-Konto verfügen, müssen Sie folgende Aktionen durchführen:

- Registrieren Sie sich für einen oben aufgeführten [Office 365 for Business-Plan](https://products.office.com/de-DE/business/compare-office-365-for-business-plans), oder
- [Nehmen Sie am Office 365 Entwicklerprogramm teil, und erhalten Sie ein kostenloses Abonnement für Office 365 für 1 Jahr](https://aka.ms/devprogramsignup).

**Microsoft Azure-Abonnement** 

- Wenn Sie über ein Microsoft Azure-Abonnement verfügen, können Sie dieses zu Ihrem Office 365 for Business-Abonnement zuordnen. 

- Andernfalls müssen Sie ein neues Azure-Abonnement erstellen und dieses Ihrem Office 365-Konto zuordnen, um Apps zu registrieren und zu verwalten.


<!---<a name="bk_AssociateExistingAzureSubscription"> </a>-->

## <a name="to-associate-an-existing-azure-subscription-with-your-office-365-account"></a>So ordnen Sie ein vorhandenes Azure-Abonnement zu Ihrem Office 365-Konto zu


1. Melden Sie sich bei dem [Microsoft Azure-Portal](https://portal.azure.com) mit Ihren vorhandenen Azure-Anmeldeinformationen an (z. B. Microsoft-ID wie user@live.com).
        
2. Wählen Sie **Active Directory**, und wählen Sie dann die Registerkarte **Verzeichnis**, und wählen Sie am unteren Rand des Bildschirms **Neu**. 
     
4. Wählen Sie im Menü **Neu**die Option **Active Directory**  >  **Verzeichnis**  >  **Benutzerdefiniert erstellen**.
    
5. Wählen Sie unter **Verzeichnis hinzufügen** in der Dropdownliste **Verzeichnis** die Option **Bestehendes Verzeichnis verwenden** aus. Aktivieren Sie das Kontrollkästchen **Ich bin jetzt für die Abmeldung bereit** in der unteren rechten Ecke. 
    
    Damit kehren Sie zum Azure-Portal zurück.
        
3. Melden Sie sich mit Ihren Office 365-Kontoinformationen an. 
    
    Sie werden gefragt, ob Sie das Verzeichnis mit Azure verwenden möchten. 
    
    >**Wichtig:** Zum Zuordnen Ihres Office 365-Kontos zu Azure AD benötigen Sie ein Office 365 Business-Konto mit globalen Administratorrechten. 
    
        
4. Wählen Sie  **Weiter**, und klicken Sie dann auf **Jetzt abmelden**.
        
5. Schließen Sie den Browser, und öffnen Sie das [Portal](https://manage.windowsazure.com) erneut. Andernfalls erhalten Sie die Fehlermeldung, dass der Zugriff verweigert wurde.
    
        
6. Melden Sie sich erneut mit Ihren vorhandenen Azure-Anmeldeinformationen an (z. B. Microsoft-ID wie user@live.com). Navigieren Sie zum Knoten **Active Directory**. Unter **Verzeichnis** sollte jetzt Ihr Office 365-Konto aufgeführt sein.
    

<!--<a name="bk_AssociateNewAzureSubscription"> </a>-->

## <a name="to-create-a-new-azure-subscription-and-associate-it-with-your-office-365-account"></a>So erstellen Sie ein neues Azure-Abonnements und ordnen es Ihrem Office 365-Konto zu


1. Melden Sie sich bei Office 365 an. Wählen Sie auf der Seite **Start** das Symbol **Admin**, um das Office 365 Admin Center zu öffnen.
2. Scrollen Sie auf der Menüseite auf der linken Seite bis **Admin** nach unten, und wählen Sie **Azure AD**.

    >**Wichtig:** Zum Öffnen des Office 365 Admin Centers und zum Zugreifen auf Azure AD benötigen Sie ein Office 365 Business-Konto mit globalen Administratorrechten. 
    
3. Erstellen Sie ein neues Abonnement.
        
    Wenn Sie eine Testversion von Office 365 verwenden, wird eine Meldung mit dem Hinweis angezeigt, dass Azure AD nur für Kunden mit kostenpflichtigen Diensten verfügbar ist. Sie können ein 30-tägiges kostenloses Azure-Abonnement erstellen, Sie müssen dann jedoch einige zusätzliche Schritte ausführen:
    
    1. Wählen Sie Ihr Land oder Ihre Region aus und wählen Sie dann **Azure-Abonnement**.
    2. Geben Sie ihre persönlichen Daten an. Geben Sie zu Verifizierungszwecken eine Telefonnummer ein, unter der Sie erreichbar sind, und geben Sie an, ob diese per Textnachricht oder Anruf erfolgen soll.
    3. Wenn Sie Ihren Verifizierungscode erhalten, geben Sie ihn ein und wählen Sie **Code verifizieren**.
    4. Geben Sie Zahlungsinformationen ein, überprüfen Sie die Vereinbarung, und wählen Sie **Registrieren**.
        
        Ihre Kreditkarte wird nicht belastet.
        
        Schließen bzw. aktualisieren Sie nicht Ihren Browser, während Ihr Azure-Abonnement erstellt wird.
            
4. Wählen Sie nach Erstellung des Azure-Abonnements **Portal** aus.
        
5. Azure Tour wird angezeigt. Sie können Azure Tour anzeigen oder**X** wählen, um es zu schließen.
        
    Jetzt sollten alle Elemente im Azure-Abonnement angezeigt werden. Es wird ein Verzeichnis mit dem Namen Ihres Office 365-Mandanten aufgeführt.
    
## <a name="see-also"></a>Siehe auch
- [Grundlegendes zur Registrierung einer Anwendung in Azure AD](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad)
- [Hinzufügen, Aktualisieren oder Entfernen einer Anwendung in Azure AD](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-integrating-applications/)
