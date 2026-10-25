# Seasonal calendar data attribution

Calendar dates: © Hong Kong Special Administrative Region Government / Hong Kong Observatory.

- Official Gregorian–Lunar conversion tables: https://www.hko.gov.hk/en/gts/time/conversion.htm
- Annual machine-readable source pattern: https://www.hko.gov.hk/en/gts/time/calendar/text/files/T2026e.txt (replace 2026 with the year).
- Government open-data catalogue: https://data.gov.hk/en-data/dataset/hk-hko-rss-gregorian-lunar-calendar-conversion-table
- Data terms: https://data.gov.hk/en/terms-and-conditions

The bundled `src/shared/seasonal-calendar.ts` contains extracted festival and solar-term dates for Gregorian years 2020–2100. The same data are compiled into both players. Calendar data remain attributable to their provider and are not represented as our original data or relicensed under the software's MIT licence. This customization has no affiliation with or endorsement from the provider.

For each annual source we check the expected number of Gregorian rows. The published T2069e.txt omits 2069/12/30 (lunar 11/17, no selected festival or term); that exact non-anchor gap is checked explicitly, with no inferred event substituted. Lunar month starts are identified from the table; a repeated month number marks an intercalary month, excluded from ordinary festival occurrences. Lunar dates extracted: 1/1, 1/15, 5/5, 7/7, 7/15, 8/15, 9/9 and 12/8. Solar terms extracted: Qingming, Frost, Heavy Snow and Winter Solstice. A Gregorian year may contain zero, one or two lunar 12/8 occurrences; all are retained. January 1, October 31 and December 25 are Gregorian fixed dates.

The action-to-event mappings are local product choices in `assets/config.jsonc`: falling leaves use Frost; snowman uses Heavy Snow. Other actions follow their named festivals, with multiple relevant anchors for fireworks, lanterns, tangyuan and dumplings. Eligibility covers the anchor date and seven local calendar days on either side, including both endpoints. Adjacent Gregorian years are checked to cover cross-year windows. Ordinary automatic selection alone is filtered; manual menu playback remains available throughout the year.

No network or system lunar-calendar conversion is used at runtime. Outside the supplied year range, missing lunar/solar-term dates fail closed. Fixed Gregorian festivals still work. The HKO notes that some far-future dates near midnight may differ by one day as astronomical predictions are refined; the data may be regenerated from revised official tables. Downloaded on 2026-10-25; source URLs and SHA-256 values are retained in the task's `work/move-season-stage2/calendar-sources.json`.
