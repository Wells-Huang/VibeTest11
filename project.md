### 專案分析報告

#### 總結

此專案是一個使用 [Jekyll](https://jekyllrb.com/) 建立的靜態網站，並採用了 [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) 主題。Jekyll 是一個靜態網站生成器，可以將 Markdown 檔案、HTML、CSS 和 JavaScript 轉換為完整的網站。Minimal Mistakes 則是一個功能豐富且可自訂的 Jekyll 主題。

網站的內容主要位於 `_posts`、`_pages` 和 `_docs` 等目錄中，設定檔為 `_config.yml`。根據檔案結構判斷，此專案不僅是一個現成的網站，同時也是一個可供他人重複使用的 Jekyll 主題樣板。

#### 主要語言

*   **Markdown**: 佔 50.15%
*   **SCSS**: 佔 30.61%
*   **HTML**: 佔 15.68%
*   **JavaScript**: 佔 3.12%
*   **Ruby**: 佔 0.38%
*   **YAML**: 佔 0.05%

#### 關鍵檔案與目錄

| 檔案/目錄 | 用途 |
| :--- | :--- |
| `_config.yml` | **Jekyll 設定檔**：包含網站標題、描述、URL、作者資訊等全域設定。 |
| `Gemfile` | **Ruby 相依性管理**：定義專案所需的 Ruby gems，例如 `jekyll` 和 `minimal-mistakes-jekyll`。 |
| `index.html` | **首頁**：網站的主要進入點。 |
| `_layouts/` | **版面配置**：定義不同類型頁面（如文章、頁面、首頁）的 HTML 結構。`default.html` 是基礎版面配置。 |
| `_includes/` | **可重用元件**：包含可在多個版面配置中重複使用的 HTML 片段，例如頁首（`masthead.html`）、頁尾（`footer.html`）和側邊欄（`sidebar.html`）。 |
| `_sass/` | **樣式表**：包含 SCSS 檔案，用於定義網站的視覺風格。`minimal-mistakes.scss` 是主要的 SCSS 檔案。 |
| `assets/` | **靜態資源**：存放 CSS、JavaScript、圖片等不需 Jekyll 處理的檔案。 |
| `_posts/` | **文章內容**：存放部落格文章的 Markdown 檔案。檔案名稱需遵循 `YYYY-MM-DD-title.md` 格式。 |
| `_pages/` | **獨立頁面**：存放「關於」、「聯絡」等獨立頁面的 Markdown 檔案。 |
| `docs/` | **文件網站**：此目錄本身包含一個完整的 Jekyll 子專案，用於建立此主題的說明文件。 |

#### 執行與啟動

要預覽此網站，您需要在本機環境中安裝 Ruby、Bundler 和 Jekyll。

1.  **安裝相依套件**：
    ```shell
    bundle install
    ```
    此指令會根據 `Gemfile` 安裝所有必要的 gems。

2.  **啟動本地伺服器**：
    ```shell
    bundle exec jekyll serve
    ```
    此指令會建置網站，並在 `http://127.0.0.1:4000` 啟動一個本地開發伺服器。您可以透過瀏覽器存取此網址即時預覽變更。

#### 結論

這是一個結構清晰、文件完整的 Jekyll 主題專案。您可以透過修改 `_config.yml` 檔案來自訂基本設定，並在 `_posts` 和 `_pages` 目錄中新增您自己的 Markdown 內容來建立個人或專案網站。若要進行更深度的自訂，可以修改 `_layouts`、`_includes` 和 `_sass` 中的檔案。
