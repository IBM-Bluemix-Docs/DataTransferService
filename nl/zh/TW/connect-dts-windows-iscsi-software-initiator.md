---

copyright:
  years: 2017, 2019
lastupdated: "2019-03-21"

---


# 在 Windows 中使用 iSCSI Software Initiator 連接至 DTS 裝置
{: #mountingDTSWindows}

若要與 Windows 中的 iSCSI LUN 互動，使用者必須使用 iSCSI Software Initiator（Microsoft 專有的 iSCSI 工具）來連接至儲存空間。對於 Windows Server 2008 或 Windows Vista 或更新版本的使用者，iSCSI Software Initiator 內建在作業系統中。Windows Server 2003、Windows XP 及 Windows 2000 的使用者，則必須先下載「啟動器」才能開始此程序。

## 連接至 iSCSI LUN

1. 從 {{site.data.keyword.slportal}} 擷取您要連接之儲存裝置的 **iSCSI 使用者名稱、密碼及儲存空間位址**。
2. 啟動 iSCSI Initiator。
3. 按一下**探索**。
4. 在**目標入口網站**區段中，按一下**新增**。
5. 在 **IP 位址或 DNS 名稱**欄位中，輸入 **iSCSI IP 位址**。
6. 按一下**進階**。
7. 更新 iSCSI 登入資訊。
   - 選取 **CHAP 登入資訊**勾選框，以啟用 CHAP 登入。
   - 在**使用者名稱**欄位中，輸入 iSCSI 使用者名稱。
   - 在**目標密碼**欄位中，輸入 iSCSI 密碼。
   - 按兩下**確定**。
8. 按一下**目標**
9. 從**目標**清單中，選取最近新增的 iSCSI。
10. 按一下**登入**。即會出現**登入目標**視窗。
11. 選取**系統啟動時自動還原此連線**，以設定在重新開機之間持續保持連線。
12. 按一下**進階**。
13. 更新 iSCSI 登入資訊。
    - 選取 **CHAP 登入資訊**勾選框，以啟用 CHAP 登入。
    - 在**使用者名稱**欄位中，輸入 iSCSI 使用者名稱。
    - 在**目標密碼**欄位中，輸入 iSCSI 密碼。
    - 按兩下**確定**。
14. 驗證在「目標」標籤上新的 iSCSI 目標顯示為「已連接」。
    - 如果您的 iSCSI 目標顯示為**已連接**，請按一下**確定**。您的 iSCSI LUN 現在已連接
    - 如果您的 iSCSI 目標沒有顯示為**已連接**，請重複之前的所有步驟，以重設連線。
