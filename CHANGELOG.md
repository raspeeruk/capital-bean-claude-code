# Capital Bean — Changelog

## 2026-02-18 — FAQ Sections Added to 9 High-Value Posts (GEO + Schema Optimization)

Added structured FAQ sections (H2 "Frequently Asked Questions" + H3 questions with concise 2-3 sentence answers) to 9 key posts that were missing them. Each FAQ has 4-6 questions targeting common search queries and optimized for LLM extraction (GEO).

### Posts Updated

**Payday Loans Cluster (Core Business):**
| Post ID | Title | FAQs Added |
|---------|-------|------------|
| 3857 | What Is A Payday Loan? (PILLAR) | 6 FAQs — definition, cost, legality, bad credit, non-repayment, alternatives |
| 3715 | Payday Loan Laws | 4 FAQs — state bans, max APR, federal laws, law changes |
| 4622 | How Much Does a Payday Loan Cost? | 4 FAQs — average cost, why expensive, fees to watch, vs credit cards |
| 1945 | Why is The APR For Payday Loans So High? | 4 FAQs — average APR, vs credit card APR, state caps, avoiding high APR |
| 4573 | Should I Get a Payday Loan? | 4 FAQs — typical users, when appropriate, risks, pre-application considerations |
| 1942 | What Happens If You Can't Repay? | 4 FAQs — missed payment, court action, rollovers, alternatives |
| 5545 | How To Get Out Of Paying Back | 4 FAQs — legal options, debt cycle warning, wage garnishment, free help |

**Other High-Value Posts:**
| Post ID | Title | FAQs Added |
|---------|-------|------------|
| 2962 | Buying a House in 2026 | 4 FAQs — mortgage rates, price trends, timing, down payment |
| 4085 | What Loan Is Best For Bad Credit? | 4 FAQs — credit score threshold, loan types, credit improvement, pre-application checks |

### FAQ Schema Finding
**Correction:** FAQ schema does NOT auto-generate from standard HTML `<h2>/<h3>` FAQ structure. Yoast requires its own Gutenberg FAQ blocks to produce FAQPage schema. The FAQ content we added is still highly valuable for:
- GEO optimization (LLMs parse and cite concise Q&A pairs)
- Content quality (visitors get quick answers)
- Long-tail SEO (question-focused content targets search queries)

**Manual task needed:** To get FAQ rich results in Google, convert FAQ sections to Yoast FAQ blocks in the WordPress Gutenberg editor. Priority posts: 3857 (pillar), 3715, 4622.

### Posts That Already Had FAQ Sections (No Action Needed)
- 5534 (Are Payday Loans A Trap?) — 4 FAQs
- 6104 (How To Beat the Debt Crisis) — 5 FAQs
- 6097 (Retirement Planning) — 10 FAQs
- 6094 (Become Debt Free in Five Years) — existing FAQ section

---

## 2026-02-18 — Phase 6: Schema & E-E-A-T Audit

### Schema Assessment (Workstream 4)

| Schema Type | Status | Notes |
|-------------|--------|-------|
| Article schema | Present (Yoast) | dateModified IS updating when posts are edited via MCP. Confirmed: shows 2026-02-18 on edited posts |
| FAQ schema | NOT auto-generating | **Correction:** Yoast does NOT auto-generate FAQ schema from standard HTML H2+H3 structure. Requires Yoast FAQ Gutenberg blocks. FAQ content still valuable for GEO/content quality. Manual conversion needed. |
| HowTo schema | Missing | Not present on any posts. Could be added to "how-to" guides for rich results. |
| Organization schema | Present | Capital Bean, social profiles (Facebook, LinkedIn) |
| Breadcrumb schema | Present | Home > Post Title format |
| Author/Person schema | Present | Richard Allan, includes bio description |
| WebPage schema | Present | Includes meta description, image |

### E-E-A-T Assessment (Workstream 6)

**About Page (`/about-us/`)** — Moderate
- Has: Company name (Capital Bean), founder (Richard Allan), founding year (2021), business model explanation (loan matching, not direct lender), claimed 275K+ users, 50+ lender partnerships, physical address, phone, email
- Missing: Editorial standards, fact-checking process, detailed founder background, industry certifications

**Management Team (`/management-team/`)** — WEAK
- Lists 12 team members with titles (CEO, COO, CFO, CTO, CMO, etc.)
- Uses **auto-generated DiceBear cartoon avatars** instead of real photographs
- **No bios, no credentials, no LinkedIn links** for any team member
- This is a significant E-E-A-T weakness — looks like placeholder content

**Contact Page (`/contact-us/`)** — Good
- Physical address: 7072 Cedarwood Dr, Los Angeles CA 90006
- Two phone numbers: 1-855-884-6520, 1-865-884-6510
- Email: info@capitalbean.com
- Contact form, social media links (Facebook, LinkedIn, YouTube, Twitter)
- Minor issue: Address on About page says "7073" but Contact page says "7072"

**Editorial Policy** — MISSING
- `/editorial-policy/` returns 404
- No editorial standards documented anywhere on the site
- This is a significant gap for a YMYL financial site

**Financial Disclaimers** — Present
- Footer contains: High-Cost Disclosure, Loan Disbursement Timeline, Military Lending Act compliance, general credit warning
- Present on all posts checked

**Author Bio** — Present but Brief
- Richard Allan listed as author with bio
- Could be enhanced with specific financial credentials, certifications, experience details

**Visible "Last Updated" Date** — Present
- Shows correctly on all updated posts (e.g., "Last updated on February 18th, 2026 at 03:07 pm")
- Matches schema dateModified timestamp

### Manual Tasks Required for Schema + E-E-A-T

**HIGH PRIORITY (E-E-A-T for YMYL compliance):**

1. **Create Editorial Policy page** (`/editorial-policy/`)
   - Explain how content is researched, fact-checked, and updated
   - Describe content review process and frequency
   - Mention source requirements (government data, financial institutions)
   - Link from footer and About page

2. **Improve Management Team page** — one of two approaches:
   - **Option A:** Replace auto-generated avatars with real team photos, add bios with credentials/experience, add LinkedIn links
   - **Option B:** If team members aren't real staff, remove the page entirely (a fake team page is worse than none for E-E-A-T)

3. **Enhance author bio for Richard Allan**
   - Add specific financial expertise/credentials
   - Add years of experience in personal finance
   - Link to LinkedIn profile
   - Consider adding to individual post author boxes

4. **Fix address inconsistency**: About page shows "7073 Cedarwood Drive" but Contact page shows "7072 Cedarwood Dr" — should match exactly

5. **Add editorial standards section to About page**
   - Brief paragraph on content quality commitment
   - Link to full Editorial Policy page (once created)

**MEDIUM PRIORITY (Schema opportunities):**

6. **Add FAQ sections to high-traffic posts that don't have them**
   - Yoast auto-generates FAQ schema from H2 "Frequently Asked Questions" + H3 question format
   - Posts already have this format and ARE getting schema. Ensure consistency.
   - Posts that could benefit from FAQ sections: pillar content like "What Is A Payday Loan?" (ID 3857)

7. **Consider HowTo schema for relevant guides**
   - Posts like "How To Budget", "How To Repay Debts", "How To Buy A Home" could benefit from HowTo structured data
   - Requires Yoast HowTo block formatting or manual JSON-LD

**LOW PRIORITY:**

8. **Verify Organization schema completeness**
   - Add founding date (2021), founder name, physical address to schema
   - Currently only has name, URL, and social profiles

9. **Add more social profile links to Organization schema**
   - YouTube and Twitter are on the Contact page but may not be in schema

---

## 2026-02-18 — P2 Home & Property Posts (1 Updated + 2 Reviewed)

### Post: What Credit Score Do You Need to Buy a House? (ID: 2964)
**URL:** https://capitalbean.com/guides/credit-score-for-house/
- Updated stale FICO data: "the average was 757 for the 6-month period ending in September 2021" → made evergreen: "the average credit score for approved mortgage applications is typically in the mid-to-high 700s"
- Removed empty H2 tag wrapping image (same pattern as other posts)

### Posts Reviewed — No Update Needed (2 Posts)
- **ID 2953** — How To Buy A Home - A Step-by-Step Guide (all 15 steps are evergreen advice, no stale data)
- **ID 2957** — How Can I Tell If I'm Ready to Buy a House? (evergreen advice, $400K example still reasonable)

---

## 2026-02-18 — P3 Content Quality Fixes (25 Posts Updated + ~45 Reviewed)

All remaining P3 (evergreen) posts across every cluster have been reviewed. Posts with typos, garbled text, stale data, empty HTML tags, or placeholder content were fixed via MCP. Posts found to be entirely clean/evergreen were left as-is.

### P3 Payday Loans — 13 Posts Updated

**Post 6096** — Is a 3 Month Payday Loan Your Best Quick Cash Solution?
- Fixed typo: "Loaan" → "Loan"

**Post 4421** — Can I Get A Payday Loan If I Just Started A Job?
- Removed stale year reference

**Post 3880** — Top 9 Uses For Payday Loans
- Updated "37 states" → "approximately 30" (reflects 18 states + DC bans)

**Post 2832** — Can Payday Lenders Sue You?
- Fixed typo: "repair" → "repay"
- Removed empty H2 tag wrapping image

**Post 4491** — Am I Eligible For A Payday Loan?
- **CRITICAL FIX:** Changed payday loan amount from "$35,000" to "$1,000" (wildly incorrect)

**Post 4514** — How Old Do I Have To Be To Get A Payday Loan?
- Fixed age requirement text
- Updated state ban count to 18 states + DC

**Post 4386** — Can I Get A Payday Loan If I Am Retired?
- Fixed SSI name reference
- Fixed demographics data
- Removed placeholder text

**Post 3889** — How Will A Payday Loan Impact My Credit Rating?
- Fixed "or" → "for", "lender" → "borrower"
- Removed empty H3 tag

**Post 3887** — Can I Repay My Payday Loan Early?
- Removed empty H2 tags
- Updated "396%" → "391%" (CFPB average)

**Post 3847** — Can I Get A Payday Loan To Repair My Car?
- Fixed "breaks" → "brakes"
- Fixed "A" → "An" (article agreement)
- Fixed secured/unsecured loan logic error

**Post 3540** — Would A Payday Lender Report To Credit Bureaus?
- Fixed 3 typos throughout

**Post 3794** — Can I Repay My Loan By Phone Or Online?
- Wrapped plain text in proper H2 heading tag

### P3 Payday Loans — Reviewed, No Update Needed (7 Posts)
- **6093** — How to Find Out if You Owe Payday Loans?
- **6100** — What Is A 3 Month Payday Loan?
- **1939** — Can You Get A Payday Loan With Bad Credit?
- **4359** — Will A Payday Lender Contact My Employer?
- **3891** — How Can I Repay My Payday Loan?
- **3851** — Can I Renew A Payday Loan?
- **4483** — Do I Need Insurance For My Payday Loan?

### P3 Credit & Debt — 4 Posts Updated

**Post 3762** — 6 Top Tips To Handle Debt Repayments
- Updated stale stat: "$841 billion" → "$1.2 trillion" (US credit card debt)
- Fixed typo: "fiver.com" → "fiverr.com"

**Post 2469** — The Best Ways To Repay Debts
- Removed stale year reference
- Updated "400%" → "391%" (CFPB average APR)
- Updated rollover stat

**Post 3055** — How To Repay Debts
- Fixed "30% is for one" → "30% is for wants" (50/30/20 budgeting rule)

**Post 6094** — How To Become Debt Free In Five Years
- Added missing conclusion paragraph (Conclusion H2 was empty)

**Post 2501** — Do Payday Loans Help Build Your Credit?
- **CRITICAL FIX:** Changed misleading "only around 15% of Americans struggle to repay" to "80% of payday loans are rolled over or renewed" (CFPB data)

### P3 Financial Planning — 1 Post Updated

**Post 2881** — Where to Find Free Budget Templates and Spreadsheets
- Updated "best apps of 2022" → "best budgeting apps available" (removed stale year)

### P3 Financial Planning — Reviewed, No Update Needed (4 Posts)
- **2877** — Envelope Budgeting System
- **2879** — How to Calculate Your Take-Home Income
- **3617** — How To Easily Save Money Day-To-Day
- **3570** — How To Save Money - Five Top Tips

### P3 Loans & Borrowing — 3 Posts Updated

**Post 6126** — What Is The Loan Funding Process?
- Fixed garbled text: "disburses the funds ler" → "to the seller"
- Fixed garbled text: "It's cru at the time of closingcial" → "It's crucial...at the time of closing"
- Fixed double comma

**Post 3471** — How Do No Credit Check Loans Work?
- Fixed "will based" → "will be based"

**Post 1961** — What is a Credit Union?
- Fixed 4 apostrophe errors ("credit union's" → "credit unions", "member's" → "members'")
- Removed empty H2 tag
- Made credit union count heading evergreen (removed stale "2023" data, updated to ~4,700 credit unions)
- Made APR reference evergreen (removed specific dated figure)

### P3 Loans & Borrowing — Reviewed, No Update Needed (6 Posts)
- **6103** — What is an Upsidedown Loan?
- **6112** — How To Leverage Loans for Growth
- **6124** — How To Get A Pool Loan With Bad Credit?
- **3526** — What Is A Credit Card Cash Advance?
- **2509** — What Is A Title Loan?
- **2080** — What is APR and How Does it Work?
- **2004** — Secured vs Unsecured Loan

### P3 Home & Property — 3 Posts Updated

**Post 3119** — Should I Pay My Mortgage Bi-Weekly?
- Fixed "they own" → "they owe"
- Fixed "your Linda" → "your lender"

**Post 2970** — Houses or Condos - What Should You Choose?
- Fixed "in want" → "and want"

**Post 2968** — Single Family Homes - What Are The Alternatives?
- Fixed "It's age" → "Its age" (possessive vs contraction)

### P3 Home & Property — Reviewed, No Update Needed (4 Posts)
- **3126** — Hidden Costs of Homeownership
- **2952** — What Is Title Insurance?
- **3842** — How To Save Money On Home Improvements
- **3088** — Home Improvements - DIY or Hire a Pro?

### P3 Savings & Banking — 2 Posts Updated

**Post 4675** — How To Save Money On Christmas Shopping
- Removed empty H2 tag wrapping image

**Post 3756** — How To Open A Bank Account
- Fixed typo: "compan" → "company"
- Changed "FCA" (UK Financial Conduct Authority) reference to appropriate US regulator (FDIC/CFPB)

### P3 Savings & Banking — Reviewed, No Update Needed (8 Posts)
- **3108** — How To Get Cash Fast
- **3385** — 7 Ways To Make Fast Cash
- **2864** — Shop Well On a Tight Budget
- **1990** — How Can I Save Money on My Car?
- **2457** — Avoid Wasting Cash With These 5 Tips
- **2451** — 5 Top Tips For Budgeting
- **2459** — How To Use Budgeting Apps
- **3099** — Switch To A New Bank

### P3 Employment & Lifestyle — 3 Posts Updated

**Post 2446** — Can I Get Financial Assistance From My Workplace?
- Fixed "Korger" → "Kroger"

**Post 2839** — How Can I Save Money When Running a Business?
- Fixed "teh" → "the"
- Removed empty H2 tag wrapping image

**Post 6115** — Best Cities To Live For Families
- **MAJOR FIX:** Rewrote Conclusion section (contained "Example City" placeholder text that was never replaced)
- **MAJOR FIX:** Rewrote FAQ answers to reference actual cities discussed in article (Plano, Madison, Raleigh, Boston, San Francisco)
- Fixed "won't stay within" → "won't strain"

### P3 Employment & Lifestyle — Reviewed, No Update Needed (3 Posts)
- **6128** — What Happens If A Bank Teller Makes A Mistake?
- **6107** — How To Master Two Jobs Without Burnout
- **6127** — Top US Living Picks: Midwest Gems

### P3 WPBakery Posts — Cannot Update via MCP (11 Posts)
The following posts use WPBakery shortcodes and require manual updates in WP Admin:

| Post ID | Title | Issues Found |
|---------|-------|-------------|
| 4274 | Can I Get A Payday Loan On Social Security? | No issues found |
| 3517 | Do I Need A Bank Account For A Payday Loan? | No issues found |
| 2745 | Do Payday Loans Affect Mortgage Application? | No issues found |
| 1949 | What is a Credit Limit and Why Does it Matter? | "net" → "next" typo |
| 3493 | Snowball Method To Debt Repayments | "net" → "next" typo |
| 3495 | Debt Avalanche | Empty H2 tag |
| 2871 | Budgeting 101 | "belp" → "help", "standar" → "standard" |
| 2875 | Zero-Based Budgeting | No issues found |
| 2883 | 35+ Budgeting Categories | "Emergencies fundy" → "Emergency fund" |
| 1997 | How to Save Money at Home | No issues found |
| 4259 | Top 10 Best Cities For Quality Of Life | Too large to scan (110K chars) |

---

## 2026-02-18 — P2 Financial Planning, Loans & Banking Posts Updated (2 Updated + 6 Reviewed)

### Post 30: How Do I Make A Financial Plan? (ID: 3547)
**URL:** https://capitalbean.com/guides/how-do-i-make-a-financial-plan/
- **CRITICAL FIX:** Updated 401(k) contribution limit from "$19,500" (2021) to "$24,500 (2026)"
- Updated 401(k) catch-up from "$26,000" to "$8,000 catch-up (total $32,500)"
- Added SECURE 2.0 "super catch-up" for ages 60-63: $11,250 (total $35,750)
- Updated Roth IRA from "$6,000/$7,000" to "$7,500 (2026) with $1,100 catch-up (total $8,600)"
- Updated emergency savings stat from "47% of Americans" (Motley Fool, outdated) to "59% can't cover $1,000" (Bankrate 2025) with source link
- Removed empty H3 tag
- Added IRS link for contribution limits

### Post 31: Fix Overdrawn Account in Collections (ID: 6098)
**URL:** https://capitalbean.com/guides/overdrawn-bank-account-went-to-collections-what-to-do/
- Fixed garbled text: "You'll Your Finances" → "Assess Your Finances"
- Fixed garbled text: "quicHere'se" → "quick reference"
- Fixed garbled text: "don't worry, don't get your strategies" → "don't worry—there are strategies"
- Fixed garbled text: "there's a clue to recovery" → "there's a clear path to recovery"
- Fixed garbled text: "it's about contestants" → "it's about consistent"
- Fixed "counteroffer counteroffer bu, but" → "counteroffer, but"

### Posts Reviewed — No Update Needed (6 Posts)
- **ID 6092** — How Often Should A Financial Checkup Be Completed? (entirely evergreen advice)
- **ID 6125** — How Does Inflation Affect Borrowers? (general educational content, no stale data)
- **ID 4085** — What Loan Is Best For Bad Credit? (general guide, minor pre-existing truncation at end)
- **ID 4075** — What Is Predatory Lending? (entirely evergreen educational content)
- **ID 6129** — Public Loan Forgiveness (steps still current; uses "PLF" instead of standard "PSLF" throughout — pre-existing naming issue)
- **ID 6133** — How To Protect Your Account From Bank Levies (entirely evergreen legal/financial advice)

---

## 2026-02-18 — P2 Credit & Debt Posts Updated (3 Updated + 7 Reviewed)

### Post 27: Should You Take Out a Loan To Pay Off Credit Card Debt? (ID: 6081)
**URL:** https://capitalbean.com/guides/should-you-take-out-a-loan-to-pay-off-credit-card-debt/
- Fixed typos: "exploress" → "explores", "addresseses" → "addresses", "providess" → "provides"
- Updated credit card APR from "often exceeding 20%" to "22.30% as of Q4 2025" with Federal Reserve link
- **MAJOR FIX:** Filled 6 completely empty H2 sections that had headings but no content:
  - "What are the downsides..." — added origination fees, risk of more debt, longer repayment, credit impact, eligibility
  - "Frequently Asked Questions" — rewrote with proper Q&A format (balance transfers, savings calculation, credit score impact)
  - "Great ways to consolidate" — added balance transfer cards, HELOCs, debt management plans, 401(k) loans
  - "Can I raise my credit score fast?" — added 5 actionable steps with internal link
  - "Pros and cons" — added comparison table
  - "Tips if loan is declined" — added 5 steps (review denial, try different lender, co-signer, work on credit, alternatives)
  - "Small loan with bad credit" — added credit unions, secured loans, online lenders, peer-to-peer options

### Post 28: How Can I Raise My Credit Score To 800? (ID: 1974)
**URL:** https://capitalbean.com/guides/how-can-i-raise-my-credit-score-to-800/
- Fixed typo "data from 2034" → "data from 2023"
- Fixed heading "2023 Credit Score Statistics and Facts" → "Credit Score Statistics and Facts" (removed year reference for longevity)
- Removed empty H2 tag

### Post 29: Credit-Building Strategies for US Immigrants (ID: 6076)
**URL:** https://capitalbean.com/guides/what-are-the-top-5-credit-building-strategies-for-us-immigrants/
- Fixed typo "Openingng" → "Opening"
- Fixed garbled text "immigrants like  who want" → "immigrants who want"
- Fixed "I regularly report to the major credit bureaus" → "Issuers regularly report..."
- Cleaned up inconsistent first-person/third-person voice throughout Credit Builder loan section

### Posts Reviewed — No Update Needed (7 Posts)
The following P2 Credit & Debt posts were reviewed and found to be entirely evergreen with no stale data:
- **ID 6110** — Tips On How To Improve Your Tier 3 Credit Scores (FICO ranges, credit factors all current)
- **ID 6114** — How Do Leases & Rental Reports Affect Your Credit (evergreen advice)
- **ID 6099** — How to Calculate Your Debt-to-Income Ratio (standard DTI thresholds unchanged)
- **ID 6069** — Understanding a Thin Credit File (evergreen educational content)
- **ID 6062** — 5 Quick Steps to Boost Your Credit Score Fast (evergreen strategies)
- **ID 2064** — How Can I Check My Credit Score (methods still current)
- **ID 3216** — What Is Debt Consolidation? (WPBakery — has "deck consolidation" typo x2, needs manual fix)

---

## 2026-02-18 — P2 Payday Loan Posts Updated (7 Posts)

### Post 20: How Much Does a Payday Loan Cost? (ID: 4622)
**URL:** https://capitalbean.com/guides/how-much-does-a-payday-loan-cost/
- Updated credit card APR from "15.91% in 2021" to "22.30% as of Q4 2025" with Federal Reserve link
- Updated state ban count to "18 states and DC"
- Added CFPB March 2025 two-strikes rule paragraph

### Post 21: Why is The APR For Payday Loans So High? (ID: 1945)
**URL:** https://capitalbean.com/guides/why-is-the-apr-for-payday-loans-so-high/
- Updated average APR from "400%" to "391%"
- Updated credit card APR from "12% to 30%" to "22.30% as of Q4 2025" with Federal Reserve link
- Updated key points: "780% APR" to "650%+ APR (e.g., Idaho at 652%)"
- Added state ban count "18 states and DC" to key points
- Updated maximum APR section with specific state figures (Idaho 652%, Utah 554%, Texas 527%)
- Removed "huge proportion of the United States still permits payday loans with no legislation" (outdated)
- Added internal link to non-repayment post

### Post 22: Are Payday Loans A Trap? (ID: 5534)
**URL:** https://capitalbean.com/guides/are-payday-loans-a-trap/
- **CRITICAL FIX:** Changed payday loan amount from "$100 to $35,000" to "$100 to $1,000" (was wildly incorrect)
- Fixed typo "Trapd" → "Trap" in FAQ heading
- Updated FAQ: added specific state ban count (18 states + DC)
- Added CFPB link and March 2025 rule reference to repayment FAQ
- Updated regulation FAQ with federal/state specifics

### Post 23: Should I Get a Payday Loan? (ID: 4573)
**URL:** https://capitalbean.com/guides/should-i-get-a-payday-loan/
- Added CFPB March 2025 two-strikes rule to "What If I Cannot Repay" section with CFPB link
- Fixed typo "then" → "than" in image caption
- Fixed punctuation on 'wage garnishment'

### Post 24: How To Get Out Of Paying Back A Payday Loan (ID: 5545)
**URL:** https://capitalbean.com/guides/how-to-get-out-of-paying-back-a-payday-loan/
- Updated "legally accessible in 37 out of the 50 states" to "approximately 30 of the 50 states"
- Added note about 18 states + DC banning/prohibiting payday lending
- Removed empty shortcodes at end of post (`[] [/][] [/]`)

### Post 25: What Happens If You Can't Repay Your Payday Loan (ID: 1942)
**URL:** https://capitalbean.com/guides/what-happens-if-you-cannot-repay-your-payday-loan/
- Fixed typo "banik" → "bank"
- Fixed "unaffordable for the lender" → "unaffordable for the borrower"
- Added CFPB March 2025 two-strikes rule to Key Points and new paragraph after rollover section
- Added CFPB link

### Post 26: What is The Cooling Off Period For Payday Loans? (ID: 6053)
**URL:** https://capitalbean.com/guides/what-is-the-cooling-off-period-for-payday-loans/
- Added "18 states and DC have banned payday lending" to Key Points
- Minor grammar fix: "follow any practices" → "follow practices designed"

---

## 2026-02-18 — Workstream 3: Content Quality Cleanup

### 3.1 Off-Topic Content — NEEDS MANUAL REMOVAL
The following posts dilute topical authority and should be 301-redirected then trashed:

| Post ID | Title | Redirect To |
|---------|-------|-------------|
| 4548 | What Is An NFT? | `/guides/how-to-avoid-credit-card-scams/` (closest finance topic linked in the post) |
| 6132 | How Do I Get On The Paid Off Game Show? | `/guides/the-best-ways-to-repay-debts/` (student debt focus) |
| 3259 | How Much Does It Cost For Cable? | `/guides/how-to-budget/` (budgeting link already in post) |

**Steps for each:** WP Admin → install Redirection plugin (or use Yoast) → add 301 redirect from old URL to target → move post to Trash.

### 3.2 Chambers of Commerce Posts — NEEDS MANUAL REVIEW
6 chambers posts found (4 published + 1 draft + 1 duplicate already flagged):

| Post ID | Title | Status | Action |
|---------|-------|--------|--------|
| 4872 | Best Chambers Of Commerce In Alabama Announced | Published | Keep (canonical) or remove — off-topic |
| 4909 | Best Chambers Of Commerce In Alabama Announced | Published | Already flagged for 301 → 4872 |
| 6662 | Top 15 Chambers of Commerce in Alabama | Draft | Delete (third duplicate) |
| 4761 | Best Chambers Of Commerce In California Announced | Published | Consider removing — off-topic |
| 4910 | Best Chambers Of Commerce In Colorado | Published | Consider removing — off-topic |
| 4956 | Best International Chambers Of Commerce in Florida | Published | Consider removing — off-topic |

**Recommendation:** These are all off-topic for a personal finance/payday loan site and dilute topical authority. Consider removing all with 301 redirects to the homepage or About page.

### 3.3 Fixed Empty Gender Gap Table (ID: 6095)
**URL:** https://capitalbean.com/guides/9-eye-opening-statistics-and-facts-about-financial-health/
- Filled previously empty gender gap table with real data:
  - Median Annual Earnings: Men $66,790 / Women $55,240 (BLS 2023)
  - Median Retirement Savings: Men $92,000 / Women $56,000 (Transamerica 2025)
  - Average Life Expectancy: Men 74.8 / Women 80.2 years (CDC 2022)
- Added source attribution line below the table
- Updated surrounding paragraph with specific BLS earnings figures

### 3.4 Merged Duplicate 3-Month Payday Loan Posts
**Kept:** ID 6100 — "What Is A 3 Month Payday Loan?" (`/guides/quick-cash-loans-what-is-a-3-month-payday-loan/`)
**Redirect needed:** ID 6096 — "Is a 3 Month Payday Loan Your Best Quick Cash Solution?" (`/guides/is-a-3-month-payday-loan-a-good-quick-cash-option/`)
- Merged the "Alternatives to a 3-Month Payday Loan" section from 6096 into 6100
- 6100 now covers: definition, how it works, benefits, eligibility, risks, alternatives, FAQ
- **Manual step:** 301 redirect 6096 → 6100, then trash 6096
- Also fixed typo "They are understanding" → "Understanding" in how-it-works section

### 3.5 State Pages APR Audit — NEEDS MANUAL UPDATE (WPBakery)
All 20 state pages use WPBakery shortcodes and cannot be updated via MCP. Key issues found:

**Alabama (ID 2011)** `/payday-loans/alabama/`
- Hero representative example shows **4000% APR** (on $400/3 months)
- Body shows **456% APR** (on $500/31 days)
- These are two different calculations but it's confusing — should clarify or standardize

**Virginia (ID 3778)** `/payday-loans/virginia/` — CRITICAL
- Hero representative example still shows **400% APR** — WRONG, Virginia caps at **36%** since Fairness in Lending Act 2020
- FAQ says "Virginia allows payday loans with triple-digit interest rates" — WRONG
- FAQ says "Virginia limits outstanding payday loans to $500" — WRONG, max is **$2,500**
- Payday loan popularity table only goes to 2019 — needs updating or removing
- Body regulation section is correct (36% cap, $2,500 max, 24-month term)

**Ohio (ID 2378)** `/payday-loans/ohio/` — CRITICAL
- Hero representative example shows **400% APR** — WRONG, Ohio caps at **28%** since 2018 Fairness in Lending Act
- Body regulation table correctly shows 28%
- FAQ says "best possible rate in Colorado" — COPY-PASTE ERROR, should say "Ohio"

**Recommendation:** Audit all 20 state pages for similar APR inconsistencies between hero/representative examples and actual state law. Virginia and Ohio are the most critical as the representative APR examples are factually incorrect given current law.

---

## 2026-02-18 — Retirement & Credit Posts Updated (1 Post + 2 Reviewed)

### Post 17: Smart Retirement Planning (ID: 6097)
**URL:** https://capitalbean.com/guides/when-and-how-to-start-your-smart-retirement-planning/
- Updated 401(k) catch-up contribution limit from "$6,500 for 2023" to "$8,000 for 2026"
- Added SECURE 2.0 "super catch-up" for ages 60-63: $11,250 (total $35,750)
- Updated standard 401(k) limit to $24,500 and IRA limit to $7,500 for 2026
- Updated IRA catch-up from "$1,000" to "$1,100 for 2026"
- Updated RMD age from "70 ½" to 73 (increasing to 75 in 2033) per SECURE 2.0 Act
- Added high-earner Roth catch-up requirement note (>$150,000 FICA wages, effective 2026)
- Added healthcare cost projection (nearly 10% increase in 2026)
- Added high-DA links: IRS (contribution limits, RMD FAQs)
- Fixed various grammatical issues

### Post 18: When Are Americans Planning Retirement? (ID: 6091)
**URL:** https://capitalbean.com/guides/when-americans-plan-retirement/
- **Reviewed — no update needed.** Content is entirely evergreen general advice with no stale statistics or dated references.

### Post 19: Understanding Bad Credit (ID: 6113) — NEEDS MANUAL UPDATE (WPBakery)
**URL:** https://capitalbean.com/guides/what-is-bad-credit/
- **NOT UPDATED VIA MCP** — uses WPBakery shortcodes ([vc_row], [vc_column], [vc_column_text], [nectar_global_section]) that would be stripped by MCP
- **Content is evergreen** — credit score ranges, factors affecting credit, improvement strategies are all still current. Low priority for manual update.

---

## 2026-02-18 — Year-in-Title Posts Updated (3 Posts)

### Post 14: Best Budgeting Books (ID: 2931)
**URL:** https://capitalbean.com/guides/best-budgeting-books/
- Updated title from "Best Budgeting Books of 2022" to "Best Budgeting Books of 2025"
- Updated "read in 2022" reference to "read in 2025"
- Fixed typos: "advcie" → "advice", "partcicular" → "particular", "phsycially" → "physically", "hten" → "then"
- Updated "two decades" reference for Rich Dad Poor Dad to "over two decades"

### Post 15: Buying a House (ID: 2962)
**URL:** https://capitalbean.com/guides/buying-a-house-2022/
- Updated title from "House Buying in 2022: What Is It Like?" to "Buying a House in 2026: What To Expect"
- Rewrote intro to reflect 2026 market ("The Great Housing Reset")
- Updated mortgage rates section: 3% (2021) → 6.3% projected (2026)
- Updated home prices: median $396,800, up 0.9% YoY (Jan 2026, NAR)
- Updated price forecast from 14.7% gains to 1-2% growth
- Updated inventory section: 4.2 months' supply, 24 months of consecutive YoY growth
- Added high-DA links: Redfin, NAR, J.P. Morgan
- Kept evergreen tips section (pre-approval, realtor, expectations, price limit)

### Post 16: Price Increases (ID: 3051)
**URL:** https://capitalbean.com/guides/price-increases-to-watch-in-2022/
- Updated title from "Price Increases To Watch in 2022" to "Price Increases To Watch in 2026"
- Complete data refresh with 2025/2026 figures:
  - Overall inflation: 2.4% (Jan 2026), down from peak 9.1% (June 2022)
  - Food: 2.9% increase in 2025; coffee +20%, beef +16%; USDA forecasts 2.3% increase in 2026
  - Gas: $2.81/gallon (Jan 2026), lowest since 2021, down 8.7% YoY
  - Healthcare: costs up 9.6% projected (2026); Medicare Part B $202.90/month
  - Energy: electricity +6.7%, utility gas +10.8%, fuel oil +7.4%
  - Housing: median $396,800, up 0.9% YoY; mortgage rates ~6.3%
- Added high-DA links: BLS, USDA, AAA, GasBuddy, Willis Towers Watson, NAR
- Added internal link to updated house buying guide

---

## 2026-02-18 — Priority 1 Blog Post Updates (2025/2026 Data Refresh)

### Post 1: Kitchen Remodeling ROI (ID: 3084)
**URL:** https://capitalbean.com/guides/how-remodeling-your-kitchen-can-return-a-great-roi/
- Updated 2022 Cost vs. Value data to 2025 figures ($28,500 average minor remodel cost, 113% ROI)
- Added note about cabinet tariff impacts on pricing
- Refreshed remodeling cost benchmarks throughout

### Post 2: Loan If Unemployed (ID: 6516)
**URL:** https://capitalbean.com/guides/can-i-get-a-loan-if-im-unemployed/
- Updated BLS employment quote from September 2024 to January 2026 data
- Changed job gains figure to 130,000 and unemployment rate to 4.3%

### Post 3: Impulse Buying Effects (ID: 6106)
**URL:** https://capitalbean.com/guides/what-are-the-negative-effects-of-impulse-buying/
- Updated impulse spending table to include 2024 ($282/mo) and 2025 ($314/mo)
- Added new stats: 54% spent $100+ on impulse buys, 73% of purchases unplanned, 40% of online spending is impulse

### Post 4: Late Tax Filing (ID: 6108)
**URL:** https://capitalbean.com/guides/what-happens-if-you-are-late-filing-taxes/
- Updated minimum penalty from $435 (2021) to $525 (2026)
- Updated IRS interest rate table to include Q1 2026 at 7%

### Post 5: Debt Crisis in America (ID: 6104)
**URL:** https://capitalbean.com/guides/young-american-debt-crisis/
- Added total U.S. household debt: $18.8 trillion (Q4 2025, NY Fed)
- Updated student loan stats: $1.83T total, 42.8M borrowers, $39,547 avg balance
- Updated credit card stats: record $1.277T total; Gen Z avg $3,493, Millennials $6,961; APR 22.30%; 72% of Gen Z carry a balance
- Updated auto loan stats: $1.67T total; Gen Z avg $20,241, Millennials $22,627; Gen Z spends 13.4% of income on car payments
- Added: 47% of Americans expect credit card debt to increase in 2026

### Post 6: Financial Health Statistics (ID: 6095)
**URL:** https://capitalbean.com/guides/9-eye-opening-statistics-and-facts-about-financial-health/
- Extended personal savings rate table through 2025 (added 2023: 3.7%, 2024: 3.8%, 2025: 4.9%)
- Added emergency savings stats: 59% can't cover $1,000 emergency, 27% have no savings, 36% have more credit card debt than savings
- Updated household debt table to Experian per-consumer data (2022–2025), avg $104,755
- Added total household debt ($18.8T) and breakdowns: credit cards $1.277T, student loans $1.66T, auto loans $1.67T

---

## 2026-02-18 — Core Payday Loan Content Updated (2 Posts + 1 Manual)

### Post 11: What Is A Payday Loan? (ID: 3857) — PILLAR CONTENT
**URL:** https://capitalbean.com/guides/what-is-a-payday-loan/
- Updated "legal in 37 states" to "approximately 30 states" (18 states + DC now ban or cap)
- Updated "12 million Americans will take out a payday loan in 2022" to current (removed year reference)
- Updated credit card APR from "12 to 30%" to "22% as of Q4 2025" with Federal Reserve link
- Updated APR from "400%" to "391%" with note about 650%+ in some states
- Updated "13" states prohibiting to "18 states and the District of Columbia"
- Added CFPB March 2025 two-strikes payment withdrawal rule
- Added high-DA links: CFPB, Pew Charitable Trusts, Federal Reserve, NCUA
- Fixed various grammatical issues

### Post 12: Payday Loan Laws (ID: 3715)
**URL:** https://capitalbean.com/guides/the-laws-in-every-state-where-payday-loans-are-legal/
- Rewrote intro to reflect 2025 regulatory landscape (18 states + DC)
- Added CFPB March 2025 payday lending rule section
- Updated Virginia row: old 500/30-day/601% APR → 2,500/24-month/36% cap (Fairness in Lending Act 2020)
- Updated Illinois row: added 2021 Predatory Loan Prevention Act, 36% APR cap
- Updated Nebraska row: added 2020 ballot initiative, 36% APR cap
- Updated Montana row: noted 2010 ballot initiative, 36% APR cap
- Updated South Dakota row: noted 2016 ballot initiative, 36% APR cap
- Updated Colorado row: noted 2018 ballot initiative, 36% APR cap
- Added asterisk (*) notation for all states with 36% APR caps
- Added note under table explaining asterisk system

### Post 13: Which US States Are Payday Loans Legal In? (ID: 2054) — NEEDS MANUAL UPDATE
**URL:** https://capitalbean.com/guides/which-us-states-are-payday-loans-legal-in/
- **NOT UPDATED VIA MCP** — uses WPBakery page builder shortcodes that may be stripped by MCP
- Needs manual update in WP Admin:
  - Change "32 states where payday loans are legal" to ~30
  - Change "12 states where payday loans are illegal" to 18 states + DC
  - Remove Virginia from "highest APR" list (now has 36% cap)
  - Remove Ohio from "highest APR" list (now 28%)
  - Update Obama/Trump regulatory references to include Biden/Trump 2.0 developments
  - Add CFPB March 2025 rule

---

## 2026-02-18 — Payday Loan Stats Posts Updated (4 Posts)

### Post 7: How Many People Take Out Payday Loans Each Year? (ID: 2042)
**URL:** https://capitalbean.com/guides/how-many-people-take-out-payday-loans-each-year/
- Updated storefront count: peaked at 23,000+ (2021), now fewer than 14,000 (2024)
- Updated industry value: US market $20 billion (2025, IBISWorld); global $35B (2023), projected $52B+ by 2033
- Updated APR figure from ~400% to 391% (average)
- Updated states banning payday loans: from "12 states + DC" to "18 states + DC"
- Removed Virginia from high-APR states list (VA enacted 36% cap in 2020)
- Added Idaho (652%), Utah (554%), Texas (527%) as highest APR states
- Added CFPB March 2025 payday lending rule (two-strikes payment withdrawal)
- Added high-DA links: CFPB, Pew Charitable Trusts, IBISWorld, Federal Register

### Post 8: How Many Payday Stores Are There in The US? (ID: 2075)
**URL:** https://capitalbean.com/guides/how-many-payday-stores-are-there-in-the-us/
- Major update: storefronts declined from 23,000+ to fewer than 14,000
- Added IBISWorld data: industry declining at 3.4% CAGR (2020-2025)
- Updated states banning payday loans to 18 + DC
- Restructured "decreasing storefronts" section with three factors: state bans, federal regulation, online migration
- Added note under state table clarifying data reflects peak 2021 counts
- Added CFPB March 2025 rule reference
- Added high-DA links: IBISWorld, CFPB, Pew Charitable Trusts

### Post 9: How Many People Don't Repay Payday Loans? (ID: 4460)
**URL:** https://capitalbean.com/guides/how-many-people-dont-repay-payday-loans/
- Updated credit card APR comparison from "30%" to "22% (Q4 2025)"
- Added CFPB March 2025 two-strikes rule to key points and conclusion
- Added high-DA links: CFPB (rollover data, new rule), Federal Reserve (credit card APR)
- Fixed repayment percentage to 15-20% range (CFPB data)

### Post 10: Average Size of a Payday Loan (ID: 2473)
**URL:** https://capitalbean.com/guides/what-is-the-average-size-of-a-payday-loan-in-the-us/
- Updated APR from "400%" to "391%" with corrected fee calculation
- Added median loan amount ($350, CFPB)
- Updated states prohibiting from "13" to "18 states + DC"
- Added stat: 70% of borrowers use loans for recurring expenses, not emergencies
- Added high-DA links: CFPB (loan data)

---

## 2026-02-18 — High-DA External Links Added

Added authoritative external links across all updated posts to strengthen domain authority signals.

### Post 1: Kitchen Remodeling ROI (ID: 3084)
- Linked "2025 Cost vs. Value Report" → remodeling.hw.net (Remodeling Magazine)
- Linked "50% tariff on imported kitchen cabinets" → nahb.org (NAHB)

### Post 3: Impulse Buying Effects (ID: 6106)
- Linked impulse spending stats → capitaloneshopping.com (Capital One Shopping Research)
- Linked $250+ impulse purchase stat → bankrate.com (Bankrate survey)
- Linked 73%/40% online spending stats → invespcro.com (Invesp)

### Post 4: Late Tax Filing (ID: 6108)
- Linked "Late filing penalties" → irs.gov/payments/failure-to-file-penalty
- Linked Q1 2026 interest rate → irs.gov/newsroom (IRS announcement)
- Linked quarterly interest rates reference → irs.gov/payments/quarterly-interest-rates
- Linked installment agreement → irs.gov/payments/online-payment-agreement-application

### Post 5: Debt Crisis in America (ID: 6104)
- Linked student loan debt total → educationdata.org (Education Data Initiative)
- Linked credit card balances → newyorkfed.org (NY Fed Household Debt Report)
- Linked credit card debt by generation → experian.com (Experian research)
- Linked auto loan data → lendingtree.com (LendingTree generation study)
- Linked 47% expect debt increase → nerdwallet.com (NerdWallet household debt study)

### Post 6: Financial Health Statistics (ID: 6095)
- Linked personal savings rate data → bea.gov (Bureau of Economic Analysis)
- Linked emergency savings report → bankrate.com (Bankrate)
- Linked total household debt → newyorkfed.org (NY Fed)
- Linked consumer debt data → experian.com (Experian Consumer Debt Study)
- Linked APA stress data → apa.org (American Psychological Association)
- Linked gender pay gap → bls.gov (Bureau of Labor Statistics)
