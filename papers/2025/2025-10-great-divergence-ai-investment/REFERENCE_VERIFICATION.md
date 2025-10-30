# Reference Verification Guide

## Status of References in `references.bib`

### ✅ VERIFIED - No Action Needed

These have DOIs or are confirmed academic sources:
- `gu2020` - Review of Financial Studies (DOI verified)
- `kelly2024` - Journal of Finance (DOI verified)
- `yang2023` - arXiv 2306.06031 (FinGPT - verified)

### ⚠️ NEEDS VERIFICATION - Check Before Publication

#### Major Consulting Firms
These reports likely exist but URLs need verification:
- **BCG reports** (bcg2025radar, bcg2024asset, bcg2024governance, bcg2025agents)
  - Action: Visit bcg.com/publications and search for actual reports
- **McKinsey report** (mckinsey2024)
  - Action: Verify at mckinsey.com

#### Regulatory Sources
- **FSB report** (fsb2025) - Check https://www.fsb.org/publications/
- **MAS Project Mindforge** (mas2025) - Check https://www.mas.gov.sg/publications

#### Industry Associations
- **Investment Association UK** (investmentassoc2024) - Check https://www.theia.org/
- **CFA Institute** (cfa2024pensions, cfa2025explainable) - Check https://www.cfainstitute.org/research

#### arXiv Papers (Future/Unverified IDs)
These arXiv IDs may be provisional or future publications:
- `columbia2025` - arXiv:2502.00342 (FinLLaVA)
- `salesforce2025` - arXiv:2410.10469 (Moirai-MoE)
- `shi2025` - arXiv:2508.02739 (Kronos)
- `xiao2024` - arXiv:2412.20138 (TradingAgents)
- `zhang2024` - arXiv:2402.18485 (FinAgent)

**Action**: Visit https://arxiv.org/abs/[ID] for each to verify

### ❌ LIKELY NOT PUBLICLY AVAILABLE

These may be internal/proprietary documents:
- `point72_2025` - Turion AI Fund report (likely internal)
- `wellsfargo2025` - SR11-7 document (likely internal)
- `vanguard2024` - Internal research
- `northern2024` - Internal research
- `validmind2025` - Vendor research

**Options**:
1. Remove these and cite only publicly available information
2. Change citation to "Personal communication" or "Proprietary research"
3. Replace with press releases or public announcements about these topics

### 🔍 VERIFY SSRN/OTHER

- `joshi2025` - SSRN:5246289 - Check https://papers.ssrn.com/
- `kim2024` - SSRN:4835311 - Check https://papers.ssrn.com/
- `aqr2024trading` - Journal of Portfolio Management citation needs verification
- `microsoft2025` - ICML 2025 (future conference)

## Recommended Actions

### Option 1: Conservative Approach (Recommended for Academic Publication)
Remove all unverifiable sources and keep only:
- Peer-reviewed journal articles with DOIs
- Verified arXiv papers
- Major institutional reports you can confirm exist
- SSRN papers you can access

### Option 2: Industry White Paper Approach (Current)
Keep all sources but:
- Add notes indicating which are based on company announcements/press releases
- Remove specific URLs that don't work
- Cite as "Institutional research" without URLs where appropriate

### Option 3: Hybrid Approach
- Keep academic sources with DOIs
- Keep major consulting firms (BCG, McKinsey, CFA) with generic URLs to their research sections
- Convert internal reports to "Cited in [press release]" format
- Remove arXiv papers that can't be verified

## Quick Fix Commands

To remove potentially problematic sources:

```bash
# Remove entries with "URL needs verification" or "Likely internal" notes
# Manually edit references.bib and remove those entries
```

## Citations in Paper That May Break

If you remove references, you'll need to remove or update citations in `paper.qmd` for:
- Wells Fargo SR11-7 framework
- Point72 Turion fund performance
- Various internal research citations

## Suggested Alternative Sources

Instead of proprietary reports, consider citing:
- **Press releases** from these firms announcing AI initiatives
- **SEC filings** for publicly traded firms
- **Conference presentations** (if publicly available)
- **News articles** in Bloomberg, Financial Times, WSJ covering these developments

## Next Steps

1. Decide which approach (1, 2, or 3) fits your needs
2. Verify critical sources you want to keep
3. Update `references.bib` accordingly
4. Check `paper.qmd` for any broken citations
5. Re-render and test

---

**Note**: This paper contains very current information (2024-2025). Some sources may not yet be publicly available or may be embargoed. Consider whether to:
- Wait until sources are published
- Replace with available alternatives
- Note that some information is based on industry announcements rather than formal publications

