---
title: Ομοσπονδία ADFS πιστοποιητικού που λήγει
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c608489be8497233d9d4f87ec53649026b823250
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28290798"
---
# <a name="adfs-federation-certificate-expiring"></a>Ομοσπονδία ADFS πιστοποιητικού που λήγει

Για να επιλύσετε αυτό το ζήτημα, ακολουθήστε τα εξής βήματα:
  
1. Εγκαταστήστε το Microsoft Azure Active Directory λειτουργική μονάδα για Windows PowerShell στον υπολογιστή (Εάν η λειτουργική μονάδα δεν είναι ήδη εγκατεστημένο). Για να γίνει αυτό, μεταβείτε στην [Διαχείριση AD Azure χρησιμοποιώντας το Windows PowerShell](https://aka.ms/aadposh).
    
2. Ακολουθήστε τα βήματα του "σενάριο 1: λήξει το πιστοποιητικό υπογραφής διακριτικό AD FS" ενότητα ["Παρουσιάστηκε ένα πρόβλημα κατά την πρόσβαση στην τοποθεσία" σφάλμα από AD FS όταν μια ομόσπονδη χρήστης υπογράφει Office 365, Azure, ή Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
3. Ακολουθήστε τα βήματα στο [πώς μπορείτε να ενημερώσετε ή να επιδιορθώσετε τις ρυθμίσεις ομόσπονδη τομέα στο Office 365, Azure, ή Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
    Για να μάθετε περισσότερα σχετικά με την ανανέωση πιστοποιητικών Ομοσπονδία, ανατρέξτε στην ενότητα " [Ανανέωση πιστοποιητικών Ομοσπονδία για Office 365 και Azure υπηρεσίας καταλόγου Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs)".
    
