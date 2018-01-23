# <a name="associate-your-office-365-account-with-azure-ad-to-create-and-manage-apps"></a><span data-ttu-id="1c403-101">Zuordnen des Office 365-Kontos zu Azure AD zum Erstellen und Verwalten von Apps</span><span class="sxs-lookup"><span data-stu-id="1c403-101">Associate your Office 365 account with Azure AD to create and manage apps</span></span>

<span data-ttu-id="1c403-p101">Um die Anwendung zu authentifizieren, müssen Sie diese in Microsoft Azure Active Directory (Azure AD) registrieren. Hier werden die Office 365-Benutzerkonto- und Anwendungsinformationen gespeichert. Zum Verwalten von Azure AD über das Azure-Portal benötigen Sie ein Microsoft Azure-Abonnement. Sie können das Portal in Microsoft Azure zum Verwalten von Benutzern, Rollen und Apps verwenden..</span><span class="sxs-lookup"><span data-stu-id="1c403-p101">To authenticate your applications using Microsoft Azure Active Directory (Azure AD), you need to register them in Azure AD. This is where Office 365 user account and application information is stored. To manage Azure AD through the Azure Management Portal, you need a Microsoft Azure subscription. You can use the management portal in Microsoft Azure to manage users, roles, and apps.</span></span> 

<span data-ttu-id="1c403-106">In diesem Artikel wird gezeigt, wie Sie Ihr Office 365-Konto zu Azure AD zuordnen, um Apps zu erstellen und zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="1c403-106">This article shows you how to associate your Office 365 account with Azure AD to create and manage apps.</span></span>

 ><span data-ttu-id="1c403-107">**Hinweis:** In diesem Artikel wird Azure AD als Authentifizierungsanbieter für Ihre App verwendet.</span><span class="sxs-lookup"><span data-stu-id="1c403-107">**Note:** This article uses Azure AD as the authentication provider for your app.</span></span> <span data-ttu-id="1c403-108">Wenn Sie den Azure AD v2.0-Endpunkt verwenden, müssen Sie diesen Schritt nicht durchführen.</span><span class="sxs-lookup"><span data-stu-id="1c403-108">Note: This article uses Azure AD as the authentication provider for your app. If you're using the Azure AD v2.0 endpoint, you don't need to perform this step. For more information, see App authentication with Microsoft Graph.</span></span> <span data-ttu-id="1c403-109">Weitere Informationen finden Sie unter [App-Authentifizierung mit Microsoft Graph](auth_overview.md).</span><span class="sxs-lookup"><span data-stu-id="1c403-109">For more information see [App authentication with Microsoft Graph](auth_overview.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c403-110">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1c403-110">Prerequisites</span></span>

<span data-ttu-id="1c403-111">**Office 365 for Business-Konten**</span><span class="sxs-lookup"><span data-stu-id="1c403-111">**Office 365 for business account**</span></span>

<span data-ttu-id="1c403-112">Wenn Sie über kein Office 365 for Business-Konto verfügen, müssen Sie folgende Aktionen durchführen:</span><span class="sxs-lookup"><span data-stu-id="1c403-112">If you don't have an existing Office 365 for business account, you can:</span></span>

- <span data-ttu-id="1c403-113">Registrieren Sie sich für einen oben aufgeführten [Office 365 for Business-Plan](http://products.office.com/de-DE/business/compare-office-365-for-business-plans), oder</span><span class="sxs-lookup"><span data-stu-id="1c403-113">Sign up for an [Office 365 for business plans](http://products.office.com/de-DE/business/compare-office-365-for-business-plans) listed above, or</span></span>
- <span data-ttu-id="1c403-114">[Nehmen Sie am Office 365 Entwicklerprogramm teil, und erhalten Sie ein kostenloses Abonnement für Office 365 für 1 Jahr](https://aka.ms/devprogramsignup).</span><span class="sxs-lookup"><span data-stu-id="1c403-114">[Join the Office 365 Developer Program and get a free 1 year subscription to Office 365](https://aka.ms/devprogramsignup).</span></span>

<span data-ttu-id="1c403-115">**Microsoft Azure-Abonnement**</span><span class="sxs-lookup"><span data-stu-id="1c403-115">**Microsoft Azure subscription**</span></span> 

- <span data-ttu-id="1c403-116">Wenn Sie über ein Microsoft Azure-Abonnement verfügen, können Sie dieses zu Ihrem Office 365 for Business-Abonnement zuordnen.</span><span class="sxs-lookup"><span data-stu-id="1c403-116">If you can have an existing Microsoft Azure subscription, you can associate your Office 365 for business subscription with it.</span></span> 

- <span data-ttu-id="1c403-117">Andernfalls müssen Sie ein neues Azure-Abonnement erstellen und dieses Ihrem Office 365-Konto zuordnen, um Apps zu registrieren und zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="1c403-117">Otherwise, you'll need to create a new Azure subscription and associate it with your Office 365 account in order to register and manage apps.</span></span>


<!---<a name="bk_AssociateExistingAzureSubscription"> </a>-->

## <a name="to-associate-an-existing-azure-subscription-with-your-office-365-account"></a><span data-ttu-id="1c403-118">So ordnen Sie ein vorhandenes Azure-Abonnement zu Ihrem Office 365-Konto zu</span><span class="sxs-lookup"><span data-stu-id="1c403-118">To associate an existing Azure subscription with your Office 365 account</span></span>


1. <span data-ttu-id="1c403-119">Melden Sie sich bei dem [Microsoft Azure-Portal](https://portal.azure.com) mit Ihren vorhandenen Azure-Anmeldeinformationen an (z. B. Microsoft-ID wie user@live.com).</span><span class="sxs-lookup"><span data-stu-id="1c403-119">Log on to the  [Microsoft Azure Management portal](https://portal.azure.com) with your existing Azure credentials (for example, your Microsoft ID such as user@live.com).</span></span>
        
2. <span data-ttu-id="1c403-120">Wählen Sie **Active Directory**, und wählen Sie dann die Registerkarte **Verzeichnis**, und wählen Sie am unteren Rand des Bildschirms **Neu**.</span><span class="sxs-lookup"><span data-stu-id="1c403-120">Select the  **Active Directory** node, then select the **Directory** tab and, at the bottom of the screen, select **New**.</span></span> 
     
4. <span data-ttu-id="1c403-121">Wählen Sie im Menü **Neu**die Option **Active Directory**  >  **Verzeichnis**  >  **Benutzerdefiniert erstellen**.</span><span class="sxs-lookup"><span data-stu-id="1c403-121">On the **New** menu, select **Active Directory** > **Directory** > **Custom Create**.</span></span>
    
5. <span data-ttu-id="1c403-122">Wählen Sie unter **Verzeichnis hinzufügen** in der Dropdownliste **Verzeichnis** die Option **Bestehendes Verzeichnis verwenden** aus.</span><span class="sxs-lookup"><span data-stu-id="1c403-122">In **Add directory**, in the **Directory** dropdown box, select  **Use existing directory**.</span></span> <span data-ttu-id="1c403-123">Aktivieren Sie das Kontrollkästchen **Ich bin jetzt für die Abmeldung bereit** in der unteren rechten Ecke.</span><span class="sxs-lookup"><span data-stu-id="1c403-123">In Add directory, in the Directory dropdown box, select  Use existing directory. Check **I am ready to be signed out**, and then select the check mark in the lower-right corner.</span></span> 
    
    <span data-ttu-id="1c403-124">Damit kehren Sie zum Azure-Portal zurück.</span><span class="sxs-lookup"><span data-stu-id="1c403-124">This brings you back to the Azure Management Portal.</span></span>
        
3. <span data-ttu-id="1c403-125">Melden Sie sich mit Ihren Office 365-Kontoinformationen an.</span><span class="sxs-lookup"><span data-stu-id="1c403-125">Log in with your Office 365 account information.</span></span> 
    
    <span data-ttu-id="1c403-126">Sie werden gefragt, ob Sie das Verzeichnis mit Azure verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="1c403-126">You will be prompted whether to use your directory with Azure.</span></span> 
    
    ><span data-ttu-id="1c403-127">**Wichtig:** Zum Zuordnen Ihres Office 365-Kontos zu Azure AD benötigen Sie ein Office 365 Business-Konto mit globalen Administratorrechten.</span><span class="sxs-lookup"><span data-stu-id="1c403-127">**Important:** To associate your Office 365 account with Azure AD, you'll need  an Office 365 business account with global administrator privileges.</span></span> 
    
        
4. <span data-ttu-id="1c403-128">Wählen Sie  **Weiter**, und klicken Sie dann auf **Jetzt abmelden**.</span><span class="sxs-lookup"><span data-stu-id="1c403-128">Select  **continue**, and then **Sign out now**.</span></span>
        
5. <span data-ttu-id="1c403-129">Schließen Sie den Browser, und öffnen Sie das [Portal](https://manage.windowsazure.com) erneut.</span><span class="sxs-lookup"><span data-stu-id="1c403-129">Close the browser and reopen the  portal. Otherwise, you will get an access denied error.</span></span> <span data-ttu-id="1c403-130">Andernfalls erhalten Sie die Fehlermeldung, dass der Zugriff verweigert wurde.</span><span class="sxs-lookup"><span data-stu-id="1c403-130">Close the browser and reopen the  portal. Otherwise, you will get an access denied error.</span></span>
    
        
6. <span data-ttu-id="1c403-131">Melden Sie sich erneut mit Ihren vorhandenen Azure-Anmeldeinformationen an (z. B. Microsoft-ID wie user@live.com).</span><span class="sxs-lookup"><span data-stu-id="1c403-131">Log on to the  Microsoft Azure Management portal with your existing Azure credentials (for example, your Microsoft ID such as user@live.com).</span></span> <span data-ttu-id="1c403-132">Navigieren Sie zum Knoten **Active Directory**. Unter **Verzeichnis** sollte jetzt Ihr Office 365-Konto aufgeführt sein.</span><span class="sxs-lookup"><span data-stu-id="1c403-132">Navigate to the **Active Directory** node and, under **Directory**, you should now see your Office 365 subscription.</span></span>
    

<!--<a name="bk_AssociateNewAzureSubscription"> </a>-->

## <a name="to-create-a-new-azure-subscription-and-associate-it-with-your-office-365-account"></a><span data-ttu-id="1c403-133">So erstellen Sie ein neues Azure-Abonnements und ordnen es Ihrem Office 365-Konto zu</span><span class="sxs-lookup"><span data-stu-id="1c403-133">To create a new Azure subscription and associate it with your Office 365 account</span></span>


1. <span data-ttu-id="1c403-134">Melden Sie sich bei Office 365 an.</span><span class="sxs-lookup"><span data-stu-id="1c403-134">Log on to your Office 365 account.</span></span> <span data-ttu-id="1c403-135">Wählen Sie auf der Seite **Start** das Symbol **Admin**, um das Office 365 Admin Center zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="1c403-135">Log on to Office 365. From the **Home** page, select the **Admin** icon to open the Office 365 admin center.</span></span>
2. <span data-ttu-id="1c403-136">Scrollen Sie auf der Menüseite auf der linken Seite bis **Admin** nach unten, und wählen Sie **Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="1c403-136">In the menu page along the left side of the page, scroll down to **Admin** and select **Azure AD**.</span></span>

    ><span data-ttu-id="1c403-137">**Wichtig:** Zum Öffnen des Office 365 Admin Centers und zum Zugreifen auf Azure AD benötigen Sie ein Office 365 Business-Konto mit globalen Administratorrechten.</span><span class="sxs-lookup"><span data-stu-id="1c403-137">**Important:** To open the Office 365 admin center, and access Azure AD, you'll need  an Office 365 business account with global administrator privileges.</span></span> 
    
3. <span data-ttu-id="1c403-138">Erstellen Sie ein neues Abonnement.</span><span class="sxs-lookup"><span data-stu-id="1c403-138">Create a new subscription.</span></span>
        
    <span data-ttu-id="1c403-p107">Wenn Sie eine Testversion von Office 365 verwenden, wird eine Meldung mit dem Hinweis angezeigt, dass Azure AD nur für Kunden mit kostenpflichtigen Diensten verfügbar ist. Sie können ein 30-tägiges kostenloses Azure-Abonnement erstellen, Sie müssen dann jedoch einige zusätzliche Schritte ausführen:</span><span class="sxs-lookup"><span data-stu-id="1c403-p107">If you're using a trial version of Office 365, you'll see a message telling you that Azure AD is limited to customers with paid services. You can still create a trial 30-day Azure subscription at no charge, but you'll need to perform a few extra steps:</span></span>
    
    1. <span data-ttu-id="1c403-141">Wählen Sie Ihr Land oder Ihre Region aus und wählen Sie dann **Azure-Abonnement**.</span><span class="sxs-lookup"><span data-stu-id="1c403-141">Select your country or region, and then choose **Azure subscription**.</span></span>
    2. <span data-ttu-id="1c403-p108">Geben Sie ihre persönlichen Daten an. Geben Sie zu Verifizierungszwecken eine Telefonnummer ein, unter der Sie erreichbar sind, und geben Sie an, ob diese per Textnachricht oder Anruf erfolgen soll.</span><span class="sxs-lookup"><span data-stu-id="1c403-p108">Enter your personal information. For verification purposes, enter a telephone number at which you can be reached, and specify whether you want to be sent a text message or called.</span></span>
    3. <span data-ttu-id="1c403-144">Wenn Sie Ihren Verifizierungscode erhalten, geben Sie ihn ein und wählen Sie **Code verifizieren**.</span><span class="sxs-lookup"><span data-stu-id="1c403-144">When you receive your verification code, enter it and choose **Verify code**.</span></span>
    4. <span data-ttu-id="1c403-145">Geben Sie Zahlungsinformationen ein, überprüfen Sie die Vereinbarung, und wählen Sie **Registrieren**.</span><span class="sxs-lookup"><span data-stu-id="1c403-145">Enter payment information, check the agreement, and select **Sign up**.</span></span>
        
        <span data-ttu-id="1c403-146">Ihre Kreditkarte wird nicht belastet.</span><span class="sxs-lookup"><span data-stu-id="1c403-146">Your credit card will not be charged.</span></span>
        
        <span data-ttu-id="1c403-147">Schließen bzw. aktualisieren Sie nicht Ihren Browser, während Ihr Azure-Abonnement erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="1c403-147">Do not close or refresh your browser while your Azure subscription is being created.</span></span>
            
4. <span data-ttu-id="1c403-148">Wählen Sie nach Erstellung des Azure-Abonnements **Portal** aus.</span><span class="sxs-lookup"><span data-stu-id="1c403-148">When your Azure subscription is created, choose  **Portal**.</span></span>
        
5. <span data-ttu-id="1c403-149">Azure Tour wird angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1c403-149">The Azure Tour appears.</span></span> <span data-ttu-id="1c403-150">Sie können Azure Tour anzeigen oder **X** wählen, um es zu schließen.</span><span class="sxs-lookup"><span data-stu-id="1c403-150">The Azure Tour appears. You can view it, or choose  **X** to close it.</span></span>
        
    <span data-ttu-id="1c403-p110">Jetzt sollten alle Elemente im Azure-Abonnement angezeigt werden. Es wird ein Verzeichnis mit dem Namen Ihres Office 365-Mandanten aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="1c403-p110">You should now see all items in your Azure subscription. It lists a directory with the name of your Office 365 tenant.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="1c403-153">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="1c403-153">See also</span></span>
- [<span data-ttu-id="1c403-154">Grundlegendes zur Registrierung einer Anwendung in Azure AD</span><span class="sxs-lookup"><span data-stu-id="1c403-154">Basics of Registering an Application in Azure AD</span></span>](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad)
- [<span data-ttu-id="1c403-155">Hinzufügen, Aktualisieren oder Entfernen einer Anwendung in Azure AD</span><span class="sxs-lookup"><span data-stu-id="1c403-155">Add, update, or remove an application in Azure AD</span></span>](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-integrating-applications/)