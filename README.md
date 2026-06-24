# oa-page-faq

橘子蘋果常見問題頁（`/faq`）的自助 landing page prototype。

## 部署網址
https://orangeapple.co/faq

## 維護方式
**只改一個地方**：`index.html` 內 `<script id="faq-data">` 的 JSON 陣列。

改完後：
- 畫面 FAQ 自動同步更新
- Google 看到的 FAQPage schema 自動同步更新
- 兩者永不脫鉤

## SEO 內建項目
- ✅ Title / meta description / canonical / robots
- ✅ Open Graph + Twitter Card
- ✅ JSON-LD: Organization + BreadcrumbList + WebPage + FAQPage
- ✅ 單一資料源 FAQ pattern
- ✅ Mobile responsive
- ✅ 時間戳記
- ✅ Rails shell 注入點（`<oa-header>` / `<oa-footer>`）

## 上線前 checklist
跑 `/oa-webpage-preflight` 確認 SEO meta、schema、CTA 屬性齊全。

## 上線後驗證
- Google [Rich Results Test](https://search.google.com/test/rich-results)
- GSC 提交 URL 索引
- 確認 sitemap 包含 `/faq/`
