sequenceDiagram
    participant User as 研究人員
    participant System as 系統

    User->>System: 輸入帳號和密碼
    System-->>User: 驗證帳號和密碼
    alt 成功
        System-->>User: 登入成功，顯示首頁
    else 失敗
        System-->>User: 顯示錯誤提示
    end

