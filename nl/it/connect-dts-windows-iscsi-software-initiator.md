---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---


# Connessione a un dispositivo DTS in Windows con iSCSI Software Initiator
{: #mountingDTSWindows}

Per interagire con una LUN iSCSI in Windows, gli utenti devono connettersi all'archiviazione utilizzando iSCSI Software Initiator, lo strumento iSCSI proprietario di Microsoft. Per gli utenti di Windows Server 2008 o Windows Vista e versioni più recenti, iSCSI Software Initiator è integrato nel sistema operativo. Gli utenti di Windows Server 2003, Windows XP e Windows 2000 devono scaricare l'Initiator prima di avviare questa procedura.

## Collegamento a una LUN iSCSI

1. Dal {{site.data.keyword.slportal}}, richiama **nome utente, password e indirizzo di archiviazione di iSCSI** dal dispositivo di archiviazione per cui vuoi stabilire la connessione.
2. Avvia l'iniziatore iSCSI.
3. Fai clic su **Discovery**.
4. Nella sezione **Target Portals**, fai clic su **Add**.
5. Nel campo **IP address or DNS name**, immetti l''**indirizzo IP iSCSI**.
6. Fai clic su **Advanced**.
7. Aggiorna le informazioni di accesso iSCSI.
   - Seleziona la casella di spunta **CHAP logon information** per abilitare l'accesso CHAP.
   - Immetti il nome utente iSCSI nel campo **user name**.
   - Immetti la password nel campo **target secret**.
   - Fai clic su **OK** due volte.
8. Fai clic su **Targets**
9. Seleziona l'iSCSI appena aggiunta dall'elenco **Targets**.
10. Fai clic su **Logon**. Viene visualizzata la finestra **Log On to Target**.
11. Seleziona **Automatically restore this connection when the system boots** e imposta la connessione in modo che persista anche quando vengono eseguiti dei riavvii.
12. Fai clic su **Advanced**.
13. Aggiorna le informazioni di accesso iSCSI.
    - Seleziona la casella di spunta **CHAP logon information** per abilitare l'accesso CHAP.
    - Immetti il nome utente iSCSI nel campo **user name**.
    - Immetti la password nel campo **target secret**.
    - Fai clic su **OK** due volte.
14. Verifica che la nuova destinazione iSCSI venga visualizzata come Connected nella scheda Targets.
    - Se la tua destinazione iSCSI viene visualizzata come **Connected**, fai clic su **OK**. La tua LUN iSCSI è ora connessa.
    - Se la tua destinazione iSCSI non viene visualizzata come **Connected**, ripeti tutta la procedura precedente per reimpostare la connessione.
