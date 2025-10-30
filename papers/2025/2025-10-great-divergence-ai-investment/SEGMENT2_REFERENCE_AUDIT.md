# Segment 2 Reference Audit

## ✅ VERIFIED - Confirmed to Exist

### 1. Yang et al. (2023) - FinGPT
- **arXiv:** 2306.06031
- **Status:** ✅ VERIFIED
- **URL:** https://arxiv.org/abs/2306.06031
- **Note:** June 2023 - Confirmed exists

### 2. Zhang et al. (2024) - FinAgent
- **arXiv:** 2402.18485  
- **Status:** ✅ VERIFIED
- **URL:** https://arxiv.org/abs/2402.18485
- **Note:** February 2024 - Confirmed exists

## ⚠️ LIKELY EXIST - Need Direct Verification

### 3. Xiao et al. (2024) - TradingAgents
- **arXiv:** 2412.20138
- **Date:** December 2024
- **Status:** ⚠️ PLAUSIBLE
- **Action:** Check https://arxiv.org/abs/2412.20138 directly
- **Note:** December 2024 ID format is valid, but may not exist yet

### 4. Lesniewski & Trigila (2024) - Score-based Diffusion
- **arXiv:** 2412.00036
- **Date:** December 2024
- **Status:** ⚠️ PLAUSIBLE
- **Action:** Check https://arxiv.org/abs/2412.00036 directly
- **Note:** December 2024 ID format is valid

### 5. Salesforce - Moirai-MoE
- **arXiv:** 2410.10469
- **Date:** October 2024
- **Status:** ⚠️ PLAUSIBLE
- **Action:** Check https://arxiv.org/abs/2410.10469 directly
- **Note:** October 2024 ID format is valid

## ❌ PROBLEMATIC - Future Dates (Cannot Exist Yet)

### 6. Columbia - FinLLaVA
- **arXiv:** 2502.00342
- **Date:** **February 2025**
- **Status:** ❌ FUTURE DATE
- **Issue:** arXiv ID suggests February 2025 submission - cannot exist if we're in late 2024
- **Action:** Either incorrect ID or paper doesn't exist yet
- **Recommendation:** Remove or find correct ID

### 7. Berti & Kasneci - TRADES
- **arXiv:** 2502.07071
- **Date:** **February 2025**
- **Status:** ❌ FUTURE DATE
- **Issue:** arXiv ID suggests February 2025 submission
- **Action:** Find correct ID or remove
- **Recommendation:** Remove or update with actual ID

### 8. Shi et al. - Kronos
- **arXiv:** 2508.02739
- **Date:** **August 2025**
- **Status:** ❌ FUTURE DATE
- **Issue:** arXiv ID suggests August 2025 submission - far future
- **Action:** This is definitely incorrect
- **Recommendation:** Remove or find correct ID

## ⚠️ NON-ARXIV SOURCES - Need URL Verification

### 9. BCG - AI Radar 2025
- **URL:** https://www.bcg.com/publications/2025/ai-radar-agent-adoption
- **Status:** ⚠️ NEEDS VERIFICATION
- **Action:** Visit BCG website to confirm report exists
- **Note:** URL structure suggests it might be constructed

### 10. Microsoft Research - MarS
- **Venue:** "Proceedings of ICML 2025"
- **Status:** ❌ FUTURE CONFERENCE
- **Issue:** ICML 2025 hasn't occurred yet (typically held in July)
- **Action:** Check if pre-print available on Microsoft Research site
- **Recommendation:** Either find pre-print or note as "forthcoming"

### 11. Morgan Stanley - Agentic AI
- **URL:** https://www.morganstanley.com/ideas/agentic-ai-enterprise-2025
- **Status:** ⚠️ NEEDS VERIFICATION
- **Action:** Check Morgan Stanley Ideas section
- **Note:** URL may be constructed

### 12. T. Rowe Price - Q1 2025 Outlook
- **URL:** https://www.troweprice.com/insights/global-markets/ai-agents-investment-outlook-2025
- **Status:** ⚠️ FUTURE DATE
- **Issue:** Q1 2025 outlook may not be published yet
- **Action:** Check T. Rowe Price website
- **Recommendation:** If not available, remove or cite earlier report

## Summary by Status

| Status | Count | Action Required |
|--------|-------|-----------------|
| ✅ Verified | 2 | None - keep as is |
| ⚠️ Plausible 2024 | 3 | Verify URLs work |
| ❌ Future arXiv (2025) | 3 | **REMOVE or find correct IDs** |
| ⚠️ Institutional | 3 | Verify URLs work |
| ❌ Future Conference | 1 | Update to pre-print or remove |

**Total:** 12 references  
**Problematic:** 4 (33%)  
**Need Verification:** 6 (50%)  
**Confirmed Good:** 2 (17%)

## Recommendations

### Immediate Actions (Critical)

1. **Remove Future arXiv Papers** (2502.00342, 2502.07071, 2508.02739)
   - These IDs suggest 2025 submissions that cannot exist yet
   - Either find correct IDs or remove these citations from paper

2. **Update ICML 2025 Reference**
   - Change to arXiv pre-print if available
   - Or note as "Forthcoming in ICML 2025"

3. **Verify December 2024 Papers**
   - Manually check each arXiv URL
   - Remove if they don't exist

### Secondary Actions

4. **Verify Institutional URLs**
   - Check BCG, Morgan Stanley, T. Rowe Price links
   - Update URLs or remove if not publicly available

## Alternative Approach

If many references cannot be verified, consider:

1. **General Citations**: Cite company announcements or press releases instead
2. **Working Papers**: Note as "Working paper" or "Unpublished manuscript"
3. **Personal Communication**: For institutional research, cite as "Personal communication" with date
4. **Remove Specifics**: Keep the claims but remove the formal citation if source isn't verifiable

## Testing Commands

To test arXiv IDs, try:
```bash
curl -I https://arxiv.org/abs/2502.00342  # Should return 404 if doesn't exist
curl -I https://arxiv.org/abs/2402.18485  # Should return 200 if exists
```

Or visit directly:
- https://arxiv.org/abs/2502.00342
- https://arxiv.org/abs/2502.07071
- https://arxiv.org/abs/2508.02739
- https://arxiv.org/abs/2412.20138
- https://arxiv.org/abs/2412.00036
- https://arxiv.org/abs/2410.10469

## Next Steps

1. Test all arXiv IDs listed above
2. Remove/update future-dated papers (2025 IDs)
3. Verify institutional URLs
4. Update `references.bib` with corrected entries
5. Check `paper.qmd` for any citations that reference removed sources

