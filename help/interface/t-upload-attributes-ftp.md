---
description: Leer hoe u klantkenmerkgegevens uploadt via FTP naar de Experience Cloud.
solution: Experience Cloud
title: Upload het bestand met klantkenmerkgegevens via FTP
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: ed9e4a8f-493a-4a0f-a87e-674c7da95b99
source-git-commit: eb2ad8a8255915be47b6002a78cc810b522170d2
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Optioneel - Het gegevensbestand uploaden via FTP

Als u niet uploadt gebruikend belemmering-en-daling, kunt u de gegevens van Attributen van de Klant via FTP aan de Experience Cloud uploaden.

U kunt de gegevens uploaden nadat u een bron van Kenmerken van de Klant en een rekening van FTP in de Experience Cloud creeert. U maakt één FTP-account per kenmerkbron. De geüploade bestanden worden opgeslagen in de hoofdmap van dat account. De gegevens moeten in `.csv` formaat, met een tweede formaat `.fin` om aan te geven dat het uploaden is voltooid.

>[!IMPORTANT]
>
>Controleren [Gegevensbestandsvereisten voor het uploaden van klantkenmerken](crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19) voordat u het bestand uploadt.

Het uploaden van bestanden naar de FTP-site met klantkenmerken kan worden uitgevoerd via FTP of SFTP:

* U hebt een client nodig die SFTP-verbindingen ondersteunt.
* U kunt verbinding maken met SFTP via gebruikersnaam/wachtwoord of zonder wachtwoord, zoals beschreven [hier](https://experienceleague.adobe.com/docs/analytics/export/ftp-and-sftp/secure-file-transfer-protocol/ftp-sftp-cert-auth.html?lang=en).

**Het gegevensbestand uploaden via FTP**

1. [Een bron voor klantkenmerken maken en het gegevensbestand uploaden...](t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78).

   Controleer of u bent aangemeld bij uw FTP-site op `ftp.adobe.com/<sftpname>`.

1. Selecteer **[!UICONTROL Actions]** > **[!UICONTROL File Upload]**.

1. Een `.fin` zodat het bestand kan worden opgehaald.

   Het bestandstype `.fin` is door de gebruiker gemaakt en geeft aan dat het uploaden is voltooid. Het kan een leeg notebookbestand zijn. Als u bijvoorbeeld uploadt [!DNL crs123.csv], uploadt u ook [!DNL crs123.fin].

   Als het uploaden is voltooid, worden beide bestanden verplaatst naar een map met de naam **verwerkt**.

   Zie [Gegevensbestandsvereisten voor het uploaden van klantkenmerken](crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19) voor belangrijke informatie over bestandsnamen en -structuur.
