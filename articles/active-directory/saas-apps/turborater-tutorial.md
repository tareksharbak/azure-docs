﻿---
title: 'Tutorial: Azure Active Directory integration with TurboRater | Microsoft Docs'
description: Learn how to configure single sign-on between Azure Active Directory and TurboRater.
services: active-directory
documentationCenter: na
author: jeevansd
manager: mtillman
ms.reviewer: joflore

ms.assetid: abb116b8-8024-4cc6-bc81-f32ef490ea17
ms.service: active-directory
ms.component: saas-app-tutorial
ms.workload: identity
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: article
ms.date: 10/03/2017
ms.author: jeedes

---
# Tutorial: Azure Active Directory integration with TurboRater

In this tutorial, you learn how to integrate TurboRater with Azure Active Directory (Azure AD).

Integrating TurboRater with Azure AD provides you with the following benefits:

- You can control in Azure AD who has access to TurboRater.
- You can enable your users to automatically get signed-on to TurboRater (Single Sign-On) with their Azure AD accounts.
- You can manage your accounts in one central location - the Azure portal.

If you want to know more details about SaaS app integration with Azure AD, see [what is application access and single sign-on with Azure Active Directory](../manage-apps/what-is-single-sign-on.md).

## Prerequisites

To configure Azure AD integration with TurboRater, you need the following items:

- An Azure AD subscription
- A TurboRater single sign-on enabled subscription

> [!NOTE]
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

## Scenario description
In this tutorial, you test Azure AD single sign-on in a test environment. 
The scenario outlined in this tutorial consists of two main building blocks:

1. Adding TurboRater from the gallery
1. Configuring and testing Azure AD single sign-on

## Adding TurboRater from the gallery
To configure the integration of TurboRater into Azure AD, you need to add TurboRater from the gallery to your list of managed SaaS apps.

**To add TurboRater from the gallery, perform the following steps:**

1. In the **[Azure portal](https://portal.azure.com)**, on the left navigation panel, click **Azure Active Directory** icon. 

	![The Azure Active Directory button][1]

1. Navigate to **Enterprise applications**. Then go to **All applications**.

	![The Enterprise applications blade][2]
	
1. To add new application, click **New application** button on the top of dialog.

	![The New application button][3]

1. In the search box, type **TurboRater**, select **TurboRater** from result panel then click **Add** button to add the application.

	![TurboRater in the results list](./media/turborater-tutorial/tutorial_turborater_addfromgallery.png)

## Configure and test Azure AD single sign-on

In this section, you configure and test Azure AD single sign-on with TurboRater based on a test user called "Britta Simon".

For single sign-on to work, Azure AD needs to know what the counterpart user in TurboRater is to a user in Azure AD. In other words, a link relationship between an Azure AD user and the related user in TurboRater needs to be established.

In TurboRater, assign the value of the **user name** in Azure AD as the value of the **Username** to establish the link relationship.

To configure and test Azure AD single sign-on with TurboRater, you need to complete the following building blocks:

1. **[Configure Azure AD Single Sign-On](#configure-azure-ad-single-sign-on)** - to enable your users to use this feature.
1. **[Create an Azure AD test user](#create-an-azure-ad-test-user)** - to test Azure AD single sign-on with Britta Simon.
1. **[Create a TurboRater test user](#create-a-turborater-test-user)** - to have a counterpart of Britta Simon in TurboRater that is linked to the Azure AD representation of user.
1. **[Assign the Azure AD test user](#assign-the-azure-ad-test-user)** - to enable Britta Simon to use Azure AD single sign-on.
1. **[Test single sign-on](#test-single-sign-on)** - to verify whether the configuration works.

### Configure Azure AD single sign-on

In this section, you enable Azure AD single sign-on in the Azure portal and configure single sign-on in your TurboRater application.

**To configure Azure AD single sign-on with TurboRater, perform the following steps:**

1. In the Azure portal, on the **TurboRater** application integration page, click **Single sign-on**.

	![Configure single sign-on link][4]

1. On the **Single sign-on** dialog, select **Mode** as	**SAML-based Sign-on** to enable single sign-on.
 
	![Single sign-on dialog box](./media/turborater-tutorial/tutorial_turborater_samlbase.png)

1. On the **TurboRater Domain and URLs** section, perform the following steps:

	![TurboRater Domain and URLs single sign-on information](./media/turborater-tutorial/tutorial_turborater_url.png)

    a. In the **Identifier** textbox, type the value as: `https://www.itcdataservices.com`
 
    b. In the **Reply URL** textbox, type the value as:
	
	| Environment | URL |
	| ---------------| --------------- |    
	| Test  | `https://ratingqa.itcdataservices.com/webservices/imp/saml/login` |
	| Live  | `https://www.itcratingservices.com/webservices/imp/saml/login` |

1. On the **SAML Signing Certificate** section, click **Metadata XML** and then save the metadata file on your computer.

	![The Certificate download link](./media/turborater-tutorial/tutorial_turborater_certificate.png) 

1. Click **Save** button.

	![Configure Single Sign-On Save button](./media/turborater-tutorial/tutorial_general_400.png)

1. To configure single sign-on on **TurboRater** side, you need to send the downloaded **Metadata XML** to [TurboRater support team](https://www.getitc.com/support). They set this setting to have the SAML SSO connection set properly on both sides.

> [!TIP]
> You can now read a concise version of these instructions inside the [Azure portal](https://portal.azure.com), while you are setting up the app!  After adding this app from the **Active Directory > Enterprise Applications** section, simply click the **Single Sign-On** tab and access the embedded documentation through the **Configuration** section at the bottom. You can read more about the embedded documentation feature here: [Azure AD embedded documentation]( https://go.microsoft.com/fwlink/?linkid=845985)

### Create an Azure AD test user

The objective of this section is to create a test user in the Azure portal called Britta Simon.

   ![Create an Azure AD test user][100]

**To create a test user in Azure AD, perform the following steps:**

1. In the Azure portal, in the left pane, click the **Azure Active Directory** button.

    ![The Azure Active Directory button](./media/turborater-tutorial/create_aaduser_01.png)

1. To display the list of users, go to **Users and groups**, and then click **All users**.

    ![The "Users and groups" and "All users" links](./media/turborater-tutorial/create_aaduser_02.png)

1. To open the **User** dialog box, click **Add** at the top of the **All Users** dialog box.

    ![The Add button](./media/turborater-tutorial/create_aaduser_03.png)

1. In the **User** dialog box, perform the following steps:

    ![The User dialog box](./media/turborater-tutorial/create_aaduser_04.png)

    a. In the **Name** box, type **BrittaSimon**.

    b. In the **User name** box, type the email address of user Britta Simon.

    c. Select the **Show Password** check box, and then write down the value that's displayed in the **Password** box.

    d. Click **Create**.
  
### Create a TurboRater test user

To enable Azure AD users to log in to TurboRater, they must be provisioned into TurboRater.  
In the case of TurboRater, provisioning is a manual task.
To create a user, please work with [TurboRater support team](https://www.getitc.com/support).

### Assign the Azure AD test user

In this section, you enable Britta Simon to use Azure single sign-on by granting access to TurboRater.

![Assign the user role][200] 

**To assign Britta Simon to TurboRater, perform the following steps:**

1. In the Azure portal, open the applications view, and then navigate to the directory view and go to **Enterprise applications** then click **All applications**.

	![Assign User][201] 

1. In the applications list, select **TurboRater**.

	![The TurboRater link in the Applications list](./media/turborater-tutorial/tutorial_turborater_app.png)  

1. In the menu on the left, click **Users and groups**.

	![The "Users and groups" link][202]

1. Click **Add** button. Then select **Users and groups** on **Add Assignment** dialog.

	![The Add Assignment pane][203]

1. On **Users and groups** dialog, select **Britta Simon** in the Users list.

1. Click **Select** button on **Users and groups** dialog.

1. Click **Assign** button on **Add Assignment** dialog.
	
### Test single sign-on

In this section, you test your Azure AD single sign-on configuration using the Access Panel.

When you click the TurboRater tile in the Access Panel, you should get automatically signed-on to your TurboRater application.
For more information about the Access Panel, see [Introduction to the Access Panel](../user-help/active-directory-saas-access-panel-introduction.md). 

## Additional resources

* [List of Tutorials on How to Integrate SaaS Apps with Azure Active Directory](tutorial-list.md)
* [What is application access and single sign-on with Azure Active Directory?](../manage-apps/what-is-single-sign-on.md)



<!--Image references-->

[1]: ./media/turborater-tutorial/tutorial_general_01.png
[2]: ./media/turborater-tutorial/tutorial_general_02.png
[3]: ./media/turborater-tutorial/tutorial_general_03.png
[4]: ./media/turborater-tutorial/tutorial_general_04.png

[100]: ./media/turborater-tutorial/tutorial_general_100.png

[200]: ./media/turborater-tutorial/tutorial_general_200.png
[201]: ./media/turborater-tutorial/tutorial_general_201.png
[202]: ./media/turborater-tutorial/tutorial_general_202.png
[203]: ./media/turborater-tutorial/tutorial_general_203.png

