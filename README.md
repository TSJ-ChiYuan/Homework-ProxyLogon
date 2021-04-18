## Homework-ProxyLogon
## 訓四子三 107362537 陳麒元

據我所知，很多公司企業都會用outlook，這次駭客利用ProxyLogon漏洞進駐受駭者系統並植入web shell程式，讓駭客得以長期從遠端控制受害組織的Exchange Server，包括竊取郵件、帳號資訊、執行任意程式碼、或在內部網路橫向移動，造成企業龐大的損失，所幸微軟有對此做出反應，去下載Microsoft Safety Scanner（MSERT）工具。管理員可以選擇全系統掃瞄或自訂掃瞄範圍。可能藏有web shell的資料夾包括：

● %IIS installation path%\aspnet_client\*

● %IIS installation path%\aspnet_client\system_web\*

● %Exchange Server installation path%\FrontEnd\HttpProxy\owa\auth\*

● 暫時性的ASP.NET files path

● %Exchange Server Installation%\FrontEnd\HttpProxy\ecp\auth\*

希望被駭的企業也能盡早把漏洞修補及web shell清除。但目前也只能發現攻擊，不保證能完全防止針對上述4項漏洞的攻擊。看來也只能等微軟盡快更新安全工具了，避免企業與機構再繼續受害。


![](https://memes.tw/user-gif-thumbnail/f8c2c3e8af3782606fd163b8ff6eb4e6.gif)
