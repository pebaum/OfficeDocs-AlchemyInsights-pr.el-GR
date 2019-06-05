---
title: Περιορισμός της πρόσβασης στο SharePoint ή OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5115a8eb6dd9cd25b556353b4f61f10ae4598ff6
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34718222"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Περιορισμός της πρόσβασης στο SharePoint ή OneDrive

<p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Υπάρχουν πολλοί τρόποι για να περιορίσετε την πρόσβαση σε υπηρεσίες SharePoint Online/OneDrive. Αυτές οι διάφορες μέθοδοι περιορισμού πρόσβασης περιγράφονται παρακάτω.</span></p> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Περιορισμός δικαιωμάτων</span></u></strong></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Στην ηλεκτρονική SharePoint και OneDrive για την επιχείρηση, μας περιορίσετε την πρόσβαση σε στοιχεία όπως τοποθεσίες, αρχεία και φακέλους παρέχοντας πρόσβαση σε αυτές τις ομάδες/άτομα που θα πρέπει να έχουν πρόσβαση μόνο.</span></p> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><a href="https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782">Προσαρμογή των δικαιωμάτων για μια λίστα ή βιβλιοθήκη SharePoint</a></span></li> </ul> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><a href="https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions">Προσαρμογή των δικαιωμάτων τοποθεσίας του SharePoint</a></span></li> </ul> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><a href="https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6">Αλλάξτε τα δικαιώματα σε έναν υποφάκελο</a></span></li> </ul> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Έλεγχος της πρόσβασης από μη διαχειριζόμενη συσκευές</span></u></strong></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Ως καθολικής διαχείρισης του Office 365 ή του SharePoint, μπορείτε να κάνετε <a href="https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices">Αποκλεισμός ή περιορισμός πρόσβασης σε περιεχόμενο του SharePoint και OneDrive από μη διαχειριζόμενη συσκευές</a> (αυτών υβριδική AD συνδεδεμένα ή συμβατός με στο Intune).</span></p> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Περιορισμός θέση δικτύου.</span></u></strong></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Ως ένας διαχειριστής IT, μπορείτε να ελέγξετε την πρόσβαση σε πόρους του SharePoint και OneDrive που βασίζονται σε αξιόπιστες τοποθεσίες δικτύου ορίζεται. Αυτό είναι επίσης γνωστό ως πολιτική που βασίζεται σε θέση. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα <a href="https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location">Έλεγχος της πρόσβασης σε ηλεκτρονική SharePoint και OneDrive δεδομένα με βάση τη θέση δικτύου</a></span></p> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Περιορισμού κλείδωμα τοποθεσίας</span></u></strong></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Εντός του SharePoint Online, έχετε τη δυνατότητα να κλειδώσετε μια συλλογή τοποθεσιών, ώστε κανείς να έχει πρόσβαση. &nbsp;Έχει οριστεί μέσω του PowerShell και την <a href="https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps">Ηλεκτρονική κέλυφος διαχείρισης του SharePoint</a> χρησιμοποιώντας το &ldquo; <em style="mso-bidi-font-style: normal;"><a href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps">Σύνολο SPOSite</a></em> <em style="mso-bidi-font-style: normal;"> -LockState</em> &rdquo; ιδιότητα.</span></p> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Περιορισμός των χρηστών από τη δημιουργία τοποθεσιών και δευτερευουσών τοποθεσιών</span></u></strong></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Ως διαχειριστής SharePoint ή καθολικής διαχείρισης του Office 365, μπορείτε να επιτρέψετε στους χρήστες σας να δημιουργήσετε και να διαχειριστείτε τις δικές τους τοποθεσίες του SharePoint, καθορίζουν το είδος των τοποθεσιών μπορούν να δημιουργήσουν, και καθορίστε τη θέση των τοποθεσιών. Για περισσότερες πληροφορίες, δείτε <a href="https://docs.microsoft.com/en-us/sharepoint/manage-site-creation">Διαχείριση δημιουργίας τοποθεσίας στο SharePoint Online</a>.</span></p>
